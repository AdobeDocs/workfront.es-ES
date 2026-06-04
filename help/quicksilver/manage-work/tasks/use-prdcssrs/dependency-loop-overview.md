---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Resumen del bucle de dependencia de tareas
description: Al añadir relaciones de predecesoras a las tareas, puede encontrar bucles de dependencia. Para obtener información sobre las tareas predecesoras, vea Información general sobre tareas predecesoras.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
TQID: https://experienceleague.adobe.com/cQbPOUES-tmSgZTpXrft8lQby-ubPmI-TZ1PjdGURMc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 68%

---

# Información general del bucle de dependencia de tareas

Al añadir relaciones de predecesoras a las tareas, puede encontrar bucles de dependencia. Para obtener información sobre las predecesoras, consulte [Información general sobre las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Información general de bucle de dependencia

Los bucles de dependencia se producen cuando tiene dos o más tareas que dependen unas de otras para completarse. Adobe Workfront no permite crear una relación de predecesora entre tareas si crea un bucle de dependencia.

**Ejemplo:** La tarea 2 es predecesora de la tarea 1, lo que significa que debe completar la tarea 2 para poder empezar a trabajar en la tarea 1.

Si intenta hacer que la Tarea 1 sea la predecesora de la Tarea 2, se producirá un error de bucle de dependencia porque no podrá iniciar la Tarea 1 hasta que se haya completado la Tarea 2, pero la Tarea 2 no podrá iniciarse hasta que finalice la Tarea 1.

![Mensaje de error de bucle de dependencia](assets/dependency-loop-error-message-350x209.png)

![Bucle de dependencia en la lista de tareas](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Consideraciones sobre los bucles de dependencia

* Los bucles de dependencia pueden implicar más de dos tareas. A veces, cualquier número de elementos primarios de las tareas que está conectando con una relación predecesora son los que crean el bucle de dependencia.
* También puede producirse un bucle de dependencia si intenta hacer que una tarea principal sea la predecesora de una secundaria.
* En el caso de un bucle de dependencia, no se pueden guardar las tareas ni el proyecto. Para corregir el bucle de dependencia, debe volver a evaluar la relación de predecesoras entre las tareas enumeradas en el mensaje de error y quitar los conflictos antes de guardar las tareas o el proyecto.


