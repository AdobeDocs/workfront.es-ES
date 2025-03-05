---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Ordenar los resultados de consulta en la API
description: Ordenar los resultados de consulta en la API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 58%

---


# Ordenar los resultados de consulta en la API

Puede ordenar los resultados por cualquier campo si anexa lo siguiente a la llamada de API:

```
&entryDate_Sort=asc
```

Por ejemplo, si desea ordenar por fecha planificada de finalización de la tarea, elimine `entryDate` y reemplace con `plannedCompletionDate`.

```
&plannedCompletionDate_Sort=asc
```

Esto funciona para la mayoría de los campos de Adobe Workfront.
