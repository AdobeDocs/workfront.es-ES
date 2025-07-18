---
title: Conceptos básicos de API de Adobe Workfront Planning
description: La meta de la API de Adobe Workfront Planning es simplificar la creación de integraciones con la planificación mediante la introducción de una arquitectura REST-ful que funcione a través de HTTP. En este documento se da por hecho que está familiarizado con las respuestas de REST y JSON y se describe el método que utiliza la API de planificación.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 58d2bf9f14b9a3adf4bacfad58f1b9862aeaf247
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 92%

---


# Conceptos básicos de la API de Adobe Workfront Planning

{{planning-important-intro}}

La meta de la API de Adobe Workfront Planning es simplificar la creación de integraciones con la planificación mediante la introducción de una arquitectura REST-ful que funcione a través de HTTP. En este documento se da por hecho que está familiarizado con las respuestas de REST y JSON y se describe el método que utiliza la API de planificación.

Estar familiarizado con el esquema de Workfront Planning le ayudará a comprender las relaciones de la base de datos que se pueden utilizar para extraer datos de Workfront Planning con fines de integración.

Puede llamar a la API de Planning desde un campo de búsqueda externa en un formulario personalizado de Workfront.

Para obtener más información sobre los campos de búsqueda externa, vea [Ejemplos del campo de búsqueda externa en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>Al utilizar la API de Planning, toda la información relacionada con el usuario se devuelve mediante el ID de usuario de Adobe Identity Management System (IMS) y no el ID de usuario de Workfront.
>
>Para obtener más información, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## URL de API de Workfront Planning

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### Operaciones

Los objetos se manipulan enviando una petición HTTP a su URI único. La operación que se va a realizar se especifica mediante el método HTTP.

Los métodos HTTP estándar corresponden a las siguientes operaciones:

* **GET**: recupera un objeto por identificador y busca todos los objetos mediante una consulta
* **POST**: inserta un nuevo objeto
* **PUT**: edita un objeto existente
* **DELETE**: elimina un objeto

Para obtener más detalles y ejemplos de cada operación, consulte la [documentación para desarrolladores de API de Workfront Planning](https://developer.adobe.com/wf-planning/).

### Tipos de campo y modificadores de búsqueda que se utilizan con ellos

Puede utilizar modificadores y filtros con campos para controlar qué datos se devolverán en los resultados.

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### Uso de modificadores de búsqueda

Workfront Planning admite los siguientes modificadores de búsqueda:

<table>
    <tr>
        <td><b>Modificador</b></td>
        <td><b>Ejemplo</b></td>
        <td><b>Descripción</b></td>
        <td><b>Valores posibles</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Devuelve registros cuyo valor de campo contiene el filtro  </td>
        <td>“Nuevo lanzamiento del producto”  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Devuelve registros donde el valor del campo no contiene el filtro  </td>
        <td>“Nuevo lanzamiento”  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Devuelve registros cuyo valor de campo coincida exactamente con el filtro  </td>
        <td>“Nuevo lanzamiento del producto”  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Devuelve registros cuyo valor de campo no coincide exactamente con el filtro  </td>
        <td>“Nuevo lanzamiento del producto”  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Devuelve registros cuyo valor de campo no esté vacío  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Devuelve registros cuyo valor de campo no esté vacío  </td>
        <td>“Nuevo lanzamiento del producto”  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Devuelve registros cuyo valor de campo sea mayor que el filtro  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Devuelve registros cuyo valor de campo sea mayor o igual que el filtro  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Devuelve registros cuyo valor de campo sea menor que el filtro  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Devuelve registros cuyo valor de campo sea menor o igual que el filtro </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Devuelve registros cuyo valor de campo esté después del filtro  </td>
        <td>“2024-05-15T20:00:00.000Z”  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Devuelve registros cuyo valor de campo esté antes del filtro </td>
        <td>“2024-05-12T20:00:00.000Z” </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Devuelve registros cuyo valor de campo esté entre el filtro  </td>
        <td><ul><li>“2024-05-12T20:00:00.000Z” </li><li>“2024-05-14T20:00:00.000Z” </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Devuelve registros cuyo valor de campo no esté entre el filtro  </td>
        <td><ul><li>“2024-05-09T20:00:00.000Z”  </li><li>“2024-05-17T20:00:00.000Z”  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Devuelve registros cuyo valor de campo sea cualquiera de los filtros  </td>
        <td><ul><li>“activo” </li><li>“completed” </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Devuelve registros cuyo valor de campo no sea ninguno del filtro </td>
        <td><ul><li>"finished"  </li><li>"fijo"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Devuelve registros cuyo valor de campo tenga alguno de los filtros  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Devuelve registros cuyo valor de campo tenga todo el filtro  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Devuelve registros cuyo valor de campo no tenga ninguno del filtro </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Devuelve registros cuyo valor de campo sea exactamente el filtro  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>

#### Tipos de campo

A continuación se muestra la lista de tipos de campo admitidos y los modificadores de búsqueda que se pueden utilizar con cada uno de estos tipos de campo

| Tipo de campo | Modificadores de búsqueda admitidos |
|---|---|
| texto | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currrency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| fecha | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| booleano | $is |
| usuario | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| fórmula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| Dirección URL | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depende del campo vinculado |

### Uso de las instrucciones “And” y “Or”

En la llamada de la API puede tener filtros basados en varios criterios combinados por instrucciones $and&quot; y &quot;$or&quot;

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

### Uso del parámetro de solicitud de campos

Puede utilizar el parámetro de solicitud de campos para especificar una lista separada por comas de campos específicos que se deben devolver. Estos nombres de campo distinguen entre mayúsculas y minúsculas.

Por ejemplo, la solicitud

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

devuelve una respuesta similar a la siguiente:


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Ordenar los resultados de consulta en la API

Puede ordenar los resultados por cualquier campo si anexa lo siguiente a la llamada de API:


`/v1/records/search`

Cuerpo de la solicitud:

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

### Límites de consultas y respuestas paginadas

De forma predeterminada, las solicitudes de API de Planning devuelven 500 resultados, empezando desde el principio de la lista. Para anular la limitación predeterminada del número de resultados, puede usar el parámetro `limit` en sus solicitudes y establecerlo en un número diferente, hasta 2000 resultados.

Le recomendamos que considere la posibilidad de utilizar respuestas paginadas para conjuntos de datos grandes añadiendo el parámetro `offset` a sus solicitudes. Las respuestas paginadas le permiten especificar la ubicación del primer resultado que se debe devolver.

Por ejemplo, si desea devolver los resultados 2001-4000, puede utilizar la siguiente solicitud. Este ejemplo devuelve 2000 registros que están en estado activo, a partir del resultado 2001:

`POST /v1/records/search `



Cuerpo de la solicitud:

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

Para asegurarse de que los resultados estén correctamente paginados, utilice un parámetro de ordenación. Esto permite que los resultados se devuelvan en el mismo orden, para que la paginación no se repita ni omita resultados.

Para obtener más información sobre la ordenación, consulte [Ordenar resultados de consultas en la API](#sorting-query-results-in-the-api) en este artículo.
