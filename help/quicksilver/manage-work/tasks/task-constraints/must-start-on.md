---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Resumen de restricción de tarea: debe comenzar el"
description: Utilice la Restricción de tarea Debe comenzar el (MSO) para programar una tarea para que comience exactamente en una fecha específica.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Información general sobre la restricción de tarea: debe comenzar el

Utilice la Restricción de tarea Debe comenzar el (MSO) para programar una tarea para que comience exactamente en una fecha específica.

La delimitación Debe comenzar el programa una tarea para que comience exactamente a la hora y fecha especificadas en el campo **Fecha planificada de inicio**.

>[!TIP]
>
>Al actualizar manualmente la fecha planificada de inicio de una tarea, se cambia la delimitación de la tarea a Debe comenzar el.

## Información general sobre la restricción Debe comenzar en la tarea

Tenga en cuenta lo siguiente al programar una tarea con una delimitación Debe comenzar el:

* Las relaciones de predecesoras no fuerzan la reprogramación de esta tarea. Workfront ignora las relaciones de predecesoras de la tarea con esta restricción.
* La tarea no muestra **En riesgo** si las predecesoras comienzan a retrasarse o retrasarse.

* Cuando se mueve o copia una tarea con una delimitación MSO a otro proyecto, la delimitación de la tarea o las fechas del proyecto pueden cambiar dependiendo de cuáles sean las fechas de delimitación y cuáles sean las fechas de inicio y finalización del proyecto. Existen los siguientes escenarios:

   * Cuando el proyecto de destino está programado desde el inicio:

      * Cuando la fecha de delimitación de la tarea es anterior a la fecha planificada de inicio del proyecto, la delimitación de la tarea cambia a Lo antes posible.
      * Cuando la fecha de delimitación de la tarea es posterior a la fecha planificada de finalización del proyecto, la fecha planificada de finalización del proyecto cambia para coincidir con la fecha de delimitación de finalización de la tarea.

      * Cuando se programa el proyecto de destino desde la finalización:

         * Cuando la fecha de delimitación de la tarea es posterior a la fecha de finalización del proyecto, la delimitación de la tarea cambia a Lo más tarde posible.
         * Cuando la fecha de delimitación de la tarea es anterior a la fecha planificada de inicio del proyecto, la fecha planificada de inicio del proyecto cambia para coincidir con la fecha de delimitación de inicio de la tarea.

      * Independientemente de la programación del proyecto, cuando la fecha de delimitación de la tarea se encuentra dentro de las Fechas de inicio y finalización del proyecto, no hay cambios en las fechas de delimitación de la tarea o del proyecto.

  Para obtener información acerca de cómo mover tareas, vea [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obtener información acerca de cómo copiar tareas, vea [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener información sobre cómo actualizar la restricción de tarea en una tarea, vea [Actualizar la restricción de tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
