---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Eliminación de los indicadores de progreso de las metas en Adobe Workfront Goals
description: Puede quitar resultados, actividades y proyectos de las metas en Adobe Workfront Goals cuando ya no sean relevantes.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 83%

---

# Eliminación de los indicadores de progreso de las metas en Adobe Workfront Goals

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Puede quitar resultados, actividades y proyectos de las metas si ya no son relevantes.

Para obtener información sobre cómo crear metas y añadirles resultados y actividades, consulte los siguientes artículos:

* [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md)
* [Añadir actividades a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Añadir resultados a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Editar resultados y actividades en Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Las metas también pueden alinearse con las metas principales, convirtiéndose en metas secundarias. Las metas secundarias también son indicadores de progreso de las metas principales.

Puede eliminar la alineación entre las metas si elimina la conexión entre ellas. Para obtener más información, consulte [Eliminar alineación de metas en Adobe Workfront Goals](../goal-alignment/remove-goal-alignment.md).

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
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

## Requisitos previos

Debe tener una meta asociada a resultados, actividades o proyectos.

## Consideraciones para quitar resultados, actividades y desconectar proyectos de metas

* Solo puede quitar resultados y actividades de las metas activas.
* Puede quitar los resultados y las actividades de una meta. Las actividades y los resultados eliminados no se pueden recuperar.
* Cuando se elimina el resultado o la actividad de una meta, el progreso del resultado eliminado o la actividad afecta al progreso general de la meta.
* No puede eliminar un proyecto de una meta, pero puede desconectarlo de esta. Al desconectar el proyecto de la meta, el porcentaje completado del proyecto ya no afecta al progreso de la meta.

  Para obtener información acerca de cómo afectan los proyectos al progreso de las metas, consulte [Añadir proyectos a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* No se puede eliminar un resultado o una actividad de una meta ni desconectar una meta secundaria o un proyecto si estos son el último indicador de progreso de la meta.
* Si un proyecto se elimina del área de Proyectos y es el último indicador de progreso de una meta, la meta se vuelve Inactiva.

## Eliminar resultados y actividades de las metas

Para quitar resultados y actividades de una meta, elimínelos. La eliminación de resultados y actividades de una meta es idéntica.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![Delete result](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **Metas**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Se abre el área de Workfront Goals y la lista de metas se muestra de forma predeterminada.

1. Haga clic en el nombre de una meta de la que desee quitar resultados y actividades.

   Se abre la página de la meta.

1. Haga clic en **Indicadores de progreso** en el panel de la izquierda.

1. Seleccione un resultado o una actividad y, a continuación, haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete-icon.png) que se encuentra en la parte superior de la lista.

1. Haga clic en **Eliminar** para confirmar la eliminación. El resultado o la actividad se elimina y no se puede recuperar. El porcentaje completado de la meta se actualiza para excluir la actividad o resultado eliminado.


## Eliminar proyectos de metas

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![Disconnect](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Haga clic en el icono **Menú principal** en la esquina superior derecha y luego haga clic en **Metas**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Se abre el área de Workfront Goals y la lista de metas se muestra de forma predeterminada.

1. Haga clic en el nombre de una meta de la que desee quitar resultados y actividades.

   Se abre la página de la meta.
1. Haga clic en **Indicadores de progreso** en el panel de la izquierda.
1. Seleccione un proyecto y luego haga clic en el icono **Desconectar** ![Desconectar](assets/disconnect-icon.png) que se encuentra en la parte superior de la lista.
1. Haga clic en **Desconectar** para confirmar.

   El proyecto ya no está conectado a la meta. El porcentaje completado de la meta se actualiza para excluir el proyecto desconectado.

