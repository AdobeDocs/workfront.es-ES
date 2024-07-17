---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Resumen de la restricción de tareas: lo antes posible"
description: Lo antes posible es una restricción de tarea que sitúa la hora de inicio de la tarea lo más cerca posible del comienzo del proyecto.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Información general sobre la restricción de tarea: lo antes posible

Lo antes posible es una restricción de tarea que sitúa la hora de inicio de la tarea lo más cerca posible del comienzo del proyecto.

## Consideraciones para utilizar la restricción Lo antes posible

* Lo antes posible es la delimitación predeterminada si un proyecto utiliza un modo de horario a partir de la fecha de inicio y si la fecha de inicio predeterminada del sistema para una nueva tarea está establecida en Basado en la fecha planificada del proyecto.

* Si un proyecto utiliza un modo de programación de Programar desde la fecha de inicio y si la fecha de inicio predeterminada del sistema o del grupo para una nueva tarea está establecida en Hoy, la restricción de tarea predeterminada es No comenzar antes del.

  Para obtener información sobre dónde establecer la restricción predeterminada para una tarea nueva, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Para obtener información sobre cómo actualizar la restricción de tarea en una tarea, vea [Actualizar la restricción de tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## La diferencia entre Lo antes posible y Lo antes posible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

La restricción Lo antes posible difiere de la restricción Lo antes posible cuando existen todos los criterios siguientes:

* Se ha programado el proyecto desde la finalización.
* Las tareas del proyecto tienen una relación de predecesoras.
* La tarea predecesora tiene una restricción de tarea flexible.

En esta situación:

* **Hora disponible más temprana:** Si se utiliza la restricción de la primera hora disponible en la tarea sucesora, se da prioridad a la restricción flexible de la predecesora.

  Por ejemplo, supongamos que la Tarea A es la predecesora de la Tarea B. La Tarea B tiene la restricción de la primera hora disponible y la Tarea A tiene la restricción de la mayor demora posible. En este caso, la tarea se programa lo más cerca posible de la finalización del proyecto.

* **Lo antes posible:** En este escenario, el uso de la restricción Lo antes posible en la tarea sucesora da prioridad a la tarea sucesora.

  Por ejemplo, supongamos que la Tarea A es predecesora de la Tarea B. La Tarea B tiene la restricción Lo antes posible y la Tarea A tiene la restricción Lo más tarde posible. En este caso, la tarea se programa lo más cerca posible del comienzo del proyecto.
