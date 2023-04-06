---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Gráfico de un informe mediante un campo personalizado de selección múltiple
description: No se puede graficar un informe mediante un campo personalizado de selección múltiple. Se debe crear un campo calculado adicional que haga referencia al campo personalizado de selección múltiple para que también se muestre el informe según el valor del campo personalizado de selección múltiple.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Gráfico de un informe mediante un campo personalizado de selección múltiple

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

No se puede graficar un informe mediante un campo personalizado de selección múltiple. Se debe crear un campo calculado adicional que haga referencia al campo personalizado de selección múltiple para que también se muestre el informe según el valor del campo personalizado de selección múltiple.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de comenzar, debe crear un campo personalizado calculado que muestre los valores seleccionados del campo personalizado de selección múltiple. Para obtener más información, consulte la [Generar un campo personalizado calculado que haga referencia a un campo personalizado de selección múltiple](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) en este artículo.

## Gráfico de un informe mediante la selección múltiple de Campos personalizados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

No se puede crear un gráfico en un informe haciendo referencia a un campo personalizado de selección múltiple. En su lugar, puede crear un campo calculado que registre los valores del campo personalizado de selección múltiple en un objeto determinado y agrupar por el campo calculado. 

* [Generar un campo personalizado calculado que haga referencia a un campo personalizado de selección múltiple](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Crear un gráfico que haga referencia a un campo personalizado calculado](#build-a-chart-that-references-a-calculated-custom-field)

### Generar un campo personalizado calculado que haga referencia a un campo personalizado de selección múltiple {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Para poder generar un campo calculado que haga referencia a un campo personalizado de selección múltiple, debe tener los siguientes requisitos previos:

* Genere el campo personalizado de selección múltiple en un formulario personalizado.\
   Para obtener información sobre la creación de formularios personalizados y la adición de campos personalizados, consulte el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* Adjunte el formulario personalizado a los objetos.
* Rellene el campo personalizado de selección múltiple con un valor en cada objeto.

Para generar el campo personalizado calculado que hace referencia al campo personalizado de selección múltiple:

1. Cree un formulario personalizado o edite uno existente.\
   Para obtener información sobre la creación de formularios personalizados, consulte el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Seleccione el objeto u objetos que va a utilizar con el formulario personalizado.
1. Haga clic en **Agregar un campo**, luego **Calculado** para agregar al formulario el campo personalizado de selección múltiple.

1. En el **Etiqueta** , asigne un nombre al nuevo campo calculado para indicar que hace referencia al campo personalizado de selección múltiple.\
   Por ejemplo: &quot;Campo de selección múltiple calculado.&quot;

1. En el **Cálculo** introduzca el siguiente código:

   ```
   {DE:Multi-select Custom Field}
   ```

1. Sustituya &quot;Campo personalizado de selección múltiple&quot; por el nombre real de su campo personalizado de selección múltiple, como aparece en Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Opcional) Si el campo personalizado de selección múltiple ya está en este formulario y si este formulario ya está adjunto a objetos, habilite la variable **Actualizar cálculos anteriores** .\
   Esto garantiza que el nuevo campo se rellene automáticamente con el valor del campo personalizado de selección múltiple, ya que se agrega a los formularios adjuntos a los objetos.

1. Haga clic en **Listo**.
1. Haga clic en **Guardar + Cerrar**.

### Crear un gráfico que haga referencia a un campo personalizado calculado {#build-a-chart-that-references-a-calculated-custom-field}

1. (Opcional) Para asegurarse de que todos los campos calculados por los que desea crear un gráfico se rellenen con valores, seleccione todos los objetos del informe que contengan el formulario personalizado con el campo personalizado de selección múltiple y el campo personalizado calculado y, a continuación, haga clic en **Editar**.
1. (Opcional y condicional) Habilite la variable **Volver a calcular expresiones personalizadas** y, a continuación, haga clic en **Guardar cambios**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >Esta opción se ha eliminado de la edición de proyectos de forma masiva.  Puede volver a calcular expresiones para proyectos de forma masiva haciendo clic en el botón **Más** icono ![](assets/more-icon-45x33.png) en la parte superior de una lista de proyectos, **Volver a calcular expresiones**.


1. Vaya al informe donde desee agregar el gráfico para el campo calculado que hace referencia al campo personalizado de selección múltiple.
1. Haga clic en **Acciones de informe**, luego **Editar**.

1. Seleccione el <strong>Agrupaciones</strong> a continuación, haga clic en <strong>Agregar agrupación</strong>.
1. Agregue la variable<strong>Campo de selección múltiple calculado</strong> se ha creado como agrupación.
1. Seleccione el <strong>Gráfico</strong> y añada un gráfico al informe.<br>Para obtener información sobre cómo agregar un gráfico a un informe, consulte la sección <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Agregar un gráfico a un informe</a> en el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.
1. Seleccione el <strong>Campo de selección múltiple calculado</strong> como uno de los campos que se van a mostrar en el gráfico.
1. Haga clic en <strong>Guardar + Cerrar</strong>.<br>El informe muestra los resultados agrupados por el campo Selección múltiple calculada en un gráfico.
