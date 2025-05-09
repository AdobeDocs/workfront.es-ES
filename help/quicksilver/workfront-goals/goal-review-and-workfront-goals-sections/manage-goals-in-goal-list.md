---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Administrar metas en la lista de metas de Adobe Workfront
description: Una vez que haya creado metas o las hayan creado otros usuarios, podrá revisar su progreso e información en la lista de metas. Para obtener información sobre la creación de metas, consulte Crear metas en Adobe Workfront Goals.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: a64f6e507d74201cba1455fbbc6af77c2b7ba058
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 85%

---

# Administrar metas en la lista de metas de Adobe Workfront

<!--Audited for P&P only: 4/2025-->

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

Una vez que haya creado metas o las hayan creado otros usuarios, podrá revisar su progreso e información en la lista de metas. Para obtener información sobre cómo crear metas, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

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
 <td role="rowheader">Nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p>  </td>
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

## Administrar metas en la lista de metas

Puede ver y administrar las metas en las siguientes secciones de Workfront Goals:

* Lista de metas
* Alineación de metas

Cada sección muestra las metas en formatos ligeramente diferentes. La sección que utilice dependerá del propósito que desee lograr al trabajar con metas.

Para obtener más información, consulte [Información general sobre las secciones de Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Este artículo describe la revisión de metas en la lista de metas.

Tenga en cuenta lo siguiente al revisar la lista de metas:

* Puede ver las metas que haya creado o las que haya creado cualquier otra persona de su organización en la lista de metas. Debe tener permisos de administración sobre las metas para poder editarlas.

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![Goal list with goal expanded](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![Right-pointing arrow](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![Alignment icon](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

Para administrar metas en la lista de metas:

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **Metas**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La sección Lista de metas se muestra de forma predeterminada. De forma predeterminada, se pueden ver las metas independientemente de su estado, período o propietario.

   La lista de metas contiene los siguientes campos con información sobre cada meta:

   * **Nombre**: nombre de la meta.
   * **Propietario**: nombre del propietario de la meta.
   * **Período**: período de tiempo para el que se ha programado la meta.
   * **Estado**: estado de la meta, que puede ser uno de los siguientes:
      * Activo
      * Borrador
      * Inactivo
      * Cerrado

     Para obtener información sobre el estado de las metas, consulte [Información general sobre el estado de las metas en Adobe Workfront Goals](../goal-management/goal-status-overview.md).

     El icono de alineación aparece en las metas que están alineadas con otras metas. Para obtener información sobre la alineación de metas, consulte [Alinear metas conectándolas en Adobe Workfront Goals](../goal-alignment/align-goals-by-connecting-them.md).

   * **Condición**: representación visual de cómo progresa la meta dentro del período de tiempo asignado para que se complete.

     La condición de una meta puede ser una de las siguientes:

      * Nuevo
      * Bien encaminado
      * En riesgo
      * Con problemas

     Para obtener información sobre las condiciones de las metas, consulte [Información general sobre el progreso y la condición de las metas en Adobe Workfront Goals](../goal-management/calculate-goal-progress.md).

   * **Progreso**: indicador de progreso de la meta como valor porcentual. El color del indicador de progreso coincide con el de la condición de la meta.

     Para obtener más información, consulte [Calcular el progreso de las metas en Adobe Workfront Goals](../goal-management/calculate-goal-progress.md).

1. Haga clic en el icono de filtro ![Icono de filtro](assets/filter-icon.png) en la esquina superior derecha de la lista de metas y aplique filtros para mostrar solo las metas que sean importantes para usted.

   Para obtener información sobre el uso de filtros en Workfront Goals, consulte [Información sobre los filtros en Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).

1. Haga clic en cualquiera de los campos de los encabezados de columna para ordenar la lista por ese campo.
Aparecerá una flecha a la derecha del campo por el que se ordena la lista.

1. (Opcional) Vuelva a hacer clic en el campo de la columna para ordenar la misma columna en orden descendente.
1. Haga clic en el nombre de una meta para abrir su página.
1. Seleccione una meta de la lista y, a continuación, haga clic en una de las siguientes opciones en la parte superior de la lista:
   * **Editar** icono ![Editar icono](assets/edit-icon.png) para editar información sobre la meta. Para obtener más información, consulte [Editar metas en Adobe Workfront Goals](../goal-management/edit-goals.md).
   * **Compartir** icono ![Compartir icono](assets/share-icon.png) para compartir el objetivo con otras personas. Para obtener más información, consulte [Compartir una meta en Adobe Workfront Goals](../workfront-goals-settings/share-a-goal.md).
   * **Icono Abrir alineación** ![Icono Abrir alineación](assets/align-icon-unshimmed.png) para abrir el área Alineación de metas. Esta opción solo se muestra cuando la meta seleccionada está alineada con otra.
   * **Eliminar** icono ![Eliminar icono](assets/delete-icon.png) para eliminar la meta y, a continuación, haga clic en **Eliminar** para confirmar.  Para obtener más información, consulte [Eliminar y desactivar metas en Adobe Workfront Goals](../goal-management/delete-and-deactivate-goals.md).





