---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Resumen de bucle de dependencia de tareas
description: Al agregar relaciones de predecesoras a las tareas, puede encontrar bucles de dependencia. Para obtener información sobre las tareas predecesoras, vea Información general sobre tareas predecesoras.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Resumen de bucle de dependencia de tareas

Al agregar relaciones de predecesoras a las tareas, puede encontrar bucles de dependencia. Para obtener información acerca de las tareas predecesoras, vea [Información general sobre las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Resumen del bucle de dependencias

Los bucles de dependencia se producen cuando tiene dos o más tareas que dependen unas de otras para completarse. Adobe Workfront no permite crear una relación de predecesora entre tareas si crea un bucle de dependencia.

**Ejemplo:** La tarea 2 es predecesora de la tarea 1, lo que significa que debe completar la tarea 2 para poder empezar a trabajar en la tarea 1.

Si intenta hacer que la Tarea 1 sea la predecesora de la Tarea 2, obtendrá un error de bucle de dependencia porque no podrá iniciar la Tarea 1 hasta que se haya completado la Tarea 2, pero la Tarea 2 no podrá iniciarse hasta que finalice la Tarea 1.

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Consideraciones sobre los bucles de dependencia

* Los bucles de dependencia pueden implicar más de dos tareas. A veces, cualquier número de elementos primarios de las tareas que está conectando con una relación predecesora son los que crean el bucle de dependencia.
* También puede producirse un bucle de dependencia si intenta hacer que un padre sea el predecesor de un hijo.
* En el caso de un bucle de dependencia, no se pueden guardar las tareas ni el proyecto. Para corregir el bucle de dependencia, debe volver a evaluar la relación de predecesoras entre las tareas enumeradas en el mensaje de error y quitar los conflictos antes de guardar las tareas o el proyecto.

 
