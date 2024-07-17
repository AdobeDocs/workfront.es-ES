---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Descripción general del proyecto Fecha proyectada de inicio
description: La fecha proyectada de inicio es la fecha en tiempo real en la que el proyecto se va a iniciar, basada en la fecha proyectada de inicio de la primera tarea del proyecto.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Descripción general del proyecto Fecha proyectada de inicio

## Información general sobre la fecha proyectada de inicio de proyectos y tareas

La fecha proyectada de inicio es la fecha en tiempo real en la que el proyecto se va a iniciar, basada en la fecha proyectada de inicio de la primera tarea del proyecto. 

Cuando planifica un proyecto por primera vez, la fecha planificada de inicio y la fecha proyectada de inicio de las tareas y del proyecto son idénticas. Como pueden producirse retrasos o puede que las tareas se completen antes, la fecha de inicio proyectada puede diferir de la fecha de inicio planificada. 

Los cambios en la Fecha proyectada de inicio de la primera tarea del déclencheur del proyecto se modificarán en la Fecha proyectada de inicio del proyecto. 

## Modificar la fecha proyectada de inicio de una tarea

La fecha proyectada de inicio de un proyecto o una tarea es un cálculo realizado por Adobe Workfront y no se puede modificar manualmente. 

Los siguientes eventos pueden almacenar en déclencheur una modificación en la Fecha proyectada de inicio de una tarea:

* Cuando empiece a trabajar en una tarea, la fecha de inicio real de la tarea se convierte en la fecha de inicio proyectada.
* Si la fecha planificada de inicio de una tarea pasa, la fecha proyectada de inicio pasa al futuro, indicando la fecha más próxima disponible para que comience la tarea.\
  Workfront tiene en cuenta la cantidad de horas planificadas en la tarea, así como la programación del proyecto o del usuario asignado a la tarea, al calcular la fecha más temprana disponible para que se inicie la tarea. 
* Las tareas predecesoras que se ejecutan con retraso afectan a la fecha de inicio proyectada de sus tareas dependientes. La fecha proyectada de inicio de las tareas dependientes se mueve según el tipo de dependencia de la relación de predecesoras y según las fechas proyectadas de las predecesoras. 

Si alguna de estas tareas es la primera tarea de un proyecto, la fecha de inicio prevista del proyecto cambia para coincidir con la fecha de inicio prevista de esta tarea. 

## Busque la fecha proyectada de inicio de un proyecto o tarea

Puede localizar la fecha proyectada de inicio de un proyecto o una tarea en las siguientes áreas de Workfront:

* Puede agregarlo a un proyecto o a una vista o informe de tareas.

  Para obtener más información acerca de cómo crear un informe, vea el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* En la sección Detalles del proyecto de un proyecto o en la sección Detalles de la tarea de una tarea.
