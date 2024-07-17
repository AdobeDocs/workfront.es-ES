---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular costo de riesgo potencial
description: El costo de riesgo potencial de un proyecto tiene en cuenta los costos potenciales de los riesgos del proyecto y su probabilidad de que ocurran.
author: Alina
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Calcular costo de riesgo potencial

El costo de riesgo potencial de un proyecto tiene en cuenta los costos potenciales de los riesgos del proyecto y su probabilidad de que ocurran.

## Descripción general del costo de riesgo potencial de un proyecto

Adobe Workfront calcula el coste de riesgo potencial de un proyecto mediante la fórmula siguiente:

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Tenga en cuenta lo siguiente al revisar el costo de riesgo potencial de un proyecto:

* El costo de riesgo planificado de un proyecto es idéntico al costo de riesgo potencial. 
* El costo de riesgo potencial no está incorporado al costo planificado de un proyecto. En su lugar, se utiliza para determinar su valor neto. .

## Localizar el costo de riesgo potencial de un proyecto

Puede encontrar los riesgos de un proyecto y su coste potencial en las siguientes áreas de Workfront:

* En la pestaña Riesgos del proyecto.
* En el Resumen del caso empresarial.\
  Para obtener más información sobre el caso comercial de un proyecto, vea el artículo [Crear un caso comercial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* En un informe de proyecto cuando agregue el campo Costo de riesgo planificado a las columnas del informe.\
  Para obtener más información acerca de cómo generar informes en Workfront, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* En el Optimizador de Portfolio, cuando el proyecto está asociado a un Portfolio, en la columna Riesgo.\
  La suma de todos los costes de riesgo potenciales de todos los proyectos del portafolio se suma al riesgo del Portfolio.\
  Para obtener más información sobre Portfolio Optimizer, consulte el artículo [Descripción general de Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Para obtener más información sobre la creación de riesgos en un proyecto, vea el artículo [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Para obtener más información sobre el caso comercial de un proyecto, vea el artículo [Crear un caso comercial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
