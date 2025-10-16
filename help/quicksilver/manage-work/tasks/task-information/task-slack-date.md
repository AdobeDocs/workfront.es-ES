---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Resumen de fecha de Task Slack
description: Las tareas a veces pueden comenzar y completarse tarde sin afectar a la fecha de finalización del proyecto. La Fecha de margen de demora muestra la fecha exacta en la que una tarea podría afectar definitivamente a la fecha de finalización del proyecto.
author: Alina
feature: Work Management
exl-id: ccdaa27d-e212-45dc-afca-08539f2b4001
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 93%

---

# Información general sobre la fecha de margen de demora de la tarea

Las tareas a veces pueden comenzar y completarse tarde sin afectar a la fecha de finalización del proyecto.

La Fecha de margen de demora muestra la fecha exacta en la que una tarea podría afectar definitivamente a la fecha de finalización del proyecto.

## Información general sobre la fecha de margen de demora

La fecha de margen de demora es diferente a la fecha de finalización prevista, ya que las relaciones de predecesoras y las restricciones de tareas aumentan el tiempo de demora.

Considere los siguientes escenarios, dependiendo de si una tarea se encuentra en la ruta crítica de un proyecto o no:

* En el caso de las tareas que se encuentran en la ruta crítica del proyecto o que tienen sucesoras que se encuentran en la ruta crítica, la fecha de margen de demora coincide con la fecha de finalización prevista de la tarea a menos que el estado de progreso de la tarea ya sea Atrasado o Retrasado.

  Para obtener información sobre la ruta crítica, consulte [Información general sobre la ruta crítica del proyecto](../../../manage-work/tasks/manage-tasks/critical-path.md).

  Para obtener información sobre el estado de progreso de las tareas, consulte [Información general sobre el estado de progreso de la tarea](../../../manage-work/tasks/task-information/task-progress-status.md).

* En el caso de las tareas que no se encuentran en la ruta crítica, el tiempo de demora aumenta cuanto antes se programe la tarea. Para estas tareas, la fecha de margen de demora permanece en el futuro hasta que las tareas se retrasan tanto que comienzan a afectar a la fecha de finalización del proyecto.

## Localizar la fecha de margen de demora de una tarea

Para ver la fecha de margen de demora de una tarea, puede añadir el campo Fecha de margen de demora a una vista de tarea o a un informe.

Para obtener información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
