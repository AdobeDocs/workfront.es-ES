---
product-previous: workfront-goals
navigation-topic: goal-management
title: Cierre y vuelva a abrir los objetivos en Objetivos de Adobe Workfront
description: Puede cerrar un objetivo cuando desee indicar que lo ha completado o que ya no está trabajando en él porque se ha vuelto obsoleto.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Cierre y vuelva a abrir los objetivos en Objetivos de Adobe Workfront

Puede cerrar un objetivo cuando desee indicar lo siguiente:

* El objetivo se logra porque lo logró o porque el período de tiempo transcurrió.
* Ya no trabajas en ello ni planeas hacerlo en el futuro inmediato.

Puede volver a abrir los objetivos que se hayan cerrado cuando vuelvan a ser relevantes.

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

Debe tener lo siguiente:

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
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Objetivos o posterior</p> <p><b>NOTA</b><p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Conceder acceso a los objetivos de Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> 
    <div> 
     <p>Administrar permisos para el objetivo</p> 
     <p>Para obtener información sobre cómo compartir objetivos, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir un objetivo en los objetivos de Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe tener lo siguiente para poder iniciar:

* Plantilla de diseño que incluye el área Objetivos del menú principal.

## Consideraciones al cerrar o reabrir objetivos

* Debe tener acceso a Editar objetivos en el nivel de acceso para poder cerrar y volver a abrir los objetivos. Para obtener información sobre la concesión de acceso a los objetivos, consulte [Conceder acceso a los objetivos de Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* Solo puede cerrar objetivos activos. No se pueden cerrar los objetivos que están en el estado de Borrador.

   Para obtener información sobre los estados de objetivos, consulte [Información general sobre el estado de los objetivos en los objetivos de Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

* El cierre de objetivos bloquea su progreso y le permite evaluar lo bien que hizo al lograrlo.

   >[!CAUTION]
   >
   >Al cerrar un objetivo que tiene objetivos de contribución activos, su progreso cambia después de cerrarse para indicar el progreso de los objetivos activos contribuyentes. Para obtener información sobre la alineación de objetivos, consulte [Alinear objetivos conectándolos en los objetivos de Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Actualice los indicadores de progreso del objetivo antes de cerrar el objetivo para garantizar que el objetivo se cierre con un valor de progreso preciso. Si se han alcanzado todos los indicadores de progreso, el porcentaje de objetivo completado debería ser del 100 % y se ha alcanzado su objetivo. Para obtener información sobre cómo actualizar los objetivos, consulte [Actualización del progreso del objetivo en los objetivos de Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Deje cualquier comentario final como una actualización de los objetivos que cierre. Para obtener información sobre cómo agregar comentarios a objetivos, consulte [Administrar comentarios de objetivo en objetivos de Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).
* Ya no puede actualizar el progreso de los resultados y las actividades en un objetivo que cierre.
* Puede volver a abrir un objetivo cerrado si desea continuar trabajando en él.
* Si no se ha alcanzado el objetivo, considere la posibilidad de copiar la mayor parte de su información al siguiente período de tiempo (trimestre o año). Se trata de una buena opción para objetivos que son los mismos entre un período de tiempo y el siguiente o objetivos que puede que todavía necesite lograr en el siguiente período de tiempo. Para obtener información sobre cómo copiar objetivos, consulte [Copiar objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/copy-goals.md). También puede actualizar el periodo de tiempo en el objetivo en lugar de copiarlo en otro periodo.
* Workfront elimina los comentarios de un objetivo cerrado cuando se vuelve a abrir. Si debe conservar los comentarios, se recomienda copiar el objetivo cerrado, incluidos los resultados asociados a él, en lugar de volver a abrirlo.


## Cerrar objetivos

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

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) > **Objetivos** en la esquina superior derecha.

   Se abre la lista de objetivos.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique los filtros para mostrar solo los objetivos que están activos.

   Para obtener información sobre el filtrado de información en los objetivos de Workfront, consulte [Filtrar información en objetivos de Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Haga clic en un objetivo activo.

   Se abre la página de objetivo.

   ![](assets/goal-page-unshimmed.png)
1. Haga clic en el **Más** menú ![](assets/more-icon.png) a la derecha del nombre del objetivo y haga clic en **Cerrar**.

   El objetivo se cierra y recibe una confirmación en la esquina superior derecha de la pantalla.

   ![](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Opcional) En el cuadro de confirmación, haga clic en **Agregar notas de cierre** para agregar comentarios sobre este objetivo y por qué debe cerrarlo.
1. Agregue notas de cierre y haga clic en **Agregar notas**.

   ![](assets/add-closing-notes-box-unshimmed.png)

   Los comentarios se muestran en la sección Detalles del objetivo de la página del objetivo, en el área Notas de cierre .

   >[!NOTE]
   >
   >Workfront elimina las notas de cierre si más adelante vuelve a abrir un objetivo cerrado.


## Volver a abrir objetivos

Puede volver a abrir los objetivos cerrados si decide que han vuelto a ser relevantes y que necesita seguir actualizando su progreso.

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

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)> **Objetivos** en la esquina superior derecha.

   Se abre la lista de objetivos.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique los filtros para mostrar solo los objetivos que están cerrados.

   Para obtener información sobre el filtrado de información en los objetivos de Workfront, consulte [Filtrar información en objetivos de Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Haga clic en el nombre de un objetivo cerrado.

   Se abre la página de objetivo.
1. Haga clic en el **Más** menú ![](assets/more-icon.png) a la derecha del nombre del objetivo, **Volver a abrir** > **Volver a abrir**.

   Se producen las siguientes cosas:
   * El objetivo ahora está abierto y tiene el estado Activo.
   * El progreso del objetivo se vuelve a calcular a partir de la fecha actual.
   * Las notas de cierre se eliminan de la página de detalles del objetivo. Las notas de cierre eliminadas no se pueden recuperar.

1. (Opcional) Modifique los filtros de nuevo para mostrar solo los objetivos activos.

   Los objetivos que ha abierto se muestran en la pantalla.

