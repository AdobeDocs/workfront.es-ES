---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Revisar gráficos para comprender las tendencias de progreso de los objetivos en los objetivos de Adobe Workfront
description: Puede ver el estado general de sus metas y su tendencia de progreso en el tiempo en la sección Gráficos de Adobe Workfront Goals. Los gráficos de esta sección no desglosan el progreso de cada meta, sino que le proporcionan una instantánea integral del estado de progreso de todas las metas, así como su tendencia de progreso a lo largo del tiempo durante un período especificado.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: a64f6e507d74201cba1455fbbc6af77c2b7ba058
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 94%

---

# Revise los gráficos para comprender las tendencias del progreso de las metas en Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Puede ver el estado general de sus metas y su tendencia de progreso en el tiempo en la sección Gráficos de Adobe Workfront Goals. Los gráficos de esta sección no desglosan el progreso de cada meta, sino que le proporcionan una instantánea integral del estado de progreso de todas las metas, así como su tendencia de progreso a lo largo del tiempo durante un período especificado.

>[!IMPORTANT]
>
>Puede ver un recuento total de sus metas en la sección Gráficos durante un período de tiempo seleccionado. Sin embargo, Workfront Goals solo tiene en cuenta las metas en estado Activo y Cerrado cuando calcula el estado de progreso general de la meta y el porcentaje completado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> 
   <p>Para la nueva estructura de plan y licencias:
  <ul><li>Un plan Ultimate </li></ul>
   </p>
<p>Para la estructura actual de plan y licencias: 
<ul><li> Pro o superior </li>
  <li>Una licencia de Adobe Workfront Goals además de una licencia de Workfront.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront*</td>
 <td>
 <p>Nueva licencia: Contributor o superior</p>
 O
 <p>Licencia actual: Request o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Producto*</td>
 <td>
    <p> Nuevo requisito de producto: Workfront</p>
    O
    <p>Requisito actual del producto: además de una licencia de Workfront, debe adquirir una licencia para Adobe Workfront Goals. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Nivel de acceso</p></td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Permisos Ver o superiores para la meta que desea ver</p>
  <p>Permisos de administración para la meta y poder editarla</p>
  <p>Para obtener información acerca de cómo compartir metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Metas en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de gráficos en Workfront Goals

Los siguientes gráficos están disponibles en la sección Gráficos de Workfront Goals:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Gráfico de estado de la meta</td> 
   <td> <p>Un gráfico de medición que muestra lo siguiente:</p> 
    <ul> 
     <li>El número total de metas para el período de tiempo seleccionado. Se tienen en cuenta las metas con cualquier estado. </li> 
     <li>El estado de progreso de las metas en estado Activo y Cerrado.</li> 
    </ul> <p>Para obtener información sobre cómo Workfront Goals calcula el estado de progreso, consulte <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Información general sobre el progreso de las metas y su condición en Adobe Workfront Goals</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gráfico de progreso de la meta</td> 
   <td> <p>Un gráfico de líneas que muestra las actualizaciones realizadas en las metas por incrementos semanales durante la duración de la meta. El gráfico de progreso de la meta muestra lo siguiente:</p> 
    <ul> 
     <li>El porcentaje completado esperado y real promedio de todas las metas activas y cerradas en el período seleccionado. El progreso de porcentaje completado se desglosa por incrementos semanales marcados mediante nodos. </li> 
     <li>El porcentaje promedio general de progreso para las metas activas y cerradas desde la semana anterior. </li> 
    </ul> <p>Sugerencia: Es posible que el gráfico de progreso de la meta no muestre ninguna información cuando se realicen actualizaciones en las metas fuera del período de tiempo seleccionado. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Revisión del progreso de la meta en gráficos

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) > **Metas** en la esquina superior derecha.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Se abrirá el área Metas de Workfront.

1. Haga clic en **Gráficos** en el panel izquierdo.

   ![Gráficos en el panel izquierdo](assets/graphs-in-left-panel.png)

   Se muestra la sección Gráficos.

   De forma predeterminada, las metas mostradas en la sección Gráficos están limitadas por los siguientes criterios:

   * Los filtros aplicados al área Gráficos.
   * Las metas que están en estado Activo y Borrador.

1. (Opcional) Seleccione el tipo de información que desee mostrar actualizando los filtros en la esquina superior derecha de la sección Gráficos.

   Para obtener más información sobre el filtrado de las metas, consulte [Filtrar información en Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >Si ha seleccionado mostrar más de un período de tiempo, se muestra un gráfico de estado (medición) así como un gráfico de progreso (línea) para cada período de tiempo.

1. Revise la información de la tabla siguiente cuando revise el gráfico de estado de la meta.

   ![Gráfico de medición](assets/gauge-graph-wf-align-350x230.png)

   | Número total de metas | El número en la parte inferior del gráfico indica la cantidad de todas las metas en el período seleccionado, en todos los estados que haya seleccionado. |
   |---|---|
   | Porcentaje completado promedio | En la parte superior del gráfico, este número indica el porcentaje completado promedio de las metas activas y cerradas en el período de tiempo seleccionado. |
   | Metas y su progreso | El número de metas para cada segmento de estado de progreso, al pasar el puntero por encima de los segmentos del gráfico. En los segmentos solo se cuentan las metas con estado Activo o Cerrado. |


1. Revise la información de la tabla siguiente cuando revise el gráfico de progreso de la meta.

   ![Gráfico de líneas](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Progreso de línea de base</td> 
      <td>La línea de pendiente en color verde indica el promedio del porcentaje completado total esperado de las metas activas y cerradas para el período de tiempo seleccionado. Se espera que se completen todas las metas dentro de un período, por lo que el progreso de línea de base siempre es del 100 % al final del período. </td> 
     </tr> 
     <tr> 
      <td>Progreso real</td> 
      <td> <p>La línea azul indica el promedio total real del porcentaje completado de las metas activas y cerradas para el período de tiempo seleccionado por incrementos semanales. Cada semana durante la duración de la meta se marca mediante un nodo en la línea. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Pase el puntero por encima del nodo de una semana en el gráfico de progreso de la meta y revise lo siguiente:

   * **Fecha de la semana**: mes, día y año de la semana seleccionada.
   * **Progreso**: promedio del porcentaje completado real de todas las metas de la semana seleccionada.
   * **Línea de base**: promedio del porcentaje completado esperado de todas las metas de la semana seleccionada.

1. (Opcional) Haga clic en **Progreso** en la parte inferior del gráfico de progreso para quitar la línea de progreso total real

   O

   Haga clic en **Línea de base** en la parte inferior del gráfico de progreso para quitar el progreso esperado del gráfico.

 
