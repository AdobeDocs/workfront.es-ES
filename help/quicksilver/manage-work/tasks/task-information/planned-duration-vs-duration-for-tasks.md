---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Diferencia entre la duración planificada y la duración de las tareas
description: Duración es la cantidad de tiempo entre la fecha planificada de inicio y la fecha planificada de finalización de un elemento de trabajo. Las tareas tienen una duración y una duración planificada en Adobe Workfront, según el tipo de duración de la tarea.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
TQID: https://experienceleague.adobe.com/tVh55DKoBvOUZdq9lZ6y72rxZQ1WOoAYL-Pz8nlU588
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 272
ht-degree: 87%

---

# Diferencia entre la duración planificada y la de las tareas

Duración es la cantidad de tiempo entre la fecha planificada de inicio y la fecha planificada de finalización de un elemento de trabajo. Las tareas tienen una duración y una duración planificada en Adobe Workfront, según el tipo de duración de la tarea.

Los problemas y proyectos no se pueden asociar a un tipo de duración y solo tienen una duración.

## Duración de la tarea

En el caso de las tareas, la duración y la duración planificada generalmente muestran el mismo valor: la cantidad de tiempo entre la fecha de inicio planificada y la fecha planificada de finalización de una tarea.

Cuando el tipo de duración de la tarea es Condicionada por el esfuerzo, la duración planificada disminuye a medida que se añaden recursos a la tarea.

**Ejemplo:** Si una tarea con un tipo de duración Condicionada por el esfuerzo tiene una duración de 3 días y se asigna a la tarea un recurso con una programación a tiempo completo, la duración planificada también será de 3 días.

Si asigna tres recursos con una programación a tiempo completo a la misma tarea, la duración permanece 3 días, pero la duración planificada pasa a ser 1 día. La Duración planificada también cambia las fechas planificadas de inicio y finalización planificada de la tarea para reflejar la nueva Duración planificada. Como resultado, la cronología del proyecto también se ve afectada.
Puede utilizar el Tipo de duración condicionada por el esfuerzo al asignar una tarea a varios recursos. Esto reduce el tiempo que tarda el trabajo en completarse en la tarea.

Para obtener más información sobre el tipo de duración condicionada por el esfuerzo, consulte [Información general sobre el tipo de duración: condicionada por el esfuerzo](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Duración del problema y del proyecto

Los problemas y proyectos solo tienen un valor de duración, que es la diferencia entre la fecha de inicio planificada y la fecha planificada de finalización del problema y del proyecto, respectivamente.
