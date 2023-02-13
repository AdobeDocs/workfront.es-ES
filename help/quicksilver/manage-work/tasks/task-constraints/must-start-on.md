---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Debe comenzar en'
description: Utilice la restricción de tareas de Must Start On (MSO) para programar un inicio de una tarea exactamente en una fecha específica.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Debe comenzar el

Utilice la restricción de tareas de Must Start On (MSO) para programar un inicio de una tarea exactamente en una fecha específica.

La restricción Debe comenzar en programa una tarea para que comience exactamente en la hora y la fecha especificadas en la variable **Fecha de inicio planeada** campo .

>[!TIP]
>
>Al actualizar manualmente la fecha de inicio prevista de una tarea, se cambia la restricción de la tarea a Must Start On.

## Información general sobre la restricción Must Start On Task

Tenga en cuenta lo siguiente al programar una tarea con una restricción Must Start On :

* Las relaciones de predecesor no obligan a esta tarea a volver a programar. Workfront ignora esencialmente cualquier relación predecesora de la tarea con esta restricción.
* La tarea sí muestra **En riesgo** si los predecesores empiezan a correr atrás o tarde.

* Cuando se mueve o copia una tarea con una restricción de MSO en otro proyecto, la restricción de la tarea o las fechas del proyecto pueden cambiar según las fechas de restricción y las fechas de inicio y finalización del proyecto. Existen los siguientes escenarios:

   * Cuando el proyecto de destino está programado Desde el inicio:

      * Cuando la fecha de restricción de la tarea es anterior a la fecha de inicio prevista del proyecto, la restricción de la tarea cambia a Tan pronto como sea posible.
      * Cuando la fecha de restricción de la tarea es posterior a la fecha de finalización prevista del proyecto, la fecha de finalización prevista del proyecto cambia para coincidir con la fecha de restricción de finalización de la tarea.

      * Cuando el proyecto de destino está programado Desde su finalización:

         * Cuando la fecha de restricción de la tarea es posterior a la fecha de finalización del proyecto, la restricción de la tarea cambia a Tan tarde como sea posible.
         * Cuando la fecha de restricción de la tarea es anterior a la fecha de inicio planeada del proyecto, la fecha de inicio planeada del proyecto cambia para coincidir con la fecha de restricción inicial de la tarea.
      * Independientemente de la programación del proyecto, cuando la fecha de restricción de la tarea se encuentra dentro de las fechas de inicio y finalización del proyecto, no hay cambios en la restricción de la tarea ni en las fechas del proyecto.

   Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obtener información sobre cómo copiar tareas, consulte [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener información sobre cómo actualizar la restricción de tareas en una tarea, consulte [Actualizar la restricción de tareas de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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
