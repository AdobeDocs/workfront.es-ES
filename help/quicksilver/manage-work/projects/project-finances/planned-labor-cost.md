---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular costo laboral planificado
description: A medida que planifica el trabajo en sus proyectos, Adobe Workfront calcula el costo de mano de obra planificado de los roles y usuarios asignados a este trabajo en función de sus valores de costo por hora.
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Calcular costo laboral planificado

A medida que planifica el trabajo en sus proyectos, Adobe Workfront calcula el costo de mano de obra planificado de los roles y usuarios asignados a este trabajo en función de sus valores de costo por hora.

El costo de mano de obra planificado de un proyecto es un cálculo entre el costo asociado con los roles o los usuarios asignados para completar el trabajo en el proyecto y la cantidad de horas planificadas (Horas planificadas) que puede requerir cada rol o usuario para completar ese trabajo.

## Visión General del Coste Laboral Planificado

El **Costo de mano de obra planificado** de un proyecto se calcula sumando todos los costos de mano de obra planificados de todas las tareas del proyecto.

>[!TIP]
>
>No hay ningún costo de mano de obra planificado asociado con los problemas o con el proyecto en sí.

Workfront calcula el coste laboral planificado de un proyecto mediante la siguiente fórmula:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

El costo de mano de obra planificado para la tarea se calcula en función de lo siguiente:

* El número de recursos de la tarea y su asignación individual a la tarea
* El tipo de costo de la tarea.

El costo de mano de obra planificado para la tarea se calcula mediante la siguiente fórmula:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Para obtener más información acerca de cómo calcula Workfront el costo de mano de obra planificado para las tareas, según las asignaciones de tareas y el tipo de costo, vea la sección &quot;Modificar tipos de costo para tareas individuales&quot; en el artículo [Control de costos](../../../manage-work/projects/project-finances/track-costs.md).

## Localice el costo laboral planificado

Puede localizar el coste laboral planificado de un proyecto en las siguientes áreas de Workfront:

* Informe de proyecto
* Una lista de proyectos
* Un informe de línea de base donde puede realizar un seguimiento a lo largo del tiempo
* Mediante la API de

Para obtener información sobre la creación de informes y el uso de la API de Workfront, consulte los siguientes artículos:

* [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Conceptos básicos de API](../../../wf-api/general/api-basics.md)
