---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Información general sobre la restricción de tarea: debe finalizar el'
description: Puede usar la restricción de tarea “Se debe finalizar el” para programar una tarea para que finalice en una fecha específica.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 98%

---

# Información general sobre la restricción de tarea: debe finalizar el

Puede usar la restricción de tarea “Se debe finalizar el” para programar una tarea para que finalice en una fecha específica.

La restricción Debe finalizar el programa una tarea para que finalice exactamente a la hora y fecha especificadas en el campo **Fecha planificada de finalización**.

>[!TIP]
>
>Al actualizar manualmente la fecha planificada de finalización de una tarea, se cambia la restricción de la tarea a Debe finalizar el.

## Información general sobre la restricción de tarea Debe finalizar el

Tenga en cuenta lo siguiente al programar una tarea con una restricción Debe finalizar el:

* Las relaciones de tareas predecesoras no fuerzan la reprogramación de la tarea. Adobe Workfront básicamente ignora las relaciones de tareas predecesoras.
* La tarea se muestra como **En riesgo** si las tareas predecesoras comienzan a retrasarse o llegan tarde.

* Cuando se mueve o copia una tarea con una restricción Debe finalizar el a otro proyecto, la restricción de la tarea o las fechas del proyecto pueden cambiar en función de cuáles sean las fechas de restricción y cuáles sean las fechas de inicio y finalización del proyecto. Se dan los siguientes escenarios:

   * Cuando el proyecto de destino se programa desde el inicio:

      * Cuando la fecha de restricción de tarea es anterior a la fecha de inicio planificada del proyecto, la restricción de tarea cambia a Lo antes posible.
      * Cuando la fecha de restricción de tarea es posterior a la fecha planificada de finalización del proyecto, la fecha planificada de finalización del proyecto cambia para coincidir con la fecha de restricción de finalización de la tarea.

      * Cuando se programa el proyecto de destino a partir de la finalización:

         * Cuando la fecha de restricción de tarea es posterior a la fecha de finalización del proyecto, la restricción de tarea cambia a Lo más tarde posible.
         * Cuando la fecha de restricción de tarea es anterior a la fecha de inicio planificada del proyecto, la fecha de inicio planificada del proyecto cambia para coincidir con la fecha de restricción de inicio de la tarea.

      * Independientemente de la programación del proyecto, cuando la fecha de restricción de tarea se encuentra dentro de las fechas de inicio y finalización del proyecto, no hay cambios en las fechas de restricción de tarea o del proyecto.

  Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obtener más información acerca de cómo copiar tareas, vea [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener más información sobre cómo actualizar la restricción de tarea en una tarea, vea [Actualizar la restricción de tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
