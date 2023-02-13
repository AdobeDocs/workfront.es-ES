---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre la fecha del Slack de tareas
description: A veces, las tareas pueden iniciarse y completarse tarde sin afectar a la fecha de finalización del proyecto.
author: Alina
feature: Work Management
exl-id: ccdaa27d-e212-45dc-afca-08539f2b4001
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Información general sobre la fecha del Slack de tareas

A veces, las tareas pueden iniciarse y completarse tarde sin afectar a la fecha de finalización del proyecto.

La fecha de Slack muestra la fecha exacta en la que una tarea podría afectar definitivamente a la fecha de finalización del proyecto.

## Información general sobre la fecha del Slack

La fecha de Slack es diferente a la fecha de finalización prevista, ya que las relaciones predecesoras y las restricciones de tareas aumentan el tiempo de espera.

Considere los siguientes escenarios, dependiendo de si una tarea está o no en la ruta crítica de un proyecto:

* Para las tareas que se encuentran en la ruta crítica del proyecto o que tienen sucesores en la ruta crítica, la fecha de Slack coincide con la fecha de finalización prevista de la tarea, a menos que el estado de progreso de la tarea ya esté atrasado o atrasado.

   Para obtener información sobre la ruta crítica, consulte [Descripción general de la ruta crítica del proyecto](../../../manage-work/tasks/manage-tasks/critical-path.md).

   Para obtener información sobre el estado de progreso de las tareas, consulte [Información general sobre el estado de progreso de la tarea](../../../manage-work/tasks/task-information/task-progress-status.md).

* Para las tareas que no están en la ruta crítica, la demora aumenta cuanto antes se programe la tarea. Para estas tareas, la Fecha de Slack permanece en el futuro hasta que las tareas se retrasen tanto que empiecen a afectar a la Fecha de Finalización del proyecto.

## Localizar la fecha Slack de una tarea

Para ver la fecha de Slack de una tarea, puede añadir el campo Fecha de Slack a una vista de tarea o a un informe.

Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
