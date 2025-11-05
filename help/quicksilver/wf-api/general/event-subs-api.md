---
content-type: api
navigation-topic: general-api
title: API de suscripción a eventos
description: API de suscripción a eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: 0fd415767680d877c9dd1de448f7903e6616d155
workflow-type: tm+mt
source-wordcount: '3097'
ht-degree: 65%

---


# API de suscripción a eventos

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Cuando se produce una acción en un objeto de Adobe Workfront compatible con las suscripciones a eventos, puede configurar Workfront para que envíe una respuesta al punto final deseado. Esto significa que las aplicaciones de terceros pueden recibir actualizaciones de las interacciones de Workfront a través de la API de Workfront poco después de que se produzcan. En general, puede esperar recibir notificaciones de webhook en menos de 5 segundos desde que se registra el cambio de datos. De media, los clientes reciben notificaciones de webhook en menos de un segundo desde que se registra el cambio de datos.

Dado que las suscripciones de eventos envían datos a otro servicio, se administran mediante comandos en lugar de a través de la aplicación de Workfront.

Para recibir cargas útiles de suscripciones a eventos a través del cortafuegos, debe añadir las siguientes direcciones IP a la lista de permitidos:

**Para clientes de Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Para clientes que no se encuentran en Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

Los siguientes temas admiten la API de suscripción a eventos:

## Objetos admitidos por suscripciones a eventos

Las suscripciones a eventos admiten los siguientes objetos de Workfront.

* Aprobación
* Fase de aprobación
* Participante de fase de aprobación
* Asignación
* Compañía
* Panel de control
* Documento
* Versión de documento
* Gasto
* Campo
* Hora
* Problema
* Nota
* Portafolio
* Programa
* Proyecto
* Aprobación de revisión
* Registro
* Tipo de registro
* Informe
* Plan de asignación de personal
* Valor del parámetro del plan de asignación de personal
* Recurso del plan de asignación de personal
* Valor de atributo de recurso de plan de plantilla
* Conjunto de valores de atributo de recurso de plan de plantilla
* Valor del parámetro de recurso del plan de asignación de personal
* Tarea
* Plantilla
* Plantilla de horas
* Usuario
* Espacio de trabajo

>[!NOTE]
>
>Para obtener una lista de los campos admitidos por los objetos de suscripción a eventos, consulte [Campos de recurso de suscripción a eventos](../../wf-api/api/event-sub-resource-fields.md).

## Autenticación de suscripción de evento

Para crear, consultar o eliminar una suscripción a eventos, el usuario de Workfront necesita lo siguiente:

