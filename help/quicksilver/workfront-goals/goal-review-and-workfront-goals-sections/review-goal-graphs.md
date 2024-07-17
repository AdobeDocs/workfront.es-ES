---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Revise los gráficos para comprender las tendencias del progreso de las metas en Adobe Workfront Goals
description: Puede ver el estado general de sus metas y la tendencia de su progreso en el tiempo en la sección Gráficos de las metas de Adobe Workfront. Los gráficos de esta sección no desglosan el progreso de cada objetivo, sino que le proporcionan una instantánea integral del estado del progreso de todas las metas, así como la tendencia del progreso a lo largo del tiempo durante un período especificado.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 0%

---

# Revise los gráficos para comprender las tendencias del progreso de las metas en Adobe Workfront Goals

<!-- drafted mostly for P&P release-->

Puede ver el estado general de sus metas y la tendencia de su progreso en el tiempo en la sección Gráficos de las metas de Adobe Workfront. Los gráficos de esta sección no desglosan el progreso de cada objetivo, sino que le proporcionan una instantánea integral del estado del progreso de todas las metas, así como la tendencia del progreso a lo largo del tiempo durante un período especificado.

>[!IMPORTANT]
>
>Puede ver un recuento total de sus objetivos en la sección Gráficos durante un período de tiempo seleccionado. Sin embargo, Workfront Goals solo tiene en cuenta las metas con un estado de Activo y Cerrado cuando calcula el progreso general de la meta y el porcentaje completado.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> 
   <p>Para el nuevo plan y la estructura de licencias:
  <ul><li>Un plan definitivo </li>
  O
  <li>Licencia adicional para objetivos de Adobe Workfront para los planes Prime o Select Adobe Workfront. </li></ul> </p>
<p>Para el plan y la estructura de licencias actuales: 
<ul><li> A Pro o superior </li>
  <li>Una licencia de Adobe Workfront Goals además de una licencia de Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront*</td>
 <td>
 <p>Nueva licencia: Colaborador o superior</p>
 O
 <p>Licencia actual: Solicitud o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias de Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Producto*</td>
 <td>
 <p> Nuevo requisito de producto, uno de los siguientes: </p>
<ul>
<li>Un plan Select or Prime Adobe Workfront y una licencia adicional de Adobe Workfront Goals.</li>
<li>Un plan Ultimate Workfront que incluye Workfront Goals de forma predeterminada. </li></ul>
 <p>O</p>
 <p>Requisito de producto actual: un plan de Workfront y una licencia adicional para los objetivos de Adobe Workfront. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Nivel de acceso</p></td>
 <td> <p>Editar acceso a Objetivos</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Ver o permisos superiores a la meta para verla</p>
  <p>Administrar permisos para el objetivo y editarlo</p>
  <p>Para obtener información acerca de cómo compartir metas, vea <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Tipos de gráficos en Workfront Goals

Los siguientes gráficos están disponibles en la sección Gráficos o en Workfront Goals:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">El gráfico de estado del objetivo</td> 
   <td> <p>Gráfico de medición que muestra lo siguiente:</p> 
    <ul> 
     <li>Un número total de metas para el período de tiempo seleccionado. Se tienen en cuenta los objetivos con cualquier estado. </li> 
     <li>El estado de progreso de los objetivos con un estado Activo y Cerrado.</li> 
    </ul> <p>Para obtener información acerca de cómo Workfront Goals calcula el estado de progreso, vea <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Información general sobre el progreso y la condición de las metas en Adobe Workfront Goals</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">El gráfico de progreso del objetivo</td> 
   <td> <p>Gráfico de líneas que muestra las actualizaciones realizadas en los objetivos en incrementos semanales durante la duración de la meta. El gráfico de progreso del objetivo muestra lo siguiente:</p> 
    <ul> 
     <li>Un porcentaje completado esperado y real promedio de todas las metas activas y cerradas en el período seleccionado. El progreso del porcentaje completado se desglosa en incrementos semanales marcados por nodos. </li> 
     <li>Porcentaje promedio general de progreso para las metas activas y cerradas desde la semana anterior. </li> 
    </ul> <p>Sugerencia: Es posible que el gráfico de progreso de la meta no muestre ninguna información cuando se realicen actualizaciones en las metas fuera del período de tiempo seleccionado. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Revisar el progreso de la meta en gráficos

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) > **Metas** en la esquina superior derecha.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Se abrirá el área Objetivos de Workfront.

1. Haga clic en **Gráficos** en el panel izquierdo.

   ![](assets/graphs-in-left-panel.png)

   Se muestra la sección Gráficos.

   De forma predeterminada, los objetivos mostrados en la sección Gráficos están limitados por los siguientes criterios:

   * Los filtros aplicados al área de Gráficos.
   * Metas que están en estado Activo y Borrador.

1. (Opcional) Seleccione el tipo de información que desea mostrar actualizando los filtros en la esquina superior derecha de la sección Gráficos.

   Para obtener más información acerca de los objetivos de filtrado, vea [Filtrar información en Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >Si ha seleccionado mostrar más de un período de tiempo, se muestra un gráfico de estado (indicador) así como un gráfico de progreso (línea) para cada período de tiempo.

1. Revise la información de la tabla siguiente cuando revise la Tabla de mantenimiento de objetivos.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Número total de metas | El número en la parte inferior del gráfico indica la cantidad de todas las metas en el período seleccionado, en todos los estados que seleccionó. |
   |---|---|
   | Porcentaje promedio completado | En la parte superior del gráfico, este número indica el porcentaje completado promedio de las metas activas y cerradas en el período de tiempo seleccionado. |
   | Metas y su progreso | El número de objetivos para cada segmento de estado de progreso, cuando pasa el ratón por encima de los segmentos del gráfico. En los segmentos solo se cuentan las metas con estado Activo o Cerrado. |


1. Revise la información de la tabla siguiente cuando revise el gráfico de progreso de objetivos.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Progreso previsto</td> 
      <td>La línea de pendiente verde indica la media de porcentaje completado total esperada de los objetivos activos y cerrados para el período de tiempo seleccionado. Se espera que se completen todas las metas dentro de un periodo, por lo que el progreso de línea de base siempre es del 100 % al final del periodo. </td> 
     </tr> 
     <tr> 
      <td>Progreso real</td> 
      <td> <p>La línea azul indica la media total de porcentaje completado de las metas activas y cerradas para el período de tiempo seleccionado en incrementos semanales. Cada semana durante la duración del objetivo se marca con un nodo en la línea. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Pase el ratón sobre el nodo de una semana en el gráfico de progreso del objetivo y revise lo siguiente:

   * **Fecha de la semana**: El mes, el día y el año de la semana seleccionada.
   * **Progreso**: Un promedio del porcentaje completado real de todas las metas de la semana seleccionada.
   * **Línea de base**: Un promedio del porcentaje esperado completado de todas las metas de la semana seleccionada.

1. (Opcional) Haga clic en **Progreso** en la parte inferior del gráfico de progreso para eliminar la línea de progreso general real

   O

   Haga clic en **Línea de base** en la parte inferior del gráfico de progreso para eliminar el progreso esperado del gráfico.

 
