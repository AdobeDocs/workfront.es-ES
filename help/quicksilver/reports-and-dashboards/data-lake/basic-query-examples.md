---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Ejemplos de consultas de Data Connect
description: Consultas de ejemplo que puede utilizar para familiarizarse con la sintaxis y la estructura de tipos específicos de consultas.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 84f7f80314e4acafb0414b806f7b1e1e4b2845fc
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Ejemplos de consultas de Workfront Data Connect

Para ayudarle a utilizar mejor los datos de Workfront Data Connect, esta página contiene consultas de ejemplo básicas que puede utilizar para familiarizarse con la sintaxis y la estructura de tipos específicos de consultas.

## Consulta de datos personalizados

En este ejemplo se muestra cómo crear una consulta para devolver los datos personalizados en Workfront, como formularios y campos personalizados.

### Escenario:

Su organización que utiliza un formulario personalizado denominado Integración financiera. El formulario se adjunta a cada proyecto y contiene los campos siguientes:

* **Unidad de negocio** - Campo personalizado que contiene una cadena.
* **ProjectID**: campo personalizado que contiene una cadena numérica.
* **Nombre de proyecto expandido**: un campo de datos personalizados calculados que concatena los valores de unidad de negocio, identificador de proyecto y el nombre de proyecto nativo de Workfront en una sola cadena.

Debe incluir esta información en la respuesta para una consulta contra Data Connect. Los valores de datos personalizados para un registro del lago de datos se encuentran en una columna denominada `parameterValues`. Esta columna se almacena como un objeto JSON.

### Consulta:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit" :: int as BusinessUnit,
    parametervalues:"DE:Project ID" :: int as ProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Respuesta

La consulta anterior devuelve los siguientes datos:

* `projectid`: el ID de proyecto nativo de Workfront
* `parametervalues`: una columna que almacena un objeto JSON
* `name`: el nombre nativo del proyecto de Workfront
* `Business Unit`: un valor de datos personalizado que se incluye en el objeto `parametervalues`
* `Project ID`: un valor de datos personalizado que se incluye en el objeto `parametervalues`
* `Expanded Project Name`: un valor de datos personalizado que se incluye en el objeto `parametervalues`

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
