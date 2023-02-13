---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el rendimiento de la inversión (ROI)
description: Retorno de la inversión (ROI) es una métrica de Adobe Workfront que permite a los administradores de portafolios ver rápidamente el rendimiento del proyecto en comparación con el coste presupuestado y el beneficio planeado original del proyecto.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Calcular el rendimiento de la inversión (ROI)

Retorno de la inversión (ROI) es una métrica de Adobe Workfront que permite a los administradores de portafolios ver rápidamente el rendimiento del proyecto en comparación con el coste presupuestado y el beneficio planeado original del proyecto.

## Resumen del rendimiento de la inversión (ROI) del proyecto

Workfront calcula el ROI mediante la fórmula siguiente:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

Los campos siguientes afectan al ROI de un proyecto:

* **Beneficios planificados para el proyecto**: Es una entrada manual especificada por el propietario del proyecto al completar el área Información del proyecto del caso empresarial. Esta es una estimación de lo que usted, como propietario del proyecto, cree que el beneficio del proyecto podría ser si completa el proyecto. Es una cantidad específica de moneda y debe ser un valor positivo.\
   Para obtener más información sobre los beneficios previstos de un proyecto, consulte la sección &quot;Información del proyecto&quot; en el artículo [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Coste presupuestado del proyecto**: Es el coste total asociado con el proyecto, tal como se calcula al iniciar el proyecto por primera vez.

   La variable **Coste presupuestado** utiliza la variable **Coste de trabajo presupuestado** que se calcula en el área de Presupuestación de Recursos del Caso de Negocio y tiene en cuenta las horas presupuestadas para las funciones de trabajo en el Planificador de Recursos y la tasa de Costo por Hora de cada rol de trabajo.\
   Para obtener más información, consulte [Calcular costo presupuestado](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Localizar el retorno de la inversión (ROI) del proyecto

Puede ver el valor de ROI de un proyecto en las siguientes áreas de Workfront:

* En Portfolio Optimizer si el proyecto está asociado con un portafolio

   >[!NOTE]
   >
   >El total de todos los valores de ROI del proyecto es el ROI de la cartera.

   Para obtener información sobre el Optimizador de Portfolio, consulte el artículo [Información general sobre Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* En el campo ROI del proyecto en las siguientes listas e informes: 

   * Proyecto
   * Tarea
   * Problema
   * Proyecto (datos financieros)
   Para obtener más información sobre la creación de informes en Workfront, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
