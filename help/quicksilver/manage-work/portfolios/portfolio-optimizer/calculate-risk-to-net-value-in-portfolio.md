---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcular el riesgo de valor neto en un portafolio
description: En el Optimizador de portafolios, el indicador [!UICONTROL Risk to Net Value] mide el riesgo potencial teniendo en cuenta el valor neto proporcionado por todos los proyectos mostrados en el Optimizador de portafolios.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 52%

---

# Calcular el [!UICONTROL Risk to Net Value] de un portafolio

En [!UICONTROL Portfolio Optimizer], el indicador [!UICONTROL Riesgo para el valor neto] mide el riesgo potencial teniendo en cuenta el [!UICONTROL valor neto] proporcionado por todos los proyectos mostrados en [!UICONTROL Portfolio Optimizer].

Para lograr la máxima eficiencia dentro del portafolio, quiere ver que el indicador [!UICONTROL Riesgo] es bajo y el indicador [!UICONTROL Valor neto] es alto.

Los indicadores [!UICONTROL Risk] y [!UICONTROL Net Value] se representan desde la perspectiva de cómo se relacionan entre sí.

[!DNL Adobe Workfront] calcula los indicadores [!UICONTROL Riesgo] y [!UICONTROL Valor neto] utilizando las siguientes fórmulas:

* El indicador [!UICONTROL Riesgo] se calcula mediante la fórmula siguiente:

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* El indicador [!DNL Net Value] se calcula mediante las siguientes fórmulas:

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  O

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>El indicador [!UICONTROL Riesgo para el valor neto] se calcula en función de los proyectos que se muestran en [!UICONTROL Portfolio Optimizer] y no en todos los proyectos asociados con el portafolio.
