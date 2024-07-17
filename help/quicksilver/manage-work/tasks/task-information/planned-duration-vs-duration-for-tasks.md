---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Diferencia entre la duración planificada y la duración de las tareas
description: Duración es la cantidad de tiempo entre la fecha planificada de inicio y la planificada de finalización de un elemento de trabajo. Las tareas tienen una Duración y una Duración planificada en Adobe Workfront, según el Tipo de duración de la tarea.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Diferencia entre la duración planificada y la duración de las tareas

Duración es la cantidad de tiempo entre la fecha planificada de inicio y la planificada de finalización de un elemento de trabajo. Las tareas tienen una Duración y una Duración planificada en Adobe Workfront, según el Tipo de duración de la tarea.

Los problemas y proyectos no se pueden asociar a un tipo de duración y solo tienen una duración.

## Duración de tarea

Para las tareas, la Duración y la Duración planificada generalmente muestran el mismo valor: la duración entre la Fecha planificada de inicio y la Fecha planificada de finalización de una tarea.

Cuando el tipo de duración de la tarea es Condicionada por el esfuerzo, la Duración planificada disminuye a medida que añade recursos a la tarea.

**Ejemplo:** Si una tarea con un tipo de duración Condicionada por el esfuerzo tiene una duración de 3 días y asigna a la tarea un recurso con una programación a tiempo completo, la duración planificada también será de 3 días.

Si asigna tres recursos con una programación a tiempo completo a la misma tarea, la duración permanece 3 días, pero la duración planificada pasa a ser 1 día. La Duración planificada también cambia las fechas planificadas de inicio y finalización planificada de la tarea para reflejar la nueva Duración planificada. Como resultado, la cronología del proyecto también se ve afectada.
Puede utilizar el Tipo de duración condicionada por el esfuerzo al asignar una tarea a varios recursos. Esto reduce el tiempo que tarda el trabajo en completarse en la tarea.

Para obtener más información sobre el tipo de duración impulsada por el esfuerzo, vea [Información general sobre el tipo de duración: impulsada por el esfuerzo](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Duración del problema y del proyecto

Los problemas y proyectos tienen un solo valor de Duración, que es la diferencia entre la fecha planificada de inicio y la fecha planificada de finalización del problema y del proyecto, respectivamente.
