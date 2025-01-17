---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formato de números, moneda y valores de porcentaje en los informes de modo de texto
description: Los valores numéricos, incluida la moneda, se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '145'
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
| 12 % | `doubleAsPercentRounded` |
| 12.34% | `doubleAsPercent` |
| (1,234.56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

