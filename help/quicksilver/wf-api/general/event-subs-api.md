---
content-type: api
navigation-topic: general-api
title: API de suscripción de evento
description: API de suscripción de evento
author: John
feature: Workfront API
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c52f1839d3d00c71c6d567084dafd586d161d8fb
workflow-type: tm+mt
source-wordcount: '2203'
ht-degree: 3%

---


# API de suscripción de evento

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Cuando se produce una acción en un objeto de Adobe Workfront compatible con suscripciones de eventos, se puede configurar Workfront para que envíe una respuesta al extremo deseado. Esto significa que las aplicaciones de terceros pueden recibir actualizaciones de las interacciones de Workfront a través de la API de Workfront poco después de que se produzcan. En general, se espera recibir notificaciones de enlace web en menos de 5 segundos desde que se registró el cambio de datos. De media, los clientes reciben notificaciones de weblinks en menos de 1 segundo desde que se registra el cambio de datos.  

Para recibir cargas útiles de suscripciones de eventos a través del cortafuegos, debe añadir las siguientes direcciones IP a la lista de permitidos:

**Para clientes de Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Para clientes en ubicaciones distintas de Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

Los siguientes temas admiten la API de suscripción de evento:

## Objetos admitidos por las suscripciones de eventos

Los siguientes objetos de Workfront son compatibles con las suscripciones de eventos.

* Asignación
* Compañía
* Panel
* Documento
* Gasto
* Hora
* Problema
* Nota
* Portafolio
* Programar
* Proyecto
* Informe
* Tarea
* Plantilla
* Hoja de horas
* Usuario

Para obtener una lista de los campos admitidos por los objetos de suscripción de eventos, consulte [Campos de recurso de suscripción de evento](../../wf-api/api/event-sub-resource-fields.md).

## Autenticación de suscripción de evento

Para crear, consultar o eliminar una suscripción de evento, el usuario de Workfront necesita lo siguiente:

* Un nivel de acceso de &quot;Administrador del sistema&quot;
* Una apiKey

   >[!NOTE]
   >
   >Si el usuario ya está utilizando la API de Workfront, el usuario debería disponer de una apiKey. Puede recuperar la apiKey a través de la siguiente solicitud HTTP:

**URL de solicitud:**

```
PUT https://<HOSTNAME>/attask/api/v7.0/USER?action=getApiKey&username=<USERNAME>&password=<PASSWORD>
```

**Solicitar encabezados:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor de encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Content-type</p> </td> 
   <td> <p>text/html</p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de respuesta:**

| Código de respuesta | Descripción |
|---|---|
| 200 (Aceptar) | La solicitud se procesó correctamente y la apiKey existente para el usuario debe devolverse en el cuerpo de la respuesta. |
| 401 (No autorizado) | El servidor reconoce la solicitud, pero no pudo procesarla porque la apiKey/usuario solicitante no tiene acceso para realizar esta solicitud. |

{style=&quot;table-layout:auto&quot;}

**Ejemplo de cuerpo de respuesta:**

```
{
               "data"{
               "result": "rekxqndrw9783j4v79yhdsakl56bu1jn"
               }
      }
```

>[!NOTE]
>
> Si es la primera vez que utiliza la API de Workfront, debe generar una apiKey que puede hacer a través de este vínculo:


```
PUT https://<HOSTNAME>/attask/api/v7.0/USER/generateApiKey?username=<USERNAME>&password=<PASSWORD>
```

## Formación del recurso de suscripción

El recurso de suscripción contiene los siguientes campos.

* objId (opcional)

   * **Cadena** : ID del objeto del objCode especificado para el que se activan eventos. Si no se especifica este campo, el usuario recibe eventos para todos los objetos del tipo especificado.

* objCode (obligatorio)

   * **Cadena** - El objCode del objeto que se va a suscribir a los cambios. Los valores posibles de objCode se enumeran en la siguiente tabla.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>Objeto</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">Asignación</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Compañía </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Panel</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Documento</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Gasto</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Hora</p></td> 
        <td scope="col">HOUR</td> 
       </tr> 
       <tr> 
        <td scope="col">Problema</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Nota</td> 
        <td scope="col">NOTA</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Portafolio</p></td> 
        <td scope="col"><p>PUERTO</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Programar</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Proyecto</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Informe</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Tarea</p></td> 
        <td scope="col"><p>TAREA</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Plantilla</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Hoja de horas</td> 
        <td scope="col">HOJA</td> 
       </tr> 
       <tr> 
        <td scope="col">Usuario</td> 
        <td scope="col">USUARIO</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (requerido)

   * **Cadena** - Un valor que representa el tipo de evento al que está suscrito el objeto. Los tipos de evento disponibles incluyen:

      * CREAR
      * ELIMINAR 
      * ACTUALIZAR

