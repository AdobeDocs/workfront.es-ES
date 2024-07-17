---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Resumen de restricción de tarea: fechas fijas"
description: Puede utilizar la delimitación de tareas Fechas fijas cuando desee especificar la fecha exacta de inicio y finalización de las tareas. Para obtener más información sobre las delimitaciones de tareas, vea Información general sobre las delimitaciones de tareas.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Información general sobre la restricción de tarea: fechas fijas

Puede utilizar la delimitación de tareas Fechas fijas cuando desee especificar la fecha exacta de inicio y finalización de las tareas. Para obtener más información acerca de las restricciones de tareas, vea [Información general sobre la restricción de tareas](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Información general sobre la restricción Fechas fijas

Tenga en cuenta lo siguiente al utilizar la restricción Fechas fijas:

* Al seleccionar la delimitación de tareas Fechas fijas (FIXT), debe especificar la Fecha planificada de inicio y la Fecha planificada de finalización de la tarea. En este caso, se ignora la relación de predecesora de la tarea.
* El campo Duración de la tarea no se puede editar al utilizar la restricción FIXT. La duración se calcula como la diferencia entre las fechas planificadas de inicio y finalización de la tarea.
* Si el Tipo de duración de la tarea es Condicionada por el esfuerzo, el número de personas asignadas a la tarea también afectará a la Duración de la tarea.
* Cuando se mueve o copia una tarea con una delimitación FIXT a otro proyecto, la delimitación de la tarea o las fechas del proyecto pueden cambiar dependiendo de cuáles sean las fechas de delimitación y cuáles sean las fechas de inicio y finalización del proyecto. Existen los siguientes escenarios:

   * Cuando el proyecto de destino está programado desde el inicio:

      * Cuando las fechas de delimitación de la tarea son anteriores a la fecha de inicio del proyecto, la delimitación de la tarea cambia a Lo antes posible.
      * Cuando una o ambas fechas de delimitación de la tarea son posteriores a la fecha planificada de finalización del proyecto, la fecha planificada de finalización del proyecto cambia para coincidir con la fecha de delimitación de finalización de la tarea.

   * Cuando se programa el proyecto de destino desde la finalización:

      * Cuando las fechas de delimitación de la tarea son posteriores a la fecha de finalización del proyecto, la delimitación de la tarea cambia a Lo más tarde posible.
      * Cuando una o ambas fechas de delimitación de la tarea son anteriores a la fecha planificada de inicio del proyecto, la fecha planificada de inicio del proyecto cambia para coincidir con la fecha de delimitación de inicio de la tarea.

   * Independientemente de la programación del proyecto, cuando las fechas de delimitación de la tarea se encuentran dentro de las fechas de comienzo y finalización del proyecto, no hay cambios en las fechas de delimitación de tarea o de proyecto.

  Para obtener información acerca de cómo mover tareas, vea [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obtener información acerca de cómo copiar tareas, vea [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener información sobre cómo actualizar la restricción de tarea en una tarea, vea [Actualizar la restricción de tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
