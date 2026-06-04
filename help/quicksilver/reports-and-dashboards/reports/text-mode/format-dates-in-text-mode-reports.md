---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formato de fechas en informes de modo de texto
description: Las fechas se pueden configurar para que se muestren en diversos formatos en los informes y las listas de Adobe Workfront. Para establecer un formato de fecha, debe modificar la línea valueformat del código de modo de texto en la columna.
author: Courtney
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-8gB8XDwLQTBCUsrex-PIAyxcF-rSPsoM2Gvw2EhTaU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 204
ht-degree: 92%

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

| **Formato** | Ejemplo  | ***valueformat=*** |
|---|---|---|
| MM/DD/AA | 10/11/18 | `atDate` |
| MM/DD/AA Hora | 10/11/18 12:00pm | `longAtDate` |
| MM/DD/AA | 10/11/18 | `shortAtDate` |
| Mes, DD, AÑO | Oct 11, 2018 | `mediumAtDate` |
| DS, Mes, Día, AÑO | Lun, Octubre 11, 2018 | `partialAtDate` |
| DS, Mes, Día AÑO Hora | Lun, 11 de octubre de 2018 12:00 pm | `fullAtDate` |
