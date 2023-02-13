---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular valor neto
description: El valor neto de un proyecto es el valor total esperado del proyecto después de calcular sus beneficios y eliminar los costos.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Calcular valor neto

El valor neto de un proyecto es el valor total esperado del proyecto después de calcular sus beneficios y eliminar los costos. 

## Resumen del valor neto del proyecto

Adobe Workfront calcula el valor neto de un proyecto mediante la fórmula siguiente: 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

Los campos siguientes pueden afectar al valor neto de un proyecto:

* **Beneficio planificado**: Esta es una entrada manual especificada por el propietario del proyecto al completar la **Información del proyecto** de Business Case.\
   Para obtener más información sobre los beneficios planificados de un proyecto, consulte la [Información del proyecto](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) sección del artículo [Información general sobre las áreas del caso empresarial](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Coste presupuestado**: Es el coste total asociado con el proyecto, tal como se calcula al iniciar el proyecto por primera vez.

   La variable **Coste presupuestado** utiliza la variable **Coste de trabajo presupuestado** que se calcula en el área de Presupuestación de Recursos del Caso de Negocio y tiene en cuenta las horas presupuestadas para las funciones de trabajo en el Planificador de Recursos y la tasa de Costo por Hora de cada rol de trabajo.\
   El coste presupuestado afecta a la variable **Valor neto** del proyecto. Para obtener más información sobre cómo se calcula el coste presupuestado, consulte [Calcular costo presupuestado](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Costo de riesgo potencial**: Este es el coste asociado a cualquier riesgo en el proyecto, tal como se define en el caso de negocio o en la pestaña Riesgos del proyecto.\
   Para obtener más información sobre el cálculo del coste de riesgo potencial de un proyecto, consulte el artículo [Calcular Coste de Riesgo Potencial](../../../manage-work/projects/project-finances/potential-risk-cost.md).

    

## Localizar el valor neto del proyecto

Puede encontrar el valor neto de un proyecto en las siguientes áreas de Workfront:

* En el área Resumen de Caso de Negocio del Caso de Negocio \
   Para obtener más información sobre el área Resumen de casos empresariales, consulte la sección &quot;Explicación del resumen de casos empresariales&quot; en el artículo [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* En Portfolio Optimizer si el proyecto está asociado con un portafolio

   >[!TIP]
   >
   >El total de todos los valores netos del proyecto es el valor neto del portafolio.

   Para obtener más información sobre el Optimizador de Portfolio, consulte [Información general sobre Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* En el campo Valor neto del proyecto de las siguientes listas e informes:

   * Proyecto
   * Tarea
   * Problema
   * Proyecto (Datos financieros)
   Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