* Se requiere un nivel de acceso de “Administrador del sistema” para utilizar las suscripciones a eventos.
* Se requiere un encabezado `sessionID` para usar la API de suscripciones a eventos

  Para obtener más información, consulte [Autenticación](api-basics.md#authentication) en [Conceptos básicos de la API](api-basics.md).

## Evitar sobrecargar suscripciones a eventos

El servicio de suscripciones a eventos está diseñado para proporcionar un envío fiable de eventos para todos los usuarios. Para garantizar esto, se han implementado salvaguardas para evitar una producción de eventos excesiva por parte de un solo usuario que podría causar posibles problemas de calidad del servicio para todos los usuarios. Como resultado, un usuario que produce demasiados eventos a una tasa alta en un corto periodo de tiempo puede experimentar interferencias y retrasos en la entrega de eventos.

## Formación del recurso de suscripción

El recurso de suscripción contiene los campos siguientes.

* objId (opcional)

   * **Cadena**: ID del objeto del objCode especificado para el que se activan los eventos. Si no se especifica este campo, el usuario recibe eventos para todos los objetos del tipo especificado.

* objCode (obligatorio)

   * **Cadena**: objCode del objeto al que se está suscribiendo a cambios. Los valores posibles de objCode se enumeran en la tabla siguiente.

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
        <td scope="col">Aprobación</td> 
        <td scope="col"><p>aprobación</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Fase de aprobación</td> 
        <td scope="col"><p>approval_stage</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Participante de fase de aprobación</td> 
        <td scope="col"><p>approval_stage_partition</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Asignación</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Compañía </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Panel de control</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Documento</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Versión de documento</p></td> 
        <td scope="col">DOCV </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Gasto</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Campo</p></td> 
        <td scope="col"><p>FIELD</p></td> 
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
        <td scope="col"><p>PORT</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Programa</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Proyecto</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Aprobación de revisión</p></td> 
        <td scope="col"><p>PRFAPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Registro</p></td> 
        <td scope="col"><p>RECORD</p></td> 
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
        <td scope="col"><p>Plan de asignación de personal</p></td> 
        <td scope="col"><p>STAFFP</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Valor del parámetro del plan de asignación de personal</p></td> 
        <td scope="col"><p>SPVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Recurso del plan de asignación de personal</p></td> 
        <td scope="col"><p>PERSONAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Valor de atributo de recurso de plan de plantilla</p></td> 
        <td scope="col"><p>ESPAVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Conjunto de valores de atributo de recurso de plan de plantilla</p></td> 
        <td scope="col"><p>SAVSET</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Valor del parámetro de recurso del plan de asignación de personal</p></td> 
        <td scope="col"><p>SRPVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Tarea</p></td> 
        <td scope="col"><p>TASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Plantilla</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Plantilla de horas</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">Usuario</td> 
        <td scope="col">USER</td> 
       </tr> 
       <tr> 
        <td scope="col">Espacio de trabajo</td> 
        <td scope="col">WORKSPACE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (obligatorio)

   * **Cadena**: valor que representa el tipo de evento al que está suscrito el objeto. Los tipos de eventos disponibles incluyen:

      * CREATE
      * ELIMINAR
      * UPDATE

* url (obligatorio)

   * **Cadena**: dirección URL del punto final al que se envían las cargas útiles de evento de suscripción a través de HTTP.

* authToken (obligatorio)

   * **Cadena**: El token de portador de OAuth2 utilizado para autenticarse con la dirección URL especificada en el campo &quot;URL&quot;.

## Creación de solicitudes de API de suscripción de evento

Después de asegurarse de que el usuario tiene acceso de administrador y de formar el recurso de suscripción, está listo para crear suscripciones a eventos.

Utilice la siguiente sintaxis para construir la dirección URL.

**URL de solicitud**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Encabezados de solicitud**

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
   <td> <p>sessionID value</p> </td> 
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

**Ejemplo de cuerpo de respuesta**

```
{
    "id": <NEW SUBSCRIPTION ID>,
    "version": <NEW SUBSCRIPTION VERSION>
}
```

| Código de respuesta | Descripción |
|---|---|
| 201 (Creado) | La suscripción al evento se ha creado correctamente. |
| 400 (Solicitud incorrecta) | El campo URL del recurso de suscripción se ha considerado no válido. |
| 401 (No autorizado) | El sessionID proporcionado estaba vacío o se consideró no válido. |
| 403 (Prohibido) | El usuario que coincide con el sessionID proporcionado no tiene acceso de administrador. |

Si se pasa un recurso de suscripción como cuerpo de una solicitud (con el tipo de contenido &quot;application/json&quot;), se crea una suscripción de evento para el objeto especificado. Un código de respuesta 201 (Creado) indica que se creó la suscripción. Un código de respuesta distinto de 201 significa que la suscripción **NO** se ha creado.

>[!NOTE]
>
> El encabezado de respuesta &quot;Ubicación&quot; contiene el URI de la suscripción de evento recién creada.

**Ejemplo de encabezados de respuesta:**

| Encabezados de respuesta | Ejemplo |
|---|---|
| Content-Length | `→0` |
| Fecha | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Ubicación | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Servidor | `→Apache-Coyote/1.1` |

## Consulta de suscripciones a eventos

Al consultar el código HTTP de Workfront, utilice el método GET. Existen dos formas de consultar suscripciones a eventos: consultar por el ID de suscripción (véase más abajo) o consultar todas las suscripciones a eventos.

### Consultar todas las suscripciones a eventos

Puede consultar todas las suscripciones a eventos de un cliente o utilizar lo siguiente para administrar la respuesta. También puede utilizar las siguientes opciones para administrar la respuesta:

* **page**: opción de parámetro de consulta para especificar el número de páginas que se van a devolver. El valor predeterminado es 1.
* **limit**: opción de parámetro de consulta para especificar el número de resultados que se devolverán por página. El valor predeterminado es 100, con un máximo de 1000.

La sintaxis de solicitud para enumerar todas las suscripciones a eventos de un cliente específico es la siguiente:

**URL de solicitud**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Encabezados de la solicitud:**

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
   <td> <p>sessionID value</p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de respuesta**

| Código de respuesta | Descripción |
|---|---|
| 200 (OK) | Se ha devuelto la solicitud con todas las suscripciones a eventos encontradas para el cliente que coinciden con el sessionID proporcionado. |
| 401 (No autorizado) | El sessionID proporcionado estaba vacío. |
| 403 (Prohibido) | El usuario, que coincide con el sessionID proporcionado, no tiene acceso de administrador. |


**Ejemplo de encabezados de respuesta**

| Encabezado de respuesta | Ejemplo |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Fecha | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Servidor | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


**Ejemplo de cuerpo de respuesta**

```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```

Donde

* **page** y **limit** son los valores proporcionados en la solicitud o el valor predeterminado si no se proporcionan valores
* **page_count** es el número total de páginas que se pueden consultar.
* **total_count** es el número total de suscripciones que coinciden con la consulta.

### Consulta por el ID de suscripción de eventos

Puede consultar suscripciones de eventos por el ID de suscripción de eventos. La sintaxis de solicitud para enumerar suscripciones de eventos es la siguiente:

**URL de solicitud**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Encabezados de solicitud**

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
   <td> <p>sessionID value</p> </td> 
  </tr> 
 </tbody> 
</table>

**Códigos de respuesta**

| Código de respuesta | Descripción |
|---|---|
| 200 (OK) | La solicitud devuelta con la suscripción al evento que coincide con el ID de suscripción proporcionado. |
| 401 (No autorizado) | El sessionID proporcionado estaba vacío. |
| 403 (Prohibido) | El usuario, que coincide con el sessionID proporcionado, no tiene acceso de administrador. |


**Ejemplo de cuerpo de respuesta**



```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```


## Versiones de suscripción de evento

Workfront tiene dos versiones de suscripciones a eventos.

La capacidad de actualizar o reducir las suscripciones a eventos garantiza que, cuando se realicen cambios en la estructura de los eventos, las suscripciones existentes no se rompan, lo que le permite probar y actualizar a la nueva versión sin interrupciones en la suscripción de evento.

Para obtener más información sobre las versiones de suscripción de evento, incluidas las diferencias específicas entre la versión y las fechas importantes, consulte [Versiones de suscripción de evento](/help/quicksilver/wf-api/general/event-subs-versioning.md).

>[!NOTE]
>
>Al actualizar o reducir la suscripción de evento a otra versión, se reciben eventos duplicados para cada entrega de evento durante un periodo de cinco minutos después del cambio de versión. Los duplicados incluyen una de cada versión de suscripción de evento 1 y una versión 2. Esto garantiza que no se pierda ningún evento debido al cambio de la versión de suscripción del evento.

### Cambio de versión de suscripción única

La sintaxis de solicitud para cambiar la versión de una sola suscripción es:

**URL de solicitud**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>/version 
```

**Cuerpo de solicitud de ejemplo**

```
{
    "version": "v2" 
}
```


**Cuerpo de respuesta de ejemplo (200)**

```
{
    "id": <SUBSCRIPTION ID>,
    "version": "v2" 
}
```

**Códigos de respuesta posibles**

* 200
* 400
* 404


### Cambio de versión de suscripción múltiple

Este punto de conexión cambia la versión de varias suscripciones, por lista de suscripciones o por indicador de todas las suscripciones del cliente.

La sintaxis de solicitud para cambiar la versión de una sola suscripción es:

**URL de solicitud**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/version
```

**Cuerpos de solicitud de ejemplo**

* Cuerpo de solicitud de lista de suscripciones

  ```
  {
      "subscriptionIds": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>],
      "version": "v2" 
  }
  ```

* Solicitar cuerpo para todas las suscripciones del cliente

  ```
  {
      "allCustomerSubscriptions": true,
      "version": "v2" 
  }
  ```

**Cuerpo de respuesta de ejemplo (200)**

```
{
    "subscription_ids": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>, ...],
    "version": "v2" 
}
```

**Códigos de respuesta posibles**

* 200
* 400

## Filtrado de suscripción a eventos

El filtrado de suscripción a eventos se puede utilizar para garantizar que solo recibe mensajes relevantes. La creación de filtros para sus suscripciones puede disminuir significativamente la cantidad de mensajes que debe consumir su punto final.

Por ejemplo, una suscripción al evento **UPDATE - TASK** solo se puede establecer para que se active solamente cuando el **newState** de una carga útil de evento define **taskStatus** como **actual**.

>[!IMPORTANT]
>
>Los siguientes atributos se aplican al filtrado de suscripción de eventos

* Cuando un campo de filtro tiene un valor que no está vacío, solo se envían mensajes con un **newState** que contiene las claves de filtro y los valores a la dirección URL suscrita
* Puede filtrar por los datos personalizados incluidos en **newState** AND/OR **oldState** del objeto
* Los filtros se evalúan únicamente en función de si equivalen o no a un valor específico
* Si la sintaxis del filtro es incorrecta o no coincide con ningún dato contenido en **newState** de la carga útil, no se devolverá un mensaje de validación para indicar que se ha producido un error
* Los filtros no se pueden actualizar en una suscripción que exista actualmente; se debe crear una nueva suscripción con nuevos parámetros de filtro.
* Se pueden aplicar varios filtros a una sola suscripción y esta solo se entregará cuando se hayan cumplido todas las condiciones de filtro.
* Aplicar varios filtros a una sola suscripción es una práctica equivalente a utilizar un operador lógico **AND**.
* Se pueden aplicar varias suscripciones de eventos a un único objeto siempre que uno o más parámetros de campo de suscripción a eventos sean diferentes entre cada suscripción a evento.
* Cuando se asignan varias suscripciones de eventos a un único objeto, todas las suscripciones de eventos asociadas a ese objeto se pueden devolver a un único punto final. Esta práctica se puede utilizar como un sustituto equivalente del operador lógico **OR** que no se puede establecer mediante parámetros de filtro.
* Los campos siguientes no se pueden filtrar:

   * DOCU.groups
   * RECORD.data
   * RECORD_TYPE.data
   * RECORD_TYPE.fields

### Uso de operadores de comparación

Puede especificar un campo de comparación junto con el campo de filtro. Utilice un operador de comparación en el campo para filtrar los resultados comparativos. Por ejemplo, puede crear una suscripción UPDATE - TASK que solo envíe una carga útil si el estado de la tarea NO es igual a actual. Puede utilizar los siguientes operadores de comparación:

#### eq: igual

Este filtro permite que los mensajes lleguen si el cambio que se produjo coincide exactamente con `fieldValue` en el filtro. El valor `fieldValue` distingue entre mayúsculas y minúsculas.

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

#### ne: no igual a

Este filtro permite que los mensajes lleguen si el cambio que se produjo no coincide exactamente con `fieldValue` en el filtro. El valor `fieldValue` distingue entre mayúsculas y minúsculas.

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

#### gt: mayor que

Este filtro permite que los mensajes lleguen si la actualización del `fieldName` especificado es mayor que el valor de `fieldValue`.

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

#### gte: mayor o igual que

Este filtro permite que los mensajes lleguen si la actualización del `fieldName` especificado es mayor o igual que el valor de `fieldValue`.

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

#### It: menor que

Este filtro permite que los mensajes lleguen si la actualización del `fieldName` especificado es menor que el valor de `fieldValue`.

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

Este filtro permite que los mensajes lleguen si la actualización del `fieldName` especificado es menor o igual que el valor de `fieldValue`.

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

Este filtro permite que se envíen mensajes si el cambio que se produjo contiene `fieldValue` en el filtro. El valor `fieldValue` distingue entre mayúsculas y minúsculas

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

#### containsOnly

Este filtro permite que los mensajes se transmitan únicamente cuando el conjunto completo de valores seleccionados coincide exactamente con fieldValue del filtro, independientemente del orden. No debe haber valores adicionales o que falten.

>[!NOTE]
>
>Se utiliza para campos de tipo matriz (selección múltiple). Esta suscripción de ejemplo que se muestra a continuación permite que los mensajes se transmitan únicamente cuando el campo `groups` contiene exactamente &quot;Opción 3&quot; y &quot;Opción 4&quot;, sin valores adicionales o que falten, e independientemente del orden. Si se especifica una cadena o un entero en `fieldValue` en lugar de una matriz, la suscripción permite que los mensajes se transmitan solo cuando el campo `groups` contiene exactamente una opción y esa opción coincide exactamente con la cadena o el entero especificado en `fieldValue`&quot;


```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": [
                "Choice 3",
                "Choice 4"
            ],
            "state": "newState",
            "comparison": "containsOnly"
        }
    ]
}
```

#### notContains

Este filtro permite que los mensajes se transmitan sólo cuando el campo especificado (`fieldName`) no contiene el valor especificado (`fieldValue`)

>[!NOTE]
>
>Se utiliza para campos de tipo matriz (selección múltiple) o cadena. Si el campo es una cadena, comprobaremos si el valor especificado no está contenido en la cadena (por ejemplo, &quot;Nuevo&quot; no está en la cadena &quot;Proyecto - Actualizado&quot;). Si el campo es una matriz y el valor de campo especificado es una cadena o un número entero, comprobaremos si la matriz no contiene el valor especificado (por ejemplo, &quot;Opción 1&quot; que no está en [&quot;Opción 2&quot;, &quot;Opción 3&quot;]). La suscripción de ejemplo siguiente permite que los mensajes se envíen únicamente cuando los campos `groups` no contienen la cadena &quot;Group 2&quot;.

```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": "Group 2",
            "state": "newState",
            "comparison": "notContains"
        }
    ]
}
```

#### cambiar

Este filtro permite que los mensajes se transmitan solo si el campo especificado (`fieldName`) tiene un valor diferente en oldstate y newstate. Al actualizar otros campos además del especificado (`fieldName`), no se devolverá ese cambio.

>[!NOTE]
>
>`fieldValue` en la matriz de filtros siguiente no tiene ningún efecto.

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

Este conector hace que el filtro se aplique al nuevo estado o al antiguo estado del objeto que se creó o actualizó. Esto resulta útil si desea saber dónde se realizó un cambio de alguna cosa a otra.
`oldState` no es posible en CREATE `eventTypes`.

>[!NOTE]
>
>La suscripción siguiente con el filtro especificado solo devolverá mensajes donde el nombre de la tarea contenga `again` en `oldState`, tal como sucedía antes de que se realizara una actualización en la tarea.
>Un caso de uso para esto sería encontrar los mensajes de objCode que han cambiado de una manera a otra. Por ejemplo, para averiguar todas las tareas que cambiaron de &quot;Investigar Algún nombre&quot; a &quot;Investigar TeamName Algún nombre&quot;

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

### Uso de filtros anidados

La suscripción a evento admite el filtrado en campos anidados de eventos mediante el uso de nombres de campo anidados. Por ejemplo, para filtrar un mensaje donde `newState.data.customField1 = 'myCustomeFieldValue'`, se puede crear la siguiente suscripción con filtro:

```
{
    "objCode": "RECORD",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedRecords",
    "filters": [
        {
            "fieldName": "data",
            "fieldValue": {
                    "customField1": "myCustomFieldValue"
            },
            "comparison": "eq",
            "state": "newState"
        }
    ]
}
```

También se pueden abordar los filtros doblemente anidados.

```
"filters": [
    {
        "fieldName": "data",
        "fieldValue": {
            "fields": {
                "children": {
                    "customerId":"customer1234",
                    "name":"New Campaign"
                }
            }
        },
        "comparison": "eq",
        "state": "newState"
    }
],
"filterConnector": 'AND'
```

### Uso de campos de conector

El campo `filterConnector` de la carga útil de suscripción le permite elegir cómo se deben aplicar los filtros. El valor predeterminado es “AND”, donde los filtros deben ser todos `true` para que se transmita el mensaje de suscripción. Si se especifica “OR&quot;, solo debe coincidir un filtro para que aparezca el mensaje de suscripción.

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

### Uso de grupos de filtros

Los grupos de filtros le permiten crear condiciones lógicas anidadas (Y/O) dentro de los filtros de suscripción de evento.

Cada grupo de filtros puede tener lo siguiente:

* Su propio conector (AND u OR).
* Varios filtros, cada uno con la misma sintaxis y el mismo comportamiento que los filtros independientes.

>[!IMPORTANT]
>
>Un grupo debe tener un mínimo de 2 filtros.


Todos los filtros de un grupo admiten lo siguiente:

* Operadores de comparación: eq, ne, gt, get, lt, lte, contains, notContains, containsOnly, changed.
* Opciones de estado: newState, oldState.
* Segmentación de campos: cualquier nombre de campo de objeto válido.

```
{
  "objCode": "TASK",
  "eventType": "UPDATE",
  "authToken": "token",
  "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
  "filters": [
    {
      "fieldName": "percentComplete",
      "fieldValue": "100",
      "comparison": "lt"
    },
    {
      "type": "group",
      "connector": "OR",
      "filters": [
        {
          "fieldName": "status",
          "fieldValue": "CUR",
          "comparison": "eq"
        },
        {
          "fieldName": "priority",
          "fieldValue": "1",
          "comparison": "eq"
        }
      ]
    }
  ],
  "filterConnector": "AND"
}
```

El ejemplo anterior contiene los siguientes componentes:

1. El filtro de nivel superior (fuera del grupo):

   * `{ "fieldName": "percentComplete", "fieldValue": "100", "comparison": "lt" }`
   * Este filtro comprueba si el campo percentComplete de la tarea actualizada es inferior a 100.

1. Grupo de filtros (filtros anidados con OR):

   * `{ "type": "group", "connector": "OR", "filters": [ { "fieldName": "status", "fieldValue": "CUR", "comparison": "eq" }, { "fieldName": "priority", "fieldValue": "1", "comparison": "eq" } ] }`
   * Este grupo evalúa dos filtros internos:

      * El primero comprueba si el estado de la tarea es igual a &quot;CUR&quot; (actual).
      * El segundo comprueba si la prioridad es igual a 1 (prioridad alta).
   * Como el conector es &quot;OR&quot;, este grupo pasará si alguna de las condiciones es verdadera.

1. Conector de nivel superior (filterConnector: AND):
   * El conector exterior entre los filtros de nivel superior es &quot;Y&quot;. Esto significa que tanto el filtro de nivel superior como el grupo deben pasar para que coincida el evento.

1. Los déclencheur de suscripción cuando se cumplen las siguientes condiciones:
   * percentComplete es inferior a 100.
   * El estado es &quot;CUR&quot; o la prioridad es igual a &quot;1&quot;.

>[!NOTE]
>
>Existen límites para garantizar un rendimiento del sistema coherente al utilizar grupos de filtros, que incluyen lo siguiente:
>
>* Cada suscripción admite hasta 10 grupos de filtros (y cada grupo contiene varios filtros).
>* Cada grupo de filtros puede incluir hasta 5 filtros para evitar una posible degradación del rendimiento durante el procesamiento de eventos.
>* Aunque se admiten hasta 10 grupos de filtros (cada uno con 5 filtros), un gran número de suscripciones activas con una lógica de filtro compleja puede provocar un retraso durante la evaluación del evento.

## Eliminación de suscripciones a eventos

Al eliminar HTTP de Workfront, utilice el método DELETE. La sintaxis de solicitud para eliminar una sola suscripción a eventos por ID de suscripción es la siguiente:

**URL de la solicitud:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Encabezados de la solicitud:**

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
   <td> <p> sessionID value </p> </td> 
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
   <th> Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (sin contenido)</td> 
   <td>El servidor eliminó correctamente la suscripción a eventos que coincide con el ID de suscripción proporcionado.</td> 
  </tr> 
  <tr> 
   <td>401 (No autorizado)</td> 
   <td>El sessionID proporcionado estaba vacío.</td> 
  </tr> 
  <tr> 
   <td>403 (Prohibido)</td> 
   <td>El usuario que coincide con el sessionID proporcionado no tiene acceso de administrador.</td> 
  </tr> 
  <tr> 
   <td>404 (No se encuentra)</td> 
   <td>El servidor no ha podido encontrar una suscripción a eventos que coincida con el ID de suscripción proporcionado para la eliminación.</td> 
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

La carga útil que recibe un usuario varía según el tipo de objeto, pero existe un formato coherente para la entrega de esas cargas útiles variables.

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
                   "eventVersion": "v2",
                   "subscriptionVersion": "v2",
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
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
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

Si se rechaza una suscripción a eventos debido a un conflicto entre los caracteres especiales contenidos en las suscripciones a eventos y la configuración de red, puede utilizar la codificación Base64 para pasar las suscripciones a eventos. Base64 es un conjunto de esquemas de codificación que pueden traducir cualquier dato arbitrario a un formato de cadena ASCII. Es importante tener en cuenta que Base64 no es una forma de cifrado de seguridad.

### Campo de codificación Base 64

El campo base64Encoding es un campo opcional que se utiliza para habilitar la codificación Base64 de las cargas útiles de suscripción a eventos. El valor predeterminado es falso y los valores posibles son: verdadero, falso y &quot; &quot; (en blanco).

### Ejemplo de una solicitud que utiliza el campo base64Encoding

Si se realiza una solicitud utilizando el campo base64Encoding establecido en true, los objetos **newState** y **oldState** de la carga útil se entregan como cadenas de codificación base 64. Si el campo base64Encoding se establece en false, se deja en blanco o no se incluye en la solicitud y la carga útil devuelta no se codificará en base 64.

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
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Método obsoleto para consultar todas las suscripciones a eventos

El siguiente punto final de API está obsoleto y no debe utilizarse para nuevas implementaciones. También recomendamos la transición de implementaciones antiguas al método en la sección **Consulta de suscripciones a eventos** descrita anteriormente.

Puede consultar todas las suscripciones a eventos de un cliente según lo especificado por el valor sessionID. La sintaxis de solicitud para enumerar todas las suscripciones a eventos de un cliente específico es la siguiente URL:

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
   <td> <p> sessionID value </p> </td> 
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
   <th> Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (sin contenido)</td> 
   <td>La solicitud devolvió correctamente todas las suscripciones a eventos encontradas para el usuario.</td> 
  </tr> 
  <tr> 
   <td>401 (No autorizado)</td> 
   <td>El sessionID proporcionado estaba vacío.</td> 
  </tr> 
  <tr> 
   <td>403 (Prohibido)</td> 
   <td>El usuario que coincide con el sessionID proporcionado no tiene acceso de administrador.</td> 
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
