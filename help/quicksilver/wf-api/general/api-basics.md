---
content-type: api
navigation-topic: general-api
title: Conceptos básicos de API
description: Conceptos básicos de API
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 319c45bc6617269f358af1e7b5f6132a8694710b
workflow-type: tm+mt
source-wordcount: '4396'
ht-degree: 98%

---


# Conceptos básicos de API

La meta de la API de Adobe Workfront es simplificar la creación de integraciones con Workfront mediante la introducción de una arquitectura REST-ful que funcione a través de HTTP. En este documento se da por hecho que está familiarizado con las respuestas de REST y JSON, y se describe el método que utiliza la API de Workfront.

Ser conocedor del esquema de Workfront le ayudará a comprender las relaciones de la base de datos que se pueden utilizar para extraer datos de Workfront con fines de integración.

## Límites y directrices

Para garantizar un rendimiento coherente del sistema bajo demanda de Workfront, la API de Workfront limita los subprocesos simultáneos de la API. Este mecanismo de protección evita problemas del sistema causados por llamadas a la API abusivas. El entorno de zona protegida tiene el mismo límite de subprocesos simultáneos de la API, lo que permite a los clientes y socios probar las llamadas a la API con precisión antes de lanzar un código a producción.

Para entornos de producción, previsualización y pruebas de unidades, las solicitudes de los usuarios finales tienen una longitud del URI máxima de 8892 bytes, ya que se enrutan a través de la CDN de Workfront (Akamai). Este límite solo se aplica a los URI que se enrutan a través de la CDN.

### Descargo de responsabilidad

Cualquier uso de la API debe probarse en un entorno beta de Workfront antes de ejecutarse en el entorno de producción. Si algún cliente utiliza la API para un proceso que Workfront considera razonablemente intenso para el software bajo demanda (es decir, el proceso causa un efecto sustancialmente negativo en el rendimiento del software para otros clientes), Workfront se reserva el derecho de solicitar que el cliente interrumpa ese proceso. Si el cliente no cumple y el problema persiste, Workfront se reserva el derecho de terminar el proceso.

## URL de la API de Workfront

