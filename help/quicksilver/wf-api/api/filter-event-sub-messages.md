---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filtrar mensajes de suscripción de evento
description: Filtrar mensajes de suscripción de evento
author: John
feature: Workfront API
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# Filtrar mensajes de suscripción de evento

Puede crear componentes de procesamiento intermedios que le ayuden a filtrar y procesar solo los mensajes de suscripción de evento que necesite su empresa.

Para obtener más información sobre las suscripciones a eventos, consulte [API de suscripción de evento](../../wf-api/general/event-subs-api.md).

## Filtrado de mensajes de eventos

Esta sección contiene fragmentos de código de filtrado que puede implementar para reducir la carga de los mensajes de suscripción de eventos.  Para ayudar a mostrar las diferencias en la sintaxis de los distintos idiomas, estos fragmentos ilustran el mismo conjunto de filtros escritos en los siguientes idiomas:

Puede ver ejemplos de filtrado en [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), donde puede ver las diferencias en la sintaxis de cada idioma y los medios de interacción con el SDK de AWS. Estos ejemplos se escriben como AWS Lambdas, que es un método común para utilizar componentes de filtrado y procesamiento intermedios.

Los siguientes fragmentos de código están casi listos para la implementación y se pueden utilizar como punto de partida para ayudarle a escribir sus propios componentes de procesamiento, más complejos y con filtros.

### Java

