---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filtrado de mensajes de suscripción de eventos
description: Filtrado de mensajes de suscripción de eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1767'
ht-degree: 0%

---

# Filtrado de mensajes de suscripción de eventos

Puede crear componentes de procesamiento intermedios que le ayuden a filtrar y procesar únicamente los mensajes de suscripción de evento que su empresa necesita.

Para obtener más información sobre las suscripciones a eventos, consulte [API de suscripción a eventos](../../wf-api/general/event-subs-api.md).

## Filtrado de mensajes de eventos

Esta sección contiene fragmentos de código de filtrado que puede implementar para reducir la carga de los mensajes de suscripción de eventos.  Para ayudar a mostrar las diferencias en la sintaxis de varios lenguajes, estos fragmentos ilustran el mismo conjunto de filtros escritos en los siguientes lenguajes:

Puede ver ejemplos del filtrado en [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), donde puede ver las diferencias en la sintaxis de cada idioma y los medios de interacción con el SDK de AWS. Estos ejemplos se escriben como Lambdas de AWS, que es un método común para emplear componentes de filtrado y procesamiento intermedios.

Los siguientes fragmentos de código están casi listos para la implementación y pueden utilizarse como punto de partida para ayudarle a escribir sus propios filtros y componentes de procesamiento más complejos.

### Java

