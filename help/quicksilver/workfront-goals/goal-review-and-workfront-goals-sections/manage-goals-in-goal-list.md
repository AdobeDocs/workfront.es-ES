---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Administrar objetivos en la lista de objetivos de Adobe Workfront
description: Una vez que usted u otros usuarios hayan creado los objetivos, puede revisar su progreso e información en la lista de objetivos. Para obtener información sobre la creación de objetivos, consulte Crear objetivos en Objetivos de Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 2%

---

# Administrar objetivos en la lista de objetivos de Adobe Workfront

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

Una vez que usted u otros usuarios hayan creado los objetivos, puede revisar su progreso e información en la lista de objetivos. Para obtener información sobre la creación de objetivos, consulte [Crear objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

## Requisitos de acceso

<!--drafted - replace the table below with this one when P&P releases: 

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

## Administrar objetivos en la lista de objetivos

Puede ver y administrar los objetivos en las siguientes secciones de los Objetivos de Workfront:

* Lista de metas
* Alineación de metas

Cada sección muestra los objetivos en formatos ligeramente diferentes. La sección que utilice dependerá del propósito que desee lograr al trabajar con los objetivos.

Para obtener más información, consulte [Información general sobre las secciones de objetivos de Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Este artículo describe cómo revisar los objetivos en la lista de objetivos.

Tenga en cuenta lo siguiente al revisar la lista de objetivos:

* Puede ver los objetivos que ha creado usted o cualquier otra persona de su organización en la lista de objetivos. Debe tener permisos de administración en objetivos para poder editarlos.

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

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

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

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

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

Para administrar los objetivos en la lista de objetivos:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)  en la esquina superior derecha, haga clic en **Objetivos**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La sección Lista de objetivos se muestra de forma predeterminada. De forma predeterminada, puede ver los objetivos independientemente de su estado, periodo o propietario.

   La lista de objetivos contiene los siguientes campos con información sobre cada objetivo:

   * **Nombre**: Nombre del objetivo.
   * **Propietario**: Nombre del propietario del objetivo.
   * **Periodo**: Período de tiempo para el que se programa el objetivo.
   * **Estado**: El estado del objetivo puede ser uno de los siguientes:
      * Activo
      * Borrador
      * Inactivo
      * Cerrado

      Para obtener información sobre el estado del objetivo, consulte [Información general sobre el estado de los objetivos en los objetivos de Adobe Workfront](../goal-management/goal-status-overview.md).

      El icono de alineación aparece en los objetivos alineados con otros objetivos. Para obtener información sobre la alineación de objetivos, consulte [Alinear objetivos conectándolos en los objetivos de Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).

   * **Condición**: Una representación visual de cómo progresa el objetivo dentro del período de tiempo asignado para que se complete el objetivo.

      La condición de un objetivo podría ser una de las siguientes:

      * Nuevo
      * Bien encaminado
      * En riesgo
      * Con problemas

      Para obtener información sobre las condiciones de objetivo, consulte [Resumen del progreso y la condición del objetivo en los objetivos de Adobe Workfront](../goal-management/calculate-goal-progress.md).

   * **Progreso**: El indicador de progreso del objetivo como valor de porcentaje. El color del indicador de progreso coincide con el color de la condición del objetivo.

      Para obtener más información, consulte [Calcular el progreso del objetivo en los objetivos de Adobe Workfront](../goal-management/calculate-goal-progress.md).



1. Haga clic en el icono de filtro ![](assets/filter-icon.png) en la esquina superior derecha de la lista de objetivos y aplique filtros para mostrar solo los objetivos que son importantes para usted.

   Para obtener información sobre el uso de filtros en los objetivos de Workfront, consulte [Filtrar información en objetivos de Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Haga clic en cualquiera de los campos de los encabezados de columna para ordenar la lista por ese campo.
A la derecha del campo por el que se ordena la lista se muestra una flecha.

1. (Opcional) Vuelva a hacer clic en el campo de la columna para ordenar la misma columna en orden descendente.
1. Haga clic en el nombre de un objetivo para abrir la página del objetivo.
1. Seleccione un objetivo en la lista y, a continuación, haga clic en una de las siguientes opciones en la parte superior de la lista:
   * **Editar** icono ![](assets/edit-icon.png) para editar información sobre el objetivo. Para obtener más información, consulte [Editar objetivos en objetivos de Adobe Workfront](../goal-management/edit-goals.md).
   * **Compartir** icono ![](assets/share-icon.png) compartir el objetivo con otras personas. Para obtener más información, consulte [Compartir un objetivo en los objetivos de Adobe Workfront](../workfront-goals-settings/share-a-goal.md).
   * **Alineación abierta** icono ![](assets/align-icon-unshimmed.png) para abrir el área Alineación de objetivo . Esta opción solo se muestra cuando el objetivo seleccionado se alinea con otro objetivo.
   * **Eliminar** icono ![](assets/delete-icon.png) para eliminar el objetivo, haga clic en **Eliminar** para confirmar.  Para obtener más información, consulte [Eliminar y desactivar objetivos en objetivos de Adobe Workfront](../goal-management/delete-and-deactivate-goals.md).





