---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Eliminar y desactivar metas en Adobe Workfront Goals
description: Cuando empiece a trabajar en una meta y esta se vuelva irrelevante en su organización, recomendamos desactivarla en lugar de eliminarla. La desactivación de una meta conserva su información histórica y le ofrece la oportunidad de reactivarla más adelante. Sin embargo, hay ocasiones en las que puede tener sentido eliminar una meta para mantener la precisión de la lista de metas.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 89%

---

# Eliminar y desactivar metas en Adobe Workfront Goals

Cuando empiece a trabajar en una meta y esta se vuelva irrelevante en su organización, recomendamos desactivarla en lugar de eliminarla. La desactivación de una meta conserva su información histórica y le ofrece la oportunidad de reactivarla más adelante. Sin embargo, hay ocasiones en las que puede tener sentido eliminar una meta para mantener la precisión de la lista de metas.

## Requisitos de acceso

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
 <td role="rowheader"><p>Nivel de acceso</p></td>
 <td> <p>Editar acceso a Goals</p> </td>
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


