---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Quitar la alineación de objetivos en Adobe Workfront Goals
description: Puede eliminar la alineación entre dos metas si ya no tiene sentido que estén conectadas.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 77%

---

# Quitar la alineación de metas en Adobe Workfront Goals

<!--Audited P&P only: 4/2025-->

Puede eliminar la alineación entre dos metas si ya no tiene sentido que estén conectadas.

Para obtener más información sobre cómo alinear metas, consulte los siguientes artículos:

* [Alinear metas conectándolas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Alinear metas convirtiendo resultados y actividades en metas](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

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
  <td> <p>paquete de Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront</td>
 <td>
 <p>Colaborador o superior</p>
 <p>Solicitud o superior</p> </td>
 </tr>
  <tr>
 <td role="rowheader">Nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <p>Permisos Ver o superiores para la meta que desea ver</p>
  <p>Permisos de administración para la meta y poder editarla</p>

</td>
 </tr>
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
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
   <p> New product requirement: Workfront</p>
   Or
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Requisitos previos

Debe tener lo siguiente para poder comenzar:

* Una meta principal que tiene al menos una meta secundaria asociada. Las metas secundarias son los indicadores del progreso de las metas principales.

## Consideraciones sobre la eliminación de la alineación de metas

Tenga en cuenta lo siguiente al eliminar la alineación entre dos metas:

* La meta principal debe tener otra meta, actividad o resultado asociado para poder permanecer Activa.
* No se puede quitar una meta secundaria alineada de una meta principal si es el único indicador de progreso de la meta principal.
* La meta secundaria se convierte en una meta independiente cuando se elimina su alineación con la meta principal.

## Eliminar alineación de metas

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![Gear icon](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![Reove alignment](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Acceda al área **Metas** en Workfront y haga clic en el nombre de una meta para abrir su página.
1. En la página de la meta de una meta principal, haga clic en **Indicadores de progreso** en el panel izquierdo.

   ![Volver a mover la alineación del objetivo](assets/remove-goal-alignment-from-list-unshimmed.png)

1. En la agrupación **Type: Goal**, seleccione una meta y haga clic en el icono **Desconectar** ![Desconectar](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) que se encuentra en la parte superior de la lista.

   Aparece la casilla Desconectar.

1. Haga clic en **Desconectar** para desconectar la meta seleccionada de su elemento principal.

   La meta se convierte en una meta independiente y ya no aparece como indicador de progreso de la meta original. El progreso de la meta desconectada ya no influye en el progreso de la meta original.

   Aparece un mensaje de éxito en la esquina superior derecha de la página para confirmar que la meta se ha desconectado.
