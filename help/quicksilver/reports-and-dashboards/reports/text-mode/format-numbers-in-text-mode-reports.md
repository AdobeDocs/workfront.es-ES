---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formato de números, moneda y valores de porcentaje en los informes de modo de texto
description: Los valores numéricos, incluida la moneda, se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 8de9c79f6c62b74a652482ec10bf38fada8c5fc8
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 7%

---

# Formato de números, moneda y valores de porcentaje en los informes de modo de texto

<!-- Audited: 2/2024 -->

Los valores numéricos, incluida la moneda, se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront.

Para modificar el formato de un valor numérico, debe editar la línea **valueformat** de la columna.

Por ejemplo, si desea mostrar la columna Presupuesto como 1000 $, la línea de formato de valor tendría el siguiente aspecto:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Para obtener más información acerca de la aplicación de formato condicional en informes y listas de Workfront mediante el modo de texto, vea [Usar formato condicional en el modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Puede dar formato a los números utilizando los siguientes valores para la línea `valueformat` de la columna:

| Ejemplo | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br> o <br><pre>int</pre> |
| 1.234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234,56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |

