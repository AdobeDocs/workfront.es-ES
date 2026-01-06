---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Revisar gráficos para comprender las tendencias de progreso de los objetivos en los objetivos de Adobe Workfront
description: Puede ver el estado general de sus metas y su tendencia de progreso en el tiempo en la sección Gráficos de Adobe Workfront Goals. Los gráficos de esta sección no desglosan el progreso de cada meta, sino que le proporcionan una instantánea integral del estado de progreso de todas las metas, así como su tendencia de progreso a lo largo del tiempo durante un período especificado.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 82%

---

# Revise los gráficos para comprender las tendencias del progreso de las metas en Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Puede ver el estado general de sus metas y su tendencia de progreso en el tiempo en la sección Gráficos de Adobe Workfront Goals. Los gráficos de esta sección no desglosan el progreso de cada meta, sino que le proporcionan una instantánea integral del estado de progreso de todas las metas, así como su tendencia de progreso a lo largo del tiempo durante un período especificado.

>[!IMPORTANT]
>
>Puede ver un recuento total de sus objetivos en la sección Gráficos durante un período de tiempo seleccionado. Sin embargo, Workfront Goals solo tiene en cuenta las metas con un estado de Activo y Cerrado cuando calcula el progreso general de la meta y el porcentaje completado.

## Requisitos de acceso

>[!NOTE]
>
>Su empresa puede optar por seguir utilizando los objetivos de Adobe Workfront si compró este paquete anteriormente. Debe hablar con el representante de su cuenta para obtener más detalles.
>
>Adobe Workfront Goals ya no se puede adquirir.

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Paquete de Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront</td>
 <td>
 <p>Colaborador o superior</p>
<p>Solicitud o superior</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuración de nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Permisos Ver o superiores para la meta que desea ver</p>
  <p>Permisos de administración para la meta y poder editarla</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores del sistema, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
    <p> New product requirement: Workfront</p>
    Or
    <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

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
     <li>Un porcentaje completado esperado y real promedio de todas las metas activas y cerradas en el período seleccionado. El progreso de porcentaje completado se desglosa por incrementos semanales marcados mediante nodos. </li> 
     <li>Porcentaje promedio general de progreso para las metas activas y cerradas desde la semana anterior. </li> 
    </ul> <p>Sugerencia: Es posible que el gráfico de progreso de la meta no muestre ninguna información cuando se realicen actualizaciones en las metas fuera del período de tiempo seleccionado. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Revisión del progreso de la meta en gráficos

{{step1-to-goals}}

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


