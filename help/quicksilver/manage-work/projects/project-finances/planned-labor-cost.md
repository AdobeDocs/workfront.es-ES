---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular coste planificado de mano de obra
description: A medida que planifica el trabajo en sus proyectos, Adobe Workfront calcula el coste planificado de mano de obra de las funciones y de los usuarios asignados a este trabajo en función de sus valores de coste por hora.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
TQID: https://experienceleague.adobe.com/xzjI7jrIuUBcwF7MpZ8fcWGuFgDrY-V2OUlAq95lDAw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 100%

---

# Calcular coste planificado de mano de obra

A medida que planifica el trabajo en sus proyectos, Adobe Workfront calcula el coste planificado de mano de obra de las funciones y de los usuarios asignados a este trabajo en función de sus valores de coste por hora.

El coste planificado de mano de obra de un proyecto es un cálculo entre el coste asociado con las funciones o los usuarios asignados para completar el trabajo en el proyecto y la cantidad de horas planificadas (Horas planificadas) que puede requerir cada función o usuario para completar dicho trabajo.

## Visión general del coste planificado de mano de obra

El **Coste planificado de mano de obra** de un proyecto se calcula sumando todos los costes planificados de mano de obra de todas las tareas del proyecto.

>[!TIP]
>
>No hay ningún coste planificado de mano de obra asociado con los problemas o con el proyecto en sí.

Workfront calcula el coste planificado de mano de obra de un proyecto mediante la siguiente fórmula:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

El coste planificado de mano de obra para la tarea se calcula en función de lo siguiente:

* El número de recursos de la tarea y su asignación individual a la tarea
* El tipo de coste de la tarea.

El coste planificado de mano de obra para la tarea se calcula mediante la siguiente fórmula:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Para obtener más información acerca de cómo calcula Workfront el coste planificado de mano de obra para las tareas, según las asignaciones de tareas y el tipo de coste, consulte la sección “Modificar tipos de coste para tareas individuales” en el artículo [Seguimiento de costes](../../../manage-work/projects/project-finances/track-costs.md).

## Localizar el coste planificado de mano de obra

Puede localizar el coste planificado de mano de obra de un proyecto en las siguientes áreas de Workfront:

* Un informe del proyecto
* Una lista de proyectos
* Un informe de línea de base donde puede realizar un seguimiento a lo largo del tiempo
* Mediante la API

Para obtener información sobre la creación de informes y el uso de la API de Workfront, consulte los siguientes artículos:

* [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Conceptos básicos de API](../../../wf-api/general/api-basics.md)
