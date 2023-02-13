---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Fechas fijas'''
description: Puede utilizar la restricción de tareas Fechas fijas cuando desee especificar la fecha de inicio y la fecha de finalización exactas de las tareas. Para obtener más información acerca de las restricciones de tareas, consulte Información general sobre la restricción de tareas.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Fechas fijas

Puede utilizar la restricción de tareas Fechas fijas cuando desee especificar la fecha de inicio y la fecha de finalización exactas de las tareas. Para obtener más información sobre las restricciones de tareas, consulte [Información general sobre la restricción de tareas](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Información general sobre la restricción Fechas fijas

Tenga en cuenta lo siguiente al utilizar la restricción Fechas fijas :

* Al seleccionar la restricción de tareas Fechas fijas (FIXT), debe especificar la Fecha de inicio planeada y la Fecha de finalización planeada de la tarea. En este caso, se ignora la relación predecesora de la tarea.
* El campo Duration de la tarea no se puede editar al utilizar la restricción FIXT. La duración se calcula como la diferencia entre las fechas de inicio y finalización planeadas de la tarea.
* Si el tipo de duración de la tarea está impulsado por el esfuerzo, el número de personas asignadas a la tarea también afecta a la duración de la tarea.
* Cuando se mueve o copia una tarea con una restricción FIXT en otro proyecto, la restricción de la tarea o las fechas del proyecto pueden cambiar según las fechas de restricción y las fechas de inicio y finalización del proyecto. Existen los siguientes escenarios:

   * Cuando el proyecto de destino está programado Desde el inicio:

      * Cuando alguna fecha de restricción de la tarea es anterior a la fecha de inicio del proyecto, la restricción de la tarea cambia a Tan pronto como sea posible.
      * Cuando una o ambas fechas de restricción de la tarea son posteriores a la fecha de finalización prevista del proyecto, la fecha de finalización prevista del proyecto cambia para coincidir con la fecha de restricción de finalización de la tarea.
   * Cuando el proyecto de destino está programado Desde su finalización:

      * Cuando cualquier fecha de restricción de la tarea es posterior a la fecha de finalización del proyecto, la restricción de la tarea cambia a Tan tarde como sea posible.
      * Cuando una o ambas fechas de restricción de la tarea son anteriores a la fecha de inicio planeada del proyecto, la fecha de inicio planeada del proyecto cambia para coincidir con la fecha de restricción de inicio de la tarea.
   * Independientemente de la programación del proyecto, cuando las fechas de restricción de la tarea se encuentran dentro de las fechas de inicio y finalización del proyecto, no hay cambios en la restricción de la tarea ni en las fechas del proyecto.

   Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obtener información sobre cómo copiar tareas, consulte [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener información sobre cómo actualizar la restricción de tareas en una tarea, consulte [Actualizar la restricción de tareas de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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
