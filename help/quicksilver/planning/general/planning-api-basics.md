---
title: Conceptos básicos de API de Adobe Workfront Planning
description: La meta de la API de Adobe Workfront Planning es simplificar la creación de integraciones con la planificación mediante la introducción de una arquitectura REST-ful que funcione a través de HTTP. En este documento se da por hecho que está familiarizado con las respuestas de REST y JSON y se describe el método que utiliza la API de planificación.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
TQID: https://experienceleague.adobe.com/SGwYFV5aZJGwfUy7ejVTaOkn0v4Dt-HJLI5hDWKVhMo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 2232
ht-degree: 11%

---

# Conceptos básicos de la API de Adobe Workfront Planning

{{planning-important-intro}}

<!--

Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 

-->

El objetivo de la API de Planning de Adobe Workfront es simplificar la creación de integraciones con Planning mediante la introducción de una arquitectura RESTful que funcione a través de HTTP. Este documento supone que está familiarizado con las respuestas de REST y JSON.

Para obtener toda la referencia de extremo, esquemas de solicitud/respuesta y detalles específicos de la versión, consulte la [documentación para desarrolladores de la API de Workfront Planning](https://developer.adobe.com/wf-planning).

## Autenticación

La API de Workfront Planning utiliza OAuth 2.0 para la autenticación. Las credenciales se configuran mediante Adobe Developer Console.

Admitimos los dos flujos siguientes en función de su tipo de integración:

* **Autenticación de servidor a servidor (JWT)**: para integraciones automatizadas y servicios back-end sin interacción del usuario. Utiliza la credencial de servidor a servidor OAuth (concesión de credenciales de cliente: la aplicación se autentica directamente mediante su ID de cliente y secreto para obtener un token de acceso, sin inicio de sesión del usuario ni paso de consentimiento).

  Para obtener más información, consulte [Autenticación de servidor a servidor](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/).

* **Autenticación de usuario (flujo de código de autorización)**: para integraciones que actúan en nombre de un usuario específico. Utiliza la credencial de aplicación web o aplicación de una sola página de OAuth (concesión de código de autorización: el usuario inicia sesión y da su consentimiento, tras lo cual la aplicación recibe un código de autorización que intercambia por un token de acceso).

  Para obtener más información, consulte [Autenticación de usuario](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/).

Para empezar, cree un proyecto en Adobe Developer Console y añada la API de Workfront Planning para obtener sus credenciales.

Para configurar las credenciales, cree una aplicación OAuth2 en Workfront.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

>[!NOTE]
>
>El extremo `/login` y la autenticación de clave de API no son compatibles con Workfront Planning. No use `sessionID` ni `apiKey` parámetros.


## Versiones de API

Las versiones de la API de Planning se realizan mediante la ruta URL.

Las siguientes son las versiones compatibles actuales:

<!--

(*****************add deprecation date column above, when we have one*****************)

-->

| Versión | Fecha de la versión |
|-----------|----------------|
| Versión 1 | Julio de 2024 |
| Versión 2 | Mayo de 2026 |

>[!NOTE]
>
>El conector de Workfront Planning para Workfront Fusion no se ha actualizado a la versión 2 de la API y seguirá utilizando la versión 1 hasta nuevo aviso.

Para obtener más información sobre las versiones compatibles actuales, consulte el artículo [Documentación para desarrolladores de API de Workfront Planning](https://developer.adobe.com/wf-planning).

Se recomienda segmentar explícitamente una versión en todas las integraciones:

```
https://{customer-domain}/maestro/api/v2/...
```

Cuando se publique una nueva versión principal, la versión anterior seguirá disponible hasta que se comunique una fecha de obsolescencia.

Siga las Notas de la versión de Workfront para mantenerse informado de los cambios de la API.


## Estructura y operaciones de URL

Los objetos se manipulan enviando una petición HTTP a su URI único. La operación se especifica mediante el método HTTP.

| Método | Operación |
|----------|----------------------------------------------------------------------|
| GET | Recuperar un solo objeto por ID u objetos de búsqueda/lista |
| POST | Crear un nuevo objeto |
| PUT | Reemplazar un objeto existente (actualización completa) |
| PATCH | Actualizar parcialmente un objeto existente (solo se modifican los campos) |
| ELIMINAR | Eliminar un objeto |

>[!NOTE]
>
>**Nota de la versión 1:** `PATCH` no es compatible con la versión 1. Usar `PUT` para todas las actualizaciones.


Para obtener rutas de acceso de extremo completas y ejemplos de solicitud/respuesta, consulte la **referencia de API** en [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

## Códigos de estado HTTP

La API de Planning devuelve códigos de estado HTTP estándar:

| Código | Significado |
|------------------------|-------------------------------------------------|
| 200 OK | GET, PUT o PATCH correctos |
| 201 Creado | Publicación correcta (recurso creado) |
| 204 Sin contenido | DELETE correcto |
| 207 Multi-Status | La operación masiva se completó con resultados mixtos, con algunos elementos correctos y otros fallidos. Consulte las respuestas de elementos individuales para obtener más detalles. |
| 400 Solicitud incorrecta | Solicitud no válida: consulte la respuesta de error para obtener más información |
| 401 No autorizado | Falta el token de autenticación o no es válido |
| 403 Prohibido | Permisos autenticados pero insuficientes |
| 404 No encontrado | El recurso no existe |
| Conflicto 409 | Conflicto de escritura, el recurso se modificó mediante otra solicitud. Vuelva a intentarlo con la versión más reciente. |
| 429 Demasiadas solicitudes | Límite de velocidad excedido |

>[!NOTE]
>
>**Nota de la versión 1:** La versión 1 devuelve `200 OK` para todas las operaciones correctas, incluidas POST y DELETE.


## Gestión de errores

La API de Planning devuelve errores en un formato coherente. Cada respuesta de error incluye un mensaje legible en lenguaje natural, un código de error legible en el equipo y un ID de solicitud para la escalación de soporte.

Ejemplo de respuesta de error:

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}
```

Use `errorCode` (no `status`) para controlar la administración de errores de programación. Proporciona la clasificación más específica del error.

>[!NOTE]
>
>**Nota de la versión 1:** Las respuestas de error de la versión 1 utilizan un campo numérico `type` (p. ej. `40001`) en lugar de una cadena `errorCode`, y ajustan los detalles en un objeto `report` en lugar de un campo `detail` de nivel superior.

## Filtrado de registros

Utilice el parámetro `filter` en las solicitudes de búsqueda de registros para devolver solo los registros que coincidan con criterios específicos. Para las solicitudes POST, `filter` es una propiedad JSON en el cuerpo de la solicitud. Para solicitudes GET, `filter` es un parámetro de consulta que contiene un grupo de filtros con codificación JSON. Los filtros utilizan una estructura compuesta con tipo con operadores lógicos explícitos.

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}
```

Los filtros se pueden anidar utilizando los operadores `AND` / `OR` para generar condiciones compuestas:

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "IS_BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}
```

>[!NOTE]
>
>**Nota de la versión 1:** La versión 1 usa operadores sin tipo Mongo-style en un objeto `filters`. Los operadores tienen el prefijo `$` (por ejemplo: `$and`, `$or`, `$is`, `$contains`, `$isBetween`). Los parámetros de paginación (`offset`, `limit`) y `recordTypeId` se pasan en el cuerpo de la solicitud en lugar de como una ruta de acceso de la dirección URL y parámetros de consulta.


## Tipos de campo y modificadores de búsqueda

Puede utilizar modificadores y filtros con campos para controlar qué datos se devolverán en los resultados.

Para ver ejemplos, consulte la [documentación para desarrolladores de API de Workfront Planning](https://developer.adobe.com/wf-planning/).

### Uso de modificadores de búsqueda

Workfront Planning admite los siguientes modificadores de búsqueda:


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>Modificador</th>
      <th>Ejemplo</th>
      <th>Descripción</th>
      <th>Valores posibles</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTAINS</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"CONTAINS","value":"product"}</td><td>Devuelve registros cuyo valor de campo contiene el filtro</td><td class="possible">“Nuevo lanzamiento del producto”</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"DOES_NOT_CONTAIN","value":"product"}</td><td>Devuelve registros donde el valor del campo no contiene el filtro</td><td class="possible">“Nuevo lanzamiento”</td></tr>
    <tr><td class="modifier">ES</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS","value":"new product launch"}</td><td>Devuelve registros cuyo valor de campo coincida exactamente con el filtro</td><td class="possible">“Nuevo lanzamiento del producto”</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT","value":"product"}</td><td>Devuelve registros cuyo valor de campo no coincide exactamente con el filtro</td><td class="possible">“Nuevo lanzamiento del producto”</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EMPTY"}</td><td>Devuelve registros cuyo valor de campo esté vacío</td><td class="possible">"" o nulo</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_EMPTY"}</td><td>Devuelve registros cuyo valor de campo no esté vacío</td><td class="possible">“Nuevo lanzamiento del producto”</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN","value":"10"}</td><td>Devuelve registros cuyo valor de campo sea mayor que el filtro</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN_OR_EQUAL","value":"10"}</td><td>Devuelve registros cuyo valor de campo sea mayor o igual que el filtro</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN","value":"10"}</td><td>Devuelve registros cuyo valor de campo sea menor que el filtro</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">MENOR_QUE_O_IGUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN_OR_EQUAL","value":"10"}</td><td>Devuelve registros cuyo valor de campo sea menor o igual que el filtro</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Devuelve registros cuyo valor de campo esté entre los dos valores de filtro</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Devuelve registros cuyo valor de campo no esté entre los dos valores de filtro</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_AFTER","value":"2024-01-01"}</td><td>Devuelve registros cuyo valor de campo de fecha es posterior al filtro</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BEFORE","value":"2024-12-31"}</td><td>Devuelve registros cuyo valor de campo de fecha sea anterior al filtro</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_ANY_OF","value":["Active","Planned"]}</td><td>Devuelve registros cuyo valor de campo coincida con cualquier valor de la lista de filtros</td><td class="possible">["Activo","Planificado","Completado"]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NONE_OF","value":["Active","Planned"]}</td><td>Devuelve registros cuyo valor de campo no coincide con ninguno de los valores de la lista de filtros</td><td class="possible">["Activo","Planificado"]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ANY_OF","value":["Tag1","Tag2"]}</td><td>Devuelve registros cuyo campo de varios valores contiene cualquiera de los valores de filtro</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ALL_OF","value":["Tag1","Tag2"]}</td><td>Devuelve registros cuyo campo de varios valores contiene todos los valores de filtro</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EXACTLY","value":["Tag1"]}</td><td>Devuelve registros cuyo campo de varios valores contiene exactamente los valores de filtro y ningún otro</td><td class="possible">["Tag1"]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_NONE_OF","value":["Tag1"]}</td><td>Devuelve registros cuyo campo de varios valores no contiene ninguno de los valores de filtro</td><td class="possible">["Tag1"]</td></tr>
  </tbody>
</table>


>[!NOTE]
>
>Nota de la versión 1: Los nombres de modificadores de la versión 1 utilizan `$-prefixed camelCase` (por ejemplo: `$contains`, `$isNot`, `$isEmpty`, `$greaterThan`, `$greaterThanOrEqual`, `$lessThan`, `$lessThanOrEqual`, `$isBetween`, `$isNotBetween`, `$isAnyOf`, `$hasAllOf`). El comportamiento de cada modificador es el mismo.


## Condiciones de filtro compatibles por tipo de campo

| Tipo de campo | Condiciones admitidas |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| texto, texto largo | CONTIENE, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| número, porcentaje y moneda | IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY |
| fecha | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| single-select | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| selección múltiple, usuario | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| booleano | ES |
| fórmula | CONTIENE, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| created-by | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF |
| updated-by | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| created-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN |
| updated-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| reference | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| lookup | Depende del tipo de campo vinculado |

>[!NOTE]
>
>**Nota de la versión 1:** La versión 1 usa nombres de operadores con prefijo `$` (por ejemplo: `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`). El conjunto de condiciones admitidas por tipo de campo es el mismo.

## Filtrado por campos de personas

Los filtros de campo Personas (`user`, `created-by`, `updated-by`, `approved-by`) aceptan tanto los identificadores de usuario de IMS de Adobe como los de usuario de Workfront. Un valor de cadena sin formato se interpreta como un ID de usuario de Adobe IMS.

Para establecer el tipo de identificador para comprobar el ID de usuario de Workfront, debe pasar explícitamente los parámetros `id` y `idType`. Los valores admitidos para `idType` son &quot;`WF`&quot; para los identificadores de usuario de Workfront y &quot;`IMS`&quot; para los identificadores de usuario de IMS de Adobe.

```
{ 
  "filter": { 
   "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<userFieldId>", 
        "condition": "HAS_ANY_OF", 
        "value": [ 
          { "id": "63e3b13000078c1795146248182d15dc", "idType": "WF" } 
        ] 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
> Nota de la versión 1: La versión 1 solo admite el filtrado por el ID de IMS de los usuarios.

## Filtrado de campos de referencia externos por ID externo

Los campos de referencia externa vinculan registros a objetos de otros sistemas de Adobe (como proyectos o AEM Assets de Workfront). Internamente, Planning asigna los ID de registro de Planning a estos objetos. Para filtrar estos campos directamente por su identificador de objeto original, agregue `"matchExternalId": true` a una condición de filtro.

Este indicador solo es válido para campos de referencia donde `referenceOptions.isExternal` es `true`; se omite para campos de referencia no externos. Si no se puede resolver un solo valor de cadena, la solicitud falla con `400 Bad Request`. Si se proporciona un valor de lista, las entradas sin resolver pasan sin cambios y simplemente no coinciden.

```
{ 
  "filter": { 
    "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<externalReferenceFieldId>", 
        "condition": "IS_ANY_OF", 
        "value": [ 
          "5f6a4f6e00000123456789abcdef0123", 
          "/content/dam/wknd/en/adventures/bali-surf-camp" 
        ], 
        "matchExternalId": true 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
>Nota de la versión 1: La versión 1 no admite el filtrado por ID de objetos externos.

## Campos de conexión externa

Los tipos de registros de Planning pueden alojar campos de referencia externos que vinculen registros a objetos de otros sistemas de Adobe en lugar de otros tipos de registros de Planning.

Para crear un campo de referencia externo a través de la API, establezca `referenceOptions.recordTypeId` en un nuevo campo `REFERENCE` al ID del tipo de registro externo deseado. El servidor deriva automáticamente `referenceOptions.isExternal=true` y los metadatos de conexión (`connectionName, objectName`) del tipo de registro de destino.

Los tipos de objetos externos admitidos son objetos de Workfront (proyectos, tareas, programas, portafolios, empresas, grupos, equipos y usuarios) y AEM Assets (recursos y fragmentos de contenido).

>[!NOTE]
>
>Nota de la versión 1: La versión 1 no admite la creación de campos de conexión externos.


## Orden

Ordene los resultados por cualquier campo incluyendo una matriz `sort` en la solicitud:

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}
```

Los campos de ordenación múltiples se evalúan en orden. Aplique siempre una ordenación al paginar para garantizar un orden coherente entre las páginas.

Para agrupar los resultados, incluya una matriz de grupo junto con el orden:

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 
```

>[!NOTE]
>
>Nota de la versión 1: V1 usa `sorting` (no `sort`), `groupingFieldIds` (matriz de identificadores de campo, no objetos `group`) y el ahora obsoleto `rowOrderViewId` para aplicar el orden de filas de una vista existente. La versión no admite ninguno de estos parámetros V1

## Proyección de campos

Para limitar qué campos se devuelven en una respuesta, utilice los parámetros de consulta `fieldIds` o `fieldAliases` con una lista separada por comas. Esto reduce el tamaño de la carga útil de respuesta y se recomienda para integraciones de gran volumen o sensibles a la latencia.

>[!NOTE]
>
>**Nota de la versión 1:** La versión 1 usa `?attributes=` para la proyección (por ejemplo: `?attributes=data,createdBy`) en lugar de `?fieldIds=` o `?fieldAliases=`.

## Paginación

La API de Planning admite respuestas paginadas para administrar conjuntos de datos grandes.

* **La paginación basada en cursor** se usa para espacios de trabajo, tipos de registro, campos y vistas. Pase un valor `cursor` de la respuesta anterior para recuperar la página siguiente. Las respuestas basadas en cursores incluyen un indicador hasMore para indicar si hay más páginas o no.
* **La paginación basada en páginas** se usa para la búsqueda de registros. Use `page` y `size` como parámetros de consulta. Aplique siempre una ordenación al paginar para garantizar un orden coherente entre las páginas. Tenga en cuenta que la paginación se basa en cero, por lo que para recuperar los resultados de la segunda página, utilice &quot;`page=1`&quot; como parámetro.

Por ejemplo, utilice la siguiente solicitud para recuperar la segunda página de 500 registros de una búsqueda de registros:

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 
```

Todas las respuestas paginadas incluyen un sobre estructurado que indica si hay más resultados disponibles. Aplique siempre una ordenación al paginar para garantizar un orden coherente entre las páginas.

>[!NOTE]
>
> **Nota de la versión 1:** V1 usa `offset` y `limit` pasó en el cuerpo de la solicitud (valor predeterminado 500, máximo 2.000). Para recuperar los registros 2001-4000, establezca &quot;`offset`&quot;: &quot;`2000`&quot;, &quot;`limit`&quot;: &quot;`2000`&quot; en el cuerpo de la solicitud. La respuesta devuelve una matriz de registros planos con un campo `totalCount`.

## Operaciones masivas

La API de Planning admite la creación, actualización, aplicación de parches y eliminación en lotes de registros en una sola solicitud. Consulte la **referencia de API** en [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning) para ver las rutas de extremos, los formatos de solicitud y los límites de registros por operación.

>[!NOTE]
>
>**Nota de la versión 1:** Las operaciones masivas no están disponibles en la versión 1.


## Permisos

Los permisos para entidades se administran mediante una API de permisos dedicada, independiente de los propios extremos de los recursos. Esto le permite leer los permisos actuales, administrar la lista de uso compartido y administrar las solicitudes de acceso independientemente de las operaciones de datos. Para obtener más información, consulte la sección &quot;Referencias de API&quot; en el artículo [API de Workfront Planning](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**Nota de la versión 1:** La versión 1 no expone una API de permisos pública. El nivel de permiso está incrustado directamente en los DTO de respuesta de recursos.

## Uso de la API de Planning con formularios personalizados de Workfront

Puede llamar a la API de Planning desde un campo de búsqueda externa en un formulario personalizado de Workfront para mostrar datos de Planning directamente en objetos de Workfront. Para obtener más información, vea [Ejemplos del campo de búsqueda externa en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Recursos relacionados

Para obtener más documentación relacionada con la API, consulte también los siguientes artículos:

* Documentación y referencia para desarrolladores de la [API de Workfront Planning](https://developer.adobe.com/wf-planning)
* [Introducción a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Información general de acceso a Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)
* [Crear aplicaciones de OAuth2 para integraciones de Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

<!--

Our version of this article before Lilit replaced it with the above: 

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes. 

You can call the planning API from an External lookup field in a Workfront custom form.

For more information on External lookup fields, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>When using the Planning API, all user-related information will be returned using the Adobe Identity Management System (IMS) user ID, and not the Workfront user ID.
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).  

## Workfront Planning API versions

* Version 1 - released in July 2024 

  For more information, see the section [Workfront Planning API Version 1](#workfront-planning-api-version-1) in this article. 

* Version 2 - released in May 2026

  For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.


## Workfront Planning API Version 1

Workfront Planning API Version 1 was released in July 2024.

The following sections described functionality that was made available in the Workfront API Version 1. 

All future API version will contain the same functionality, unless otherwise specified. 

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

#### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
#### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

### Using "And" and "Or" statements 

In the API call you can have filters that are based on several criteria combined by $and" and "$or" statements  

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Using the fields request parameter 

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

returns a response similar to the following: 

  
```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sorting query results in the API 

You can sort your results by any field if you append the following to your API call: 


`/v1/records/search`

Request body:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Query limits and paginated responses 

By default, Planning API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use the `limit` parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding the `offset` parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. 

For example, if you want to return the results 2001-4000, you can use the following request. This example returns 2000 records that are in active status, starting from the 2001st result: 

`POST /v1/records/search`


Request body: 

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. 

For more information on sorting, see [Sorting query results in the API](#sorting-query-results-in-the-api) in this article.


Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->