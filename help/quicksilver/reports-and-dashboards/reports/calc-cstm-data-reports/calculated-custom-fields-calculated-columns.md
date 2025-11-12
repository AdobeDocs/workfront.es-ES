---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Campos personalizados calculados frente a columnas calculadas
description: Para agregar varios campos en Adobe Workfront y mostrar ese valor agregado en un nuevo campo, puede crear un campo personalizado calculado en un formulario personalizado o una columna calculada en una vista.
author: Jenny
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: ce986a912c2ee231b9dc2e1c7a3e9587b20aa0ba
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 93%

---

# Campos personalizados calculados frente a columnas calculadas

Para agregar varios campos en Adobe Workfront y mostrar ese valor agregado en un nuevo campo, puede crear lo siguiente:

* Un campo personalizado calculado en un formulario personalizado\
  Para obtener más información sobre cómo añadir un campo personalizado calculado a un formulario personalizado, consulte [Añadir campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Una columna calculada en una vista\
  Para obtener más información sobre el uso de cálculos en una vista, consulte la sección [Usar el modo de texto en las vistas](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) en el artículo [Información general sobre usos comunes del modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Aunque utilice el modo de texto para generar campos calculados y columnas calculadas, la sintaxis para generarlos es diferente. Consulte los artículos enumerados anteriormente para obtener más información sobre la generación de campos calculados y columnas calculadas. Para obtener información acerca de la distinta sintaxis que se usa en las expresiones de datos calculados, como campos personalizados calculados y columnas calculadas, consulte la sección [Sintaxis de campos personalizados calculados frente a columnas personalizadas calculadas](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) en este artículo.

Puede utilizar los mismos cálculos en ambos campos calculados, así como en una columna calculada. Sin embargo, según cuál sea el propósito de estos cálculos, podría considerar si le interesa generar uno u otro.

## Sintaxis de campos personalizados calculados frente a columnas personalizadas calculadas

Aunque las funciones que se utilizan son las mismas, la sintaxis para crear una expresión en un campo personalizado calculado puede ser diferente de la que se utiliza para crear una columna personalizada calculada.

Por ejemplo:

* En un campo personalizado, en un formulario personalizado para tareas, se utilizaría lo siguiente para generar el nombre del proyecto principal de la tarea donde se adjunta el formulario personalizado:

  `{project}.{name}`

* En una columna personalizada de un informe, se utilizaría lo siguiente para añadir una columna personalizada Nombre del proyecto en un informe de tareas:

  `valuefield=project:name`

  O

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >La misma sintaxis se aplica a todos los elementos de creación de informes en modo de texto donde se utilizan expresiones calculadas: vistas, filtros, agrupaciones e indicaciones.

Las diferencias entre las dos sintaxis son:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizado calculado</strong></td>
   <td><strong>Elemento de creación de informe personalizado calculado</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Utilice el nombre de los campos tal como aparecen en la interfaz de Workfront.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>ejemplo de nombre de campo usado en un campo personalizado calculado: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Utilice el nombre de los objetos o campos tal como aparecen en la base de datos de Workfront. Los nombres de los objetos y campos se escriben en minúsculas o en mayúsculas/minúsculas, si son nombres compuestos. </p> <p>Para obtener un inventario de todos los objetos y campos de Workfront tal como aparecen en la base de datos, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>ejemplo de nombre de campo utilizado en un elemento de creación de informe personalizado calculado: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Escriba los nombres de los campos entre paréntesis o llaves</td> 
   <td> <p>No escriba los nombres de los campos entre corchetes o paréntesis cuando los utilice en una línea <code>valuefield </code>.</p> <p>Escriba los nombres de los campos entre llaves cuando los utilice en una línea <code>valueexpression</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Separe los campos con puntos</td> 
   <td> <p>Separe los campos con dos puntos cuando los utilice en una línea <code>valuefield</code>.</p> <p>Separe los campos por puntos cuando los utilice en una línea <code>valueexpression</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información acerca de la sintaxis que debe usar en una columna personalizada calculada, consulte [Información general del modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Cuándo se deben utilizar campos personalizados calculados

* Cuando desee agrupar los resultados agregados en un informe o mostrar esta información en un gráfico
* Cuando desee agregar los datos más allá de la agregación que se calcula en el campo
* Cuando no le preocupe la precisión de los datos, ya que esos datos no se actualizan y podrían cambiar con el tiempo

## Acciones que activan la actualización de un campo personalizado calculado

* En la página principal de un objeto, haga clic en el icono Más ![Icono Más](assets/more-icon.png) y, a continuación, haga clic en **Volver a calcular expresiones**

* Edición masiva de varios objetos cuando **Volver a calcular expresiones personalizadas** está habilitado.
* Edición masiva de varios objetos al hacer clic en **Volver a calcular expresiones** desde el menú Más en una lista de objetos.
* Editar un formulario personalizado cuando **Actualizar cálculos anteriores** está habilitado para el campo personalizado calculado.

Para obtener más información, consulte [Editar información en campos de formulario personalizados](/help/quicksilver/workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Cuándo se deben utilizar columnas calculadas en una vista

* Cuando desee que los datos en tiempo real estén disponibles en un informe.

  Las vistas calculadas siempre están actualizadas porque el cálculo se realiza cuando se ejecuta el informe o se aplica la vista.

* Cuando no tenga planes de agrupar por resultados agregados ni de utilizar esta información en un gráfico.
* Cuando no planee agregar los datos más allá de la agregación calculada en la columna (los datos solo se pueden agregar una vez).
* Cuando desee que el cálculo incluya una referencia a la fecha actual utilizando los comodines $$TODAY o $$NOW.

  >[!TIP]
  >
  >No utilice esta referencia en campos personalizados calculados porque solo se vuelven a calcular cuando se edita el objeto adjunto. Estos tipos de cálculos quedan obsoletos.

## Ejemplos de campos personalizados calculados y columnas

Para ver ejemplos de campos personalizados calculados, consulte [Datos personalizados calculados en informes](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Para ver ejemplos de columnas personalizadas calculadas en vistas, consulte los siguientes artículos:

* [Información general sobre los usos comunes del modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Ejemplos de vistas, filtros y agrupaciones personalizados: índice de artículos](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
