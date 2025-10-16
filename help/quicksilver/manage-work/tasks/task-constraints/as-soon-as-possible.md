---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Información General Sobre La Restricción De Tareas: Lo Antes Posible'
description: Lo antes posible es una restricción de tareas que sitúa la hora de inicio de la tarea lo más cerca posible del comienzo del proyecto.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 98%

---

# Información general sobre la restricción de tareas: lo antes posible

Lo antes posible es una restricción de tareas que sitúa la hora de inicio de la tarea lo más cerca posible del comienzo del proyecto.

## Consideraciones de uso de la restricción Lo antes posible

* Lo antes posible es la restricción predeterminada en caso de que un proyecto use un modo de programación de Programar desde la fecha de inicio y en caso de que la fecha de inicio predeterminada del sistema para una nueva tarea se establezca en Basada en la fecha de planificación del proyecto.

* En caso de que un proyecto use un modo de programación de Programar desde la fecha de inicio y en caso de que la fecha de inicio predeterminada del sistema o del grupo para una nueva tarea se establezca en Hoy, la restricción de tarea predeterminada será No comenzar antes del.

  Para obtener información sobre dónde establecer la restricción predeterminada de una tarea nueva, consulte [Configuración de preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Para obtener información sobre cómo actualizar la restricción de la tarea de una tarea, consulte [Actualizar la restricción de la tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## Diferencia entre Lo más temprano disponible y Lo antes posible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

La restricción Lo más temprano disponible difiere de la restricción Lo antes posible cuando se cumplen todos los criterios siguientes:

* Se programó el proyecto desde la finalización.
* Las tareas del proyecto tienen una relación predecesora.
* La tarea predecesora tiene una restricción de tarea flexible.

En esta situación:

* **Lo más temprano disponible:** en caso de utilizar la restricción Lo más temprano disponible en la tarea sucesora, se dará prioridad a la restricción flexible de la predecesora.

  Por ejemplo, supongamos que la Tarea A fuera la predecesora de la Tarea B. La Tarea B tiene la restricción Lo más temprano disponible y la Tarea A tiene la restricción Lo más tarde posible. En este caso, la tarea se programará lo más cerca posible de la finalización del proyecto.

* **Lo antes posible:** en este escenario, el uso de la restricción Lo antes posible en la tarea sucesora dará prioridad a la tarea sucesora.

  Por ejemplo, supongamos que la Tarea A fuera predecesora de la Tarea B. La Tarea B tiene la restricción Lo antes posible y la Tarea A tiene la restricción Lo más tarde posible. En este caso, la tarea se programará lo más cerca posible del inicio del proyecto.
