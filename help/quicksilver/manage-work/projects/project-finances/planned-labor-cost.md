---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el costo laboral planificado
description: A medida que planifica el trabajo en sus proyectos, Adobe Workfront calcula el costo laboral planeado para las funciones y los usuarios asignados a este trabajo en función de sus valores de costo por hora.
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Calcular el costo laboral planificado

A medida que planifica el trabajo en sus proyectos, Adobe Workfront calcula el costo laboral planeado para las funciones y los usuarios asignados a este trabajo en función de sus valores de costo por hora.

El costo laboral planeado de un proyecto es un cálculo entre el costo asociado con las funciones de trabajo o los usuarios asignados para completar el trabajo en el proyecto y la cantidad de horas planificadas (horas planificadas) que puede tomar cada rol o usuario para completar ese trabajo.

## Visión General del Coste Laboral Planificado

La variable **Coste laboral planificado** de un proyecto se calcula añadiendo todos los costes laborales previstos de todas las tareas del proyecto.

>[!TIP]
>
>No hay ningún costo laboral planificado asociado con problemas o con el propio proyecto.

Workfront calcula el coste laboral planificado de un proyecto mediante la fórmula siguiente:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

El costo laboral planificado para la tarea se calcula en función de lo siguiente:

* El número de recursos de la tarea y su asignación individual a la tarea
* El tipo de coste de la tarea.

El Coste Laboral Planificado de Tareas se calcula mediante la fórmula siguiente:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Para obtener más información sobre cómo calcula Workfront el coste laboral planeado para las tareas, en función de las asignaciones de tareas y el tipo de coste, consulte la sección &quot;Modificación de tipos de coste para tareas individuales&quot; en el artículo [Seguimiento de costes](../../../manage-work/projects/project-finances/track-costs.md).

## Localizar el costo laboral planificado

Puede localizar el costo laboral planificado de un proyecto en las siguientes áreas de Workfront:

* Un informe de proyecto
* Una lista de proyectos
* Informe de línea de base donde se puede realizar un seguimiento a lo largo del tiempo
* A través de la API

Para obtener información sobre la creación de informes y el uso de la API de Workfront, consulte los siguientes artículos:

* [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Conceptos básicos de API](../../../wf-api/general/api-basics.md)
