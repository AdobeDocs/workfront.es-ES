---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcular el riesgo para el valor neto en un portafolio
description: En el Optimizador de Portfolio, la variable [!UICONTROL Riesgo para el valor neto] El indicador mide el riesgo potencial teniendo en cuenta el valor neto proporcionado por todos los proyectos mostrados en Portfolio Optimizer.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Calcular el [!UICONTROL Riesgo para el valor neto] en un portafolio

En el [!UICONTROL Optimizador de Portfolio], el [!UICONTROL Riesgo para el valor neto] El indicador mide el riesgo potencial teniendo en cuenta el [!UICONTROL Valor neto] proporcionado por todos los proyectos mostrados en la variable [!UICONTROL Optimizador de Portfolio]. 

Para lograr la mayor eficiencia dentro del portafolio, desea ver que la variable [!UICONTROL Riesgo] el indicador es bajo y la variable [!UICONTROL Valor neto] el indicador es alto. 

La variable [!UICONTROL Riesgo] y [!UICONTROL Valor neto] los indicadores se representan desde la perspectiva de cómo se relacionan entre sí.

[!DNL Adobe Workfront] calcula la variable [!UICONTROL Riesgo] y [!UICONTROL Valor neto] indicadores que utilizan las siguientes fórmulas:

* La variable [!UICONTROL Riesgo] el indicador se calcula mediante la fórmula siguiente:

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* La variable [!DNL Net Value] se calcula mediante las siguientes fórmulas:

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   O

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>La variable [!UICONTROL Riesgo para el valor neto] el indicador se calcula en función de los proyectos que se muestran en la [!UICONTROL Optimizador de Portfolio], y no en todos los proyectos asociados al portafolio. 
