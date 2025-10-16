---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Eliminar y desactivar metas en Adobe Workfront Goals
description: Cuando empiece a trabajar en una meta y esta se vuelva irrelevante en su organización, recomendamos desactivarla en lugar de eliminarla. La desactivación de una meta conserva su información histórica y le ofrece la oportunidad de reactivarla más adelante. Sin embargo, hay ocasiones en las que puede tener sentido eliminar una meta para mantener la precisión de la lista de metas.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 77%

---

# Eliminar y desactivar metas en Adobe Workfront Goals

<!--Audited for P&P only: 10/2025-->

Cuando empiece a trabajar en una meta y esta se vuelva irrelevante en su organización, recomendamos desactivarla en lugar de eliminarla. La desactivación de una meta conserva su información histórica y le ofrece la oportunidad de reactivarla más adelante. Sin embargo, hay ocasiones en las que puede tener sentido eliminar una meta para mantener la precisión de la lista de metas.

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
<p>Solicitud o superior</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuración de nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
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
 <tr>
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

## Desactivar metas

Puede desactivar una meta que ya no sea relevante y que quizá desee reactivar en el futuro.

* [Consideraciones al desactivar metas](#considerations-when-deactivating-goals)
* [Desactivar metas](#deactivate-goals)

### Consideraciones al desactivar metas

Al desactivar metas, recuerde lo siguiente:

* Solo puede desactivar las metas en estado Activo. Para obtener información sobre cómo activar una meta, consulte [Activar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >No se pueden desactivar las metas en estado de Borrador.

* Workfront deja de calcular el progreso de las metas desactivadas.
* Las metas inactivas ya no se muestran en la sección Gráficos de Workfront Goals o no se tienen en cuenta. Para obtener información acerca de los gráficos de Workfront Goals, consulte [Revisar gráficos para entender las tendencias del progreso de las metas en Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Ya no puede realizar actualizaciones en los objetivos desactivados.
* Puede editar información sobre el objetivo y su alineación.
* Puede reactivar una meta desactivada anteriormente.

### Desactivar metas

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Deactivate**.

   ![Deactivate goal](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **Metas**.

   Se muestra la lista de metas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique los filtros para mostrar solo las metas que están activas.

   Para obtener información sobre cómo filtrar información en Workfront Goals, consulte [Filtrar información en Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).

1. Haga clic en un objetivo activo.

   Se abre la página de la meta.

   ![Página de metas](assets/goal-page-unshimmed.png)

1. Haga clic en el **icono Más** del menú ![Más](assets/more-icon.png) a la derecha del nombre de la meta y, a continuación, haga clic en **Desactivar**.

1. El objetivo se desactiva y su estado pasa a ser Inactivo.

## Eliminar metas

Puede eliminar las metas que ya no son relevantes o que es posible que nunca lo sean.

* [Consideraciones al eliminar metas](#considerations-when-deleting-goals)
* [Eliminar metas](#delete-goals)

### Consideraciones al eliminar metas {#considerations-when-deleting-goals}

* Puede eliminar metas en cualquier estado, incluso las metas cerradas.
* No puede recuperar las metas eliminadas.
* También se eliminan las actividades de la barra de progreso Resultados y Manual adjuntas a la meta.
* Los proyectos asociados con metas no se eliminan; sin embargo, su asociación con la meta se eliminará.

### Eliminar metas

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Delete**.

   ![Delete goal](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Haga clic en el icono del menú principal ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **Metas**.

   Se muestra la lista de metas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Haga clic en el nombre de una meta. Se abre la página de la meta.
1. Haga clic en el **icono Más** del menú ![Más](assets/more-icon.png) a la derecha del nombre de la meta, luego haga clic en **Eliminar meta** y después en **Eliminar**.

   La meta, sus actividades y resultados también se eliminarán y no se podrán recuperar. No se eliminarán los proyectos asociados con la meta o las metas secundarias.


