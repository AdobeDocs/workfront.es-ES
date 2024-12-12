---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el coste potencial de riesgos
description: El coste potencial de riesgos de un proyecto tiene en cuenta los posibles costes de los riesgos del proyecto y su probabilidad de ocurrencia.
author: Lisa
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 85%

---

# Calcular el coste potencial de riesgos

El coste potencial de riesgos de un proyecto tiene en cuenta los posibles costes de los riesgos del proyecto y su probabilidad de ocurrencia.

## Información general sobre el coste potencial de riesgos de un proyecto

Adobe Workfront calcula el coste de riesgo potencial de un proyecto mediante la fórmula siguiente:

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Tenga en cuenta lo siguiente al revisar el costo de riesgo potencial de un proyecto:

* El coste planificado de riesgos de un proyecto es idéntico al coste potencial de riesgos.
* El coste potencial de riesgos no está incorporado al coste planificado de un proyecto. En su lugar, se utiliza para determinar su valor neto.

## Localizar el costo de riesgo potencial de un proyecto

Puede encontrar los riesgos de un proyecto y su coste potencial en las siguientes áreas de Workfront:

* En la ficha Riesgos del proyecto.
* En el Resumen del caso empresarial.\
  Para obtener más información sobre el caso empresarial de un proyecto, consulte el artículo [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* En un informe de proyecto, cuando añada el campo Coste planificado de riesgos a las columnas del informe.\
  Para obtener más información acerca de cómo generar informes en Workfront, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* En el Optimizador de portafolios, cuando el proyecto está asociado a un portafolios, en la columna Riesgo.\
  La suma de todos los costes potenciales de riesgo de todos los proyectos del portafolios se suma al riesgo del portafolio.\
  Para obtener más información sobre el Optimizador de portafolios, consulte el artículo [Información general sobre el Optimizador de portafolios](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Para obtener más información sobre la creación de riesgos en un proyecto, consulte el artículo [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Para obtener más información sobre el caso empresarial de un proyecto, consulte el artículo [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
