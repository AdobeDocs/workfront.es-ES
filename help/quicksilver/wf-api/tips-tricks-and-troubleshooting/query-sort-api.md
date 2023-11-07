---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Ordenar los resultados de las consultas en la API
description: Ordenar los resultados de las consultas en la API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Ordenar los resultados de las consultas en la API

Puede ordenar los resultados por cualquier campo si anexa lo siguiente a la llamada de API:

```
&entryDate_Sort=asc
```

Por ejemplo, si desea ordenar por fecha planificada de inicio de la tarea, quite `entryDate` y reemplácelo por `plannedCompletionDate`.

Esto funciona para la mayoría de los campos de Adobe Workfront.
