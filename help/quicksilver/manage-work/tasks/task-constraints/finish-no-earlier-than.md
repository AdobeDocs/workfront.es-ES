---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Finalizar No Antes De'
description: Finalizar no antes de (FNET) es una restricción de tareas que programa una tarea para que se complete después de la fecha especificada.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Finalizar no antes del

Finalizar no antes de (FNET) es una restricción de tareas que programa una tarea para que se complete después de la fecha especificada.

## Información general sobre la restricción Finalizar No antes del

Tenga en cuenta lo siguiente cuando utilice la restricción No anterior a (FNET) para una tarea:

* Debe utilizar esta restricción cuando el proyecto esté programado desde la fecha de finalización. En este caso, puede proporcionar una restricción suave a la tarea antes de forzar que otras tareas dependientes se muestren En riesgo.
* Cuando se utiliza FNET en un proyecto programado **Desde la fecha de inicio**, la restricción programa la tarea tal como la programaría si la restricción fuera lo antes posible.
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