* url (obligatorio)

   * **Cadena** - La dirección URL del extremo al que se envían las cargas del evento de suscripción mediante HTTP.

* authToken (requerido)

   * **Cadena** - El token al portador de OAuth2 utilizado para autenticarse con la URL especificada en el campo &quot;URL&quot;. 

## Creación de solicitudes de API de suscripción de evento

Después de asegurarse de que el usuario tiene acceso de administrador y de que forma el recurso de suscripción, está listo para crear suscripciones de eventos.

Utilice la siguiente sintaxis para construir la URL.

**URL de solicitud:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Solicitar encabezados:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor de encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorización</p> </td> 
   <td> <p>valor apiKey</p> </td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo del cuerpo de la solicitud:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

| Código de respuesta | Descripción |
|---|---|
| 201 (Creado) | La suscripción al evento se creó correctamente. |
| 400 (solicitud incorrecta) | El campo URL del recurso de suscripción se consideró no válido. |
| 401 (No autorizado) | La apiKey proporcionada estaba vacía o se consideró no válida. |
| 403 (Prohibido) | El usuario, que coincide con la apiKey proporcionada, no tiene acceso de administrador. |

Al pasar un recurso de suscripción como el cuerpo de una solicitud (siendo el tipo de contenido &quot;application/json&quot;), se crea una suscripción de evento para el objeto especificado. Un código de respuesta de 201 (Creado) indica que se creó la suscripción. Un código de respuesta distinto de 201 significa que la suscripción era **NOT** creada.

>[!NOTE]
 El encabezado de respuesta &quot;Ubicación&quot; contiene el URI de la suscripción de evento recién creada.

**Ejemplo de encabezados de respuesta:**

| Encabezados de respuesta | Ejemplo |
|---|---|
| Content-Length | `→0` |
| Fecha | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Ubicación | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Servidor | `→Apache-Coyote/1.1` |

## Consulta de suscripciones de eventos

Al consultar HTTP de Workfront, utilice el método de GET . Existen dos formas de consultar las suscripciones a eventos: Consulte por ID de suscripción (consulte a continuación) o consulte todas las suscripciones de eventos.

### Consultar Todas Las Suscripciones De Eventos

Puede consultar todas las suscripciones de eventos de un cliente según se especifica en el valor apiKey . También puede utilizar las siguientes opciones para administrar la respuesta:

* **página**: parámetro de consulta para especificar el número de páginas que se van a devolver. El valor predeterminado es 1.
* **límite**: parámetro de consulta para especificar el número de resultados que se van a devolver por página. El valor predeterminado es 100 con un máximo de 1000.

La sintaxis de la solicitud para listar todas las suscripciones de eventos para un cliente específico es la siguiente:

**URL de solicitud:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Solicitar encabezados:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor de encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Autorización</p> </td> 
   <td> <p>valor apiKey</p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de respuesta:**

| Código de respuesta | Descripción |
|---|---|
| 200 (Aceptar) | La solicitud se devolvió con todas las suscripciones de eventos encontradas para el cliente que coincidían con la apiKey proporcionada. |
| 401 (No autorizado) | La apiKey proporcionada estaba vacía. |
| 403 (Prohibido) | El usuario, que coincide con la apiKey proporcionada, no tiene acceso de administrador. |


**Ejemplo de encabezados de respuesta:**

| Encabezado de respuesta | Ejemplo |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Fecha | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Servidor | `→Apache-Coyote/1.1` |
| Transferir-Codificación | `→chunked` |


**Ejemplo de cuerpo de respuesta:**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

Donde

* **página** y **límite** son los valores proporcionados en la solicitud o el valor predeterminado si no se proporcionan valores
* **page_count** es el número total de páginas que se pueden consultar.
* **total_count** es el número total de suscripciones que coinciden con la consulta.

### Consulta por ID de suscripción de evento

Puede consultar las suscripciones de eventos según el ID de la suscripción del evento. La sintaxis de la solicitud para listar suscripciones de eventos es la siguiente:

**URL de solicitud:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Solicitar encabezados:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor de encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Autorización</p> </td> 
   <td> <p>valor apiKey</p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de respuesta:**

| Código de respuesta | Descripción |
|---|---|
| 200 (Aceptar) | La solicitud se devolvió con la suscripción de evento que coincide con el ID de suscripción proporcionado. |
| 401 (No autorizado) | La apiKey proporcionada estaba vacía. |
| 403 (Prohibido) | El usuario, que coincide con la apiKey proporcionada, no tiene acceso de administrador. |


**Ejemplo de cuerpo de respuesta:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## Filtro de suscripción de evento

