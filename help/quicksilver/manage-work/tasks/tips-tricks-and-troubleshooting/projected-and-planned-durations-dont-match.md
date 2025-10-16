---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: La duración proyectada no coincide con la duración planificada
description: 'En este artículo se describe la solución de problemas en Adobe Workfront en los casos en los que podría recibir el siguiente mensaje: "La duración proyectada de una tarea o problema ha pasado a ser 0 y no coincide con la duración planificada".'
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 83%

---

# La duración prevista no coincide con la duración planificada

## Problema

Recibe el siguiente mensaje de error: “La duración prevista de una tarea/problema ha pasado a 0 y no coincide con la duración planificada.”

## Causa

Esto ocurre cuando la Fecha proyectada de inicio coincide con la de finalización.

## Solución

Existen muchos factores que pueden hacer que las fechas proyectadas de inicio y finalización coincidan. Este problema está en gran medida vinculado a la asignación de tiempo en la tarea o el problema en cuestión.

En la mayoría de los casos, dependiendo del tipo de duración y la restricción de tarea en la tarea, la asignación debería extender la fecha de finalización proyectada mucho más de lo esperado. Sin embargo, en algunos casos, según la forma en que se configuren el tipo de duración y la restricción de tarea, es posible que sea cero.

Estas son las mejores cosas que comprobar en esos casos con vínculos a sus artículos de apoyo:

* Fecha proyectada de finalización: [Información general sobre la fecha proyectada de finalización de proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)
* Restricción de Tarea: [Información general de la Restricción de Tarea](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)
* Tipo de duración: [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)

Si la fecha proyectada de finalización, la restricción de tarea o el tipo de duración están funcionando como se espera, contacta con soporte para obtener información más detallada.
