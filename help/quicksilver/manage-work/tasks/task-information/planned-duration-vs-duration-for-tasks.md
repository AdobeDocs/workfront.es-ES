---
content-type: reference
product-area: projects
navigation-topic: task-information
title: Diferencia entre la duración prevista y la duración de las tareas
description: Duración es la cantidad de tiempo entre la Fecha de Inicio Planificado y la Fecha de Finalización Planificada de un elemento de trabajo. Las tareas tienen una duración y una duración planificadas en Adobe Workfront, según el tipo de duración de la tarea.
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Diferencia entre la duración prevista y la duración de las tareas

Duración es la cantidad de tiempo entre la Fecha de Inicio Planificado y la Fecha de Finalización Planificada de un elemento de trabajo. Las tareas tienen una duración y una duración planificadas en Adobe Workfront, según el tipo de duración de la tarea.

Los problemas y proyectos no se pueden asociar con un tipo de duración y solo tienen una duración.

## Duración de la tarea

Para las tareas, la Duración y la Duración planeada generalmente muestran el mismo valor: el periodo entre la fecha de inicio planeada y la fecha de finalización planeada de una tarea.

Cuando el tipo de duración de la tarea está impulsado por el esfuerzo, la duración prevista disminuye a medida que agrega recursos a la tarea.

**Ejemplo:** Si una tarea con un tipo de duración de esfuerzo impulsado tiene una duración de 3 días y se asigna un recurso con una programación de tiempo completo a la tarea, la duración planeada también es de 3 días.

Si asigna tres recursos con una programación de tiempo completo a la misma tarea, la duración se mantiene en 3 días, pero la duración prevista se convierte en 1 día. La duración planeada también cambia las fechas de inicio y finalización planificadas de la tarea para reflejar la nueva duración planificada. Como resultado, la cronología del proyecto también se ve afectada.
Puede utilizar el Tipo de duración impulsada por esfuerzo cuando asigna una tarea a varios recursos. Esto reduce el tiempo que tarda el trabajo en completarse en la tarea.

Para obtener más información sobre el tipo de duración impulsada por esfuerzo, consulte [Información general del tipo de duración: Impulsado por el esfuerzo](../../../manage-work/tasks/taskdurtn/effort-driven.md).

## Emisión y duración del proyecto

Los problemas y proyectos tienen un solo valor de duración, que es la diferencia entre la fecha de inicio planeada y la fecha de finalización planeada de la emisión y del proyecto, respectivamente.
