---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formato de fechas en informes de modo de texto
description: Las fechas se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront. Para establecer un formato de fecha, debe modificar la línea de formato de valor del código de modo de texto en la columna.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Formato de fechas en informes de modo de texto

Las fechas se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront. Para establecer un formato de fecha, debe modificar la línea `valueformat` del código de modo de texto en la columna.

`valueformat= [new date format]` Por ejemplo, si desea que la fecha proyectada de finalización se muestre como MM/DD/AA, el código tendría el siguiente aspecto:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Si desea mostrar la fecha planificada de finalización como *Mes, DD, Año*, el código tendría el siguiente aspecto:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Para obtener más información acerca de la aplicación de formato condicional en informes y listas de Workfront mediante el modo de texto, vea [Usar formato condicional en el modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Puede dar formato a las fechas mediante los siguientes métodos

```
valueformat
```

 valores del modo de texto:

| **Formato** | Ejemplo  | ***valueformat=*** |
|---|---|---|
| DD/MM/AA | 10/11/18 | `atDate` |
| Hora de MM/DD/AA | 11/10/18 12:00 h | `longAtDate` |
| DD/MM/AA | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11 de octubre de 2018 | `mediumAtDate` |
| DW, Mth, Day, YR | Lun, 11 de octubre de 2018 | `partialAtDate` |
| DW, Mth, Day, YR Time | Lun, 11 de octubre de 2018 12:00 pm | `fullAtDate` |
