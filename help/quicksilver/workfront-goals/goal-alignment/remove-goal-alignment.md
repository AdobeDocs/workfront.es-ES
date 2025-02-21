---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Quitar la alineación de metas en Adobe Workfront Goals
description: Puede eliminar la alineación entre dos metas si ya no tiene sentido que estén conectadas.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 94%

---

# Quitar la alineación de metas en Adobe Workfront Goals

Puede eliminar la alineación entre dos metas si ya no tiene sentido que estén conectadas.

Para obtener más información sobre cómo alinear metas, consulte los siguientes artículos:

* [Alinear metas conectándolas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Alinear metas convirtiendo resultados y actividades en metas](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Plan de Adobe Workfront</td>
 <td>
 <p>Cualquiera</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront*</td>
 <td>
 <p>Nueva licencia: Contributor o superior</p>
 O
 <p>Licencia actual: Request o superior</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Producto*</td>
 <td>
 <p> Nuevo requisito de producto, uno de los siguientes: </p>
<ul>
<li>Un plan Select or Prime Adobe Workfront y una licencia adicional de Adobe Workfront Goals.</li>
<li>Un plan Ultimate Workfront que incluye Workfront Goals de forma predeterminada. </li></ul>
 <p>O</p>
 <p>Requisito de producto actual: un plan de Workfront y una licencia adicional para Adobe Workfront Goals. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <p>Permisos Ver o superiores para la meta que desea ver</p>
  <p>Permisos de administración para la meta y poder editarla</p>
  <p>Para obtener información acerca de cómo compartir metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Metas en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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