El siguiente ejemplo de Java muestra cómo filtrar las cargas del proyecto en función del ID de grupo del proyecto, tal como se hace en [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Establezca el ID de grupo que está buscando y créelo como una constante estática.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   En este ejemplo, el método handleRequest , que es un nombre de método estándar de AWS Lambda, toma un tipo Map como su primer parámetro, que es el contenido del mensaje de suscripción de evento.\
   El segundo parámetro que toma es el contexto de la solicitud de proxy Lambda actual.\
   El objeto Context se utiliza para obtener un registrador Lambda, que se utiliza para escribir un mensaje en CloudWatchLogs.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Al invocar el método handleRequest , obtenga el atributo &quot;newState&quot; del mensaje de suscripción de evento, que representa el estado actualizado del recurso.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Para obtener más información sobre el nuevo formato State, consulte [Formato de mensaje de salida para suscripciones de evento](../../wf-api/api/message-format-event-subs.md).

3. Después de analizar el mapa &quot;newState&quot; del mensaje, asegúrese de que el ID de grupo del objeto coincide con el ID de grupo que identificó en el paso 1.

4. (Condicional) Si los ID **no** coincide, suelte el mensaje para que se devuelva una respuesta vacía.

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
   >Devolver una respuesta vacía y exitosa es crucial. Cualquier cosa que no sea una respuesta de 200 niveles se considera un envío fallido.

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

   El SDK de AWS se utiliza para invocar a otro Lambda, responsable de enviar el mensaje filtrado a nuestro punto final deseado.

   El propósito de pasar la responsabilidad de enviar el mensaje a otra Lambda es evitar un tiempo de espera de la solicitud de envío proveniente del servicio de suscripción de eventos. Actualmente, el tiempo de espera permitido para la entrega se establece en cinco segundos. Si el filtro tarda más de lo permitido por la configuración, puede procesar la solicitud, pero el servicio de suscripción de evento agotará el tiempo de espera y caerá en un bucle de reintentos hasta que reciba una respuesta de 200 niveles dentro del periodo de espera.

   Para obtener más información sobre la administración de la entrega de mensajes, consulte [Mejora del envío de mensajes al aceptar tiempos de espera](#improving-message-delivery-while-accommodating-timeouts).

### Python

La principal diferencia entre los ejemplos de Java y Python es que en el ejemplo de Java el mensaje de suscripción de evento se recibe como el primer parámetro, y en el ejemplo de Python el primer parámetro es un &quot;evento&quot; de proxy Lambda, que contiene el mensaje de suscripción de evento junto con información sobre la solicitud de proxy de AWS Lambda.

El siguiente ejemplo de Python muestra cómo filtrar las cargas del proyecto en función del ID de grupo del proyecto, tal como se hace en  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Establezca el ID de grupo que está buscando y créelo como una constante estática.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   El primer parámetro es el &quot;evento&quot; del proxy Lambda, que contiene el mensaje de suscripción de evento y alguna información adicional que debe analizarse.\
   El segundo parámetro es el contexto de la solicitud de proxy Lambda actual.\
   En este ejemplo, el objeto Context se utiliza para obtener un registrador Lambda, que se utiliza para escribir un mensaje en CloudWatchLogs.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Analice el mensaje desde el evento.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Obtenga el atributo &quot;newState&quot; del mensaje de suscripción de evento.\
   El atributo newState representa el estado actualizado del recurso.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Para obtener más información sobre el nuevo formato State, consulte [Formato de mensaje de salida para suscripciones de evento](../../wf-api/api/message-format-event-subs.md).

1. Después de analizar el mapa &quot;newState&quot; del mensaje, asegúrese de que el ID de grupo del objeto coincide con el ID de grupo que identificó en el paso 1.

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
   >Devolver una respuesta vacía y exitosa es crucial. Cualquier cosa que no sea una respuesta de 200 niveles se considera un envío fallido.

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

   El SDK de AWS se utiliza para invocar a otro Lambda, responsable de enviar el mensaje filtrado a nuestro punto final deseado.

   El propósito de pasar la responsabilidad de enviar el mensaje a otra Lambda es evitar un tiempo de espera de la solicitud de envío proveniente del servicio de suscripción de eventos. Actualmente, el tiempo de espera para la entrega se establece en cinco segundos. Si el filtro tarda más de lo permitido por la configuración, puede procesar la solicitud, pero el servicio de suscripción de evento agotará el tiempo de espera y caerá en un bucle de reintentos hasta que reciba una respuesta de 200 niveles dentro del periodo de espera.


### Node.js

El ejemplo Node.js del filtrado de ID de grupo de proyectos es similar a los ejemplos de Java y Python. Como en el ejemplo de Python, el primer parámetro es un evento proxy de Lambda y el segundo parámetro es el contexto de Lambda.

El siguiente ejemplo en Node.js muestra cómo filtrar las cargas del proyecto en función del ID de grupo del proyecto, tal como se hace en  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Establezca el ID de grupo que está buscando y créelo como una constante estática.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   El primer parámetro es el &quot;evento&quot; del proxy Lambda, que contiene el mensaje de suscripción de evento y alguna información adicional que debe analizarse.\
   El segundo parámetro es el contexto de la solicitud de proxy Lambda actual.\
   En este ejemplo, el objeto Context se utiliza para obtener un registrador Lambda, que se utiliza para escribir un mensaje en CloudWatchLogs.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Analice el mensaje desde el evento.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Obtenga el projectGroupID del atributo &quot;newState&quot; del mensaje de suscripción de evento y, a continuación, haga coincidir con el ID de grupo del grupo que identificó en el paso 1.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Para obtener más información sobre el nuevo formato State, consulte [Formato de mensaje de salida para suscripciones de evento](../../wf-api/api/message-format-event-subs.md).

4. (Condicional) Si los ID no coinciden, suelte el mensaje para que se devuelva una respuesta vacía.\
   El siguiente ejemplo muestra ID de grupo coincidentes:

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
   >Devolver una respuesta vacía y exitosa es crucial. Cualquier cosa que no sea una respuesta de 200 niveles se considera un envío fallido.

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

   El SDK de AWS se utiliza para invocar a otro Lambda, responsable de enviar el mensaje filtrado a nuestro punto final deseado.\
   El propósito de pasar la responsabilidad de enviar el mensaje a otra Lambda es evitar un tiempo de espera de la solicitud de envío proveniente del servicio de suscripción de eventos. Actualmente, el tiempo de espera para la entrega se establece en cinco segundos. Si el filtro tarda más de lo permitido por la configuración, puede procesar la solicitud, pero el servicio de suscripción de evento agotará el tiempo de espera y caerá en un bucle de reintentos hasta que reciba una respuesta de 200 niveles dentro del periodo de espera.\
   Para obtener más información sobre la administración de la entrega de mensajes, consulte [Mejora del envío de mensajes al aceptar tiempos de espera](#improving-message-delivery-while-accommodating-timeouts).

## Mejora del envío de mensajes al aceptar tiempos de espera

El servicio de suscripción de eventos tiene un tiempo de espera estricto **cinco segundos** para todas las solicitudes de envío. En el caso de que el envío de un mensaje supere el tiempo permitido, el servicio de suscripción de evento inicia un ciclo de reintentos para ese mensaje.

Por ejemplo, se crea un filtro de ID de grupo de proyectos similar a uno de los ejemplos encontrados en [Filtrado de mensajes de eventos](#filtering-event-messages) e incluye una búsqueda en la base de datos para determinar si el mensaje es necesario. Es posible que la búsqueda de la base de datos junto con el tiempo necesario para el procesamiento necesario y para que Lambda se inicie en frío puedan tardar más de cinco segundos, lo que provoca que el servicio de suscripción de eventos vuelva a intentar enviar el mensaje.

Puede evitar un reintento si separa las partes del proceso que requieren mucho tiempo de la lógica responsable de determinar si el mensaje es uno que desea procesar y enviar. Al hacerlo, puede aceptar el mensaje y enviar una respuesta de 200 niveles al servicio de suscripción de eventos, mientras continúa procesando o filtrando el mensaje en segundo plano de forma asíncrona (consulte el paso 5 de [Java](#java) por ejemplo).


Aunque el procesamiento o filtrado no supere el tiempo de espera de cinco segundos, sigue siendo conveniente separar el primer punto de contacto de filtrado o procesamiento de mensajes de los demás pasos de procesamiento o envío del lado del cliente. De este modo, el envío del mensaje al destino desde el servicio de suscripción de evento tiene un impacto mínimo en el tiempo y el rendimiento para ambas partes.

Para obtener más información sobre el mecanismo de reintento, consulte [Reintentos de suscripción de eventos](../../wf-api/api/event-sub-retries.md).

## Implementación de filtros alojados en una arquitectura sin nube

Si no puede aprovechar una arquitectura de nube para el filtrado de suscripciones de eventos, puede seguir utilizando los ejemplos de [Filtrado de mensajes de eventos](#filtering-event-messages) como hojas de ruta sobre cómo implementar sus propios filtros alojados o componentes de procesamiento.

### Ajuste de ejemplos de filtrado para servicios independientes

Antes de utilizar los ejemplos de filtrado en un entorno sin nube, haga lo siguiente:

* Omita los fragmentos de los ejemplos específicos de Lambda, como el parámetro Context .

* Cambie las invocaciones de otros Lambdas en los ejemplos a realizar solicitudes HTTP asincrónicas adicionales a otros filtros o componentes de procesamiento que aloje.

* Si hace referencia a los ejemplos de Python y Node.js, sustituya el primer parámetro de evento por el primer parámetro de carga útil mostrado en el ejemplo de Java. Consulte el paso 1 de [Java](#java).

* Implementar los filtros o procesadores con una API basada en web.

### Prevención de mensajes de suscripción de eventos perdidos

En ocasiones, en una arquitectura sin color, es posible que los servicios responsables de la recepción de mensajes de suscripción de eventos no estén disponibles. En un evento de este tipo, los mensajes pueden superar el límite de reintentos y perderse, sin necesidad de recuperar la información dentro de los mensajes.

Le recomendamos que, durante el inicio del servicio, implemente una consulta en la que se solicite el estado más reciente de todos los recursos que podrían haberse incluido en los mensajes perdidos. Como se muestra en el siguiente ejemplo, puede usar los criterios de filtro para consultar los recursos que coincidan con ese criterio y luego procesar su estado actual.

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v9.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
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

Al consultar los recursos, se asegura de que los sistemas integradores tengan la versión más actual de los recursos.

### Implementación del procesamiento asincrónico en la entrega de mensajes

Todos los ejemplos de la sección [Filtrado de mensajes de eventos](#filtering-event-messages) pasa la responsabilidad de enviar mensajes filtrados a otra Lambda de AWS. Esto se hace para evitar superar el tiempo de espera de cinco segundos en la solicitud de entrega, que es reforzado por el servicio de suscripción de eventos que emite la solicitud.

En una arquitectura sin color, es posible que necesite implementar un mecanismo de procesamiento asincrónico similar a como el SDK de AWS permite las llamadas asincrónicas a otros Lambdas de AWS. La mayoría de los lenguajes de programación modernos tienen bibliotecas principales o de terceros que administran el procesamiento asincrónico, lo que le permite aprovechar el estilo asíncrono de procesamiento implementado en nuestros ejemplos.
