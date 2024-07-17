---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Editar resultados y actividades en Adobe Workfront Goals
description: Una vez que el administrador de Adobe Workfront le haya concedido el acceso correcto a las Metas de Adobe Workfront, podrá crear y editar metas, resultados y actividades.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---

# Editar resultados y actividades en Adobe Workfront Goals

Una vez que el administrador de Adobe Workfront le haya concedido el acceso correcto a las Metas de Adobe Workfront, podrá crear y editar metas, resultados y actividades.

Para obtener información sobre la creación de objetivos, resultados y actividades, consulte los siguientes artículos:

* [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md)
* [Introducción a resultados y actividades en Adobe Workfront Goals](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Agregar resultados a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Añadir actividades a objetivos en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

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

## Consideraciones al editar resultados y actividades

<!--
According to Vazgen, access levels will add more considerations.)
-->

* Puede editar los resultados y las actividades que pertenecen a las metas que ha creado o a metas para las que tiene permisos de administración.
* No puede editar el progreso de los proyectos que están conectados a objetivos como actividades desde Objetivos de Workfront. El progreso de los proyectos se actualiza cuando se completan las tareas del proyecto. Puede quitar proyectos de la meta desconectándolos. Para obtener más información, vea la sección &quot;Desconectar proyectos&quot; en el artículo [Quitar resultados, actividades y proyectos de las metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).

  >[!NOTE]
  >
  >Si la siguiente información del proyecto se actualiza en el nivel de proyecto, Workfront Goals la actualiza automáticamente en el nivel de objetivo:
  >
  >   
  >   
  >   * Propietario del proyecto
  >   * Nombre de proyecto
  >   * Porcentaje completado del proyecto
  >   
  >   
  >Para obtener información acerca de cómo conectar proyectos con metas, vea [Agregar proyectos a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Puede eliminar los resultados y las actividades de las metas cuando ya no sean relevantes para el progreso de la meta. Las actividades y los resultados eliminados no se pueden recuperar. Para obtener información acerca de cómo eliminar resultados y actividades, vea [Quitar resultados, actividades y proyectos de las metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).
* Puede editar los resultados y las actividades asociadas con los objetivos de cualquier periodo de tiempo, incluso en el pasado.
* La edición de resultados y actividades actualiza su configuración y no actualiza su progreso. Debe actualizar el progreso de los resultados y las actividades. Para obtener información sobre cómo actualizar el progreso en las metas, los resultados y las actividades, consulte [Actualizar el progreso de las metas en Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

## Editar resultados

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![](assets/results-gear-icon-options-350x85.png)

1. Click **Edit** to edit the following information:

   | Field |Description|
   |---|---|
   | Name |The name of the result. |
   | Owner |The owner of result.  |
   | Value |How you measure the progress of the result. |
   | Initial |The original value of the result. |
   | Target |The desired value when the result is completed. |

1. Click **Save**.
-->


1. Haga clic en el **Menú principal** ![](assets/main-menu-icon.png) y luego en **Metas**.
1. En la Lista de metas, haga clic en el nombre de una meta para abrir su página.
1. Haga clic en **Indicadores de progreso** en el panel izquierdo.
1. Seleccione un resultado en la lista Progress indicators y haga clic en el icono **Editar** ![](assets/edit-icon.png).

   Se abrirá el cuadro Editar resultado.

   ![](assets/edit-result-box-unshimmed.png)

1. Edite la siguiente información:
   * **Nombre del resultado**: El nombre del resultado. Utilice un nombre descriptivo que ilustre qué resultado debe obtener para completar el objetivo.
   * **Propietario del resultado**: El propietario del resultado. El propietario debe ser un usuario activo de Workfront.
   * **Tipo de valor**: Cómo se mide el progreso del resultado.
   * **Valor inicial**: El valor original del resultado.
   * **Valor de destino**: El valor deseado cuando se complete el resultado.
Para obtener más información acerca de los campos de resultados, vea [Agregar resultados a metas](../results-and-activities/add-results-to-goals.md).
1. Haga clic en **Guardar**.

## Editar actividades

<!--
Editing activities differs depending on which environment you use.

### Edit activities in the Production environment

>[!TIP]
>
>You cannot edit the Activity Type after you saved an activity on a goal.

1. Go to the goal for which you want to edit an activity and click the goal name to open the **Goal Details** panel.
1. Click **Activities**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. Haga clic en el **Menú principal** ![](assets/main-menu-icon.png) y luego en **Metas**.
1. En la Lista de metas, haga clic en el nombre de una meta para abrir su página.
1. Haga clic en **Indicadores de progreso** en el panel izquierdo.
1. Seleccione una actividad en la lista Progress indicators y haga clic en el icono **Editar** ![](assets/edit-icon.png).

   Se abrirá el cuadro Editar actividad.

   ![](assets/edit-activity-box-unshimmed.png)

1. Edite la siguiente información:
   * **Nombre de actividad**: El nombre de la actividad. Utilice un nombre descriptivo que ilustre qué actividad debe realizar para indicar que el objetivo se completa.
   * **Propietario de la actividad:** El propietario de la actividad. El propietario debe ser un usuario activo de Workfront.\
     Para obtener más información acerca de los campos de actividad, vea [Agregar actividades a los objetivos](../results-and-activities/add-activities-to-goals.md).
1. Haga clic en **Guardar**.


