---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formato de números, moneda y valores de porcentaje en los informes de modo de texto
description: Los valores numéricos, incluida la moneda, se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/z96Rvp54iQcZxVWJ4Evoe1Qasl-VrEZ-IrVy11n9cDc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 145
ht-degree: 35%

---

# Formato de números, moneda y valores de porcentaje en los informes de modo de texto

<!-- Audited: 1/2025 -->

Los valores numéricos, incluida la moneda, se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront.

Para modificar el formato de un valor numérico, debe editar la línea **valueformat** de la columna.

Por ejemplo, si desea mostrar la columna Presupuesto como 1000 $, la línea de formato de valor tendría el siguiente aspecto:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Para obtener más información sobre la aplicación de formato condicional en informes y listas de Workfront mediante el modo de texto, consulte [Usar formato condicional en el modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Puede dar formato a los números utilizando los siguientes valores para la línea `valueformat` de la columna:

| Ejemplo | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br>o<br>`int` |
| 1.234 | `doubleAsInt` |
| $1,234 | `currencyStringCurrencyRounded` |
| 1234,56 | `doubleAsDouble` |
| $1,234.56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12.34% | `doubleAsPercent` |
| (1,234.56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

