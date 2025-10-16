---
product-previous: workfront-goals
navigation-topic: goal-management
title: Cerrar y volver a abrir las metas en Adobe Workfront Goals
description: Puede cerrar un objetivo cuando desee indicar que lo ha completado o que ya no está trabajando en él porque ha quedado obsoleto.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 18%

---

# Cerrar y volver a abrir metas en Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Puede cerrar un objetivo cuando desee indicar lo siguiente:

* El objetivo se realiza, ya sea porque lo ha conseguido o porque ha transcurrido el período de tiempo.
* Ya no está trabajando en ello ni tiene previsto hacerlo en el futuro inmediato.

Puede volver a abrir los objetivos que se han cerrado cuando vuelvan a ser relevantes.

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
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront</td>
 <td>
 <p>Colaborador o superior</p>
 <p>Solicitud o superior</p></td>
 </tr>
 <td role="rowheader">Configuración de nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr>
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
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <td role="rowheader">Access level</td>
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

## Consideraciones al cerrar o volver a abrir las metas

* Debe tener acceso a Editar metas en su nivel de acceso para poder cerrar y volver a abrir las metas. Para obtener información sobre cómo conceder acceso a las metas, consulte [Concesión de acceso a Adobe Workfront Goals](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* Solo puede cerrar las metas activas. No se pueden cerrar los objetivos que están en estado de Borrador.

  Para obtener información sobre los estados de metas, consulte [Información general sobre el estado de las metas en Adobe Workfront Goals](../../workfront-goals/goal-management/goal-status-overview.md).

* Cerrar metas bloquea su progreso y le permite calificar lo bien que lo logró.

  >[!CAUTION]
  >
  >Al cerrar una meta que tiene metas de contribución activas, su progreso cambia después de cerrarse para indicar el progreso de las metas de contribución activas. Para obtener información sobre la alineación de metas, consulte [Alinear metas conectándolas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

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

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![Closing goals with active aligned goals](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) > **Metas** en la esquina superior derecha.

   Se abre la Lista de metas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique los filtros para mostrar solo las metas que están activas.

   Para obtener información sobre cómo filtrar información en Workfront Goals, consulte [Filtrar información en Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).
1. Haga clic en un objetivo activo.

   Se abre la página de la meta.

   ![Página de metas](assets/goal-page-unshimmed.png)
1. Haga clic en el icono **Más** del menú ![Más](assets/more-icon.png) a la derecha del nombre de la meta y, a continuación, haga clic en **Cerrar**.

   La meta se cerrará y recibirá una confirmación en la esquina superior derecha de la pantalla.

   ![Confirmación de cierre de meta](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Opcional) En el cuadro de confirmación, haga clic en **Agregar notas de cierre** para agregar comentarios sobre este objetivo y sobre el motivo por el que debe cerrarlo.
1. Agregue notas de cierre y, a continuación, haga clic en **Agregar notas**.

   ![Agregar cuadro de notas de cierre](assets/add-closing-notes-box-unshimmed.png)

   Los comentarios se muestran en la sección Detalles del objetivo de la página del objetivo, en el área Notas de cierre.

   >[!NOTE]
   >
   >Workfront elimina las notas de cierre si más tarde vuelve a abrir una meta cerrada.


## Volver a abrir metas

Puede volver a abrir los objetivos cerrados si decide que vuelven a ser relevantes y que necesita seguir actualizando su progreso.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png)> **Metas** en la esquina superior derecha.

   Se abre la Lista de metas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique los filtros para mostrar solo las metas cerradas.

   Para obtener información sobre cómo filtrar información en Workfront Goals, consulte [Filtrar información en Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).
1. Haga clic en el nombre de una meta cerrada.

   Se abre la página de la meta.
1. Haga clic en el **icono Más** del menú ![Más](assets/more-icon.png) a la derecha del nombre de la meta y, a continuación, **Volver a abrir** > **Volver a abrir**.

   Ocurren lo siguiente:
   * La meta ahora está abierta y tiene el estado Activo.
   * El progreso de la meta se vuelve a calcular a partir de la fecha actual.
   * Todas las notas de cierre se eliminan de la página de detalles de Objetivo. Las notas de cierre eliminadas no se pueden recuperar.

1. (Opcional) Vuelva a modificar los filtros para que solo se muestren las metas activas.

   Los objetivos que ha abierto se muestran en la pantalla.

