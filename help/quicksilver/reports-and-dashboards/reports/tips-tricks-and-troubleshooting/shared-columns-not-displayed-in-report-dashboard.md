---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Los datos de las columnas compartidas no se muestran en los informes del panel de control
description: Los datos de las columnas compartidas no se muestran cuando el informe se coloca en un diseño de panel de control con varias columnas, pero sí que se muestran en un diseño de una sola columna. También se anulan los saltos de línea.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 162
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

Acceda a la vista que se utiliza en el informe y abra el modo de texto. (Para obtener más información, vea [Editar una vista en modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Etiquete todas las columnas del informe, incluidas las utilizadas en una columna compartida/combinada, con

```
shortview=true
```

. Las columnas del informe se mostrarán correctamente en el panel de control.
