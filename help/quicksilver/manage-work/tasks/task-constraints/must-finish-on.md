---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Debe finalizar el'
description: Puede utilizar la restricción de tareas Debe finalizar en (MFO) para programar que una tarea finalice en una fecha específica.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Debe finalizar el

Puede utilizar la restricción de tareas Debe finalizar en (MFO) para programar que una tarea finalice en una fecha específica.

La restricción Debe finalizar en programa una tarea para que finalice exactamente en la fecha y hora especificadas en la variable **Fecha de finalización planeada** campo .

>[!TIP]
>
>Al actualizar manualmente la fecha de finalización planificada de una tarea, se cambia la restricción de la tarea a Must Finish On.

## Información general sobre la restricción Debe finalizar en la tarea

Tenga en cuenta lo siguiente al programar una tarea con una restricción Must Finish On :

* Las relaciones anteriores al decesor no obligan a reprogramar la tarea. Adobe Workfront ignora esencialmente las relaciones predecesoras.
* La tarea se muestra como **En riesgo** si los predecesores empiezan a quedarse atrás o se retrasan.

* Cuando se mueve o copia una tarea con una restricción MFO en otro proyecto, la restricción de la tarea o las fechas del proyecto pueden cambiar según las fechas de restricción y las fechas de inicio y finalización del proyecto. Existen los siguientes escenarios:

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
