---
product-area: projects
navigation-topic: manage-tasks
title: Eliminar tareas
description: Puede eliminar tareas que puedan ser duplicadas o que se hayan creado por error.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# Eliminar tareas

Puede eliminar tareas que puedan ser duplicadas o que se hayan creado por error.

Para las tareas que tienen información histórica (actualizaciones, cambios de programación, estado u otros campos), recomendamos que los cierre o los marque como Inactivos, en lugar de eliminarlos. Esto le ayuda a mantener la información histórica de sus proyectos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos con acceso para Eliminar</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a las tareas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Conceder acceso a tareas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de contribución al proyecto con capacidad para agregar tareas o superior</p> <p>Al crear una tarea, recibe automáticamente permisos de administración para la tarea</p> <p> Para obtener información sobre los permisos de tareas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartir una tarea </a>. </p> <p>Para obtener información sobre cómo solicitar permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Comprender el proceso de eliminación de tareas

* [Limitaciones para eliminar tareas](#limitations-for-deleting-tasks)
* [Impacto de la eliminación de tareas](#the-impact-of-deleting-tasks)

### Limitaciones para eliminar tareas  {#limitations-for-deleting-tasks}

* Cuando un proyecto tiene el estado Completo, solo puede eliminar tareas si el administrador de Workfront o de un grupo lo han permitido en el área de Preferencias del proyecto. Para obtener información sobre la configuración de preferencias de proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si la tarea ha registrado horas, el administrador del grupo o de Workfront debe permitir la eliminación de estas tareas configurando las Preferencias de tareas y problemas en la instancia de Workfront. Esto también se aplica cuando intenta eliminar proyectos que tienen tareas con horas registradas en ellos.

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  Para obtener más información sobre cómo habilitar la eliminación de tareas en las que se registran horas, consulte la sección &quot;Eliminación&quot; en [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Impacto de la eliminación de tareas {#the-impact-of-deleting-tasks}

Al eliminar una tarea, se afectan otros objetos vinculados a la tarea.

Los siguientes objetos adjuntos a una tarea también se eliminan al eliminarla:

* Documentos

  No se puede eliminar una tarea que tenga un documento desprotegido adjunto. Para obtener más información sobre la retirada de documentos, consulte [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

* Problemas
* Subtareas
* Notas
* Rutas de aprobación

Según la forma en que el administrador de Workfront configure las preferencias de eliminación de proyectos, tareas o problemas en las preferencias de plantilla de horas y horas de la instancia de Workfront, las horas registradas para las tareas se gestionan de una de las siguientes maneras al eliminar una tarea:

* Mover al proyecto y no se restaurará en la tarea, si esta se restaura posteriormente.
* Se eliminan y se restaurarán en la tarea, si esta se restaura posteriormente.

  Esto también se aplica cuando intenta eliminar proyectos que tienen tareas con horas registradas en ellos.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

  Para obtener más información sobre la configuración de las preferencias de eliminación para los problemas de horas de sesión, consulte [Configurar preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Los gastos de la tarea se moverán al proyecto.

* Los usuarios asignados a la tarea o a la aprobación de la tarea permanecen en el equipo del proyecto.

  Para obtener más información sobre los equipos de proyecto, consulte [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Eliminar tareas

* [Eliminar varias tareas simultáneamente en un proyecto](#delete-multiple-tasks-in-a-project-simultaneously)
* [Eliminar una sola tarea](#delete-a-single-task)

### Eliminar varias tareas simultáneamente en un proyecto  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Clic **Proyectos**.
1. Haga clic en el nombre del proyecto que contiene las tareas que desea eliminar.
1. Clic **Tareas** en el panel izquierdo.
1. Realice una de las siguientes acciones:

   1. (Condicional) Cuando la variable **Autoguardar** La opción está activada:

      1. Seleccione las tareas que desee eliminar y haga clic en **Más**
      1. Clic **Eliminar**, entonces **Sí, eliminarla** para confirmar la eliminación.

         Las tareas se eliminan.

   1. (Condicional) Haga clic en **Modo de planificación** y seleccione **Guardado manual** si desea invertir los cambios realizados en la lista de tareas.

      ![Seleccione Guardar manualmente](assets/manual-save-option.png)

      Haga lo siguiente:

      1. Seleccione las tareas que desee eliminar.
      1. Clic **Eliminar**.
      1. (Opcional) Haga clic en **Deshacer** para invertir el cambio y no eliminar las tareas.
      1. Clic **Rehacer** si desea conservar el cambio y eliminar la tarea.
      1. Clic **Guardar** para eliminar las tareas.

         Las tareas solo se eliminan después de guardar los cambios.

### Eliminar una sola tarea {#delete-a-single-task}

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Clic **Proyectos**.
1. Haga clic en el nombre del proyecto que contiene la tarea que desea eliminar.
1. Clic **Tareas** en el panel izquierdo.
1. Haga clic en el nombre de la tarea que desee eliminar.
1. Haga clic en **Más** icono ![](assets/qs-more-menu.png)en la esquina superior derecha.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Clic **Eliminar tarea**.
1. Si la eliminación está permitida, haga clic en **Sí, eliminarla**.

   Es posible que el administrador de Workfront o el administrador del grupo no permitan la eliminación de tareas en las que se registran horas.

   Para obtener más información sobre el acceso y los permisos necesarios para eliminar una tarea, consulte la sección [Limitaciones para eliminar tareas](#limitations-for-deleting-tasks) en este artículo.

## Restaurar tareas eliminadas

Un administrador de Workfront o de grupo puede restaurar tareas en un plazo de 30 días después de eliminarlas, tal como se describe en [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
