---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Finalizar No Más Tarde Que'
description: Finalizar no más tarde del (FNLT) es una restricción de tarea que programa una tarea para que se complete antes de la fecha especificada.
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Finalizar a más tardar

Finalizar no más tarde del (FNLT) es una restricción de tarea que programa una tarea para que se complete antes de la fecha especificada.

## Información general sobre la restricción Terminar no más tarde que

Tenga en cuenta lo siguiente cuando utilice la restricción Finalizar no después de (FNLT) para una tarea:

* Debe utilizar esta restricción cuando el proyecto esté programado desde la fecha de inicio. En este caso, puede proporcionar una restricción suave a una tarea antes de que obligue a otras tareas dependientes a mostrarse como En riesgo.
* Cuando se utiliza la restricción FNLT con un proyecto de Programar desde la fecha de finalización, esta restricción programa la tarea como lo haría con una tarea tan tarde como sea posible.
* Cuando se mueve o copia una tarea con una restricción FNET en otro proyecto, la restricción de la tarea o las fechas del proyecto pueden cambiar dependiendo de cuáles sean las fechas de restricción y cuáles son las fechas de inicio y finalización del proyecto. Existen los siguientes escenarios:

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
<h2>Use the Finish No Later Than constraint</h2>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Finish No Later Than</strong>.</p> <p> <img src="assets/fnlt-350x266.png" alt="FNLT.png" style="width: 350;height: 266;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>You must complete the task on and not later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
