---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Información general sobre la restricción de tarea: debe comenzar el'
description: Utilice la restricción de tarea Debe iniciarse el (MSO) para programar que una tarea comience exactamente en una fecha específica.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
TQID: https://experienceleague.adobe.com/I2hGr2ET8y5xR-SYx1dKNWlhgHdI1UfnS0IcQqQOQLs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 395
ht-degree: 98%

---

# Información general sobre la restricción de tarea: Debe iniciarse el

Utilice la restricción de tarea Debe iniciarse el (MSO) para programar que una tarea comience exactamente en una fecha específica.

Lo que hace la restricción Debe iniciarse el es programar una tarea para que comience exactamente a la hora y fecha especificadas en el campo **Fecha de inicio planificada**.

>[!TIP]
>
>Al actualizar manualmente la fecha de inicio planificada de una tarea, la restricción de tarea cambia a Debe iniciarse el.

## Información general sobre la restricción de tarea Debe iniciarse el

Tenga en cuenta lo siguiente al programar una tarea con una restricción Debe iniciarse el:

* Las relaciones de predecesoras no fuerzan la reprogramación de esta tarea. Básicamente, con esta restricción Workfront ignora las relaciones de predecesoras de la tarea.
* La tarea no muestra **En riesgo** si las predecesoras comienzan a ir con cierto retraso o a retrasarse.

* Cuando se mueve o copia una tarea con una restricción MSO a otro proyecto, la restricción de tarea o las fechas del proyecto pueden cambiar dependiendo de cuáles sean las fechas de restricción y cuáles las de inicio y finalización del proyecto. Se dan los siguientes escenarios:

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
