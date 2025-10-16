---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Diferencia entre la duración planificada y la duración de las tareas
description: Duración es la cantidad de tiempo entre la fecha planificada de inicio y la fecha planificada de finalización de un elemento de trabajo. Las tareas tienen una duración y una duración planificada en Adobe Workfront, según el tipo de duración de la tarea.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 97%

---

# Diferencia entre la duración planificada y la de las tareas

Duración es la cantidad de tiempo entre la fecha planificada de inicio y la fecha planificada de finalización de un elemento de trabajo. Las tareas tienen una duración y una duración planificada en Adobe Workfront, según el tipo de duración de la tarea.

Los problemas y proyectos no se pueden asociar a un tipo de duración y solo tienen una duración.

## Duración de la tarea

En el caso de las tareas, la duración y la duración planificada generalmente muestran el mismo valor: la cantidad de tiempo entre la fecha de inicio planificada y la fecha planificada de finalización de una tarea.

Cuando el tipo de duración de la tarea es Condicionada por el esfuerzo, la duración planificada disminuye a medida que se añaden recursos a la tarea.

**Ejemplo:** Si una tarea con un tipo de duración Condicionada por el esfuerzo tiene una duración de 3 días y se asigna a la tarea un recurso con una programación a tiempo completo, la duración planificada también será de 3 días.

Si asigna tres recursos con una programación a tiempo completo a la misma tarea, la duración permanece 3 días, pero la duración planificada pasa a ser de 1 día. La duración planificada también cambia las fechas de inicio planificado y finalización planificada de la tarea, para reflejar la nueva duración planificada. Como resultado, la línea de tiempo del proyecto también se verá afectada.
Puede utilizar el tipo de duración Condicionada por el esfuerzo cuando asigne una tarea a varios recursos. Esto reduce el tiempo que el trabajo tarda en completarse en la tarea.

Para obtener más información sobre el tipo de duración condicionada por el esfuerzo, consulte [Información general sobre el tipo de duración: condicionada por el esfuerzo](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Duración del problema y del proyecto

Los problemas y proyectos solo tienen un valor de duración, que es la diferencia entre la fecha de inicio planificada y la fecha planificada de finalización del problema y del proyecto, respectivamente.
