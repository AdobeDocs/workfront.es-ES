---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Información general sobre las restricciones de tareas: No iniciar después del'
description: No comenzar después del (SNLT) es una delimitación de tarea que programa una tarea para que comience antes de la fecha especificada.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
TQID: https://experienceleague.adobe.com/eX2KAzQkOb0AmYcR5Zc6SPeySBTDKjM74QYi7ox4A0w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 436
ht-degree: 53%

---

# Información general sobre la restricción de tarea: no iniciar después de

No comenzar después del (SNLT) es una delimitación de tarea que programa una tarea para que comience antes de la fecha especificada.

Tenga en cuenta lo siguiente al trabajar con la restricción SNLT:

* Debe usar la restricción No comenzar después del cuando el proyecto esté programado desde la fecha de finalización. En este caso, puede proporcionar una restricción suave a una tarea antes de que obligue a otras tareas dependientes a mostrarse como En riesgo.
* No comenzar después de es la delimitación predeterminada si un proyecto utiliza un modo de programación de Programar desde la fecha de finalización y el valor predeterminado del sistema o grupo para la fecha de inicio de una tarea es Hoy. Para obtener información sobre dónde establecer la restricción predeterminada de una tarea nueva, consulte [Configuración de preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Cuando se utiliza la restricción SNLT con un proyecto Programar desde la fecha de inicio, Adobe Workfront programa la tarea como lo haría con una tarea Lo antes posible.
* Cuando se mueve o copia una tarea con una delimitación SNLT a otro proyecto, la delimitación de la tarea o las fechas del proyecto pueden cambiar dependiendo de cuáles sean las fechas de delimitación y cuáles sean las fechas de inicio y finalización del proyecto. Se dan los siguientes escenarios:

   * Cuando el proyecto de destino se programa desde el inicio:

      * Cuando la fecha de restricción de tarea es anterior a la fecha de inicio planificada del proyecto, la restricción de tarea cambia a Lo antes posible.
      * Cuando la fecha de restricción de tarea es posterior a la fecha planificada de finalización del proyecto, la fecha planificada de finalización del proyecto cambia para coincidir con la fecha de restricción de finalización de la tarea.

      * Cuando se programa el proyecto de destino a partir de la finalización:

         * Cuando la fecha de restricción de tarea es posterior a la fecha de finalización del proyecto, la restricción de tarea cambia a Lo más tarde posible.
         * Cuando la fecha de restricción de tarea es anterior a la fecha de inicio planificada del proyecto, la fecha de inicio planificada del proyecto cambia para coincidir con la fecha de restricción de inicio de la tarea.

      * Independientemente de la programación del proyecto, cuando la fecha de restricción de tarea se encuentra dentro de las fechas de inicio y finalización del proyecto, no hay cambios en las fechas de restricción de tarea o del proyecto.

  Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

  Para obtener más información acerca de cómo copiar tareas, vea [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Para obtener información sobre cómo actualizar la restricción de tarea en una tarea, consulte [Actualizar la restricción de tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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
