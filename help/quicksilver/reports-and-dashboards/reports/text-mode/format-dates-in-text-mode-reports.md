---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formato de fechas en informes de modo de texto
description: Las fechas se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront. Para establecer un formato de fecha, debe modificar la línea valueformat del código de modo de texto en la columna.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 94%

---

# Formato de fechas en informes de modo de texto

<!-- Audited: 1/2025 -->

Las fechas se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront. Para establecer un formato de fecha, debe modificar la línea `valueformat` del código de modo de texto en la columna.

`valueformat= [new date format]` Por ejemplo, si desea que la fecha proyectada de finalización se muestre como MM/DD/AA, el código sería el siguiente:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Si desea mostrar la fecha planificada de finalización como *mes, día, año*, el código tendría el siguiente aspecto:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Para obtener más información sobre la aplicación de formato condicional en informes y listas de Workfront mediante el modo de texto, consulte [Usar formato condicional en el modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Puede dar formato a las fechas utilizando los siguientes `valueformat` valores del modo de texto:

| **Formato** | Ejemplo | ***valueformat=*** |
|---|---|---|
| MM/DD/AA | 10/11/18 | `atDate` |
| MM/DD/AA Hora | 10/11/18 12:00 h | `longAtDate` |
| MM/DD/AA | 10/11/18 | `shortAtDate` |
| Mes, DD, AÑO | Oct 11, 2018 | `mediumAtDate` |
| DS, Mes, Día, AÑO | Lun, Octubre 11, 2018 | `partialAtDate` |
| DS, Mes, Día AÑO Hora | Lun, Oct 11, 2018 12:00 pm | `fullAtDate` |
