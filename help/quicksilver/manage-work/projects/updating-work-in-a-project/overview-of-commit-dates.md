---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Información general sobre la fecha de confirmación
description: La fecha de confirmación es la fecha en la que un usuario asignado a una tarea o un problema se compromete a completar la tarea o el problema. Esto es diferente a la fecha planificada de finalización, ya que es una estimación más realista de la fecha de finalización dada por el usuario que está directamente a cargo del trabajo.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 38%

---

# Información general sobre la fecha de confirmación

<!--Audited: 05/2025-->

<!-- <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

La fecha de confirmación es la fecha en la que un usuario asignado a una tarea o un problema se compromete a completar la tarea o el problema. Esto difiere de la fecha planificada de finalización de una tarea o problema ya que es una estimación más realista de la fecha de finalización dada únicamente por el usuario a cargo del trabajo.

Para obtener información acerca de la fecha planificada de finalización, vea [Información general sobre la fecha planificada de finalización de una tarea](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Información general sobre la fecha de confirmación

Al trabajar con fechas de compromiso, tenga en cuenta lo siguiente:

* Solo las tareas y los problemas tienen una fecha de compromiso.
* Adobe Workfront no establece automáticamente las fechas de confirmación. Al crear una tarea o un problema, no hay ninguna fecha de compromiso asignada.
* Si se le asigna una tarea o un problema, puede establecer la fecha de compromiso mediante uno de los procedimientos siguientes:

   * Permitir que Workfront establezca la fecha de compromiso para que coincida con la fecha planificada de finalización existente de la tarea o problema al hacer clic en Trabajar en ello, Iniciar problema o Iniciar tarea en la tarea o problema. Para obtener más información, vea [Reemplazar el botón Trabajar en ello por un botón Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Establezca manualmente la fecha de confirmación en función de cuándo cree que se completará la tarea o el problema. Esta es su estimación y compromiso, como persona asignada, con el administrador del proyecto de que la tarea o problema se habrá completado en una fecha determinada. Para obtener más información, consulte [Actualizar fechas de compromiso de tareas y problemas](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

>[!NOTE]
>
>Debe ser el propietario de la tarea para cambiar la fecha de compromiso de una tarea. Los siguientes usuarios no pueden cambiar la fecha de confirmación de una tarea:
>
>* Propietario del proyecto
>* Patrocinador de proyecto
>* Gerente de recursos
>* Administrador del sistema
>* Cualquier otro usuario asignado a la tarea
>* Cualquier otro usuario con permisos para la tarea
>
>Para obtener más información sobre el propietario de la tarea, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Localizar la fecha de compromiso de las tareas y los problemas

Puede encontrar la fecha de confirmación de las tareas y problemas en las siguientes áreas de Workfront:

* La página Detalles
* El Panel de resumen, después de que un administrador de Workfront o de un grupo, lo añada a la plantilla de diseño. Para obtener más información, consulte [Personalizar el panel de resumen con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Encabezado de una tarea o problema después de que un administrador de Workfront o de grupo lo añada a la plantilla de diseño. Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Notificaciones y actualizaciones activadas al cambiar la fecha de compromiso {#notifications-and-updates-triggered-by-changing-the-commit-date}

Cuando un usuario asignado a una tarea o a un problema cambia manualmente una fecha de compromiso a una fecha diferente a la fecha planificada de finalización establecida por el propietario del proyecto, hay varias notificaciones y actualizaciones que avisan al propietario del proyecto y a otros usuarios de este cambio.

>[!NOTE]
>
>Los cambios realizados en la fecha de compromiso no cambian automáticamente las fechas planificadas, y los cambios realizados en las fechas planificadas no cambian automáticamente la fecha de compromiso.

La configuración manual de la fecha de compromiso para una tarea o un problema desencadena los siguientes cambios:

* El cambio de fecha de confirmación se rellena en las pestañas Actividad del sistema y Todos de la sección Actualización de la tarea o el problema.

  ![Notificar cambio de fecha de confirmación](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  El cambio de fecha de confirmación se muestra en el área de Actualizaciones de la tarea o del problema cuando el administrador de Workfront habilita esta actualización en el área de Fuentes de actualizaciones en Configuración.Para obtener más información, consulte [Actualizaciones rastreadas por el sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

  Si el propietario del proyecto no desea aceptar el cambio, le recomendamos que realice un comentario para el usuario que propone una nueva fecha con la pestaña Comentarios en la sección Actualizaciones, que vuelva a cambiar la fecha de compromiso a la fecha planificada original o que seleccione una nueva fecha.

  Si el propietario de un proyecto acepta el cambio, puede ajustar manualmente la fecha planificada de finalización para que coincida con la fecha de confirmación ofrecida por el usuario asignado al elemento mediante la edición de la tarea o el problema.

  Debe tener acceso para administrar la tarea o el problema y editarlos.

  >[!TIP]
  >
  >Puede pedir al administrador del sistema o del grupo que añada el campo Fecha de confirmación al panel de resumen o al encabezado para facilitar la actualización.
  >
  >Para obtener más información, consulte los siguientes artículos:
  >
  >* [Resumen general](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [Personalizar el panel de resumen mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [Personalizar encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* La fecha proyectada de finalización de la tarea o problema se establece en la misma fecha porque la tarea tiene ahora una indicación más precisa de cuándo es probable que se complete.

  Para obtener más información, consulte [Información general sobre la fecha proyectada de finalización para proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* En el área Notificaciones se notifica al propietario del proyecto de que ha cambiado la fecha de confirmación de una tarea o problema.

  ![Notificar cambio de fecha de confirmación](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >La notificación de que la fecha de confirmación ha cambiado se envía al propietario del proyecto solo cuando el administrador de Workfront habilita la visualización de la fecha de confirmación en el área Fuentes de actualizaciones en Configuración. Para obtener más información, consulte [Actualizaciones con seguimiento del sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Para obtener información acerca de la funcionalidad adicional disponible al actualizar un elemento de trabajo, vea [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Para obtener información sobre cómo actualizar las fechas de confirmación de tareas y problemas, consulte [Actualizar las fechas de confirmación de tareas y problemas](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
