---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Eliminar y desactivar objetivos en objetivos de Adobe Workfront
description: Cuando empiece a trabajar en un objetivo y este se vuelva irrelevante en su organización, le recomendamos que lo desactive, en lugar de eliminarlo. Desactivar un objetivo mantiene su información histórica y le ofrece la oportunidad de reactivarla más tarde. Sin embargo, hay ocasiones en las que puede tener sentido borrar un objetivo, para mantener la lista de objetivos correcta.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Eliminar y desactivar objetivos en objetivos de Adobe Workfront

Cuando empiece a trabajar en un objetivo y este se vuelva irrelevante en su organización, le recomendamos que lo desactive, en lugar de eliminarlo. Desactivar un objetivo mantiene su información histórica y le ofrece la oportunidad de reactivarla más tarde. Sin embargo, hay ocasiones en las que puede tener sentido borrar un objetivo, para mantener la lista de objetivos correcta.

## Requisitos de acceso

<!--drafted for P&P release: 

You must have the following:

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
   <td> <p>Editar acceso a Objetivos o posterior</p> <p><b>NOTA</b>

<p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte:</p> 
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

## Desactivar objetivos

Puede desactivar un objetivo que ya no sea relevante y que desee reactivar en el futuro.

* [Consideraciones al desactivar objetivos](#considerations-when-deactivating-goals)
* [Desactivar objetivos](#deactivate-goals)

### Consideraciones al desactivar objetivos

Recuerde lo siguiente al desactivar objetivos:

* Solo puede desactivar objetivos en un estado Activo. Para obtener información sobre cómo activar un objetivo, consulte [Activar objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

   >[!TIP]
   >
   >No se pueden desactivar objetivos en estado de borrador.

* Workfront deja de calcular el progreso de los objetivos desactivados.
* Los objetivos inactivos ya no se muestran ni se tienen en cuenta en la sección Gráficos de los objetivos de Workfront. Para obtener información sobre los gráficos de objetivos de Workfront, consulte [Revisar gráficos para comprender las tendencias de progreso de objetivos en los objetivos de Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

   <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Ya no puede realizar actualizaciones en los objetivos desactivados.
* Puede editar información sobre el objetivo y su alineación.
* Puede reactivar un objetivo previamente desactivado.

### Desactivar objetivos

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **Objetivos**.

   Se muestra la lista de objetivos.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique los filtros para mostrar solo los objetivos que están activos.

   Para obtener información sobre el filtrado de información en los objetivos de Workfront, consulte [Filtrar información en objetivos de Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Haga clic en un objetivo activo.

   Se abre la página de objetivo.

   ![](assets/goal-page-unshimmed.png)

1. Haga clic en el **Más** menú ![](assets/more-icon.png) a la derecha del nombre del objetivo y haga clic en **Desactivar**.

1. El objetivo se desactiva y su estado se vuelve Inactivo.

## Eliminar objetivos

Puede eliminar objetivos que ya no sean relevantes o que nunca lo sean.

* [Consideraciones al eliminar objetivos](#considerations-when-deleting-goals)
* [Eliminar objetivos](#delete-goals)

### Consideraciones al eliminar objetivos {#considerations-when-deleting-goals}

* Puede eliminar objetivos en cualquier estado, incluidos los objetivos cerrados.
* No se pueden recuperar los objetivos eliminados.
* También se eliminan las actividades de la barra de progreso manual y de resultados asociadas al objetivo.
* Los proyectos asociados con objetivos no se eliminan, pero su asociación con el objetivo se elimina.

### Eliminar objetivos

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **Objetivos**.

   Se muestra la lista de objetivos.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Haga clic en el nombre de un objetivo. Esto abre la página de objetivo.
1. Haga clic en el **Más** menú ![](assets/more-icon.png) a la derecha del nombre del objetivo y haga clic en **Eliminar objetivo**, luego **Eliminar**.

   El objetivo y sus actividades y resultados también se eliminan y no se pueden recuperar. Los proyectos asociados con el objetivo o los objetivos secundarios no se eliminan.


