---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Descripción general de la fecha de inicio prevista del proyecto
description: La Fecha de inicio prevista es una fecha en tiempo real del momento en que se va a iniciar el proyecto, basada en la Fecha de inicio prevista de la primera tarea del proyecto.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Descripción general de la fecha de inicio prevista del proyecto

## Descripción general de la fecha de inicio prevista para proyectos y tareas

La Fecha de inicio prevista es una fecha en tiempo real del momento en que se va a iniciar el proyecto, basada en la Fecha de inicio prevista de la primera tarea del proyecto. 

Cuando planifica por primera vez un proyecto, la fecha de inicio planeada y la fecha de inicio proyectada de las tareas y del proyecto son idénticas. Como pueden producirse retrasos o las tareas se pueden completar antes, la Fecha de inicio prevista puede diferir de la Fecha de inicio planeada. 

Los cambios en la Fecha de inicio prevista de la primera tarea del déclencheur del proyecto cambian en la Fecha de inicio prevista del proyecto. 

## Modificación de la fecha de inicio prevista de una tarea

La fecha de inicio prevista para un proyecto o una tarea es un cálculo realizado por Adobe Workfront y no se puede modificar manualmente. 

Los siguientes eventos pueden almacenar en déclencheur una modificación en la Fecha de inicio prevista de una tarea:

* Cuando comienza a trabajar en una tarea, la Fecha de inicio real de la tarea pasa a ser su Fecha de inicio prevista.
* Si la fecha de inicio prevista de una tarea pasa, la fecha de inicio prevista se mueve al futuro, indicando la fecha más próxima disponible para que la tarea comience.\
   Workfront tiene en cuenta la cantidad de horas planificadas en la tarea, así como la programación del proyecto o del usuario asignado a la tarea al calcular la fecha más temprana disponible para que se inicie la tarea. 
* Las tareas del predecesor que se ejecutan detrás tienen un impacto en la Fecha de inicio prevista de sus tareas dependientes. La Fecha de inicio prevista de las tareas dependientes se mueve según el tipo de dependencia de la relación predecesora y según las fechas proyectadas de los predecesores. 

Si alguna de estas tareas es la primera tarea de un proyecto, la Fecha de inicio prevista del proyecto cambia para coincidir con la Fecha de inicio prevista de esta tarea. 

## Localizar la fecha de inicio prevista de un proyecto o tarea

Puede localizar la Fecha de inicio prevista de un proyecto o una tarea en las siguientes áreas de Workfront:

* Puede agregarla a un proyecto o a un informe o una vista de tareas.

   Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* En la sección Detalles del proyecto de un proyecto o en la sección Detalles de la tarea de una tarea.
