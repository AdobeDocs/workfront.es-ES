---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Visión General de Restricción de Tareas: Lo Más Temprano Disponible'
description: La hora más temprana disponible es una restricción de tarea que programa una tarea para que comience a la hora más temprana posible después de considerar cualquier relación de predecesora.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 97%

---

# Información general sobre la restricción de tarea: Lo más temprano disponible

La hora más temprana disponible es una restricción de tarea que programa una tarea para que comience a la hora más temprana posible después de considerar cualquier relación de predecesora.

Para obtener información sobre cómo actualizar la restricción de tarea en una tarea, consulte [Actualizar la restricción de tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## Diferencia entre Lo más temprano disponible y Lo antes posible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

La restricción Lo más temprano disponible difiere de la restricción Lo antes posible cuando se cumplen todos los criterios siguientes:

* El proyecto se ha programado desde la finalización
* Las tareas del proyecto tienen una relación de predecesoras
* La tarea predecesora tiene una restricción de tarea flexible

En esta situación:

* **Lo más temprano disponible:** si se utiliza la restricción Lo más temprano disponible en la tarea sucesora, se da prioridad a la restricción flexible de la predecesora.

  **EJEMPLO**

  La Tarea A es la predecesora de la Tarea B. La Tarea B tiene la restricción Lo más temprano disponible y la Tarea A tiene la restricción Lo más tarde posible. En este caso, la Tarea B se programa lo más cerca posible de la finalización del proyecto.

  ![Restricción Lo más temprano disponible cuando la tarea tiene fechas cercanas a la fecha de finalización del proyecto](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **Lo antes posible:** en este escenario, el uso de la restricción Lo antes posible en la tarea sucesora da prioridad a la tarea sucesora.

  **EJEMPLO**

  La Tarea A es la predecesora de la Tarea B. La Tarea B tiene la restricción Lo antes posible y la Tarea A tiene la restricción Lo más tarde posible. En este caso, la Tarea B se programa lo más cerca posible del comienzo del proyecto.

  ![Restricción Lo antes posible cuando la tarea tiene fechas cercanas a la fecha de inicio del proyecto](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
