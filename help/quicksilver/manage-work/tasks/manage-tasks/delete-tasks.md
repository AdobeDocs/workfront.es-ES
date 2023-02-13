---
product-area: projects
navigation-topic: manage-tasks
title: Eliminar tareas
description: Puede eliminar tareas que puedan ser duplicados o que se hayan creado por error.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---

# Eliminar tareas

Puede eliminar tareas que puedan ser duplicados o que se hayan creado por error.

Para las tareas que tienen información histórica (actualizaciones, cambios de programación, estado u otros campos), se recomienda cerrarlas o marcarlas como Muertas en lugar de eliminarlas. Esto le ayuda a mantener la información histórica de sus proyectos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y proyectos con acceso a Eliminar</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a las tareas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Concesión de acceso a tareas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute para el proyecto con capacidad para agregar tareas o superior</p> <p>Cuando crea una tarea, automáticamente recibe permisos de gestión para la tarea</p> <p> Para obtener información sobre los permisos de tareas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartir una tarea </a>. </p> <p>Para obtener información sobre la solicitud de permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Comprender el proceso de eliminación de tareas

* [Limitaciones para eliminar tareas](#limitations-for-deleting-tasks)
* [El impacto de la eliminación de tareas](#the-impact-of-deleting-tasks)

### Limitaciones para eliminar tareas  {#limitations-for-deleting-tasks}

* Cuando un proyecto tiene el estado Completado, solo puede eliminar tareas si el administrador de Workfront o un administrador de grupo lo han permitido en el área Preferencias del proyecto. Para obtener información sobre la configuración de las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si la tarea ha registrado horas, el administrador de Workfront o del grupo debe permitir la eliminación de estas tareas configurando las Preferencias de tarea y problema en la instancia de Workfront. Esto también se aplica cuando intenta eliminar proyectos que tienen tareas con horas registradas.

   <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

   Para obtener más información sobre cómo habilitar la eliminación de tareas en las que se registran horas, consulte la sección &quot;Eliminación&quot; en [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### El impacto de la eliminación de tareas {#the-impact-of-deleting-tasks}

Al eliminar una tarea, se ven afectados otros objetos vinculados a ella.

Los siguientes objetos adjuntos a una tarea también se eliminan al eliminar una tarea:

* Documentos

   No se puede eliminar una tarea que tenga un documento extraído adjunto. Para obtener más información sobre la comprobación de documentos, consulte [Ver documentos](../../../documents/managing-documents/check-out-documents.md).

* Problemas
* Subtareas
* Notas
* Rutas de aprobación

Según la configuración del administrador de Workfront de las preferencias de eliminación de proyectos, tareas o problemas en las preferencias de horario y hora de la instancia de Workfront, las horas registradas para las tareas se gestionan de una de las siguientes maneras al eliminar una tarea:

* Mover al proyecto y no se restaurará en la tarea si la tarea se restaura más tarde.
* Se eliminan y se restauran en la tarea si esta se restaura más tarde.

   Esto también se aplica cuando intenta eliminar proyectos que tienen tareas con horas registradas.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

   Para obtener más información sobre la configuración de las preferencias de eliminación para las horas registradas en los problemas, consulte [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Los gastos de la tarea se trasladarán al proyecto.

* Los usuarios asignados a la tarea o a la aprobación de la tarea permanecen en el equipo del proyecto.

   Para obtener más información sobre los equipos de proyecto, consulte [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Eliminar tareas

* [Eliminar varias tareas de un proyecto simultáneamente](#delete-multiple-tasks-in-a-project-simultaneously)
* [Eliminar una sola tarea](#delete-a-single-task)

### Eliminar varias tareas de un proyecto simultáneamente  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Proyectos**.
1. Haga clic en el nombre del proyecto que contiene las tareas que desea eliminar.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Realice una de las siguientes acciones:

   1. (Condicional) Cuando la variable **Autoguardar** la opción está activada:

      1. Seleccione las tareas que desee eliminar y haga clic en **Más**
      1. Haga clic en **Eliminar**, luego **Sí, Eliminarlo** para confirmar la eliminación.

         Las tareas se eliminan.
   1. (Condicional) Haga clic en el **Modo de plan** y seleccione **Guardar manualmente** si desea revertir los cambios realizados en la lista de tareas.

      ![](assets/nwe-autosave-off-manual-highlighted-350x58.png)

      Haga lo siguiente:

      1. Seleccione las tareas que desee eliminar.
      1. Haga clic en **Eliminar**.
      1. (Opcional) Haga clic en **Deshacer** para invertir el cambio y no eliminar las tareas.
      1. Haga clic en **Rehacer** si desea mantener el cambio y eliminar la tarea.
      1. Haga clic en **Guardar** para eliminar las tareas.

         Las tareas se eliminan únicamente después de guardar los cambios.


### Eliminar una sola tarea {#delete-a-single-task}

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Proyectos**.
1. Haga clic en el nombre del proyecto que contiene la tarea que desea eliminar.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Haga clic en el nombre de la tarea que desee eliminar.
1. Haga clic en el **Más** icono ![](assets/qs-more-menu.png)en la esquina superior derecha.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Haga clic en **Eliminar tarea**.
1. Si la eliminación está permitida, haga clic en **Sí, elimínelo**.

   Es posible que el administrador de Workfront o el administrador de grupos no permitan la eliminación de tareas en las que se registran horas.

   Para obtener más información sobre el acceso y los permisos necesarios para eliminar una tarea, consulte la sección [Limitaciones para eliminar tareas](#limitations-for-deleting-tasks) en este artículo.

## Restaurar tareas eliminadas

Un administrador de Workfront o de grupo puede restaurar tareas en un plazo de 30 días después de eliminarlas, tal como se describe en [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
