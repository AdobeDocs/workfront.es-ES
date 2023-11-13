---
content-type: api
navigation-topic: general-api
title: API de suscripción de evento
description: API de suscripción de evento
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c08bd3311892d24a9bd40af138169957f5ea2ca4
workflow-type: tm+mt
source-wordcount: '2126'
ht-degree: 4%

---


# API de suscripción de evento

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Cuando se produce una acción en un objeto Adobe Workfront compatible con las suscripciones de evento, puede configurar Workfront para que envíe una respuesta al extremo deseado. Esto significa que las aplicaciones de terceros pueden recibir actualizaciones de las interacciones de Workfront a través de la API de Workfront poco después de que se produzcan. En general, puede esperar recibir notificaciones de ganchos web en menos de 5 segundos desde que se registró el cambio de datos. De media, los clientes reciben notificaciones de ganchos web en menos de 1 segundo desde que se registra el cambio de datos.  

Para recibir cargas útiles de suscripciones de eventos a través del cortafuegos, debe añadir las siguientes direcciones IP a la lista de permitidos:

**Para clientes de Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Para clientes de ubicaciones distintas de Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

Los siguientes temas admiten la API de suscripción a evento:

## Objetos admitidos por suscripciones a eventos

Las suscripciones a eventos admiten los siguientes objetos de Workfront.

* Asignación
* Compañía
* Panel
* Documento
* Gasto
* Campo
* Hora
* Problema
* Nota
* Portafolio
* Programar
* Proyecto
* Registro
* Tipo de registro
* Informe
* Tarea
* Plantilla
* Hoja de horas
* Usuario
* Espacio de trabajo

Para obtener una lista de los campos admitidos por los objetos de suscripción de evento, consulte [Campos de recurso de suscripción de evento](../../wf-api/api/event-sub-resource-fields.md).

## Autenticación de suscripción de evento

Para crear, consultar o eliminar una suscripción de evento, el usuario de Workfront necesita lo siguiente:

