---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Información general sobre la restricción de tarea: no finalizar después de"
description: No finalizar después del es una delimitación de tarea que programa una tarea para que finalice antes de la fecha especificada.
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Información general sobre la restricción de tarea: no finalizar después del

No finalizar después del es una delimitación de tarea que programa una tarea para que finalice antes de la fecha especificada.

## Descripción general de la restricción No finalizar después del

Tenga en cuenta lo siguiente al utilizar la delimitación No finalizar después del (FNLT) para una tarea:

* Debe utilizar esta restricción cuando el proyecto esté programado desde la fecha de inicio. En este caso, puede proporcionar una restricción suave a una tarea antes de que obligue a otras tareas dependientes a mostrarse como En riesgo.
* Cuando se utiliza la delimitación FNLT con un proyecto Programar desde la fecha de finalización, esta delimitación programa la tarea como lo haría con una tarea Lo más tarde posible.
* Cuando se mueve o copia una tarea con una delimitación FNET a otro proyecto, la delimitación de la tarea o las fechas del proyecto pueden cambiar dependiendo de cuáles sean las fechas de delimitación y cuáles sean las fechas de inicio y finalización del proyecto. Existen los siguientes escenarios:

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
