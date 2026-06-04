---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: La duración proyectada no coincide con la duración planificada
description: 'En este artículo se describe la solución de problemas en Adobe Workfront en los casos en los que podría recibir el siguiente mensaje: "La duración proyectada de una tarea o problema ha pasado a ser 0 y no coincide con la duración planificada".'
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
TQID: https://experienceleague.adobe.com/cdGUhn51Xeqie8iW75phQTQKMvdO2ub-HSjcCjcHLec
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 234
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
