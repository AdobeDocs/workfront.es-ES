---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Datos de columnas compartidas que no se muestran en los informes de tablero
description: Los datos de las columnas compartidas no se muestran cuando el informe se coloca en un diseño de tablero de varias columnas, pero sí se muestran en un diseño de una sola columna. Los saltos de línea también se anulan.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Datos de columnas compartidas que no se muestran en los informes de tablero

## Problema

Los datos de las columnas compartidas no se muestran cuando el informe se coloca en un diseño de tablero de varias columnas, pero sí se muestran en un diseño de una sola columna. Los saltos de línea también se anulan.

## Causa

Solo las columnas marcadas como

```
shortview=true
```

se incluyen en la vista de panel del informe cuando el diseño del tablero tiene la división izquierda/derecha o la división izquierda/centro/derecha configurada.

## Solución

Acceda a la vista utilizada en el informe y abra el modo de texto. (Para obtener más información, consulte [Edición de una vista mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Etiquete todas las columnas del informe, incluidas las columnas utilizadas en una columna compartida/combinada, con

```
shortview=true
```

. A continuación, las columnas del informe se mostrarán correctamente en el tablero.