El filtrado de suscripciones de eventos se puede utilizar para garantizar que solo reciba mensajes relevantes. La creación de filtros para las suscripciones puede reducir significativamente el número de mensajes que el punto final debe consumir.

Por ejemplo, un **ACTUALIZACIÓN: TAREA** la suscripción de evento solo se puede establecer en déclencheur cuando la variable **newState** de una carga útil de evento define el **taskStatus** como **current**.

>[!IMPORTANT]
Los siguientes atributos se aplican al filtrado de suscripciones de eventos

* Cuando un campo de filtro tiene un valor no vacío, solo mensajes con un **newState** que contienen las claves y los valores del filtro se envían a la dirección URL suscrita
* Puede filtrar por los datos personalizados incluidos en la variable **newState** Y/O **oldState** del objeto
* Los filtros se evalúan únicamente si son iguales o no a un valor específico
* Si la sintaxis del filtro es incorrecta o no coincide con ningún dato contenido en la variable **newState** de la carga útil, no se devolverá un mensaje de validación para indicar que se ha producido un error
* Los filtros no se pueden actualizar en una suscripción que existe actualmente; se debe crear una nueva suscripción con nuevos parámetros de filtro.
* Se pueden aplicar varios filtros a una sola suscripción y la suscripción solo se entregará cuando se hayan cumplido todas las condiciones de filtro.
* La aplicación de varios filtros a una sola suscripción es una práctica equivalente al uso de una **Y** operador lógico.
* Se pueden aplicar varias suscripciones de eventos a un único objeto siempre que uno o más parámetros de campo de suscripción de eventos sean diferentes entre cada suscripción de evento.
* Cuando se asignan varias suscripciones de eventos a un único objeto, todas las suscripciones de eventos asociadas a ese objeto se pueden devolver a un único extremo. Esta práctica puede utilizarse como sustituto equivalente del operador lógico **O** que no se puede configurar utilizando parámetros de filtro.

### Uso de operadores de comparación

Puede especificar un campo de comparación junto con el campo de filtro. Utilice un operador de comparación en este campo a para filtrar para obtener resultados comparativos. Por ejemplo, puede crear una suscripción UPDATE - TASK que solo envíe una carga útil si el estado de la tarea NO es igual a la actual. Puede utilizar los siguientes operadores de comparación:

#### eq: equal

Este filtro permite que los mensajes surjan si el cambio que se ha producido coincide con `fieldValue` en el filtro exactamente. La variable `fieldValue` distingue entre mayúsculas y minúsculas.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne: not equal

Este filtro permite que los mensajes surjan si el cambio que se ha producido no coincide con `fieldValue` en el filtro exactamente. La variable `fieldValue` distingue entre mayúsculas y minúsculas.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt: bueno que

Este filtro permite que los mensajes surjan si la actualización del `fieldName` es bueno que el valor de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### get: bueno que o igual a

Este filtro permite que los mensajes surjan si la actualización del `fieldName` es bueno o igual al valor de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt: menor que

Este filtro permite que los mensajes surjan si la actualización del `fieldName` es menor que el valor de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte: menor o igual que

Este filtro permite que los mensajes surjan si la actualización del `fieldName` es menor o igual que el valor de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### contiene

Este filtro permite que los mensajes se transmitan si el cambio que se ha producido contiene la variable `fieldValue` en el filtro . La variable `fieldValue` distingue entre mayúsculas y minúsculas.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### cambiar

Este filtro permite que los mensajes surjan solo si el campo especificado (`fieldName`) tiene un valor diferente en oldstate y newstate. Actualización de otros campos además del especificado (`fieldName`) no devolverá ese cambio.

>[!NOTE]
`fieldValue` en la matriz de filtros siguiente no tiene ningún efecto.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### state

Este conector hace que el filtro se aplique al nuevo estado o al estado antiguo del objeto creado o actualizado. Esto es útil cuando desea saber dónde se realizó un cambio de algo a otro.
`oldState` no es posible en CREATE `eventTypes`.

>[!NOTE]
La suscripción siguiente con el filtro dado solo devuelve mensajes donde el nombre de la tarea contiene `again` en el `oldState`, lo que era antes de que se actualizara la tarea.
Un caso de uso para esto sería encontrar los mensajes objCode que han cambiado de una cosa a otra. Por ejemplo, para averiguar todas las tareas que cambiaron de &quot;Buscar un nombre&quot; a &quot;Nombre del equipo de investigación&quot;.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### Uso de campos de conector

La variable `filterConnector` en la carga útil de suscripción le permite elegir cómo se deben aplicar los filtros. El valor predeterminado es &quot;AND&quot;, donde todos los filtros deben estar `true` para que aparezca el mensaje de suscripción. Si se especifica &quot;OR&quot;, solo debe coincidir un filtro para que llegue el mensaje de suscripción.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## Eliminación de suscripciones de eventos

