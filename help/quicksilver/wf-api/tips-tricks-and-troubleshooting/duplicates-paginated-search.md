---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicados devueltos durante una búsqueda paginada grande
description: Duplicados devueltos durante una búsqueda paginada grande
author: John
feature: Workfront API
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Duplicados devueltos durante una búsqueda paginada grande

## Problema

Al realizar una búsqueda paginada grande en la API de un objeto, el cliente recibe entradas duplicadas y registros que faltan.

## Solución

Cuando el pedido no se define formalmente, dependemos del orden de las filas devueltas por la base de datos de Oracle, que no garantiza ningún orden determinístico. Por ejemplo, dos llamadas consecutivas con la misma consulta podrían devolver filas en un orden diferente. Del mismo modo, al realizar la paginación, las filas pueden asignarse aleatoriamente a &quot;páginas&quot; diferentes, lo que da lugar a duplicados. La solución más sencilla puede ser agregar clasificación por ID:

```
&ID_Sort=asc
```