* Se requiere un nivel de acceso de &quot;Administrador del sistema&quot; para utilizar Suscripciones de eventos.
* A `sessionID`  se requiere para utilizar la API de suscripciones a eventos

  Para obtener más información, consulte [Autenticación](api-basics.md#authentication) in [Conceptos básicos de API](api-basics.md).

## Formación del recurso de suscripción

El recurso de suscripción contiene los campos siguientes.

* objId (opcional)

   * **Cadena** : ID del objeto del objCode especificado para el que se activan los eventos. Si no se especifica este campo, el usuario recibe eventos para todos los objetos del tipo especificado.

* objCode (obligatorio)

   * **Cadena** - El objCode del objeto al que se está suscribiendo cambia. Los valores posibles de objCode se enumeran en la tabla siguiente.

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
        <td scope="col"><p>ASIGNAR</p></td> 
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
        <td scope="col"><p>Campo</p></td> 
        <td scope="col"><p>CAMPO</p></td> 
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
        <td scope="col"><p>PROYECTO</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Registro</p></td> 
        <td scope="col"><p>REGISTRO</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Tipo de registro</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
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
        <td scope="col">HOJA TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">Usuario</td> 
        <td scope="col">USUARIO</td> 
       </tr> 
       <tr> 
        <td scope="col">Espacio de trabajo</td> 
        <td scope="col">WORKSPACE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (obligatorio)

   * **Cadena** - Un valor que representa el tipo de evento al que está suscrito el objeto. Los tipos de eventos disponibles incluyen:

      * CREAR
      * ELIMINAR 
      * ACTUALIZACIÓN

* url (obligatorio)

   * **Cadena** : URL del punto de conexión al que se envían las cargas de evento de suscripción mediante HTTP.

* authToken (obligatorio)

   * **Cadena** : el token de portador de OAuth2 utilizado para autenticarse con la URL especificada en el campo &quot;URL&quot;. 

## Creación de solicitudes de API de suscripción de evento

Después de asegurarse de que el usuario tiene acceso de administrador y de formar el recurso de suscripción, está listo para crear suscripciones de evento.

Utilice la siguiente sintaxis para construir la dirección URL.

**URL de solicitud:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Encabezados de solicitud:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor del encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valor sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo de cuerpo de solicitud:**

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
| 201 (Creado) | La suscripción al evento se ha creado correctamente. |
| 400 (Solicitud incorrecta) | El campo URL del recurso de suscripción se ha considerado no válido. |
| 401 (No autorizado) | El ID de sesión proporcionado estaba vacío o se consideró no válido. |
| 403 (Prohibido) | El usuario que coincide con el sessionID proporcionado no tiene acceso de administrador. |

Si se pasa un recurso de suscripción como cuerpo de una solicitud (con el tipo de contenido &quot;application/json&quot;), se crea una suscripción de evento para el objeto especificado. Un código de respuesta 201 (Created) indica que se creó la suscripción. Un código de respuesta distinto de 201 significa que la suscripción fue **NO** creado.

>[!NOTE]
>
> El encabezado de respuesta &quot;Ubicación&quot; contiene el URI de la suscripción de evento recién creada.

**Ejemplo de encabezados de respuesta:**

| Encabezados de respuesta | Ejemplo |
|---|---|
| Content-Length | `→0` |
| Fecha | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Ubicación | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Servidor | `→Apache-Coyote/1.1` |

## Consulta de suscripciones a eventos

Al consultar el código HTTP de Workfront, utilice el método de GET. Existen dos formas de consultar suscripciones a eventos: consultar por ID de suscripción (consulte a continuación) o consultar todas las suscripciones a eventos.

### Consultar todas las suscripciones a eventos

Puede consultar todas las suscripciones de eventos de un cliente o utilizar lo siguiente para administrar la respuesta. También puede utilizar las siguientes opciones para administrar la respuesta:

* **página**: opción de parámetro de consulta para especificar el número de páginas que se devolverán. El valor predeterminado es 1.
* **límite**: opción de parámetro de consulta para especificar el número de resultados que se devuelven por página. El valor predeterminado es 100, con un máximo de 1000.

La sintaxis de solicitud para enumerar todas las suscripciones de evento de un cliente específico es la siguiente:

**URL de solicitud:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Encabezados de solicitud:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor del encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valor sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de respuesta:**

| Código de respuesta | Descripción |
|---|---|
| 200 (OK) | Se ha devuelto la solicitud con todas las suscripciones de evento encontradas para el cliente que coinciden con el ID de sesión proporcionado. |
| 401 (No autorizado) | El ID de sesión proporcionado estaba vacío. |
| 403 (Prohibido) | El usuario, que coincide con el sessionID proporcionado, no tiene acceso de administrador. |


**Ejemplo de encabezados de respuesta:**

| Encabezado de respuesta | Ejemplo |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Fecha | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Servidor | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


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

* **página** y **límite** son los valores proporcionados en la solicitud o los predeterminados si no se proporcionan valores
* **page_count** es el número total de páginas que se pueden consultar.
* **total_count** es el número total de suscripciones que coinciden con la consulta.

### Consulta por ID de suscripción de evento

Puede consultar suscripciones a eventos por el ID de suscripción a eventos. La sintaxis de solicitud para enumerar suscripciones de eventos es la siguiente:

**URL de solicitud:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Encabezados de solicitud:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor del encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valor sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de respuesta:**

| Código de respuesta | Descripción |
|---|---|
| 200 (OK) | La solicitud devuelta con la suscripción de evento que coincide con el ID de suscripción proporcionado. |
| 401 (No autorizado) | El ID de sesión proporcionado estaba vacío. |
| 403 (Prohibido) | El usuario, que coincide con el sessionID proporcionado, no tiene acceso de administrador. |


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

## Filtrado de suscripción de eventos

El filtrado de suscripción de eventos se puede utilizar para garantizar que solo recibe mensajes relevantes. La creación de filtros para sus suscripciones puede disminuir significativamente la cantidad de mensajes que debe consumir su punto final.

Por ejemplo, un **ACTUALIZACIÓN - TAREA** la suscripción de evento se puede establecer en déclencheur solo cuando la variable **newState** de una carga útil de evento define la variable **taskStatus** as **corriente**.

>[!IMPORTANT]
>
Los atributos siguientes se aplican al filtrado de suscripción de evento

* Cuando un campo de filtro tiene un valor no vacío, solo se muestran mensajes con **newState** que contiene las claves de filtro y los valores se envían a la dirección URL suscrita
* Puede filtrar por datos personalizados incluidos en la variable **newState** Y/O **oldState** del objeto
* Los filtros se evalúan únicamente en función de si son o no iguales a un valor específico
* Si la sintaxis del filtro es incorrecta o no coincide con ningún dato contenido en la variable **newState** de la carga útil, no se devolverá un mensaje de validación para indicar que se ha producido un error
* Los filtros no se pueden actualizar en una suscripción que exista actualmente; se debe crear una nueva suscripción con nuevos parámetros de filtro.
* Se pueden aplicar varios filtros a una sola suscripción y esta solo se entregará cuando se hayan cumplido todas las condiciones de filtro.
* La aplicación de varios filtros a una sola suscripción es una práctica equivalente a utilizar un **Y** operador lógico.
* Se pueden aplicar varias suscripciones de evento a un único objeto siempre que uno o más parámetros de campo de suscripción de evento sean diferentes entre cada suscripción de evento.
* Cuando se asignan varias suscripciones de evento a un único objeto, todas las suscripciones de evento asociadas con ese objeto se pueden devolver a un único extremo. Esta práctica puede utilizarse como sustituto equivalente del operador lógico **O** que no se puede configurar con parámetros de filtro.

### Uso de operadores de comparación

Puede especificar un campo de comparación junto con el campo de filtro. Utilice un operador de comparación en el campo para filtrar los resultados comparativos. Por ejemplo, puede crear una suscripción UPDATE - TASK que solo envíe una carga útil si el estado de la tarea NO es igual a actual. Puede utilizar los siguientes operadores de comparación:

#### eq: equal

Este filtro permite que los mensajes lleguen si el cambio que se ha producido coincide `fieldValue` en el filtro exactamente. El `fieldValue` El valor distingue entre mayúsculas y minúsculas.

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

#### ne: no es igual a

Este filtro permite que los mensajes lleguen si el cambio que se ha producido no coincide `fieldValue` en el filtro exactamente. El `fieldValue` El valor distingue entre mayúsculas y minúsculas.

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

#### gt: greater than

Este filtro permite que los mensajes lleguen si la actualización del especificado `fieldName` es mayor que el valor de `fieldValue`.

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

#### get: greater than or equal to

Este filtro permite que los mensajes lleguen si la actualización del especificado `fieldName` es mayor o igual que el valor de `fieldValue`.

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

#### lt: less than

Este filtro permite que los mensajes lleguen si la actualización del especificado `fieldName` es menor que el valor de `fieldValue`.

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

Este filtro permite que los mensajes lleguen si la actualización del especificado `fieldName` es menor o igual que el valor de `fieldValue`.

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

Este filtro permite que los mensajes lleguen si el cambio que se produjo contiene el `fieldValue` en el filtro. El `fieldValue` El valor distingue entre mayúsculas y minúsculas

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

Este filtro permite que los mensajes lleguen únicamente si el campo especificado (`fieldName`) tiene un valor diferente en oldstate y newstate. Actualizando otros campos además del especificado (`fieldName`) no devolverá ese cambio.

>[!NOTE]
>
`fieldValue` en la matriz de filtros a continuación no tiene ningún efecto.

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

Este conector hace que el filtro se aplique al nuevo estado o al antiguo estado del objeto que se creó o actualizó. Esto resulta útil cuando desea saber dónde se realizó un cambio de algo a otro.
`oldState` no es posible en CREATE `eventTypes`.

>[!NOTE]
>
La suscripción siguiente con el filtro dado solo devolverá mensajes donde el nombre de la tarea contenga `again` en el `oldState`, lo que había antes de realizar una actualización de la tarea.
Un caso de uso para esto sería encontrar los mensajes de objCode que han cambiado de una cosa a otra. Por ejemplo, para averiguar todas las tareas que cambiaron de &quot;Buscar un nombre&quot; a &quot;Buscar un nombre de equipo&quot;

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

El `filterConnector` en la carga útil de suscripción le permite elegir cómo se deben aplicar los filtros. El valor predeterminado es &quot;Y&quot;, donde todos los filtros deben estar `true` para que aparezca el mensaje de suscripción. Si se especifica &quot;OR&quot;, solo debe coincidir un filtro para que aparezca el mensaje de suscripción.

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

## Eliminación de suscripciones a eventos

Al eliminar HTTP de Workfront, utilice el método DELETE. La sintaxis de solicitud para eliminar una sola suscripción de evento por ID de suscripción es la siguiente:

**URL de solicitud:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Encabezados de solicitud:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor del encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> valor sessionID </p> </td> 
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
   <td>El servidor eliminó correctamente la suscripción de evento que coincide con el ID de suscripción proporcionado.</td> 
  </tr> 
  <tr> 
   <td>401 (No autorizado)</td> 
   <td>El ID de sesión proporcionado estaba vacío.</td> 
  </tr> 
  <tr> 
   <td>403 (Prohibido)</td> 
   <td>El usuario que coincide con el sessionID proporcionado no tiene acceso de administrador.</td> 
  </tr> 
  <tr> 
   <td>404 (No encontrado)</td> 
   <td>El servidor no ha podido encontrar una suscripción de evento que coincida con el ID de suscripción proporcionado para la eliminación.</td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo de encabezados de respuesta:**

| Encabezado de respuesta | Ejemplo |
|---|---|
| Fecha | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Servidor | `→Apache-Coyote/1.1` |


**Ejemplo de cuerpo de respuesta:** N/D

## Ejemplos de cargas útiles de eventos

La carga útil que recibe un usuario varía según el tipo de objeto, pero existe un formato coherente para el cual se entregan esas cargas útiles variables.

Por ejemplo, las siguientes propiedades siguen siendo coherentes en todas las cargas útiles de evento:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Aunque son coherentes en cuanto a formato, los valores contenidos en las propiedades varían entre diferentes objetos y tipos de objetos.

A continuación se muestran ejemplos de cargas útiles para un evento UPDATE y un evento CREATE. Observe que en el ejemplo UPDATE los objetos oldState y newState son los mismos, mientras que en el ejemplo CREATE el objeto oldState está vacío (no es NULL).

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

A continuación se muestra un ejemplo de carga útil para un evento CREATE:

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

El campo base64Encoding es un campo opcional que se utiliza para habilitar la codificación Base64 de las cargas útiles de suscripción de eventos. El valor predeterminado es false y los valores posibles son: true, false y &quot;&quot; (en blanco).

### Ejemplo de una solicitud que utiliza el campo base64Encoding

Si se realiza una solicitud utilizando el campo base64Encoding establecido en true, la variable **newState** y **oldState** Los objetos de la carga útil se entregan como cadenas de codificación base 64. Si el campo base64Encoding se establece en false, se deja en blanco o no se incluye en la solicitud, la carga útil devuelta no se codificará en base 64.

A continuación se muestra un ejemplo de una solicitud que utiliza el campo base64Encoding:

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

### Ejemplos de cargas útiles de respuesta en codificación base 64

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

## Método obsoleto para consultar todas las suscripciones a eventos

El siguiente extremo de API está obsoleto y no debe utilizarse para nuevas implementaciones. También recomendamos la transición de implementaciones antiguas al método en el **Consulta de suscripciones a eventos** sección descrita anteriormente.

Puede consultar todas las suscripciones de evento de un cliente según lo especificado por el valor sessionID. La sintaxis de solicitud para enumerar todas las suscripciones de evento de un cliente específico es la siguiente URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Encabezados de solicitud:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nombre del encabezado</p> </th> 
   <th> <p>Valor del encabezado</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> valor sessionID </p> </td> 
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
   <td>La solicitud devolvió correctamente todas las suscripciones de evento encontradas para el usuario.</td> 
  </tr> 
  <tr> 
   <td>401 (No autorizado)</td> 
   <td>El ID de sesión proporcionado estaba vacío.</td> 
  </tr> 
  <tr> 
   <td>403 (Prohibido)</td> 
   <td>El usuario que coincide con el ID de sesión proporcionado no tiene acceso de administrador.</td> 
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
