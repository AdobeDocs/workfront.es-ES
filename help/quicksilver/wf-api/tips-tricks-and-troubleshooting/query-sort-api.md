---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Clasificación de resultados de consulta en la API
description: Clasificación de resultados de consulta en la API
author: John
feature: Workfront API
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Clasificación de resultados de consulta en la API

Puede ordenar los resultados por cualquier campo si añade lo siguiente a su llamada de API:

```
&entryDate_Sort=asc
```

Por ejemplo, si desea ordenar por tarea Fecha de inicio planeada, elimine `entryDate` y reemplácelo por `plannedCompletionDate`.

Esto funciona para la mayoría de los campos de Adobe Workfront.
