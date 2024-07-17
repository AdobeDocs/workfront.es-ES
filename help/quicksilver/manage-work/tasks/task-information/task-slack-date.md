---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Resumen de fecha de Slack de tarea
description: Las tareas a veces pueden comenzar y completarse tarde sin afectar a la fecha de finalización del proyecto.
author: Alina
feature: Work Management
exl-id: ccdaa27d-e212-45dc-afca-08539f2b4001
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Resumen de fecha de Slack de tarea

Las tareas a veces pueden comenzar y completarse tarde sin afectar a la fecha de finalización del proyecto.

La fecha de Slack muestra la fecha exacta en la que una tarea podría afectar definitivamente a la fecha de finalización del proyecto.

## Resumen de fecha del Slack

La fecha de Slack es diferente a la fecha de finalización prevista, ya que las relaciones de predecesoras y las restricciones de tareas aumentan el tiempo de demora.

Considere los siguientes escenarios, dependiendo de si una tarea se encuentra en la ruta crítica de un proyecto o no:

* En el caso de las tareas que se encuentran en la ruta crítica del proyecto o que tienen sucesoras que se encuentran en la ruta crítica, la fecha de Slack coincide con la fecha proyectada de finalización de la tarea a menos que el estado de progreso de la tarea ya sea Retrasado o Retrasado.

  Para obtener información sobre la ruta crítica, consulte [Información general sobre la ruta crítica del proyecto](../../../manage-work/tasks/manage-tasks/critical-path.md).

  Para obtener información sobre el estado de progreso de las tareas, consulte [Resumen del estado de progreso de la tarea](../../../manage-work/tasks/task-information/task-progress-status.md).

* En el caso de las tareas que no se encuentran en la ruta crítica, el tiempo de demora aumenta cuanto antes se programe la tarea. Para estas tareas, la fecha de Slack permanece en el futuro hasta que las tareas se retrasan tanto que comienzan a afectar a la fecha de finalización del proyecto.

## Localizar la fecha de Slack de una tarea

Para ver la fecha de Slack de una tarea, puede agregar el campo Fecha de Slack a una vista de tareas o a un informe.

Para obtener información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
