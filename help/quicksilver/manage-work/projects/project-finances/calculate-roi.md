---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular el retorno de la inversión (ROI)
description: El retorno de la inversión (ROI) es una métrica de Adobe Workfront que permite a los administradores de portafolios ver rápidamente el desempeño del proyecto en comparación con el beneficio planificado y el coste presupuestado originales del proyecto.
author: Lisa
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '348'
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
