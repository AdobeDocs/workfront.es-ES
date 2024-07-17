---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Información general sobre la restricción de tarea: Lo más temprano disponible"
description: La hora disponible más temprana es una delimitación de tarea que programa una tarea para que comience en el momento disponible más temprano después de considerar cualquier relación de predecesoras.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Información general sobre la restricción de tarea: Lo más temprano disponible

La hora disponible más temprana es una delimitación de tarea que programa una tarea para que comience en el momento disponible más temprano después de considerar cualquier relación de predecesoras.

Para obtener información sobre cómo actualizar la restricción de tarea en una tarea, vea [Actualizar la restricción de tarea de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## La diferencia entre Lo antes posible y Lo antes posible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

La restricción Lo antes posible difiere de la restricción Lo antes posible cuando existen todos los criterios siguientes:

* El proyecto está programado desde la finalización
* Las tareas del proyecto tienen una relación de predecesoras
* La tarea predecesora tiene una restricción de tarea flexible

En esta situación:

* **Hora disponible más temprana:** Si se utiliza la restricción de la primera hora disponible en la tarea sucesora, se da prioridad a la restricción flexible de la predecesora.

  **EJEMPLO**

  La Tarea A es la predecesora de la Tarea B. La Tarea B tiene la restricción de la primera hora disponible y la Tarea A tiene la restricción de la mayor demora posible. En este caso, la Tarea B se programa lo más cerca posible de la finalización del proyecto.

  ![Restricción de tiempo disponible más temprano cuando la tarea tiene fechas cercanas a la fecha de finalización del proyecto](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **Lo antes posible:** En este escenario, el uso de la restricción Lo antes posible en la tarea sucesora da prioridad a la tarea sucesora.

  **EJEMPLO**

  La Tarea A es la predecesora de la Tarea B. La Tarea B tiene la restricción Lo antes posible y la Tarea A tiene la restricción Lo más tarde posible. En este caso, la Tarea B se programa lo más cerca posible del comienzo del proyecto.

  ![Restricción lo antes posible cuando la tarea tiene fechas cercanas a la fecha de inicio del proyecto](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
