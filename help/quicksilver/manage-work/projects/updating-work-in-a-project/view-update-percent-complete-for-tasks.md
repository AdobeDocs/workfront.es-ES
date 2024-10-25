---
product-area: projects
navigation-topic: update-work-in-a-project
title: Ver y actualizar el porcentaje completado de las tareas
description: Puede actualizar el porcentaje completado de una tarea para indicar el progreso que ha realizado en la tarea hacia completarla.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Ver y actualizar el porcentaje completado de las tareas

<!--Audited:01/2024-->

Puede actualizar el porcentaje completado de una tarea para indicar el progreso que ha realizado en la tarea hacia completarla.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para actualizar las tareas manualmente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nueva licencia: Standard</p> 
   O
   <p>Licencia actual: Trabajo o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para la tarea</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Áreas en las que se puede actualizar el porcentaje completado de una tarea

Puede actualizar el porcentaje completado de una tarea en cualquiera de las siguientes áreas:

* **En una lista de tareas**: puede actualizar el porcentaje completado de una tarea cuando se muestre la columna Porcentaje completado.\
  Para obtener más información acerca de la edición en línea, vea [Editar elementos en línea en una lista de Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **En la vista Hito**: puede actualizar el porcentaje completado de una tarea al usar la vista Hito en una lista de proyectos o un informe de proyectos. Para obtener más información, vea [Usar la vista de Hito](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **En el encabezado de tarea**: puede actualizar el porcentaje completado de una tarea en el encabezado de tarea. Para obtener más información, consulte [Editar tareas](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **En el panel de resumen de una tarea**: puede actualizar el porcentaje completado de una tarea en la parte superior del panel de resumen al ver la tarea en las siguientes áreas:

   * Lista de tareas o informe
   * Hoja de horas
   * Distribuidor de cargas de trabajo

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  Para obtener más información, consulte [Resumen](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Inicio**: puede actualizar el porcentaje completado de una tarea o problema desde el Panel de resumen en el área de Inicio o desde el widget Mi trabajo.

  Para obtener más información, consulte [Introducción a Inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

## Consideraciones acerca de la actualización del porcentaje completado de una tarea

* Cuando marca una tarea como 100% completada, el estado de la tarea se actualiza a Completada.
* Los siguientes escenarios existen para tareas principales:
   * No se puede actualizar el porcentaje completado de una tarea principal al 100% cuando el modo de finalización de resumen del proyecto está establecido en automático y las subtareas no se han completado.
   * Puede actualizar el porcentaje completado de una tarea principal al 100% cuando el modo de finalización de resumen del proyecto esté establecido en Manual y las subtareas estén completadas o incompletas.

  Para obtener más información, consulte [Editar proyectos](../manage-projects/edit-projects.md).

## Actualizar el porcentaje completado de una tarea

1. Vaya a cualquiera de las siguientes áreas de Workfront:

   * Una lista de tareas
   * Una lista de proyectos y aplicar la vista de Hito
   * Una tarea, accediendo a la página de tareas
1. Busque el campo **Porcentaje completado** para la tarea cuyo porcentaje completado desee actualizar.

   >[!TIP]
   >
   >  El campo Porcentaje completado siempre se muestra en la parte superior del panel Resumen.


1. Haga clic dentro del campo **Porcentaje completado** y escriba un número entre 0 y 100

   O

   Haga clic en la barra **Porcentaje completado** y arrástrela hasta el número necesario para indicar la cantidad de la tarea que ha completado, cuando esté disponible.

   >[!NOTE]
   >
   >Cuando indique que se ha completado el 100 % de la tarea, el estado de la tarea también se actualizará a Completada.


1. Pulse Intro en el teclado para guardar el porcentaje completado.

El porcentaje completado del proyecto también se actualiza automáticamente.