Para obtener más información acerca de la dirección URL que usará para llamar a la API de Workfront, vea [Formato de dominio para llamadas a la API de Adobe Workfront](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## Conceptos básicos de REST

Esta sección proporciona una introducción de alto nivel sobre cómo interactuar con la API de REST de Workfront para los siguientes principios de REST:

### URI de objeto

A cada objeto del sistema se le asigna un URI único que consta del tipo de objeto y el ID. Los siguientes ejemplos muestran algunas URI que describen tres objetos únicos:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

El tipo de objeto no distingue entre mayúsculas y minúsculas y puede ser el ObjCode abreviado (como proj) o el nombre de objeto alternativo (proyecto).

Para obtener una lista de objetos, códigos de objeto válidos y campos de objeto, consulte  [Explorador de API](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>En el contexto de la API de Workfront, un formulario personalizado es un objeto `Category` y un campo personalizado es un objeto `Parameter`.

### Operaciones

Los objetos se manipulan enviando una petición HTTP a su URI único. La operación que se va a realizar se especifica mediante el método HTTP.

Los métodos HTTP estándar corresponden a las siguientes operaciones:

* **GET**: recupera un objeto a través del ID, busca todos los objetos mediante una consulta, ejecuta informes o ejecuta consultas con nombre
* **POST**: inserta un nuevo objeto
* **PUT**: edita un objeto existente
* **DELETE**: elimina un objeto

Para evitar deficiencias de cliente o límites de longitud de protocolo, se puede utilizar el parámetro de método para anular el comportamiento HTTP. Por ejemplo, se puede implementar una operación de GET publicando el siguiente URI:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Respuesta

Cada solicitud recibe una respuesta en formato JSON. La respuesta tiene un atributo de datos si la solicitud se realizó correctamente o un atributo de error si hubo un problema. Por ejemplo, la solicitud

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

devuelve una respuesta JSON similar a la siguiente:


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Brand New Project",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Al ejecutar una petición GET a través de la barra de direcciones del explorador, no es necesario incluir el ID de sesión como parte de la solicitud.

Se ha añadido seguridad especial en torno a las peticiones PUT, POST y DELETE. Cualquier solicitud que resulte de la escritura o eliminación en la base de datos solo se puede ejecutar si **sessionID=abc123** está incluido en el URI. Los siguientes ejemplos muestran el aspecto que tendría esto para una petición DELETE:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Autenticación

La API autentica todas las solicitudes para garantizar que el cliente tenga acceso para ver o modificar el objeto solicitado.

La autenticación se realiza pasando un ID de sesión, el cual se puede proporcionar mediante uno de los métodos siguientes:

#### Autenticación del encabezado de la solicitud

El método de autenticación preferido es pasar un encabezado de solicitud denominado SessionID que contenga el token de sesión. Esto tiene la ventaja de estar protegido contra ataques de [falsificación de solicitud en sitios múltiples (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) y de no interferir con el URI con fines de almacenamiento en caché.

A continuación se muestra un ejemplo de encabezado de solicitud:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Autenticación basada en cookies

La API utiliza la misma autenticación basada en cookies que la IU web utiliza el sistema. En el que, si un cliente inicia sesión en Workfront mediante la interfaz de usuario web, cualquier llamada AJAX realizada desde el mismo explorador utiliza la misma autenticación.

>[!NOTE]
>
>Para protegerse contra la posibilidad de ataques CSRF (falsificación de solicitud en sitios múltiples), este método de autenticación solo está disponible para operaciones de solo lectura.

## Inicio de sesión

>[!IMPORTANT]
>
>Workfront ya no recomienda el uso del punto final ni de las claves API `/login`. En lugar de ello, utilice uno de los siguientes métodos de autenticación:
>
>* Autenticación de servidor con JWT
>* Autenticación de usuario con OAuth2
>
>Para obtener instrucciones sobre cómo configurar estos métodos de autenticación, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Para obtener instrucciones sobre el uso de la autenticación de servidor en Workfront, consulte [Configuración y uso de las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo JWT](../../wf-api/api/oauth-app-jwt-flow.md)
>
>Para obtener instrucciones sobre el uso de la autenticación de usuarios en Workfront, consulte [Configuración y uso de las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo del código de autorización](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
>El procedimiento descrito en esta sección se aplica solo a las organizaciones que todavía no se han incorporado a Adobe Business Platform. El inicio de sesión en Workfront a través de la API de Workfront no está disponible si su organización se ha incorporado a Adobe Business Platform.
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Business Platform o no, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Si utiliza un nombre de usuario y una contraseña válidos, puede utilizar la siguiente solicitud para obtener un ID de sesión:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Esto establece una cookie para autenticar solicitudes futuras, así como para devolver una respuesta JSON con el ID de sesión recién creado, el ID de usuario del usuario que ha iniciado sesión y otros atributos de sesión.

>[!NOTE]
>
>Si tiene un usuario de API designado que también sea administrador, Workfront le recomienda encarecidamente que utilice una clave de API para iniciar sesión.

**Generación de una clave de API**

Puede generar una clave de API al iniciar sesión en el sistema como ese usuario, tal como se muestra en el siguiente ejemplo:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Recuperación de una clave de API generada anteriormente**

También puede recuperar una clave de API que se haya generado anteriormente para un usuario en particular ejecutando getApiKey:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Puede utilizar este resultado para autenticar cualquier llamada de API añadiendo &quot;apiKey&quot; como el parámetro de solicitud con este valor en lugar de un ID de sesión o un nombre de usuario y contraseña. Esto es beneficioso desde el punto de vista de la seguridad.

La siguiente solicitud es un ejemplo de recuperación de datos de un proyecto mediante apiKey:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalidar una clave de API**

Si el valor de apiKey se ha visto comprometido, puede ejecutar &quot;clearApiKey&quot; para invalidar la clave de API actual, tal como se muestra en el siguiente ejemplo:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Una vez borrada, puede volver a ejecutar getApiKey para generar una nueva clave de API.

### Cerrar sesión

Cuando finaliza una sesión, puede utilizar la siguiente solicitud para cerrar la sesión del usuario, lo cual impide que se siga accediendo con el ID de sesión.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

El ID de sesión que se va a cerrar se puede especificar como cookie, encabezado de solicitud o parámetro de solicitud.

Para cerrar la sesión de un usuario:

1. Vaya a la pantalla de inicio de sesión, pero no inicie la sesión.
1. Cambie la dirección URL a /attask/api/v15.0/project/search.\
   Observe que no se encuentra la página.
1. Reemplace la palabra *search* por login?username=admin&amp;password=user, sustituyendo su nombre de usuario y contraseña por *admin* y *user\
   *Esta sesión se almacena en el explorador como una cookie y no es necesario reiniciarla en cada petición GET posterior.

1. Vuelva a cambiar la dirección URL a **/attask/api/v15.0/project/search**.
1. Observe la respuesta recibida.

Siempre debe incluir el ID de sesión proporcionado después del inicio de sesión al realizar peticiones PUT, POST y DELETE.

## El comportamiento de GET

Utilice el método HTTP GET para recuperar uno o varios objetos y ejecutar informes.

### Recuperación de objetos

Se puede mejorar la búsqueda de objetos mediante modificadores y filtros.

#### Recuperación de un objeto mediante el ID de objeto

Si conoce el ID de un objeto, puede recuperar el objeto accediendo a su URI único. Por ejemplo, la solicitud

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

devuelve una respuesta similar a la siguiente:

<pre>{<br>    "percentComplete": 0,<br>    "estado": "CUR",<br>    "prioridad": 2,<br>    "nombre": "Proyecto completamente nuevo",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


Para recuperar varios objetos en la misma solicitud, especifique el parámetro de solicitud de ID y proporcione una lista de ID separados por comas, como se muestra en el siguiente ejemplo:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Observe que la solicitud /attask/api/v15.0/project?id=... es la misma que la solicitud `/attask/api/v15.0/project/...`.

#### Recuperación de un objeto mediante el URI

Si desea recuperar un objeto mediante criterios distintos al ID, puede buscar el URI.

Por ejemplo, puede utilizar la siguiente solicitud para devolver una lista de todos los proyectos del sistema:

```
GET /attask/api/v15.0/project/search
```

Puede especificar filtros utilizando los parámetros de solicitud como pares de nombre-valor. Por ejemplo, el siguiente ejemplo muestra una solicitud que buscaría todos los proyectos actuales:

```
GET /attask/api/v15.0/project/search?status=CUR
```

La siguiente solicitud encuentra todas las tareas que aún no se han completado y que se han asignado a un usuario llamado John.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Uso de modificadores de búsqueda

En la tabla siguiente se enumeran algunos de los modificadores que puede utilizar con la API de Workfront.

| **Modificador** | **Descripción** | **Ejemplo** |
| --- | --- | --- |
| eq | devuelve los resultados que están en estado de cerrado | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | devuelve resultados que no están en estado de cerrado | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | devuelve resultados con un porcentaje completado mayor o igual que 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=get...</pre> |
| lte | devuelve resultados con un porcentaje completado inferior o igual a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | devuelve resultados donde la descripción es nula | <pre>...description_Mod=isnull...</pre> |
| notnull | devuelve resultados donde la descripción no es nula | <pre>...description_Mod=notnull...</pre> |
| contiene | devuelve resultados donde name contiene &quot;Workfront&quot; | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| entre | devuelve resultados que tienen una fecha de entrada en los últimos 7 días | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>Las solicitudes de búsqueda distinguen entre mayúsculas y minúsculas. Si recibe un error, asegúrese de que  **_Mod** y **_Range** tienen las mayúsculas correctas.

#### Uso de instrucciones OR

Puede mejorar una búsqueda añadiendo un parámetro que incluya &quot;OR&quot;, así como un número, para indicar el nivel de un filtro o una serie de filtros.

Una instrucción OR devuelve únicamente los registros de la llamada a la API que cumplen los criterios de filtrado de la instrucción OR. Los filtros no están implícitos en todos los niveles de instrucción OR.

Por ejemplo, si desea filtrar por

* Tareas con un nombre que contenga “Planificación” OR
* Tareas en un portafolio llamado “FixedAssets” AND asignadas a alguien con un nombre que contenga “Steve” OR
* Tareas que tengan una tarea principal llamada “Tarea final”

a continuación, utilice la siguiente llamada de API con sus diferentes instrucciones OR:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Uso de parámetros de filtro

Un posible inconveniente del uso de parámetros de URL para los filtros de búsqueda es que Workfront analiza ciertos parámetros antes de comprobar si hay diferentes métodos de autenticación (por ejemplo: nombre de usuario, contraseña, apiKey o cookie). Cuando esto suceda, los parámetros no se utilizarán como filtros en la llamada. 

Para evitar este problema, coloque estos valores en parámetros de filtro con formato JSON.  Por ejemplo, si quisiera filtrar por el usuario usuariodeprueba, en lugar de utilizar 
<pre>/attask/api/v15.0/user/search?username=usuariodeprueba@workfront.com</pre>pase el parámetro de URL en un filtro, tal y como se muestra en el siguiente ejemplo:
<pre>/attask/api/v15.0/user/search?filters={"username":"usuariodeprueba@workfront.com"}</pre>

#### Uso del parámetro de solicitud de asignación

De forma predeterminada, los datos devueltos por una búsqueda son una matriz JSON. Según el caso de uso, podría ser más eficaz obtener el resultado como objeto JSON indexado por ID. Esto se puede hacer utilizando el parámetro de solicitud de asignación. Por ejemplo, la solicitud 
<pre>/attask/api/v15.0/task/search?map=true</pre>devuelve una respuesta indexada por ID similar a la siguiente:
<pre>{<br>    "datos": {<br>        "4c9a97db0000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "estado": "NUEVO",<br>            "nombre": "primera tarea",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "estado": "INP:A",<br>            "nombre": "segunda tarea",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Uso del parámetro de solicitud de campos

De forma predeterminada, la recuperación de un objeto devolverá solo el subconjunto de campos más utilizado.

Use el parámetro de solicitud de campos para especificar que se devuelva una lista separada por comas de campos específicos. Por ejemplo, la solicitud
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>devuelve una respuesta similar a la siguiente:
<pre>{<br>    "priority": 2,<br>    "name": "first task",<br>    "ID": "4c7c08fa0000002ff924e298ee148df4",<br>    "plannedStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
>
>Estos nombres de campo distinguen entre mayúsculas y minúsculas.

Para obtener una lista de posibles referencias de campo, consulte la [API Explorer](../../wf-api/general/api-explorer.md)

#### Búsqueda de objetos anidados

Es posible buscar objetos anidados. De forma predeterminada, los objetos anidados solo se devuelven con el nombre y el ID. Por ejemplo, para obtener todos los problemas junto con sus propietarios, utilice la siguiente solicitud:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Si se requiere más información, es posible solicitar un campo anidado mediante la sintaxis de dos puntos. Por ejemplo, la siguiente solicitud busca todos los problemas junto con el nombre, ID, título y número de teléfono del propietario
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>y devuelve lo siguiente: 
<pre>&lbrace;{<br>    "name": "an important issue",<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "owner": {<br>        "title": "Operations Specialist",<br>        "phoneNumber": "555-1234",<br>        "name": "Admin User",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### Recuperación de colecciones anidadas

Es posible recuperar colecciones anidadas de objetos. Por ejemplo, para obtener un proyecto con todas sus tareas, utilice la siguiente solicitud:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>La siguiente solicitud obtiene asignaciones de tareas:
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### Buscar varios campos anidados

De forma predeterminada, solo se devuelve el nombre y el ID de cada tarea, pero se pueden especificar campos anidados adicionales con sintaxis de dos puntos. Para ver todos los campos disponibles para un objeto o colección relacionado, simplemente añada dos puntos y un asterisco a la referencia de objeto o colección.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### Recuperación de datos personalizados

Es posible recuperar campos de datos personalizados con el prefijo “DE:”. Por ejemplo, para solicitar un proyecto con un parámetro llamado “TextoPersonalizado”, utilice la siguiente solicitud:
<pre>/attask/api/v15.0/project/search?fields=DE:TextoPersonalizado</pre>que devolvería
<pre>{<br>    "nombre": "proyecto de datos personalizados",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "tarea b" <br>}</pre>También es posible recuperar todos los datos personalizados de un objeto solicitando el campo parameterValues. Por ejemplo: 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>devolverá datos similares a los siguientes:
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br>}</pre>

#### Uso de consultas con nombre

Algunos tipos de objetos tienen búsquedas con nombre que se ejecutan habitualmente y están disponibles añadiendo el nombre de la consulta al final del URI del tipo de objeto. Por ejemplo, la siguiente solicitud recuperará los elementos de trabajo (tareas y problemas) a los que esté asignado el usuario en ese momento:
<pre>/attask/api/v15.0/work/myWork</pre>Las consultas con nombre admiten la solicitud del parámetro fields para recuperar campos adicionales. Algunas consultas con nombre también aceptan filtros adicionales. Para obtener una lista de las consultas con nombre permitidas para un objeto, consulte la pestaña Acción del objeto en la [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

#### Uso de `Count`

Es posible usar `count` para devolver el número de resultados que coincida con su consulta. Esto resultará útil cuando no se necesiten los datos en los resultados. Al devolver solo el recuento, el servidor podrá procesar la solicitud más rápidamente y ahorrar ancho de banda. Por ejemplo, la solicitud
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>devuelve el número de resultados en el siguiente formato:
<pre>{<br>    "count": 3 <br>}</pre>Devolver un recuento supone una transferencia de datos mucho menor que si se devuelven objetos completos. La sintaxis es idéntica al comando de búsqueda.

### Solicitar un informe

Es posible realizar una solicitud de informe donde solo se desee el acumulado de algún campo con una o más agrupaciones. Tal y como se muestra en el ejemplo siguiente, la sintaxis del informe es la misma que la de la API de SOAP:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>que devuelve el siguiente resultado
<pre>&lbrace;{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>     "Second Project": { <br>        "sum_hours": 30 <br>    } <br>}</pre>Si se añade el parámetro $$ROLLUP=true, se incluirá un total en cada nivel de agrupación:
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>    "Second Project": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### Ordenar los resultados de consulta en la API

Puede ordenar los resultados por cualquier campo si anexa lo siguiente a la llamada de API:

&amp;entryDate_Sort=asc

Por ejemplo, si desea ordenar por fecha de inicio planificada de la tarea, elimine entryDate y reemplácelo por plannedCompletionDate.

Esto funcionará para la mayoría de los campos de Workfront.

### Consideración de límites de consulta

Al consultar objetos, se debe tener especial consideración con respecto a la relación de los objetos relacionados y las limitaciones de búsqueda. Por ejemplo, como se muestra en la tabla siguiente, una consulta de proyectos no puede devolver más de 2000 proyectos. Estos 2000 proyectos se consideran “objetos primarios”. Al consultar el campo Tareas en los proyectos, el campo Tareas, que es una colección, se convertirá en un objeto secundario del objeto principal Proyecto. Una consulta para el campo Tareas puede incluir miles de tareas en proyectos. En total, el número combinado de objetos (proyectos y tareas) devueltos no puede superar el máximo de 50 000.

Para garantizar un rendimiento óptimo, la siguiente tabla muestra las limitaciones impuestas a las solicitudes de búsqueda. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Resultado de consulta</th> 
   <th>Limitación</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Número predeterminado de resultados</td> 
   <td>100</td> 
   <td> Si no se especifica ningún límite en el filtro de consulta (es decir, $$LIMIT), el resultado no podrá contener más de 100 objetos principales. <br>Consulte <a href="#using-paginated-responses" class="MCXref xref">Uso de respuestas paginadas</a> para obtener instrucciones sobre cómo anular esta limitación. </td> 
  </tr> 
  <tr> 
   <td>Número máximo de resultados</td> 
   <td>2.000</td> 
   <td>El filtro de consulta (es decir, $$LIMIT) no puede devolver más de 2000 resultados. Consulte “Respuestas paginadas” para obtener más información.</td> 
  </tr> 
  <tr> 
   <td>Profundidad máxima del campo</td> 
   <td>4</td> 
   <td>Al identificar los campos que se desean mostrar, no es posible alejarse más de cuatro niveles del objeto que se está consultando.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de objetos</td> 
   <td>50.000</td> 
   <td>El conjunto de resultados no puede incluir 50 000 objetos primarios y secundarios.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de campos</td> 
   <td nowrap>1.000.000</td> 
   <td>Cuando el conjunto de resultados es menor de 50 000 objetos, los resultados podrían incluir un máximo de 1 000 000 de campos.</td> 
  </tr> 
  <tr> 
   <td>Número máximo de creaciones/actualizaciones de lotes</td> 
   <td>100</td> 
   <td>El límite máximo de creación o actualización de lotes es de 100.</td> 
  </tr> 
 </tbody> 
</table>

### Uso de respuestas paginadas {#using-paginated-responses}

Para anular la limitación de la consulta Número predeterminado de resultados y permitir 200 resultados, incluya el filtro `$$LIMIT=200` en la consulta, tal y como se muestra en el ejemplo siguiente:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

Para garantizar la fiabilidad y el rendimiento de otros inquilinos del sistema, el límite máximo de resultados permitidos por consulta es de 2000 objetos. Si se intentase especificar un límite mayor, aparecerá un mensaje de error de `IllegalArgumentException`.

Por lo tanto, se recomienda considerar la posibilidad de utilizar respuestas paginadas para conjuntos de datos grandes. Para especificar qué primer resultado se devolverá, añada el filtro `$$FIRST`. Por ejemplo, la siguiente solicitud devuelve los resultados 201-250 de una consulta:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

Observe que en el ejemplo anterior, `$$FIRST=200` devuelve el resultado 201. `$$FIRST=0` devolverá el primer resultado. Puede ser útil considerar el valor $$FIRST como el número de resultados que desea omitir antes de devolver los resultados.

Para asegurarse de que los resultados estén correctamente paginados, utilice un parámetro de ordenación. Esto permite que los resultados se devuelvan en el mismo orden, para que la paginación no se repita ni omita resultados. Por ejemplo, para ordenar usando el identificador de objeto, use `ID_Sort=asc`.

### Creación de una regla de acceso

Puede crear una regla de acceso para determinar quién puede acceder a un objeto. Los siguientes son ejemplos de reglas de acceso que puede establecer:

Para configurar un proyecto de modo que se comparta únicamente con un usuario con el ID “abc123”, utilice la siguiente solicitud:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Como alternativa, para compartir solo con una persona nueva y mantener intactos los permisos existentes:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Para recuperar las reglas de acceso existentes:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## Comportamiento de POST

POST inserta un nuevo objeto. La sintaxis es idéntica a PUT, pero con algunas excepciones. Dado que el nuevo objeto aún no existe, no tiene un ID. Por este motivo, el URI no incluye el ID.

### Creación de un objeto

A continuación se muestra un ejemplo de una solicitud para crear un nuevo proyecto:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>La respuesta incluye el proyecto recién creado junto con su nuevo ID y cualquier otro campo especificado.

### Copia de un objeto

Algunos objetos admiten ser copiados. Para estos tipos de objetos, es posible crear nuevos objetos publicando con un parámetro copySourceID. Por ejemplo, la siguiente solicitud copia el proyecto dado y le asigna un nombre nuevo:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Carga de documentos

Puede cargar documentos a través de la siguiente URL de API:
<pre>POST /attask/api/v15.0/upload</pre>La API espera que el tipo de contenido sea multipart/form-data. El nombre del parámetro para el archivo debe ser uploadFile. El servidor devuelve los siguientes datos JSON:
<pre>{<br>    "handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Puede utilizar el identificador y enviarlo a la siguiente URL al crear un documento de Workfront:
<pre>POST /attask/api/v15.0/document?updates={<br>}    name: aFileName,<br>    handle: abc...123, (identificador de la carga del archivo)<br>    docObjCode: PROJ, (o TAREA, OPTASK, etc.)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br></pre>

## Comportamiento de PUT

PUT se utiliza para actualizar un objeto existente.

La respuesta de PUT es idéntica a GET. En ambos casos, el servidor devuelve el nuevo estado del objeto después de la actualización. Todas las reglas utilizadas para modificar una respuesta a una petición GET también funcionan con PUT, como especificar los campos adicionales que se van a devolver, los datos personalizados, etc.

### Edición de objetos

Las actualizaciones de objetos siempre se realizan mediante el ID. utilizando el URI único del objeto. Los campos que se van a actualizar se especifican como parámetros de solicitud. Por ejemplo, para cambiar el nombre de un proyecto puede enviar una solicitud similar a la siguiente:
<pre>PUT /attask/api/v15.0/project/4c7...?name=Nuevo nombre de proyecto <br>PUT /attask/api/v15.0/project?id=4c7...&amp;name=Nuevo nombre de proyecto</pre>Dado que la actualización requiere un ID, esta operación no se realizará correctamente (sin inserción) si el objeto no existe en el servidor.

### Especificación de ediciones JSON

Como se muestra en el ejemplo siguiente, puede utilizar el parámetro de solicitud de actualizaciones para especificar los campos que se actualizarán con la sintaxis JSON:
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{<br>     name: "New Project Name", <br>     status: "CUR", <br>     ... <br>}</pre>

### Realización de actualizaciones anidadas

Algunos objetos tienen colecciones de propiedad privada que se pueden actualizar. Por ejemplo, en el siguiente ejemplo se muestra cómo sobrescribir las asignaciones existentes de una tarea determinada:
<pre>PUT /attask/api/v15.0/task/4c7...?updates= <br>{<br>    assignments: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent: 50.0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Aunque las actualizaciones realizadas en el nivel superior son dispersas, las actualizaciones de una colección o de un objeto anidado reemplazan por completo a la colección existente. Para editar una única asignación en una tarea sin afectar a los objetos, utilice PUT en la asignación en lugar de en la tarea.

El siguiente ejemplo convierte un proyecto en una cola del servicio de asistencia público. Tenga en cuenta que las propiedades de cola existentes se reemplazan.
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>&lbrace; <br>    queueDef: { <br>        isPublic: 1 <br>    } <br></pre>

### Uso del parámetro de solicitud de acción

Algunos objetos admiten acciones adicionales que se pueden realizar además de ediciones simples. Puede especificar estas acciones mediante el parámetro de solicitud de acción. Por ejemplo, la siguiente solicitud recalcula la cronología de un proyecto determinado:
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>or<br><br>PUT /attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### Mover objetos

A continuación se muestra la sintaxis para mover una tarea de un proyecto a otro:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>Aquí se proporciona un ejemplo para cada tipo de acción: (??)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApprova<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Solo la acción de mover requiere la identificación de atributos adicionales para especificar el proyecto donde se moverá el elemento de trabajo.

A continuación se muestra un ejemplo de cada tipo de acción: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Compartir objetos

En el siguiente ejemplo se muestra la sintaxis para compartir un proyecto con un equipo:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Al editar un objeto, puede reemplazar todas las reglas de acceso de un objeto haciendo PUT y enviando actualizaciones similares al ejemplo siguiente:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>El ejemplo siguiente muestra la sintaxis para mover una tarea de un proyecto a otro:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## Comportamiento de DELETE

DELETE elimina un objeto. En todos los casos, el URI puede incluir el parámetro force=true para que el servidor elimine los datos especificados y sus dependientes. En el ejemplo siguiente, se elimina una tarea ejecutando el método DELETE HTTP en un URI:
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Actualizaciones masivas

Una instrucción de actualización en lote actualiza varios objetos al mismo tiempo dentro de una sola llamada de API. Una llamada de API en lote se crea de forma similar a una llamada de actualización normal, tal como se muestra en los ejemplos siguientes:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>o <pre>PUSH /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>que da como resultado un resultado similar al siguiente:
<pre>data: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    name: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    name: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>}]</pre>También puede realizar una actualización masiva similar a la siguiente:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>que da como resultado un resultado similar al siguiente:
<pre>data: [ {<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     name: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>     priority: 0,<br>     projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    status: "CUR"<br>}]</pre>Si desea que todas las operaciones se realicen en la misma transacción, añada "atomic=true" a la llamada de API por lotes como parámetro de solicitud. De este modo, si alguna de las operaciones falla, todas las operaciones se revierten.

>[!NOTE]
>
>Las operaciones por lotes atómicas solo pueden devolver &quot;success: true&quot; o un error.

