---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: Agrupar un informe por un campo personalizado de selección múltiple
description: Puede agrupar por el valor de un campo personalizado de selección múltiple en un informe de Adobe Workfront solo con el modo de texto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 530dff59-0d4c-490e-b464-1d3bb1d0f36f
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Agrupar un informe por un campo personalizado de selección múltiple

Puede agrupar por el valor de un campo personalizado de selección múltiple en un informe de Adobe Workfront solo con el modo de texto.

Estos son algunos ejemplos de campos personalizados de selección múltiple:

* Casillas de verificación
* Menús desplegables de selección múltiple

Para obtener información acerca del uso del modo de texto, vea el artículo [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Consideraciones al agrupar por un campo personalizado de selección múltiple

* No se puede crear un gráfico de un informe que utilice una agrupación en modo de texto. Se debe crear un campo calculado adicional que haga referencia al campo personalizado de selección múltiple para representar también gráficamente el informe por el valor del campo personalizado de selección múltiple.

  Para obtener más información, vea [Crear gráficos de un informe mediante un campo personalizado de selección múltiple](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/chart-report-by-multi-select-custom-field.md).
* Los elementos que tengan cualquiera de las opciones seleccionadas se contabilizan solo una vez.

  Por ejemplo, si tiene un campo personalizado Casilla de verificación con la opción 1 y la opción 2 como opciones y adjunta el formulario a las tareas, las tareas que tienen seleccionadas la opción 1 y la opción 2 se agrupan por separado de las tareas que sólo tienen seleccionada la opción 1 o la opción 2.


## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar una agrupación </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una agrupación</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Agrupar un informe por campos personalizados de selección múltiple

Para poder agrupar por un campo personalizado de selección múltiple, debe tener los siguientes requisitos previos:

* Cree el campo personalizado de selección múltiple en un formulario personalizado.\
  Para obtener información sobre cómo crear formularios personalizados y agregarles campos personalizados, consulte el artículo [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Adjuntar el formulario personalizado a objetos.
* Rellene el campo personalizado de selección múltiple con un valor para cada objeto. 

Para agrupar por un campo personalizado de selección múltiple en un informe:

1. Cree un informe o edite uno existente en el que desee agregar una agrupación para un campo personalizado de selección múltiple.\
   Para obtener información sobre cómo crear informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Seleccione la ficha **Agrupaciones**.
1. Haga clic en **Cambiar al modo de texto**.

1. Seleccione el texto en el cuadro **Agrupar su informe** y reemplácelo por el siguiente código:

   <pre>
   group.0.displayname=Nombre de campo personalizado de selección múltiple
   group.0.valueexpression={DE:Nombre de campo personalizado de selección múltiple}
   group.0.valueformat=HTML
   group.0.textmode=true
   </pre>

1. Sustituya &quot;Nombre de campo personalizado de selección múltiple&quot; por el nombre real del campo personalizado de selección múltiple, tal como aparece en Workfront.
1. Haga clic en **Guardar y cerrar**.

   Los objetos del informe se agrupan por los valores del campo personalizado de selección múltiple.

   ![](assets/grouping-by-multi-select-field-text-mode-ui-example.png)

   El nombre de las agrupaciones del informe son los nombres del campo personalizado de selección múltiple seguido de los valores seleccionados en el campo.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Chart a report by multi-select Custom Fields</h2>
<p>(NOTE: this moved to its own article, linked in the Note above!)</p>
<p>You cannot build a chart in a report by referencing a multi-select custom field. Instead, you can create a calculated field that records the values of the multi-select custom field on a given object and group by the calculated field.&nbsp;</p>
<ul>
<li><a href="#build-a-calculated-custom-field-that-references-a-multi-select-custom-field" class="MCXref xref">Build a calculated custom field that references a multi-select custom field</a> </li>
<li><a href="#build-a-chart-that-references-a-calculated-custom-field" class="MCXref xref">Build a chart that references a calculated custom field</a> </li>
</ul>
<p><strong>Build a calculated custom field that references a multi-select custom field</strong></p>
<p>To be able to build a calculated field that references a multi-select custom field, you must have the following prerequisites:</p>
<ul>
<li>Build the multi-select custom field in a custom form.<br>.</li>
<li>Attach the custom form to objects.</li>
<li>Populate the multi-select custom field with a value on each object.</li>
</ul>
<p>To build the calculated custom field that references the multi-select custom field:</p>
<ol>
<li value="1">Create a custom form, or edit an existing one.<br>.</li>
<li value="2">Click<strong>Add a Field</strong>, then <strong>Calculated</strong> to add the multi-select custom field to the form.</li>
<li value="3">In the <strong>Label</strong> box, name the new calculated field to indicate that it references the multi-select custom field.<br>For example: "Calculated Multi-select Field."</li>
<li value="4"> <p>In the <strong>Calculation</strong> box, enter the following code:</p><pre>{DE:Multi-select Custom Field}</pre> <p> <img src="assets/calculated-multi-select-custom-field-350x201.png" style="width: 350;height: 201;"> <br> </p> </li>
<li value="5">Replace "Multi-select Custom Field" with the actual name of your multi-select custom field, as it appears in Workfront.</li>
<li value="6"> <p>(Optional) If the multi-select custom field is already on this form and if this form is already attached to objects, enable the <strong>Update previous calculations</strong>&nbsp;option.</p> <p>This ensures that the new field is automatically populated with the value from the multi-select custom field as it is added to the forms attached to the objects already.</p> </li>
<li value="7">Click <strong>Done</strong>.</li>
<li value="8">Click <strong>Save +Close</strong>.</li>
</ol>
<p><strong>Build a chart that references a calculated custom field</strong></p>
<ol>
<li value="1"> Go to the report where you want to add the chart for the calculated field that references the multi-select custom field. </li>
<li value="2"> (Optional) To ensure that all the calculated fields that you want to chart by are populated with values, select all the objects in your report, then click <strong>Edit</strong>. </li>
<li value="3"> <p> (Optional and conditional) Enable the <strong>Recalculate Custom Expressions</strong> field, then click <strong>Save Changes</strong>.</p> <p> <img src="assets/recalculate-custom-expressions-350x259.png" style="width: 350;height: 259;"> <br> </p> </li>
<li value="4"> Click <strong>Report Actions</strong>, then <strong>Edit</strong>. </li>
<li value="5">Select the <strong>Groupings</strong> tab, then click <strong>Add Grouping</strong>. </li>
<li value="6">Add the<strong>Calculated Multi-select Field</strong> you created as your grouping. </li>
<li value="7"> <p>Select the <strong>Chart</strong> tab, and add a chart to your report.</p> <p>For information about adding a chart to a report, see the section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Add a chart to a report</a> in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li>
<li value="8">Select the <strong>Calculated Multi-select Field</strong> as one of the fields to display in the chart. </li>
<li value="9"> <p>Click <strong>Save + Close</strong>.</p> <p>The report displays the results grouped by the Calculated Multi-select Field in a chart. </p> </li>
</ol>
</div>
-->
