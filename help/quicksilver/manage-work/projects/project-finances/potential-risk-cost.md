---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular Coste de Riesgo Potencial
description: El costo potencial de riesgo de un proyecto tiene en cuenta los costos potenciales de los riesgos del proyecto y su probabilidad de que se produzcan.
author: Alina
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Calcular Coste de Riesgo Potencial

El costo potencial de riesgo de un proyecto tiene en cuenta los costos potenciales de los riesgos del proyecto y su probabilidad de que se produzcan.

## Visión General del Costo de Riesgo Potencial de un Proyecto

Adobe Workfront calcula el coste de riesgo potencial de un proyecto mediante la fórmula siguiente:

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Tenga en cuenta lo siguiente al revisar el Coste de Riesgo Potencial de un proyecto:

* El coste de riesgo planeado de un proyecto es idéntico al coste de riesgo potencial. 
* El Coste de Riesgo Potencial no se incorpora en el Coste Planificado de un proyecto. En su lugar, se utiliza para determinar su valor neto. .

## Localizar el costo de riesgo potencial de un proyecto

Puede encontrar los riesgos de un proyecto y su coste potencial en las siguientes áreas de Workfront:

* En la pestaña Riesgos del proyecto.
* En el resumen del caso empresarial.\
   Para obtener más información sobre el caso empresarial de un proyecto, consulte el artículo [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* En un informe de proyecto, cuando se agrega el campo Costo de riesgo planeado a las columnas del informe.\
   Para obtener más información sobre la creación de informes en Workfront, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* En el Optimizador de Portfolio, cuando el proyecto está asociado con un Portfolio, en la columna Riesgo .\
   La suma de todos los costes de riesgo potenciales de todos los proyectos de la cartera suman el riesgo del Portfolio.\
   Para obtener más información sobre el Portfolio Optimizer, consulte el artículo [Información general sobre Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Para obtener más información sobre la creación de riesgos en un proyecto, consulte el artículo [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Para obtener más información sobre el caso empresarial de un proyecto, consulte el artículo [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
