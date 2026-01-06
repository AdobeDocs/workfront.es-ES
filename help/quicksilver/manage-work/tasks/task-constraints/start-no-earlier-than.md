---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visión General de Restricciones de Tareas: No Iniciar Antes Del'
description: Utilice la delimitación de tareas No comenzar antes del (ENVIAR) para programar el comienzo de una tarea después de la fecha especificada.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 41%

---

# Información general sobre la restricción de tarea: No comenzar antes del

Utilice la delimitación de tareas No comenzar antes del (ENVIAR) para programar el comienzo de una tarea después de la fecha especificada.

## Información general sobre la restricción No comenzar antes de la tarea

Tenga en cuenta lo siguiente al utilizar la restricción No comenzar antes de la tarea:

* Debe utilizar la restricción No comenzar antes del cuando el proyecto esté programado desde la fecha de inicio. En este caso, puede proporcionar una restricción suave a una tarea antes de que obligue a otras tareas dependientes a mostrarse como En riesgo.
* No comenzar antes de es la delimitación predeterminada si un proyecto está programado desde la fecha de inicio y si la fecha de inicio predeterminada del sistema o grupo para una nueva tarea está establecida en Hoy. Para obtener información acerca de cómo configurar los valores predeterminados de las tareas, vea [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Si se programa el proyecto desde la fecha de inicio y la fecha de inicio predeterminada del sistema para una nueva tarea se establece en Basada en la fecha planificada del proyecto, la restricción predeterminada para una nueva tarea será Lo antes posible.
* Si se programa el proyecto desde la fecha de finalización y la fecha de inicio predeterminada del sistema para una tarea nueva se establece en Hoy, la delimitación No comenzar antes del programa la tarea como lo haría con una tarea Lo más tarde posible.
* Cuando se mueve o copia una tarea con una delimitación SNET a otro proyecto, la delimitación de la tarea o las fechas del proyecto pueden cambiar dependiendo de cuáles sean las fechas de delimitación y cuáles sean las fechas de inicio y finalización del proyecto. Se dan los siguientes escenarios:

   * Cuando el proyecto de destino se programa desde el inicio:

      * Cuando la fecha de restricción de tarea es anterior a la fecha de inicio planificada del proyecto, la restricción de tarea cambia a Lo antes posible.
      * Cuando la fecha de restricción de tarea es posterior a la fecha planificada de finalización del proyecto, la fecha planificada de finalización del proyecto cambia para coincidir con la fecha de restricción de finalización de la tarea.

      * Cuando se programa el proyecto de destino a partir de la finalización:

         * Cuando la fecha de restricción de tarea es posterior a la fecha de finalización del proyecto, la restricción de tarea cambia a Lo más tarde posible.
         * Cuando la fecha de restricción de tarea es anterior a la fecha de inicio planificada del proyecto, la fecha de inicio planificada del proyecto cambia para coincidir con la fecha de restricción de inicio de la tarea.

      * Independientemente de la programación del proyecto, cuando la fecha de restricción de tarea se encuentra dentro de las fechas de inicio y finalización del proyecto, no hay cambios en las fechas de restricción de tarea o del proyecto.

  Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obtener más información acerca de cómo copiar tareas, vea [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener información sobre cómo actualizar la restricción de tarea en una tarea, consulte [Actualizar la restricción de tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
