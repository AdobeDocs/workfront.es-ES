---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Campos personalizados calculados frente a columnas calculadas
description: Para agregar varios campos en Adobe Workfront y mostrar ese valor agregado en un nuevo campo, puede crear un campo personalizado calculado en un formulario personalizado o una columna calculada en una vista.
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Campos personalizados calculados frente a columnas calculadas

Para agregar varios campos en Adobe Workfront y mostrar ese valor agregado en un nuevo campo, puede crear lo siguiente:

* Campo personalizado calculado en un formulario personalizado\
  Para obtener más información sobre cómo agregar un campo personalizado calculado a un formulario personalizado, vea [Agregar campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Una columna calculada en una vista\
  Para obtener más información acerca del uso de cálculos en una vista, vea la sección [Usar el modo de texto en las vistas](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) en el artículo [Información general sobre usos comunes del modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Aunque se utiliza el modo de texto para crear campos calculados y columnas calculadas, la sintaxis para crearlos es diferente. Consulte los artículos enumerados anteriormente para aprender a crear campos calculados y columnas calculadas. Para obtener información acerca de las distintas sintaxis que se usan en las expresiones de datos calculados, como campos personalizados calculados y columnas, vea la sección [Sintaxis de los campos personalizados calculados frente a columnas personalizadas calculadas](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) en este artículo.

Puede utilizar los mismos cálculos en ambos campos calculados, así como en una columna calculada. Sin embargo, según cuál sea el propósito de estos cálculos, puede que desee considerar la posibilidad de crear uno frente al otro.

## Sintaxis de campos personalizados calculados frente a columnas personalizadas calculadas

Aunque las funciones que utiliza son las mismas, la sintaxis para crear una expresión en un campo personalizado calculado puede ser diferente de la que se utiliza para crear una columna personalizada calculada.

Por ejemplo:

* En un campo personalizado, en un formulario personalizado para tareas, debe utilizar lo siguiente para generar el nombre del proyecto principal de la tarea donde se adjunta el formulario personalizado:

  `{project}.{name}`

* En una columna personalizada de un informe, utilizaría lo siguiente para agregar una columna personalizada Nombre del proyecto en un informe de tareas:

  `valuefield=project:name`

  O

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >La misma sintaxis se aplica a todos los elementos de creación de informes en modo de texto donde se utilizan expresiones calculadas: vistas, filtros, agrupaciones y peticiones de datos.

Las diferencias entre las dos sintaxis son las siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizado calculado</strong></td>
   <td><strong>Elemento de informe personalizado calculado</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Utilice el nombre de los campos tal como aparecen en la interfaz de Workfront.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Ejemplo de nombre de campo usado en un campo personalizado calculado: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Utilice el nombre de los objetos o campos tal como aparecen en la base de datos de Workfront. Los nombres de los objetos y campos se escriben en minúsculas o en minúscula, si son nombres compuestos. </p> <p>Para obtener un inventario de todos los objetos y campos de Workfront tal como aparecen en la base de datos, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Ejemplo de nombre de campo utilizado en un elemento de informe personalizado calculado: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Escriba los nombres de los campos entre paréntesis o llaves</td> 
   <td> <p>No escriba los nombres de los campos entre corchetes o paréntesis cuando los utilice en una línea <code>valuefield </code>.</p> <p>Escriba los nombres de los campos entre llaves cuando los utilice en una línea de <code>valueexpression</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Separar los campos por puntos</td> 
   <td> <p>Separe los campos por dos puntos cuando los utilice en una línea <code>valuefield</code>.</p> <p>Separe los campos por puntos cuando los utilice en una línea <code>valueexpression</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información acerca de la sintaxis que debe usar en una columna personalizada calculada, vea [Introducción al modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Cuándo utilizar campos personalizados calculados

* Cuando desee agrupar los resultados agregados en un informe o mostrar esta información en un gráfico
* Si desea agregar los datos más allá de la agregación que se calcula en el campo
* Cuando no le preocupe la puntualidad de los datos, ya que estos no se actualizan y podrían cambiar con el tiempo

## Acciones que almacenan en déclencheur la actualización de un campo personalizado calculado

* En la página principal de un objeto, haga clic en el icono Más ![](assets/more-icon.png) y, a continuación, en **Volver a calcular expresiones**

* Edición masiva de varios objetos cuando **Volver a calcular expresiones personalizadas** está habilitado
* Editar un formulario personalizado cuando **Actualizar cálculos anteriores** está habilitado para el campo personalizado calculado

## Cuándo utilizar columnas calculadas en una vista

* Si desea que los datos en tiempo real estén disponibles en un informe.

  Las vistas calculadas siempre son nuevas porque el cálculo se realiza cuando se ejecuta el informe o se aplica la vista.

* Cuando no tenga planes de agrupar por resultados agregados ni utilice esta información en un gráfico.
* Cuando no planea acumular los datos más allá de la agregación calculada en la columna (los datos solo se pueden acumular una vez).
* Cuando desee que el cálculo incluya una referencia a la fecha actual utilizando los comodines $$TODAY o $$NOW.

  >[!TIP]
  >
  >No utilice esta referencia en campos personalizados calculados porque sólo se vuelven a calcular cuando se edita el objeto adjunto. Estos tipos de cálculos quedan obsoletos.

## Ejemplos de campos personalizados calculados y columnas

Para ver ejemplos de campos personalizados calculados, vea [Datos personalizados calculados en los informes](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Para ver ejemplos de columnas personalizadas calculadas en vistas, consulte los siguientes artículos:

* [Información general sobre usos comunes del modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Ejemplos de vistas, filtros y agrupaciones personalizadas: índice de artículos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
