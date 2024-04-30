---
product-previous: workfront-goals
navigation-topic: goal-management
title: Actualizar metas en el panel Detalles de metas de Adobe Workfront Goals
description: Puede actualizar la información de las metas individuales accediendo al panel Detalles de las metas.
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 1%

---

# Actualice las metas en la sección Detalles de las metas de Adobe Workfront Goals

<!--drafted for the goal redesign:
- change the title for Production to Update goals in the Goal details section in Adobe Workfront Goals. 
- update the description in the metadata above
-->

Puede actualizar la información de las metas individuales accediendo al panel Detalles de las metas.

>[!NOTE]
>
>No se pueden actualizar las metas que tengan el estado Cerrado.


## Requisitos de acceso

Debe tener lo siguiente:

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
 <p>Requisito de producto actual: un plan de Workfront y una licencia adicional para los objetivos de Adobe Workfront. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para utilizar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nivel de acceso*</td>
 <td> <p>Editar acceso a Objetivos</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Ver o permisos superiores a la meta para verla</p>
  <p>Administrar permisos para el objetivo y editarlo</p>
  <p>Para obtener información sobre cómo compartir objetivos, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
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

## Actualizar metas en la sección Detalles de las metas

Puede acceder a una meta individual desde una lista de metas.

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![](assets/more-icon.png), then click any of the following options:

   1. **Edit**. For information about editing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
   1. **Copy**. For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).
   1. **Activate**. This option is available only for drafted and inactive goals.

      For information about activating goals, see [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md). 
   
   1. **Close**, then click**Close Goal**. This option is available only for active goals.

      For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. **Deactivate**. This option is available only for active goals. This deactivates the goal immediately.

      For information about deactivating goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).
   
   1. **Delete**, then click **Yes, Delete**.

      For information about deleting goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

      >[!NOTE]
      >
      >Deleted goals cannot be recovered.

   1. **Reopen**, then click **Reopen**. This option is available only for closed goals that are from a current time period.

      For information about reopening goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. (Conditional) If you clicked any of the options between steps a-i above except Delete or Reopen, click **Save**.    
   
      (!--ensure this is accurate)--)

1. Click **Align to another goal** in the upper-right of the Summary tab, then specify the name of a goal in the **Align to** **another goal** field that you want to align the current goal to. The current goal becomes the child of the goal you align it to. For information about child and parent goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md). 
1. Click **Add results**. Results drive the progress of your goal. For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

1. Click **Add activities**. Activities drive the progress of your goal. For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 

1. Click the **Updates** tab. Here, you can view goal comments and review the entire editing history of the goal, activities, and results, to understand who changed what and when.

   ![](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab.&nbsp;They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. Haga clic en el nombre de una meta en la Lista de metas y, a continuación, haga clic en el nombre de una meta.

   Esto abre el **Detalles de la meta** de la izquierda.

   ![](assets/goal-page-unshimmed.png)

1. Haga clic en **Icono Editar** ![](assets/edit-icon.png) en la esquina superior derecha, haga clic en **Editar todo** o **Información general**

   O

   Empiece a escribir información en uno de los campos editables de la sección Detalles del objetivo. La sección se vuelve editable.

   >[!IMPORTANT]
   >
   >No se pueden editar todos los campos que se muestran en la sección Detalles del objetivo. Workfront calcula algunos de los campos y son de solo lectura.

1. Actualice o revise los siguientes campos:

   * **Descripción**: Añada o actualice información sobre la meta.
   * **Progreso**: indica qué porcentaje del objetivo se ha completado hasta el momento. No se puede actualizar manualmente el progreso de una meta. El progreso del objetivo es un cálculo de todos los indicadores de progreso.
   * **Condición**: indica si el objetivo es nuevo y no se ha actualizado aún, si está en el objetivo para completarse a tiempo o si se queda rezagado. No se puede actualizar la condición de un objetivo. Workfront calcula automáticamente la condición del objetivo.\
     Para obtener más información sobre la condición de objetivo y el progreso, consulte
     [Información general sobre el progreso y la condición de los objetivos en Adobe Workfront Goals](../goal-management/calculate-goal-progress.md).
   * **Estado**: no se puede actualizar manualmente el estado de un objetivo. Para obtener más información, consulte [Información general sobre el estado de las metas en Adobe Workfront Goals](../goal-management/goal-status-overview.md).
   * **Propietario de meta**: Haga clic en para actualizar el nombre del propietario de la meta. Empiece a escribir el nombre de un usuario, equipo, grupo o el nombre de su organización y, a continuación, selecciónela cuando se muestre en la lista. Solo puede tener un propietario para un objetivo.
   * **Meta principal**: Comience a escribir el nombre de una meta que desee establecer como principal de la meta seleccionada. El progreso de la meta seleccionada actualizará automáticamente el progreso de la meta principal.

     >[!TIP]
     >
     >No se puede actualizar la siguiente información sobre un objetivo principal:
     >    * Período de la meta principal
     >    * Progreso de la meta principal
     >    * Propietario del objetivo principal.
     >      
     >Debe actualizar esta información en la propia meta principal.

   * **Periodo**: haga clic en para actualizar el periodo de tiempo de la meta\
     O\
     Seleccionar **Habilitar fechas personalizadas** para especificar las fechas de la meta **Inicio** y **Fechas de finalización**.
   * **Notas de cierre**: este campo solo es visible para los objetivos con un estado Cerrado. Las metas cerradas no se pueden editar. Volver a abrir un objetivo cerrado elimina permanentemente las notas de cierre.


