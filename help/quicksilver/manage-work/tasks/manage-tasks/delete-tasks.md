---
product-area: projects
navigation-topic: manage-tasks
title: Eliminar tareas
description: Puede eliminar tareas que puedan ser duplicadas o que se hayan creado por error.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '774'
ht-degree: 26%

---

# Eliminar tareas

Puede eliminar tareas que puedan ser duplicadas o que se hayan creado por error.

Para las tareas que tienen información histórica (actualizaciones, cambios de programación, estado u otros campos), recomendamos que los cierre o los marque como Inactivos, en lugar de eliminarlos. Esto le ayuda a mantener la información histórica de sus proyectos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos con acceso para Eliminar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de aportación para el proyecto con capacidad para Añadir tareas o superior</p> <p>Al crear una tarea, recibe automáticamente permisos de administración para dicha tarea</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects with access to&nbsp;Delete</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Comprender el proceso de eliminación de tareas

* [Limitaciones para eliminar tareas](#limitations-for-deleting-tasks)
* [Impacto de la eliminación de tareas](#the-impact-of-deleting-tasks)

### Limitaciones para eliminar tareas  {#limitations-for-deleting-tasks}

* Cuando un proyecto tiene el estado Completo, solo puede eliminar tareas si el administrador de Workfront o de un grupo lo han permitido en el área de Preferencias del proyecto. Para obtener información sobre cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias del proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si la tarea ha registrado horas, el administrador del grupo o de Workfront debe permitir la eliminación de estas tareas configurando las Preferencias de tareas y problemas en la instancia de Workfront. Esto también se aplica cuando se intenta eliminar proyectos que tienen tareas con horas registradas en ellos.

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  Para obtener más información acerca de cómo habilitar la eliminación de tareas en las que se registran horas, consulte la sección &quot;Eliminación&quot; en [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Impacto de la eliminación de tareas {#the-impact-of-deleting-tasks}

Al eliminar una tarea, se afectan otros objetos vinculados a la tarea.

Los siguientes objetos adjuntos a una tarea también se eliminan al eliminarla:

* Documentos

  No se puede eliminar una tarea que tenga un documento desprotegido adjunto. Para obtener más información sobre cómo desproteger documentos, consulte [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

* Problemas
* Subtareas
* Notas
* Rutas de aprobación

Según la forma en que el administrador de Workfront configure las preferencias de eliminación de proyectos, tareas o problemas en las preferencias de plantilla de horas y horas de la instancia de Workfront, las horas registradas para las tareas se gestionan de una de las siguientes maneras al eliminar una tarea:

* Mover al proyecto y no se restaurará en la tarea, si esta se restaura posteriormente.
* Se eliminan y se restaurarán en la tarea, si esta se restaura posteriormente.

  Esto también se aplica cuando se intenta eliminar proyectos que tienen tareas con horas registradas en ellos.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

  Para obtener más información acerca de cómo configurar las preferencias de eliminación para los problemas de horas registradas, consulte [Configurar preferencias de plantilla de horas y de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Los gastos de la tarea se moverán al proyecto.

* Los usuarios asignados a la tarea o a la aprobación de la tarea permanecen en el equipo del proyecto.

  Para obtener más información sobre los equipos del proyecto, consulte [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Eliminar tareas

* [Eliminar varias tareas simultáneamente en un proyecto](#delete-multiple-tasks-in-a-project-simultaneously)
* [Eliminar una sola tarea](#delete-a-single-task)

### Eliminar varias tareas simultáneamente en un proyecto  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Proyectos**.
1. Haga clic en el nombre del proyecto que contiene las tareas que desea eliminar.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Realice una de las siguientes acciones:

   1. (Condicional) Cuando la opción **Guardar automáticamente** esté habilitada:

      1. Seleccione las tareas que desee eliminar y haga clic en **Más**
      1. Haga clic en **Eliminar** y luego en **Eliminar** para confirmar la eliminación.

         Las tareas se eliminan.

   1. (Condicional) Haga clic en el icono **Modo de planificación** y seleccione **Guardar de forma manual** si desea revertir los cambios que realiza en la lista de tareas.

      ![Seleccione Guardar de forma manual](assets/manual-save-option.png)

      Haga lo siguiente:

      1. Seleccione las tareas que desee eliminar.
      1. Haga clic **eliminar**.
      1. (Opcional) Haga clic en **Deshacer** para revertir el cambio y no eliminar las tareas.
      1. Haga clic en **Rehacer** si desea conservar el cambio y eliminar la tarea.
      1. Haga clic en **Guardar** para eliminar las tareas.

         Las tareas solo se eliminan después de guardar los cambios.

### Eliminar una sola tarea {#delete-a-single-task}

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Proyectos**.
1. Haga clic en el nombre del proyecto que contiene la tarea que desea eliminar.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Haga clic en el nombre de la tarea que desee eliminar.
1. Haga clic en el icono **Más** ![](assets/qs-more-menu.png)en la esquina superior derecha.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Haga clic en **Eliminar tarea**.
1. Si la eliminación está permitida, haga clic en **Eliminar**.

   Es posible que el administrador de Workfront o el administrador del grupo no permitan la eliminación de tareas en las que se registran horas.

   Para obtener más información acerca del acceso y los permisos necesarios para eliminar una tarea, consulte la sección [Limitaciones para eliminar tareas](#limitations-for-deleting-tasks) en este artículo.

## Restaurar tareas eliminadas

Un administrador de Workfront o de un grupo puede restaurar tareas dentro de los 30 días posteriores a su eliminación, tal como se describe en [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
