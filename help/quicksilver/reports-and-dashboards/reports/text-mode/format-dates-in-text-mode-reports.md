---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formato de fechas en informes de modo de texto
description: Las fechas se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront. Para establecer un formato de fecha, debe modificar la línea valueformat del código de modo de texto en la columna.
author: Courtney
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 90%

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

You can format dates using the following `valueformat` text mode values:

| **Formato** | Ejemplo | ***valueformat=*** |
|---|---|---|
| MM/DD/AA | 10/11/18 | `atDate` |
| MM/DD/AA Hora | 10/11/18 12:00pm | `longAtDate` |
| MM/DD/AA | 10/11/18 | `shortAtDate` |
| Mes, DD, AÑO | Oct 11, 2018 | `mediumAtDate` |
| DS, Mes, Día, AÑO | Lun, Octubre 11, 2018 | `partialAtDate` |
| DS, Mes, Día AÑO Hora | Mon, Oct, 11, 2018 12:00 pm | `fullAtDate` |
