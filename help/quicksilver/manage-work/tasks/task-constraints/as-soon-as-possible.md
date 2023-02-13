---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Tan pronto como sea posible'''
description: Lo antes posible es una restricción de tareas que sitúa la hora de inicio de la tarea lo más cerca posible del comienzo del proyecto.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Lo antes posible

Lo antes posible es una restricción de tareas que sitúa la hora de inicio de la tarea lo más cerca posible del comienzo del proyecto.

## Consideraciones sobre el uso de la restricción Lo antes posible

* Lo antes posible es la restricción predeterminada si un proyecto utiliza el modo de programación desde la fecha de inicio y si la fecha de inicio predeterminada del sistema para una nueva tarea está establecida en Basado en la fecha planificada del proyecto.

* Si un proyecto utiliza el modo de programación Programar desde la fecha de inicio y si el sistema o el grupo define la fecha de inicio predeterminada para una nueva tarea como Hoy, la restricción de tareas predeterminada es Iniciar no antes que

   Para obtener información sobre dónde establecer la restricción predeterminada para una nueva tarea, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Para obtener información sobre cómo actualizar la restricción de tareas en una tarea, consulte [Actualizar la restricción de tareas de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## La diferencia entre la hora más temprana disponible y lo antes posible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

La restricción Tiempo disponible más temprano difiere de la restricción Lo antes posible cuando existen todos los criterios siguientes:

* El proyecto está programado para su finalización.
* Las tareas del proyecto tienen una relación predecesora.
* La tarea predecesora tiene una restricción de tareas flexible.

En esta situación:

* **Hora más temprana disponible:** El uso de la restricción de Tiempo disponible más temprano en la tarea sucesora da prioridad a la restricción flexible del predecesor.

   Por ejemplo, supongamos que la Tarea A es el predecesor de la Tarea B. La Tarea B tiene la restricción de tiempo disponible más temprana y la Tarea A tiene la restricción Tan tarde como sea posible. En este caso, la tarea está programada lo más cerca posible de la finalización del proyecto.

* **Lo Antes Posible:** En este escenario, el uso de la restricción Tan pronto como sea posible en la tarea sucesora da prioridad a la tarea sucesora.

   Por ejemplo, supongamos que la Tarea A es la predecesora de la Tarea B. La Tarea B tiene la restricción Tan pronto como sea posible y la Tarea A tiene la restricción Tan tarde como sea posible. En este caso, la tarea se programa lo más cerca posible del inicio del proyecto.
