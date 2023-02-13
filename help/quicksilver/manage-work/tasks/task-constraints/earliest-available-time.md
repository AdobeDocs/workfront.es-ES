---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Hora disponible más temprana'''
description: El Tiempo Disponible Más Temprano es una Restricción de Tareas que programa una tarea para que comience lo antes posible después de considerar cualquier relación predecesora.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Hora disponible más temprana

El Tiempo Disponible Más Temprano es una Restricción de Tareas que programa una tarea para que comience lo antes posible después de considerar cualquier relación predecesora.

Para obtener información sobre cómo actualizar la restricción de tareas en una tarea, consulte [Actualizar la restricción de tareas de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## La diferencia entre la hora más temprana disponible y lo antes posible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

La restricción Tiempo disponible más temprano difiere de la restricción Lo antes posible cuando existen todos los criterios siguientes:

* El proyecto está programado a partir de su finalización
* Las tareas del proyecto tienen una relación predecesora
* La tarea predecesora tiene una restricción de tarea flexible

En esta situación:

* **Hora más temprana disponible:** El uso de la restricción de Tiempo disponible más temprano en la tarea sucesora da prioridad a la restricción flexible del predecesor.

   **Ejemplo:** La tarea A es la predecesora de la tarea B. La tarea B tiene la restricción de tiempo disponible más temprana y la tarea A tiene la restricción lo más tarde posible. En este caso, la tarea B está programada lo más cerca posible de la finalización del proyecto.

   ![Restricción de tiempo disponible más temprana cuando la tarea tiene las fechas cercanas a la fecha de finalización del proyecto](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **Lo Antes Posible:** En este escenario, el uso de la restricción Tan pronto como sea posible en la tarea sucesora da prioridad a la tarea sucesora.

   **Ejemplo:**  La tarea A es la predecesora de la tarea B. La tarea B tiene la restricción Lo antes posible y la tarea A tiene la restricción Lo más tarde posible. En este caso, la tarea B está programada lo más cerca posible del inicio del proyecto.

   ![Restricción tan pronto como sea posible cuando la tarea tiene las fechas cercanas a la Fecha de inicio del proyecto](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
