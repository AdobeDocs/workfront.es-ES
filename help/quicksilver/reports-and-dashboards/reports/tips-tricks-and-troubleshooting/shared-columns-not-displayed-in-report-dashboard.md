---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Los datos de las columnas compartidas no se muestran en los informes del panel
description: Los datos de las columnas compartidas no se muestran cuando el informe se coloca en un diseño de panel de varias columnas, pero sí en un diseño de una sola columna. También se anulan los saltos de línea.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Los datos de las columnas compartidas no se muestran en los informes del panel

## Problema

Los datos de las columnas compartidas no se muestran cuando el informe se coloca en un diseño de panel de varias columnas, pero sí en un diseño de una sola columna. También se anulan los saltos de línea.

## Causa

Solo las columnas marcadas como

```
shortview=true
```

se incluyen en la vista de panel del informe cuando el diseño del panel tiene la división izquierda/derecha o la división izquierda/central/derecha configurada.

## Solución

Acceda a la vista utilizada en el informe y abra el modo de texto. (Para obtener más información, vea [Editar una vista en modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Etiquete todas las columnas del informe, incluidas las utilizadas en una columna compartida/combinada, con

```
shortview=true
```

. Las columnas del informe se mostrarán correctamente en el panel.
