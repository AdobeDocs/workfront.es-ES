---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Información General Sobre Restricciones De Tareas: No Finalizar Antes De'
description: No finalizar antes del (FNET) es una delimitación de tarea que programa una tarea para que finalice después de la fecha especificada.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 52%

---

# Información general sobre la restricción de tarea: No finalizar antes del

No finalizar antes del (FNET) es una delimitación de tarea que programa una tarea para que finalice después de la fecha especificada.

## Descripción general de la restricción No terminar antes del

Tenga en cuenta lo siguiente cuando utilice la delimitación No finalizar antes del (FNET) para una tarea:

* Debe utilizar esta restricción cuando el proyecto esté programado desde la fecha de finalización. En este caso, puede proporcionar una restricción suave a la tarea antes de forzar a que otras tareas dependientes muestren En riesgo.
* Cuando se usa FNET en un proyecto programado **Desde la fecha de inicio**, la restricción programa la tarea como lo haría si la restricción fuera Lo antes posible.
* Cuando se mueve o copia una tarea con una delimitación FNET a otro proyecto, la delimitación de la tarea o las fechas del proyecto pueden cambiar dependiendo de cuáles sean las fechas de delimitación y cuáles sean las fechas de inicio y finalización del proyecto. Se dan los siguientes escenarios:

   * Cuando el proyecto de destino se programa desde el inicio:

      * Cuando la fecha de restricción de tarea es anterior a la fecha de inicio planificada del proyecto, la restricción de tarea cambia a Lo antes posible.
      * Cuando la fecha de restricción de tarea es posterior a la fecha planificada de finalización del proyecto, la fecha planificada de finalización del proyecto cambia para coincidir con la fecha de restricción de finalización de la tarea.

   * Cuando se programa el proyecto de destino a partir de la finalización:

      * Cuando la fecha de restricción de tarea es posterior a la fecha de finalización del proyecto, la restricción de tarea cambia a Lo más tarde posible.
      * Cuando la fecha de restricción de tarea es anterior a la fecha de inicio planificada del proyecto, la fecha de inicio planificada del proyecto cambia para coincidir con la fecha de restricción de inicio de la tarea.

   * Independientemente de la programación del proyecto, cuando la fecha de restricción de tarea se encuentra dentro de las fechas de inicio y finalización del proyecto, no hay cambios en las fechas de restricción de tarea o del proyecto.

  Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md). Para obtener más información acerca de cómo copiar tareas, vea [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

  Para obtener más información sobre cómo actualizar la restricción de tarea en una tarea, vea [Actualizar la restricción de tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Earlier Than constraint</h2>
<p>(NOTE: replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Finish No Earlier Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>Finish No Earlier Than</strong>.</p> <p> <img src="assets/fnet-350x267.png" alt="FNET.png" style="width: 350;height: 267;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete no earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes.</strong> </li>
</ol>
</div>
-->
