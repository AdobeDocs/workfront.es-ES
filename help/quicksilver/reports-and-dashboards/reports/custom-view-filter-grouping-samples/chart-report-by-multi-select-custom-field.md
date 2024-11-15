---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Trazar un informe con un campo personalizado de selección múltiple
description: Puede crear un gráfico de un informe mediante un campo personalizado de selección múltiple solo después de crear un campo calculado adicional que capture las opciones seleccionadas en el campo personalizado de selección múltiple.
author: Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 66de6c952272f52876f8e912c96d1526575b6f0b
workflow-type: tm+mt
source-wordcount: '1004'
ht-degree: 0%

---

# Crear un gráfico de un informe utilizando un campo personalizado de selección múltiple

<!--Audited: 11/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

En lugar de crear un gráfico con un campo personalizado de selección múltiple, se recomienda crear campos independientes para cada opción de un campo personalizado de selección múltiple.

Estos son algunos ejemplos de campos personalizados de selección múltiple:

* Casillas de verificación
* Menús desplegables de selección múltiple

Para obtener información acerca del uso del modo de texto, vea el artículo [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Sin embargo, si no es posible tener campos independientes para cada opción de un campo de selección múltiple, puede crear un gráfico de un informe por un campo personalizado de selección múltiple utilizando campos personalizados calculados para agrupar primero las opciones del campo de selección múltiple. Después, puede crear un gráfico del informe según los campos calculados.

>[!NOTE]
>
>Los elementos que tengan cualquiera de las opciones seleccionadas se contabilizan solo una vez.
>
>Por ejemplo, si tiene un campo personalizado Casilla de verificación con la opción 1 y la opción 2 como opciones y adjunta el formulario a las tareas, las tareas que tienen la opción 1 y la opción 2 se muestran en un elemento de gráfico independiente al de las tareas que sólo tienen seleccionada la opción 1 o la opción 2.
>
>Las tareas que tienen la Opción 1 seleccionada no se muestran en el mismo elemento de gráfico que las tareas que tienen la Opción 1 y la Opción 2 seleccionadas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de empezar, debe crear un campo personalizado calculado que muestre los valores seleccionados del campo personalizado de selección múltiple. Para obtener más información, consulte la sección [Crear un campo personalizado calculado que haga referencia a un campo personalizado de selección múltiple](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) en este artículo.

## Crear gráficos de un informe mediante campos personalizados de selección múltiple

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

No se puede crear un gráfico en un informe haciendo referencia a un campo personalizado de selección múltiple. En su lugar, puede crear un campo calculado que registre los valores del campo personalizado de selección múltiple en un objeto determinado y agrupar por el campo calculado. 

* [Crear un campo personalizado calculado que haga referencia a un campo personalizado de selección múltiple](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Crear un gráfico que haga referencia a un campo personalizado calculado](#build-a-chart-that-references-a-calculated-custom-field)

### Crear un campo personalizado calculado que haga referencia a un campo personalizado de selección múltiple {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Para generar un campo calculado que haga referencia a un campo personalizado de selección múltiple, debe cumplir los siguientes requisitos previos:

* Campo personalizado de selección múltiple en un formulario personalizado.\
  Para obtener información sobre cómo crear formularios personalizados y agregarles campos personalizados, consulte el artículo [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Un formulario personalizado con el campo personalizado de selección múltiple adjunto a los objetos.
* Valores del campo personalizado de selección múltiple para cada objeto.

Para generar el campo personalizado calculado que hace referencia al campo personalizado de selección múltiple:

1. Cree un formulario personalizado o edite uno existente.

   Para obtener información sobre cómo crear formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Seleccione el objeto u objetos que planea utilizar con el formulario personalizado.
1. Haga clic en **Agregar campo** y después en **Calculado** para agregar el campo personalizado de selección múltiple al formulario.

1. En el cuadro **Etiqueta**, asigne un nombre al nuevo campo calculado para indicar que hace referencia al campo personalizado de selección múltiple.

   Por ejemplo: &quot;Campo de selección múltiple calculado&quot;.

1. En el cuadro **Cálculo**, escriba el siguiente código:

   `{DE:Multi-select Custom Field}`

   Esto agrega las opciones seleccionadas en el campo personalizado de selección múltiple al campo personalizado calculado. Por ejemplo, si el formulario está adjunto a tareas y la opción 1 está seleccionada en el campo personalizado de selección múltiple, el campo personalizado calculado muestra el valor &quot;Opción 1&quot;. Si las opciones 1 y 2 están seleccionadas para una tarea diferente, el campo personalizado calculado muestra el valor &quot;Opción 1, Opción 2&quot;.

1. Sustituya &quot;Campo personalizado de selección múltiple&quot; por el nombre real del campo personalizado de selección múltiple, tal como aparece en Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Opcional) Si el campo personalizado de selección múltiple ya está en este formulario y si este formulario ya está adjunto a objetos, habilite la opción **Aplicar a cálculos existentes**.

   Esto garantiza que el nuevo campo calculado se rellene automáticamente con el valor del campo personalizado de selección múltiple a medida que se agrega a los formularios ya adjuntos a los objetos.

1. Haga clic en **Aplicar**.
1. Haga clic en **Guardar y cerrar**.

   El campo personalizado calculado se agrega al formulario personalizado y, si el formulario está adjunto actualmente a objetos, el campo se rellena con información del campo personalizado de selección múltiple.

### Crear un gráfico que haga referencia a un campo personalizado calculado {#build-a-chart-that-references-a-calculated-custom-field}

1. (Opcional) Para asegurarse de que todos los campos calculados por los que desea crear un gráfico se rellenen con valores, en la pestaña Detalles del informe, seleccione todos los objetos que contienen el formulario personalizado con el campo personalizado de selección múltiple y el campo personalizado calculado y, a continuación, haga clic en **Editar**.
1. (Opcional y condicional) Seleccione el campo **Volver a calcular expresiones personalizadas** y, a continuación, haga clic en **Guardar cambios**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >Esta opción se ha eliminado de la edición de proyectos por lotes.  Puede seguir recalculando expresiones para proyectos por lotes haciendo clic en el icono **Más** ![](assets/more-icon-45x33.png) en la parte superior de una lista de proyectos y, a continuación, en **Volver a calcular expresiones**.

1. Vaya al informe donde desee agregar el gráfico para el campo calculado que hace referencia al campo personalizado de selección múltiple.
1. Haga clic en **Acciones de informe** y luego en **Editar**.

1. Seleccione la ficha <strong>Agrupaciones</strong> y, a continuación, haga clic en <strong>Agregar agrupación</strong>.
1. Agregue el <strong>Campo de selección múltiple calculado</strong> que creó como agrupación.
1. Seleccione la ficha <strong>Gráfico</strong> y agregue un gráfico al informe.

   Por ejemplo, elija un gráfico de **columnas**.
   <br>Para obtener información sobre cómo agregar un gráfico a un informe, consulte la sección <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Agregar un gráfico a un informe</a> en el artículo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Crear un informe personalizado</a>.
1. En el campo **Eje inferior (X)**, seleccione el <strong>Campo de selección múltiple calculado</strong> que se mostrará en el gráfico.
1. Haga clic en <strong>Guardar + Cerrar</strong>.

   El informe muestra los resultados agrupados por el Campo de selección múltiple calculado en un gráfico.

   ![](assets/chart-multi-select-field-column-chart-example.png)