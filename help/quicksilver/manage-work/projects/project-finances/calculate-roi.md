---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el retorno de la inversión (ROI)
description: El retorno de la inversión (ROI) es una métrica de Adobe Workfront que permite a los administradores de portafolios ver rápidamente el desempeño del proyecto en comparación con el beneficio planificado y el coste presupuestado originales del proyecto.
author: Lisa
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
TQID: https://experienceleague.adobe.com/x7MGrAZbtlDd0oTePPgRdLQfUg8-M4GkkQdeWXUTyh4
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
source-wordcount: 348
ht-degree: 74%

---

# Calcular el retorno de la inversión (ROI)

El retorno de la inversión (ROI) es una métrica de Adobe Workfront que permite a los administradores de portafolios ver rápidamente el desempeño del proyecto en comparación con el beneficio planificado y el coste presupuestado originales del proyecto.

## Descripción general del retorno de la inversión (ROI) del proyecto

Workfront calcula el retorno de la inversión utilizando la siguiente fórmula:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

Los siguientes campos afectan al ROI de un proyecto:

* **Beneficio planificado del proyecto**: se trata de una entrada manual especificada por el propietario del proyecto al completar el área de información del proyecto del caso empresarial. Esta es una estimación de lo que usted, como propietario del proyecto, piensa que podría ser el beneficio del proyecto si completa el proyecto. Se trata de una cantidad de dinero específica y debe ser un valor positivo.\
  Para obtener más información sobre el beneficio planificado de un proyecto, consulte la sección “Información del proyecto” en el artículo [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Costo presupuestado del proyecto**: Este es el costo total asociado con el proyecto que se estimó al iniciar el proyecto por primera vez.

  El **Costo presupuestado** usa el valor **Costo de mano de obra presupuestado** que se calcula en el área de Presupuestación de recursos del caso empresarial y tiene en cuenta las horas presupuestadas para sus roles en el Planificador de recursos y la tasa de Costo por hora de cada rol.\
  Para obtener más información, consulte [Calcular coste presupuestado](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Localice el Retorno de la inversión (ROI) del proyecto

Puede ver el valor de ROI de un proyecto en las siguientes áreas de Workfront:

* En Portfolio Optimizer si el proyecto está asociado a un portafolio

  >[!NOTE]
  >
  >El total de todos los valores de ROI del proyecto es el ROI del portafolio.

  Para obtener información acerca del Optimizador de portafolios, consulte el artículo [Información general del Optimizador de portafolios](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* En el campo ROI del proyecto, en las siguientes listas e informes:

   * Proyecto
   * Tarea
   * Problema
   * Proyecto (Datos financieros)

  Para obtener más información acerca de cómo generar informes en Workfront, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
