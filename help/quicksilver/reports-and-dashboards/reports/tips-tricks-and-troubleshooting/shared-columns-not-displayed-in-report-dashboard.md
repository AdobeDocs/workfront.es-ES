---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Los datos de las columnas compartidas no se muestran en los informes del panel de control
description: Los datos de las columnas compartidas no se muestran cuando el informe se coloca en un diseño de panel de control con varias columnas, pero sí que se muestran en un diseño de una sola columna. También se anulan los saltos de línea.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 83%

---

# Los datos de las columnas compartidas no se muestran en los informes del panel de control

## Problema

Los datos de las columnas compartidas no se muestran cuando el informe se coloca en un diseño de panel de control con varias columnas, pero sí que se muestran en un diseño de una sola columna. También se anulan los saltos de línea.

## Causa

Solo las columnas marcadas como

```
shortview=true
```

se incluyen en la vista de panel de control del informe cuando el diseño del panel de control tiene la división izquierda/derecha o la división izquierda/central/derecha configurada.

## Solución

Acceda a la vista que se utiliza en el informe y abra el modo de texto. (Para obtener más información, vea [Editar una vista utilizando el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Etiqueta todas las columnas del informe, incluidas las columnas utilizadas en una columna compartida o combinada, con

```
shortview=true
```

. Las columnas del informe se mostrarán correctamente en el panel de control.
