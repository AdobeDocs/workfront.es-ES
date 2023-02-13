---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Última hora disponible'''
description: El último tiempo disponible (LAT) es un tipo de restricción de tareas en Adobe Workfront.
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Última hora disponible

El último tiempo disponible (LAT) es un tipo de restricción de tareas en Adobe Workfront.

## Usar la restricción de tiempo disponible más reciente

Puede utilizar la restricción LAT cuando desee programar un inicio de una tarea a más tardar en el momento disponible después de considerar las relaciones predecesor-sucesor en el proyecto.

Esta restricción difiere de lo antes posible en que no obligará a los predecesores o sucesores a volver a programarse. En su lugar, solo afecta a la programación de la tarea a la que está asociada, estableciéndola en el último tiempo disponible en función de su relación con otras tareas.

Para obtener información sobre cómo actualizar la restricción de tareas en una tarea, consulte [Actualizar la restricción de tareas de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## La diferencia entre la última hora disponible y la más tarde posible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

La restricción Última hora disponible difiere de la restricción Lo más tarde posible cuando existen los siguientes criterios:

* El proyecto está programado desde la fecha de inicio
* Las tareas del proyecto tienen una relación predecesora
* La tarea sucesora tiene una restricción de tarea flexible

En esta situación:

* **Última hora disponible:** El uso de la restricción de tiempo disponible más reciente en la tarea predecesora da prioridad a la restricción flexible del sucesor.

   **Ejemplo:** Por ejemplo, la tarea A es la predecesora de la tarea B. La tarea A tiene la última restricción de tiempo disponible y la tarea B tiene la restricción Lo antes posible. En este caso, la tarea A está programada lo más cerca posible del inicio del proyecto.

   ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **Tan Tarde Como Sea Posible:** En este escenario, el uso de la restricción Tan tarde como sea posible en la tarea predecesora da prioridad a la tarea predecesora.

   **Ejemplo:** Por ejemplo, la tarea A es la predecesora de la tarea B. La tarea A tiene la restricción Lo más tarde posible y la tarea B tiene la restricción Lo antes posible. En este caso, la tarea A está programada lo más cerca posible del final del proyecto.

   ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