El siguiente ejemplo en Java muestra cómo filtrar las cargas útiles del proyecto en función del ID de grupo del proyecto, como se hace en [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Establezca el ID de grupo que está buscando y créelo como una constante estática.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   En este ejemplo, el método handleRequest, que es un nombre de método estándar de AWS Lambda, toma un tipo Map como primer parámetro, que es el contenido del mensaje de suscripción de evento.\
   El segundo parámetro que toma es el contexto de la solicitud actual de proxy Lambda.\
   El objeto Context se utiliza para obtener un registrador lambda, que se utiliza para escribir un mensaje en CloudWatchLogs.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Al invocar el método handleRequest, obtenga el atributo &quot;newState&quot; del mensaje de suscripción de evento, que representa el estado actualizado del recurso.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Para obtener más información sobre el formato newState, consulte [Formato de mensaje saliente para suscripciones a eventos](../../wf-api/api/message-format-event-subs.md).

3. Después de analizar el mapa &quot;newState&quot; a partir del mensaje, asegúrese de que el ID de grupo del objeto coincida con el ID de grupo identificado en el paso 1.

4. (Condicional) Si los identificadores **no coinciden**, suelte el mensaje para que se devuelva una respuesta vacía.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >Devolver una respuesta vacía y correcta es crucial. Cualquier cosa que no sea una respuesta de 200 niveles se considera un envío fallido.

5. Procese el mensaje.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   El SDK de AWS se utiliza para invocar otro Lambda, que es responsable de enviar el mensaje filtrado al punto de conexión deseado.

   El objetivo de transferir la responsabilidad de enviar el mensaje a otro Lambda es evitar que se agote el tiempo de espera de la solicitud de envío procedente del servicio de suscripción a evento. Actualmente, el tiempo de espera permitido para la entrega se establece en cinco segundos. Si el filtro tarda más de lo permitido por la configuración, puede procesar la solicitud, pero el servicio Suscripción de evento agotará el tiempo de espera y entrará en un bucle de reintentos hasta que reciba una respuesta de 200 niveles dentro del período de tiempo de espera.

   Para obtener más información sobre la administración de la entrega de mensajes, consulte [Mejora de la entrega de mensajes al aceptar los tiempos de espera](#improving-message-delivery-while-accommodating-timeouts).

### Python

La principal diferencia entre los ejemplos de Java y Python es que en el ejemplo de Java el mensaje de suscripción de evento se recibe como el primer parámetro y en el ejemplo de Python el primer parámetro es un &quot;evento&quot; de proxy Lambda, que contiene el mensaje de suscripción de evento junto con información sobre la solicitud de proxy Lambda de AWS.

El siguiente ejemplo en Python muestra cómo filtrar las cargas útiles del proyecto en función del ID de grupo del proyecto, como se hace en [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Establezca el ID de grupo que está buscando y créelo como una constante estática.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   El primer parámetro es el &quot;evento&quot; del proxy Lambda, que contiene el mensaje de suscripción de evento y cierta información adicional que debe analizarse.\
   El segundo parámetro es el contexto de la solicitud de proxy Lambda actual.\
   En este ejemplo, el objeto Context se utiliza para obtener un registrador lambda, que se utiliza para escribir un mensaje en CloudWatchLogs.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Analice el mensaje del evento.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Obtenga el atributo &quot;newState&quot; del mensaje de suscripción de evento.\
   El atributo newState representa el estado actualizado del recurso.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Para obtener más información sobre el formato newState, consulte [Formato de mensaje saliente para suscripciones a eventos](../../wf-api/api/message-format-event-subs.md).

1. Después de analizar el mapa &quot;newState&quot; a partir del mensaje, asegúrese de que el ID de grupo del objeto coincida con el ID de grupo identificado en el paso 1.

1. (Condicional) Si los ID no coinciden, suelte el mensaje para que se devuelva una respuesta vacía.

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >Devolver una respuesta vacía y correcta es crucial. Cualquier cosa que no sea una respuesta de 200 niveles se considera un envío fallido.

1. Procese el mensaje.

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   El SDK de AWS se utiliza para invocar otro Lambda, que es responsable de enviar el mensaje filtrado al punto de conexión deseado.

   El objetivo de transferir la responsabilidad de enviar el mensaje a otro Lambda es evitar que se agote el tiempo de espera de la solicitud de envío procedente del servicio de suscripción a evento. Actualmente, el tiempo de espera de la entrega es de cinco segundos. Si el filtro tarda más de lo permitido por la configuración, puede procesar la solicitud, pero el servicio Suscripción de evento agotará el tiempo de espera y entrará en un bucle de reintentos hasta que reciba una respuesta de 200 niveles dentro del período de tiempo de espera.


### Node.js

El ejemplo de Node.js de filtrado de ID de grupo de proyectos es similar a los ejemplos de Java y Python. Al igual que con el ejemplo de Python, el primer parámetro es un evento de proxy Lambda y el segundo parámetro es el contexto Lambda.

El siguiente ejemplo de Node.js muestra cómo filtrar las cargas útiles del proyecto en función del Id. de grupo del proyecto, como se hace en [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Establezca el ID de grupo que está buscando y créelo como una constante estática.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   El primer parámetro es el &quot;evento&quot; del proxy Lambda, que contiene el mensaje de suscripción de evento y cierta información adicional que debe analizarse.\
   El segundo parámetro es el contexto de la solicitud de proxy Lambda actual.\
   En este ejemplo, el objeto Context se utiliza para obtener un registrador lambda, que se utiliza para escribir un mensaje en CloudWatchLogs.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Analice el mensaje del evento.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Obtenga projectGroupID del atributo &quot;newState&quot; del mensaje de suscripción de evento y, a continuación, compárelo con el ID de grupo del grupo identificado en el paso 1.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Para obtener más información sobre el formato newState, consulte [Formato de mensaje saliente para suscripciones a eventos](../../wf-api/api/message-format-event-subs.md).

4. (Condicional) Si los ID no coinciden, suelte el mensaje para que se devuelva una respuesta vacía.\
   El siguiente ejemplo muestra los ID de grupo coincidentes:

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >Devolver una respuesta vacía y correcta es crucial. Cualquier cosa que no sea una respuesta de 200 niveles se considera un envío fallido.

5. Procese el mensaje.

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   El SDK de AWS se utiliza para invocar otro Lambda, que es responsable de enviar el mensaje filtrado al punto de conexión deseado.\
   El objetivo de transferir la responsabilidad de enviar el mensaje a otro Lambda es evitar que se agote el tiempo de espera de la solicitud de envío procedente del servicio de suscripción a evento. Actualmente, el tiempo de espera de la entrega es de cinco segundos. Si el filtro tarda más de lo permitido por la configuración, puede procesar la solicitud, pero el servicio Suscripción de evento agotará el tiempo de espera y entrará en un bucle de reintentos hasta que reciba una respuesta de 200 niveles dentro del período de tiempo de espera.\
   Para obtener más información sobre la administración de la entrega de mensajes, consulte [Mejora de la entrega de mensajes al aceptar los tiempos de espera](#improving-message-delivery-while-accommodating-timeouts).

## Mejora De La Entrega De Mensajes Al Adaptarse A Los Tiempos De Espera

El servicio Suscripción a eventos tiene un tiempo de espera estricto de **cinco segundos** para todas las solicitudes de envío. En el caso de que el envío de un mensaje supere el tiempo permitido, el servicio de suscripción a eventos inicia un ciclo de reintentos para ese mensaje.

Por ejemplo, genera un filtro de Id. de grupo de proyecto similar a uno de los ejemplos encontrados en [Filtrado de mensajes de eventos](#filtering-event-messages) e incluye una búsqueda en la base de datos para determinar si el mensaje es necesario. Es posible que la búsqueda de la base de datos junto con el tiempo necesario para el procesamiento necesario y para que Lambda se inicie en frío pueda tardar más de cinco segundos, lo que provoca que el servicio Suscripción de evento vuelva a intentar enviar el mensaje.

Puede evitar un reintento separando las partes del proceso que consumen tiempo de la lógica que es responsable de determinar si el mensaje es uno que desea procesar y enviar. Al hacerlo, puede aceptar el mensaje y enviar una respuesta de 200 niveles al servicio Suscripción a eventos, mientras continúa procesando o filtrando asincrónicamente el mensaje en segundo plano (consulte el paso 5 en [Java](#java) para ver un ejemplo).


Incluso si el procesamiento o el filtrado no superan el tiempo de espera de cinco segundos, sigue siendo ventajoso separar el primer punto de contacto del filtrado o procesamiento de mensajes de los demás pasos de procesamiento o envío del lado del cliente. De este modo, el envío del mensaje al destino desde el servicio de suscripción de evento tiene un impacto mínimo en el tiempo y el rendimiento de ambas partes.

Para obtener más información sobre el mecanismo de reintentos, consulte [Reintentos de suscripción de evento](../../wf-api/api/event-sub-retries.md).

## Implementación de filtros alojados en una arquitectura sin nubes

Si no puede aprovechar una arquitectura de nube para el filtrado de suscripciones a eventos, puede seguir utilizando los ejemplos de [Filtrado de mensajes de eventos](#filtering-event-messages) como hoja de ruta para implementar sus propios filtros alojados o componentes de procesamiento.

### Ajuste de ejemplos de filtrado para servicios independientes

Antes de usar los ejemplos de filtrado en un entorno sin nubes, haga lo siguiente:

* Omita las partes específicas de Lambda de los ejemplos, como el parámetro Context.

* Cambie las invocaciones de otros Lambda en los ejemplos para realizar solicitudes HTTP asincrónicas adicionales a otros filtros o componentes de procesamiento que aloje.

* Si se hace referencia a los ejemplos de Python y Node.js, sustituya el primer parámetro de evento por el primer parámetro de carga útil que se muestra en el ejemplo de Java. Consulte el Paso 1 en [Java](#java).

* Implemente los filtros o procesadores con una API basada en web.

### Prevención de mensajes de suscripción de eventos perdidos

En ocasiones, en una arquitectura sin nubes, es posible que los servicios responsables de recibir mensajes de suscripción de eventos no estén disponibles. En un evento de este tipo, los mensajes podrían superar el límite de reintentos y perderse, sin forma de recuperar la información dentro de los mensajes.

Le recomendamos que, durante el inicio del servicio, implemente una consulta que solicite el estado más reciente de todos los recursos que puedan haberse incluido en los mensajes omitidos. Como se muestra en el ejemplo siguiente, puede utilizar los criterios de filtro para consultar los recursos que coinciden con esos criterios y, a continuación, procesar su estado actual.

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v15.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

Al consultar los recursos, se asegura de que los sistemas integrados tengan la versión más actual de los recursos.

### Implementación del procesamiento asincrónico en la entrega de mensajes

Todos los ejemplos de la sección [Filtrado de mensajes de eventos](#filtering-event-messages) pasan la responsabilidad de enviar mensajes filtrados a otro AWS Lambda. Esto se hace para evitar superar el tiempo de espera de cinco segundos en la solicitud de envío, que aplica el servicio de suscripción de evento que emite la solicitud.

En una arquitectura sin nubes, es posible que deba implementar un mecanismo de procesamiento asincrónico similar a cómo el SDK de AWS permite las llamadas asincrónicas a otras Lambdas de AWS. La mayoría de los lenguajes de programación modernos tienen bibliotecas de terceros o principales que administran el procesamiento asincrónico, lo que le permite aprovechar el estilo asincrónico de procesamiento implementado en nuestros ejemplos.