Al eliminar HTTP de Workfront, utilice el método de DELETE . La sintaxis de la solicitud para eliminar una suscripción de evento único por ID de suscripción es la siguiente:

**URL de solicitud:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Solicitar encabezados:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor de encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Autorización</p> </td> 
   <td> <p> apiKey del usuario </p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de respuesta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Código de respuesta</p> </th> 
   <th> Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (sin contenido)</td> 
   <td>El servidor eliminó correctamente la suscripción de evento que coincidía con el subscriptionID proporcionado.</td> 
  </tr> 
  <tr> 
   <td>401 (No autorizado)</td> 
   <td>La apiKey proporcionada estaba vacía.</td> 
  </tr> 
  <tr> 
   <td>403 (Prohibido)</td> 
   <td>El usuario que coincide con la apiKey proporcionada no tiene acceso de administrador.</td> 
  </tr> 
  <tr> 
   <td>404 (No encontrado)</td> 
   <td>El servidor no pudo encontrar una suscripción de evento que coincida con el subscriptionID proporcionado para la eliminación.</td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo de encabezados de respuesta:**

| Encabezado de respuesta | Ejemplo |
|---|---|
| Fecha | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Servidor | `→Apache-Coyote/1.1` |


**Ejemplo de cuerpo de respuesta:** N/D

## Ejemplos de cargas de eventos

La carga útil que recibe un usuario varía en función del tipo de objeto, pero hay un formato coherente para el que se envían las diferentes cargas útiles.

Por ejemplo, las siguientes propiedades se mantienen coherentes en todas las cargas de eventos:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Aunque es coherente en el formato , los valores contenidos en las propiedades varían entre los distintos objetos y tipos de objetos.

A continuación se muestran ejemplos de cargas útiles para un evento UPDATE y un evento CREATE. Observe en el ejemplo UPDATE que los objetos oldState y newState son los mismos, mientras que en el ejemplo CREATE el objeto oldState está vacío (no es NULL).

A continuación se muestra un ejemplo de carga útil para un evento UPDATE:

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

A continuación se muestra un ejemplo de carga útil para un evento CREATE :

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Codificación base 64

Si se rechaza una suscripción de evento debido a un conflicto entre los caracteres especiales contenidos en las suscripciones de evento y la configuración de red, puede utilizar la codificación Base64 para pasar las suscripciones de evento. Base64 es un conjunto de esquemas de codificación que pueden traducir cualquier dato arbitrario a un formato de cadena ASCII. Es importante tener en cuenta que Base64 no es una forma de cifrado de seguridad.

### Campo de codificación base 64

El campo base64Encoding es un campo opcional que se utiliza para habilitar la codificación Base64 de las cargas de suscripción de eventos. El valor predeterminado es false y los valores posibles son: true, false y &quot;&quot; (en blanco).

### Ejemplo de una solicitud utilizando el campo base64Encoding

Si se realiza una solicitud utilizando el campo base64Encoding establecido en true, la variable **newState** y **oldState** Los objetos de la carga útil se envían como cadenas de codificación base 64. Si el campo base64Encoding se define como false, se deja en blanco o no se incluye en la solicitud, la carga útil devuelta no se codificará en base 64.

El siguiente es un ejemplo de solicitud que utiliza el campo base64Encoding :

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### Ejemplos de cargas de respuesta en la codificación base 64

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Método obsoleto para consultar todas las suscripciones de eventos

El siguiente extremo de API está obsoleto y no debe usarse para nuevas implementaciones. También se recomienda migrar las implementaciones antiguas al método en la variable **Consulta de suscripciones de eventos** descrita anteriormente.

Puede consultar todas las suscripciones de eventos de un cliente según se especifica en el valor apiKey . La sintaxis de la solicitud para listar todas las suscripciones de eventos para un cliente específico es la siguiente URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Solicitar encabezados:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor de encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Autorización</p> </td> 
   <td> <p> apiKey del usuario </p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de respuesta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Código de respuesta</p> </th> 
   <th> Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (sin contenido)</td> 
   <td>La solicitud devolvió correctamente todas las suscripciones de eventos encontradas para el usuario.</td> 
  </tr> 
  <tr> 
   <td>401 (No autorizado)</td> 
   <td>La apiKey proporcionada estaba vacía.</td> 
  </tr> 
  <tr> 
   <td>403 (Prohibido)</td> 
   <td>El usuario que coincide con la apiKey proporcionada no tiene acceso de administrador.</td> 
  </tr> 
 </tbody> 
</table>

 

### Ejemplo de cuerpo de respuesta

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
