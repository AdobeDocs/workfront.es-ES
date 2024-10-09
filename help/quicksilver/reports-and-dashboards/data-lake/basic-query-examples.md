---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Ejemplos de consultas de Data Connect
description: Consultas de ejemplo que puede utilizar para familiarizarse con la sintaxis y la estructura de tipos específicos de consultas.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Ejemplos de consultas de Workfront Data Connect

Para ayudarle a utilizar mejor los datos de Workfront Data Connect, esta página contiene consultas de ejemplo básicas que puede utilizar para familiarizarse con la sintaxis y la estructura de tipos específicos de consultas.

## Consulta de datos personalizados

En este ejemplo se muestra cómo crear una consulta para devolver los datos personalizados en Workfront, como formularios y campos personalizados.

### Escenario:

Su organización utiliza un formulario personalizado denominado Integración financiera. El formulario se adjunta a cada proyecto y contiene los campos siguientes:

* **Unidad de negocio** - Campo personalizado que contiene una cadena.
* **ProjectID**: campo personalizado que contiene una cadena numérica.
* **Nombre de proyecto expandido**: un campo de datos personalizados calculados que concatena los valores de unidad de negocio, identificador de proyecto y el nombre de proyecto nativo de Workfront en una sola cadena.

Debe incluir esta información en la respuesta para una consulta contra Data Connect. Los valores de datos personalizados para un registro del lago de datos se encuentran en una columna denominada `parametervalues`. Esta columna se almacena como un objeto JSON.

### Consulta:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Respuesta:

La consulta anterior devuelve los siguientes datos:

* `projectid`: el ID de proyecto nativo de Workfront
* `parametervalues`: una columna que almacena un objeto JSON
* `name`: el nombre nativo del proyecto de Workfront
* `Business Unit`: un valor de datos personalizado que se incluye en el objeto `parametervalues`
* `Project ID`: un valor de datos personalizado que se incluye en el objeto `parametervalues`
* `Expanded Project Name`: un valor de datos personalizado que se incluye en el objeto `parametervalues`

### Explicación:

Al consultar el objeto JSON `parametervalues`, se puede acceder a cada campo de datos personalizado como una columna mediante lo siguiente:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` es el nombre del objeto JSON en la tabla que se está consultando. En el caso de los datos personalizados, siempre será `parametervalues`.
* `<parameter_name>` es la cadena `parametername` que se encuentra en la herramienta de configuración de formularios, aunque no siempre coincide con este valor.

>[!NOTE]
>
>Si el nombre del parámetro se cambia en la herramienta de configuración de formularios de Workfront, se representará como una nueva columna en el objeto JSON. Por lo tanto, se recomienda no cambiar el nombre de una columna una vez que se haya creado en la herramienta de configuración de formularios. Sin embargo, la etiqueta se puede cambiar sin afectar al objeto JSON.
>
>Si la cadena de texto del nombre del parámetro es incorrecta, la columna devolverá un valor NULL, en lugar de un error.

* `<data_type>` convierte el valor devuelto por el objeto JSON en un tipo de datos apropiado para el campo. Si se elige un tipo de datos incompatible para el valor que se devuelve, se producirá un error de no coincidencia de tipos de datos. Los tipos de datos posibles incluyen:

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (por ejemplo, `Number(32,4)` devolvería 1234.0987)
   * `date`
   * `timestamp`

* `<column_name>` es la etiqueta que crea para cada columna de datos personalizada.

>[!NOTE]
>
>Solo se incluirán en el objeto JSON los parámetros que tengan valores asignados en el formulario. Si un campo de datos personalizados está vacío en el formulario, no aparecerá.

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
