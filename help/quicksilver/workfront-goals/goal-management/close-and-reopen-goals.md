---
product-previous: workfront-goals
navigation-topic: goal-management
title: Cerrar y volver a abrir metas en Adobe Workfront Goals
description: Puede cerrar un objetivo cuando desee indicar que lo ha completado o que ya no está trabajando en él porque ha quedado obsoleto.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# Cerrar y volver a abrir metas en Adobe Workfront Goals

Puede cerrar un objetivo cuando desee indicar lo siguiente:

* El objetivo se realiza, ya sea porque lo ha conseguido o porque ha transcurrido el período de tiempo.
* Ya no está trabajando en ello ni tiene previsto hacerlo en el futuro inmediato.

Puede volver a abrir los objetivos que se han cerrado cuando vuelvan a ser relevantes.

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
 <td role="rowheader">Nivel de acceso</td>
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

## Consideraciones al cerrar o volver a abrir las metas

* Debe tener acceso a Editar metas en su nivel de acceso para poder cerrar y volver a abrir las metas. Para obtener información sobre cómo conceder acceso a las metas, consulte [Conceder acceso a las metas de Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* Solo puede cerrar las metas activas. No se pueden cerrar los objetivos que están en estado de Borrador.

  Para obtener información sobre los estados de objetivos, consulte [Información general sobre el estado de los objetivos en Adobe Workfront Goals](../../workfront-goals/goal-management/goal-status-overview.md).

* Cerrar metas bloquea su progreso y le permite calificar lo bien que lo logró.

  >[!CAUTION]
  >
  >Al cerrar una meta que tiene metas de contribución activas, su progreso cambia después de cerrarse para indicar el progreso de las metas de contribución activas. Para obtener información acerca de cómo alinear metas, vea [Alinear metas conectándolas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Actualice los indicadores de progreso de la meta antes de cerrarla para asegurarse de que se cierra con un valor de progreso preciso. Si se han alcanzado todos los indicadores de progreso, el porcentaje de objetivo completado debe ser del 100 % y se ha alcanzado el objetivo. Para obtener información sobre cómo actualizar tus metas, consulta [Actualizar progreso de metas en Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Deje los comentarios finales como una actualización de los objetivos que cierre. Para obtener información sobre cómo agregar comentarios a las metas, consulte [Administrar comentarios sobre las metas en Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
* Ya no se puede actualizar el progreso de los resultados y las actividades de un objetivo que se cierre.
* Puede volver a abrir una meta cerrada si desea continuar trabajando en ella.
* Si no se ha alcanzado el objetivo, considere la posibilidad de copiar la mayor parte de su información al siguiente período de tiempo (trimestre o año). Esta es una excelente opción para los objetivos que son iguales de un período de tiempo al siguiente o para los objetivos en los que es posible que tenga que trabajar para lograr en el próximo periodo de tiempo. Para obtener información sobre cómo copiar metas, consulte [Copiar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md). También puede actualizar el periodo de tiempo de la meta en lugar de copiarlo a otro periodo.
* Workfront elimina los comentarios de un objetivo cerrado cuando se vuelve a abrir. Si debe conservar los comentarios, le recomendamos que copie el objetivo cerrado, incluidos los resultados asociados a él, en lugar de volver a abrirlo.


## Cerrar metas

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) > **Metas** en la esquina superior derecha.

   Se abre la Lista de metas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique los filtros para mostrar solo las metas que están activas.

   Para obtener información sobre cómo filtrar información en Workfront Goals, consulte [Filtrar información en Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).
1. Haga clic en un objetivo activo.

   Se abre la página de la meta.

   ![](assets/goal-page-unshimmed.png)
1. Haga clic en el menú **Más** ![](assets/more-icon.png) que se encuentra a la derecha del nombre de la meta y luego haga clic en **Cerrar**.

   La meta se cerrará y recibirá una confirmación en la esquina superior derecha de la pantalla.

   ![](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Opcional) En el cuadro de confirmación, haga clic en **Agregar notas de cierre** para agregar comentarios sobre este objetivo y sobre el motivo por el que debe cerrarlo.
1. Agregue notas de cierre y, a continuación, haga clic en **Agregar notas**.

   ![](assets/add-closing-notes-box-unshimmed.png)

   Los comentarios se muestran en la sección Detalles del objetivo de la página del objetivo, en el área Notas de cierre.

   >[!NOTE]
   >
   >Workfront elimina las notas de cierre si más tarde vuelve a abrir una meta cerrada.


## Volver a abrir metas

Puede volver a abrir los objetivos cerrados si decide que vuelven a ser relevantes y que necesita seguir actualizando su progreso.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png)> **Metas** en la esquina superior derecha.

   Se abre la Lista de metas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique los filtros para mostrar solo las metas cerradas.

   Para obtener información sobre cómo filtrar información en Workfront Goals, consulte [Filtrar información en Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).
1. Haga clic en el nombre de una meta cerrada.

   Se abre la página de la meta.
1. Haga clic en el menú **Más** ![](assets/more-icon.png) que se encuentra a la derecha del nombre de la meta y, a continuación, **Volver a abrir** > **Volver a abrir**.

   Ocurren lo siguiente:
   * La meta ahora está abierta y tiene el estado Activo.
   * El progreso de la meta se vuelve a calcular a partir de la fecha actual.
   * Todas las notas de cierre se eliminan de la página de detalles de Objetivo. Las notas de cierre eliminadas no se pueden recuperar.

1. (Opcional) Vuelva a modificar los filtros para que solo se muestren las metas activas.

   Los objetivos que ha abierto se muestran en la pantalla.

