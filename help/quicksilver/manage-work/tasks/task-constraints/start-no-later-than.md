---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Iniciar no más tarde de"'
description: Start No Later Than (SNLT) es una restricción de tarea que programa una tarea para que se inicie antes de la fecha especificada.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Iniciar a más tardar

Start No Later Than (SNLT) es una restricción de tarea que programa una tarea para que se inicie antes de la fecha especificada.

Tenga en cuenta lo siguiente al trabajar con la restricción SNLT:

* Debe utilizar la restricción Iniciar no más tarde que cuando el proyecto esté programado desde la fecha de finalización. En este caso, puede proporcionar una restricción suave a una tarea antes de que obligue a otras tareas dependientes a mostrarse como En riesgo.
* Iniciar no más tarde de es la restricción predeterminada si un proyecto utiliza un modo de programación de Fecha de finalización y el valor predeterminado del sistema o grupo para la Fecha de inicio de una tarea es Hoy. Para obtener información sobre dónde establecer la restricción predeterminada para una nueva tarea, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Cuando se utiliza la restricción SNLT con un proyecto Programar desde fecha de inicio, Adobe Workfront programa la tarea como lo haría en una tarea tan pronto como sea posible.
* Cuando se mueve o copia una tarea con una restricción SNLT en otro proyecto, la restricción de la tarea o las fechas del proyecto pueden cambiar según las fechas de restricción y las fechas de inicio y finalización del proyecto. Existen los siguientes escenarios:

   * Cuando el proyecto de destino está programado Desde el inicio:

      * Cuando la fecha de restricción de la tarea es anterior a la fecha de inicio prevista del proyecto, la restricción de la tarea cambia a Tan pronto como sea posible.
      * Cuando la fecha de restricción de la tarea es posterior a la fecha de finalización prevista del proyecto, la fecha de finalización prevista del proyecto cambia para coincidir con la fecha de restricción de finalización de la tarea.

      * Cuando el proyecto de destino está programado Desde su finalización:

         * Cuando la fecha de restricción de la tarea es posterior a la fecha de finalización del proyecto, la restricción de la tarea cambia a Tan tarde como sea posible.
         * Cuando la fecha de restricción de la tarea es anterior a la fecha de inicio planeada del proyecto, la fecha de inicio planeada del proyecto cambia para coincidir con la fecha de restricción inicial de la tarea.
      * Independientemente de la programación del proyecto, cuando la fecha de restricción de la tarea se encuentra dentro de las fechas de inicio y finalización del proyecto, no hay cambios en la restricción de la tarea ni en las fechas del proyecto.

   Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

   Para obtener información sobre cómo copiar tareas, consulte [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener información sobre cómo actualizar la restricción de tareas en una tarea, consulte [Actualizar la restricción de tareas de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Later Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Later Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>.<br></li>
</ol>
</div>
-->
