---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Campos personalizados calculados vs. columnas calculadas
description: 'Para acumular varios campos en Adobe Workfront y mostrar ese valor agregado en un nuevo campo, puede hacer lo siguiente: EDITAR ME.'
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Campos personalizados calculados vs. columnas calculadas

Para agregar varios campos en Adobe Workfront y mostrar ese valor agregado en un nuevo campo, puede hacer lo siguiente:

* Un campo personalizado calculado en un formulario personalizado\
   Para obtener más información sobre cómo agregar un campo personalizado calculado a un formulario personalizado, consulte la sección [Agregar un campo calculado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) en el artículo [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Una columna calculada en una vista\
   Para obtener más información sobre el uso de cálculos en una vista, consulte la sección [Uso del modo de texto en las vistas](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) en el artículo [Descripción general de los usos comunes del modo Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Aunque se utiliza el modo de texto para crear campos calculados y columnas calculadas, la sintaxis para crearlos es diferente. Consulte los artículos enumerados anteriormente para aprender a crear campos calculados y columnas calculadas. Para obtener información sobre las distintas sintaxis utilizadas en expresiones de datos calculadas, como columnas y campos personalizados calculados, consulte la sección [Sintaxis de campos personalizados calculados frente a columnas personalizadas calculadas](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns-syntax) en este artículo.

Puede utilizar los mismos cálculos en los campos calculados, así como en una columna calculada. Sin embargo, según el propósito de estos cálculos, puede considerar la posibilidad de crear uno frente al otro.

## Sintaxis de campos personalizados calculados frente a columnas personalizadas calculadas

Aunque las funciones que utiliza son las mismas, la sintaxis para crear una expresión en un campo personalizado calculado puede ser diferente que para crear una columna personalizada calculada.

Por ejemplo:

* En un campo personalizado, en un formulario personalizado para tareas, se utilizaría lo siguiente para generar el nombre del proyecto principal de la tarea donde está adjunto el formulario personalizado:

   ```
   {project}.{name}
   ```

* En una columna personalizada de un informe, utilizaría lo siguiente para agregar una columna personalizada Nombre del proyecto en un informe de tareas:

   ```
   valuefield=project:name
   ```

   O

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >La misma sintaxis se aplica a todos los elementos de informes en modo de texto donde se utilizan expresiones calculadas: vistas, filtros, agrupaciones, mensajes.

Las diferencias entre las dos sintaxis son:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campo personalizado calculado</td> 
   <td>Elemento de informe personalizado calculado</td> 
  </tr> 
  <tr> 
   <td> <p>Utilice el nombre de los campos tal como aparecen en la interfaz de Workfront.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Ejemplo de nombre de campo utilizado en un campo personalizado calculado: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Utilice el nombre de los objetos o campos tal como aparecen en la base de datos de Workfront. Los nombres de los objetos y campos se escriben en minúsculas o en mayúsculas, si son nombres compuestos. </p> <p>Para ver un inventario de todos los objetos y campos de Workfront tal como aparecen en la base de datos, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Ejemplo del nombre de campo utilizado en un elemento de informe personalizado calculado: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Incluir nombres de campo entre paréntesis o llaves</td> 
   <td> <p>No escriba nombres de campo entre corchetes o paréntesis al utilizarlos en una <code>valuefield </code>línea.</p> <p>Rellene los nombres de campo entre llaves al utilizarlos en una <code>valueexpression</code> línea.</p> </td> 
  </tr> 
  <tr> 
   <td>Separe los campos por períodos</td> 
   <td> <p>Separe los campos por dos puntos al utilizarlos en una <code>valuefield </code>line</p> <p>Separe los campos por puntos al utilizarlos en un <code>valueexpression </code>línea. </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre la sintaxis que debe utilizar en una columna personalizada calculada, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Cuándo utilizar campos personalizados calculados

* Cuando desee agrupar los resultados agregados en un informe o mostrar esta información en un gráfico
* Cuando desee acumular los datos más allá de la agregación que se calcula en el campo
* Cuando no le preocupa la puntualidad de los datos, ya que los datos no se actualizan y podrían cambiar con el tiempo

## Acciones que tienen como déclencheur la actualización de un campo personalizado calculado

* En la página principal de un objeto, haga clic en el icono Más ![](assets/more-icon.png)y, a continuación, haga clic en **Volver a calcular expresiones**

* Edición masiva de varios objetos al **Volver a calcular expresiones personalizadas** está habilitado
* Edición de un formulario personalizado al **Actualizar cálculos anteriores** está habilitado para el campo personalizado calculado

## Cuándo utilizar columnas calculadas en una vista

* Cuando desee que los datos en tiempo real estén disponibles en un informe.

   Las vistas calculadas siempre son nuevas, ya que el cálculo se realiza cuando se ejecuta el informe o se aplica la vista.

* Cuando no tiene planes de agrupar por resultados agregados ni utilizar esta información en un gráfico.
* Cuando no planee acumular los datos más allá de la agregación que se calcula en la columna (los datos solo se pueden acumular una vez).
* Cuando desee que el cálculo incluya una referencia a la fecha actual utilizando los comodines $$TODAY o $$AHORA.

   >[!TIP]
   >
   >No utilice esta referencia en campos personalizados calculados porque solo se vuelven a calcular cuando se edita el objeto adjunto. Estos tipos de cálculos quedan obsoletos.

## Ejemplos de columnas y campos personalizados calculados

Para ver ejemplos de campos personalizados calculados, consulte [Datos personalizados calculados en informes](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Para ver ejemplos de columnas personalizadas calculadas en las vistas, consulte los siguientes artículos:

* [Descripción general de los usos comunes del modo Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Ejemplos de vista, filtro y agrupamiento personalizados](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
