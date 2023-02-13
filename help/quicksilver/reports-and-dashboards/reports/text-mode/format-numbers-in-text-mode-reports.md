---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formato de números, moneda y valores de porcentaje en los informes de modo de texto
description: Los valores numéricos, incluida la moneda, se pueden configurar para que se muestren en diversos formatos en los informes y listas de Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 7%

---

# Formato de números, moneda y valores de porcentaje en los informes de modo de texto

Los valores numéricos, incluida la moneda, se pueden configurar para que se muestren en diversos formatos en los informes y listas de Adobe Workfront.

Para modificar el formato de un valor numérico, debe editar la variable **valueformat** línea de la columna.

Por ejemplo, si desea mostrar la columna Presupuesto como 1000 $, la línea de formato de valor tendría el siguiente aspecto:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Para obtener más información sobre la aplicación de formato condicional en informes y listas de Workfront que utilizan el modo de texto, consulte [Utilizar el formato condicional en modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Puede dar formato a los números utilizando los valores siguientes para la variable `valueformat` línea de la columna:

| Ejemplo | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>o <br><pre>int</pre> |
| 1.234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRound</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRound</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRound</pre> |
