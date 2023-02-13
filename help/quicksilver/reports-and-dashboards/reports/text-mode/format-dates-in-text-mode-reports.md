---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formato de fechas en informes en modo de texto
description: Las fechas se pueden configurar para que se muestren en diversos formatos en informes y listas en Adobe Workfront. Para establecer un formato de fecha, debe modificar la línea value-format del código de modo de texto en la columna .
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 2%

---

# Formato de fechas en informes en modo de texto

Las fechas se pueden configurar para que se muestren en diversos formatos en informes y listas en Adobe Workfront. Para establecer un formato de fecha, debe modificar la variable `valueformat` línea del código de modo de texto en la columna .

`valueformat= [new date format]` Por ejemplo, si desea que la Fecha de finalización prevista se muestre como MM/DD/AA, el código tendría el siguiente aspecto:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Si desea mostrar la fecha de finalización planeada como *Mth, DD, Year*, el código tendría el siguiente aspecto:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Para obtener más información sobre la aplicación de formato condicional en informes y listas de Workfront que utilizan el modo de texto, consulte [Utilizar el formato condicional en modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Puede dar formato a las fechas utilizando lo siguiente

```
valueformat
```

 valores del modo de texto:

| **Formato** | Ejemplo  | ***valueformat=*** |
|---|---|---|
| MM/DD/AA | 10/11/18 | `atDate` |
| MM/DD/AA | 11/10/18 12:00 pm | `longAtDate` |
| MM/DD/AA | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11 de octubre de 2018 | `mediumAtDate` |
| DW, Mth, Day, YR | Lunes, 11 de octubre de 2018 | `partialAtDate` |
| DW, Mth, Day, YR Time | Lunes, octubre, 11, 2018 12:00 pm | `fullAtDate` |
