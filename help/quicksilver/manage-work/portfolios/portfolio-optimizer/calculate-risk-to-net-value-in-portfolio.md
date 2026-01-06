---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcular el riesgo de valor neto en un portafolio
description: En el Optimizador de portafolios, el indicador [!UICONTROL Risk to Net Value] mide el riesgo potencial teniendo en cuenta el valor neto proporcionado por todos los proyectos mostrados en el Optimizador de portafolios.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '178'
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
