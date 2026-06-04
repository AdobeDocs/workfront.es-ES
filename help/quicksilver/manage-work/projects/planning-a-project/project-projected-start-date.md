---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre la fecha de inicio proyectada del proyecto
description: La fecha de inicio proyectada es la fecha en tiempo real en la que el proyecto va a comenzar, basada en la fecha de inicio proyectada de la primera tarea del proyecto.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
TQID: https://experienceleague.adobe.com/2rcx201EGt4cqRpqfXws6P-NbRnXyVlFoTbJrQJBipg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 430
ht-degree: 96%

---

# Información general sobre la fecha de inicio proyectada del proyecto

## Información general sobre la fecha de inicio proyectada de proyectos y tareas

La fecha de inicio proyectada es la fecha en tiempo real en la que el proyecto va a comenzar, basada en la fecha de inicio proyectada de la primera tarea del proyecto.

Cuando planifica un proyecto por primera vez, la fecha de inicio planificada y la fecha de inicio proyectada de las tareas y del proyecto son idénticas. Como pueden producirse retrasos o puede que las tareas se completen antes, la fecha de inicio proyectada puede diferir de la fecha de inicio planificada.

Los cambios en la fecha de inicio proyectada de la primera tarea del proyecto activa cambios en la fecha de inicio proyectada del proyecto.

## Modificación de la fecha de inicio proyectada de una tarea

La fecha de inicio proyectada de un proyecto o una tarea es un cálculo realizado por Adobe Workfront y no se puede modificar manualmente.

Los siguientes eventos pueden activar una modificación en la fecha de inicio proyectada de una tarea:

* Cuando empiece a trabajar en una tarea, la fecha de inicio real de la tarea se convierte en la fecha de inicio proyectada.
* Si la fecha de inicio planificada de una tarea pasa, la fecha de inicio proyectada se traslada a una fecha futura para indicar la fecha más próxima disponible para que comience la tarea.\
  Workfront tiene en cuenta la cantidad de horas planificadas en la tarea, así como la programación del proyecto o del usuario asignado a la tarea, al calcular la fecha más temprana disponible para que se inicie la tarea.
* Las tareas predecesoras que llevan retraso en su ejecución afectan a la fecha de inicio proyectada de sus tareas dependientes. La fecha de inicio proyectada de las tareas dependientes se mueve según el tipo de dependencia de la relación predecesora y según las fechas proyectadas de las predecesoras.

Si alguna de estas tareas es la primera tarea de un proyecto, la fecha de inicio proyectada del proyecto cambia para coincidir con la fecha de inicio proyectada de esta tarea.

## Búsqueda de la fecha de inicio proyectada de un proyecto o tarea

Puede encontrar la fecha de inicio proyectada de un proyecto o una tarea en las siguientes áreas de Workfront:

* Puede añadirla a un proyecto o a una vista o informe de tareas.

  Para obtener más información sobre la creación de un informe, consulte el artículo [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* En la sección Detalles del proyecto de un proyecto o en la sección Detalles de la tarea de una tarea.
