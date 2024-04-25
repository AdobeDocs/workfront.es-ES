---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Eliminar y desactivar metas en Adobe Workfront Goals
description: Cuando empiece a trabajar en un objetivo y este se vuelva irrelevante en su organización, recomendamos desactivarlo, en lugar de eliminarlo. La desactivación de una meta conserva su información histórica y le da la oportunidad de reactivarla más adelante. Sin embargo, hay ocasiones en que puede tener sentido eliminar una meta para mantener la precisión de la lista de metas.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Eliminar y desactivar metas en Adobe Workfront Goals

Cuando empiece a trabajar en un objetivo y este se vuelva irrelevante en su organización, recomendamos desactivarlo, en lugar de eliminarlo. La desactivación de una meta conserva su información histórica y le da la oportunidad de reactivarla más adelante. Sin embargo, hay ocasiones en que puede tener sentido eliminar una meta para mantener la precisión de la lista de metas.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">plan de Adobe Workfront</td>
 <td>
 <p>Cualquiera</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront*</td>
 <td>
 <p>Nueva licencia: Colaborador o superior</p>
 O
 <p>Licencia actual: Solicitud o superior</p> </td>
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
 <td role="rowheader"><p>Nivel de acceso</p></td>
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

## Desactivar metas

Puede desactivar un objetivo que ya no sea relevante y que quizá desee reactivar en el futuro.

* [Consideraciones al desactivar metas](#considerations-when-deactivating-goals)
* [Desactivar metas](#deactivate-goals)

### Consideraciones al desactivar metas

Al desactivar metas, recuerde lo siguiente:

* Solo puede desactivar las metas en estado Activo. Para obtener información sobre cómo activar un objetivo, consulte [Activar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >No se pueden desactivar las metas en estado de Borrador.

* Workfront deja de calcular el progreso de las metas desactivadas.
* Las metas inactivas ya no se muestran en la sección Gráficos de las metas de Workfront o no se tienen en cuenta. Para obtener información sobre los gráficos de Workfront Goals, consulte [Revise los gráficos para comprender las tendencias del progreso de las metas en Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

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

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **Metas**.

   Se muestra la lista de metas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Opcional) Modifique los filtros para mostrar solo las metas que están activas.

   Para obtener información sobre el filtrado de información en Workfront Goals, consulte [Filtrar información en Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).

1. Haga clic en un objetivo activo.

   Se abre la página de la meta.

   ![](assets/goal-page-unshimmed.png)

1. Haga clic en **Más** menú ![](assets/more-icon.png) a la derecha del nombre de la meta y haga clic en **Desactivar**.

1. El objetivo se desactiva y su estado se vuelve Inactivo.

## Eliminar metas

Puede eliminar los objetivos que ya no son relevantes o que es posible que nunca lo sean.

* [Consideraciones al eliminar metas](#considerations-when-deleting-goals)
* [Eliminar metas](#delete-goals)

### Consideraciones al eliminar metas {#considerations-when-deleting-goals}

* Puede eliminar metas en cualquier estado, incluidas las metas cerradas.
* No puede recuperar las metas eliminadas.
* También se eliminan las actividades de la barra de progreso Resultados y Manual adjuntas a la meta.
* Los proyectos asociados con metas no se eliminan, pero su asociación con la meta se elimina.

### Eliminar metas

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

1. Haga clic en el icono Menú principal ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **Metas**.

   Se muestra la lista de metas.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Haga clic en el nombre de una meta. Se abre la página de objetivo.
1. Haga clic en **Más** menú ![](assets/more-icon.png) a la derecha del nombre de la meta y haga clic en **Eliminar meta**, entonces **Eliminar**.

   El objetivo, sus actividades y resultados también se eliminan y no se puede recuperar. No se eliminan los proyectos asociados con la meta o las metas secundarias.


