---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Descripción general de "Restricción de tareas": Tan Tarde como sea posible'''
description: Tan tarde como sea posible (ALAP) es una restricción de tareas de Adobe Workfront que coloca la hora de finalización de la tarea lo más cerca posible del final del proyecto.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Información general sobre la restricción de tareas: Tan Tarde como sea posible

Tan tarde como sea posible (ALAP) es una restricción de tareas de Adobe Workfront que coloca la hora de finalización de la tarea lo más cerca posible del final del proyecto.

El uso de esta restricción puede hacer que el predecesor o las tareas dependientes se reprogramen.

Para obtener más información sobre las relaciones predecesoras, consulte [Usar predecesores de tareas](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

Tan tarde como sea posible es la restricción predeterminada si un proyecto utiliza un modo de programación de Fecha de finalización y el valor predeterminado del sistema o grupo para la Fecha de inicio de una tarea se basa en la fecha planificada del proyecto.

Para obtener información sobre dónde establecer la restricción predeterminada para una nueva tarea, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Para obtener información sobre cómo actualizar la restricción de tareas en una tarea, consulte [Actualizar la restricción de tareas de una tarea](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible:&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click&nbsp;<strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the&nbsp;<strong>Overview</strong>&nbsp;section, expand the&nbsp;<strong>Task Constraint</strong>&nbsp;drop-down menu.</p> </li>
<li value="4"> <p>Select&nbsp;<strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

## La diferencia entre la última hora disponible y la más tarde posible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
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
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest&nbsp;Available Time constraint differs from the As Late&nbsp;As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest&nbsp;Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest&nbsp;Available Time constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close&nbsp;to the start&nbsp;of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late&nbsp;As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late&nbsp;As Possible&nbsp;constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close to the end&nbsp;of the project as possible.</p> </li>
</ul>
</div>
-->
