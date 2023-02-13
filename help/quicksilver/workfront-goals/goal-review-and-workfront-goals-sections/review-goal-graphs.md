---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Revisar gráficos para comprender las tendencias de progreso de objetivos en los objetivos de Adobe Workfront
description: Puede ver el estado general de sus objetivos y la tendencia del progreso en el tiempo en la sección Gráficos de los objetivos de Adobe Workfront. Los gráficos de esta sección no desglosan el progreso de cada objetivo, sino que ofrecen una instantánea holística del estado de progreso de todos los objetivos, así como de su tendencia de progreso en el tiempo durante un período especificado.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Revisar gráficos para comprender las tendencias de progreso de objetivos en los objetivos de Adobe Workfront

<!-- drafted mostly for P&P release-->

Puede ver el estado general de sus objetivos y la tendencia del progreso en el tiempo en la sección Gráficos de los objetivos de Adobe Workfront. Los gráficos de esta sección no desglosan el progreso de cada objetivo, sino que ofrecen una instantánea holística del estado de progreso de todos los objetivos, así como de su tendencia de progreso en el tiempo durante un período especificado.

>[!IMPORTANT]
>
>Puede ver un recuento total de los objetivos en la sección Gráficos durante un período de tiempo seleccionado. Sin embargo, los objetivos de Workfront solo tienen en cuenta los objetivos con un estado Activo y Cerrado al calcular el estado general del progreso del objetivo y el porcentaje completado.

## Requisitos de acceso

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>Debe adquirir una licencia adicional para los objetivos de Adobe Workfront para acceder a la funcionalidad que se describe en este artículo. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para utilizar los objetivos de Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver o tener más acceso a los objetivos</p> <p><b>NOTA</b><p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Conceder acceso a los objetivos de Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> 
    <div> 
     <p>Ver o permisos superiores en objetivos</p> 
     <p>Para obtener información sobre cómo compartir objetivos, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir un objetivo en los objetivos de Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe tener lo siguiente para poder iniciar:

* Plantilla de diseño que incluye el área Objetivos del menú principal.

## Tipos de gráficos en objetivos de Workfront

Los siguientes gráficos están disponibles en la sección Gráficos o en los Objetivos de Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">El gráfico de salud de los objetivos</td> 
   <td> <p>Gráfico de medición que muestra lo siguiente:</p> 
    <ul> 
     <li>Un número total de objetivos para el período de tiempo seleccionado. Se tienen en cuenta los objetivos que tengan cualquier estado. </li> 
     <li>El estado de progreso de los objetivos con el estado Activo y Cerrado.</li> 
    </ul> <p>Para obtener información sobre cómo calculan el estado del progreso los objetivos de Workfront, consulte <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Resumen del progreso y la condición del objetivo en los objetivos de Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gráfico de progreso de los objetivos</td> 
   <td> <p>Gráfico de líneas que muestra las actualizaciones realizadas en los objetivos en incrementos semanales durante la duración del objetivo. El gráfico de progreso del objetivo muestra lo siguiente:</p> 
    <ul> 
     <li>Porcentaje promedio esperado y real completado de todos los objetivos activos y cerrados en el período seleccionado. El progreso del porcentaje completado se desglosa en incrementos semanales marcados por nodos. </li> 
     <li>El porcentaje medio general de progreso de los objetivos activos y cerrados desde la semana anterior. </li> 
    </ul> <p>Sugerencia: Es posible que el gráfico de progreso del objetivo no muestre información cuando se realizan actualizaciones de los objetivos fuera del período de tiempo seleccionado. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Revisar el progreso del objetivo en los gráficos

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) > **Objetivos** en la esquina superior derecha.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Se abrirá el área Objetivos de Workfront .

1. Haga clic en **Gráficos** en el panel izquierdo.

   ![](assets/graphs-in-left-panel.png)

   Se muestra la sección Gráficos .

   De forma predeterminada, los objetivos mostrados en la sección Gráficos están limitados por los siguientes criterios:

   * Los filtros aplicados al área Gráficos.
   * Los objetivos que están en estado Activo y Borrador.

1. (Opcional) Para seleccionar el tipo de información que desea mostrar, actualice los filtros de la esquina superior derecha de la sección Gráficos .

   Para obtener más información sobre los objetivos de filtrado, consulte [Filtrar información en objetivos de Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   Si ha seleccionado mostrar más de un período de tiempo, se muestra un gráfico de estado (medición) así como un gráfico de progreso (línea) para cada período de tiempo.

1. Revise la información de la tabla siguiente cuando revise el Gráfico de estado de objetivos.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Número total de objetivos | El número situado en la parte inferior del gráfico indica el número de todos los objetivos del período seleccionado, en todos los estados seleccionados. |
   |---|---|
   | Porcentaje medio completado | En la parte superior del gráfico, este número indica el porcentaje promedio completado de objetivos activos y cerrados en el período de tiempo seleccionado. |
   | Objetivos y progreso | El número de objetivos para cada segmento de estado del progreso, cuando pasa el ratón por encima de los segmentos del gráfico. En los segmentos solo se cuentan los objetivos en un estado Activo o Cerrado. |


1. Revise la información de la tabla siguiente cuando revise el cuadro de progreso de los objetivos.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Progreso de línea de base</td> 
      <td>La línea de pendiente verde indica el promedio de porcentaje total completado esperado de objetivos activos y cerrados para el período de tiempo seleccionado. Se espera que todos los objetivos dentro de un periodo se completen, por lo que el progreso de línea de base siempre es del 100% al final del periodo. </td> 
     </tr> 
     <tr> 
      <td>Progreso real</td> 
      <td> <p>La línea azul indica el promedio total real de los objetivos activos y cerrados en porcentaje completado para el período de tiempo seleccionado en incrementos semanales. Cada semana durante la duración del objetivo se marca mediante un nodo en la línea . </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Pase el ratón por encima de un nodo de semana en el gráfico de progreso del objetivo y revise lo siguiente:

   * **Fecha de la semana**: Mes, día y año de la semana seleccionada.
   * **Progreso**: Un promedio del porcentaje real completado de todos los objetivos para la semana seleccionada.
   * **Línea de base**: Un promedio del porcentaje esperado de finalización de todos los objetivos para la semana seleccionada.

1. (Opcional) Haga clic en **Progreso** en la parte inferior del gráfico de progreso para eliminar la línea de progreso general real

   O

   Haga clic en **Línea de base** en la parte inferior del gráfico de progreso para eliminar el progreso esperado del gráfico.

 
