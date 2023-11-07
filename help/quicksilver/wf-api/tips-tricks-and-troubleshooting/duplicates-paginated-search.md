---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicados devueltos durante una búsqueda paginada grande
description: Duplicados devueltos durante una búsqueda paginada grande
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Duplicados devueltos durante una búsqueda paginada grande

## Problema

Al realizar una búsqueda paginada de gran tamaño en la API para un objeto, el cliente recibe entradas duplicadas y registros faltantes.

## Solución

Cuando el orden no está definido formalmente, nos basamos en el orden de las filas devueltas por la base de datos de Oracle, lo que no garantiza ningún orden determinista. Por ejemplo, dos llamadas consecutivas con la misma consulta podrían devolver filas en un orden diferente. Del mismo modo, al realizar la paginación, las filas pueden asignarse aleatoriamente a distintas &quot;páginas&quot;, lo que provoca duplicados. La solución más sencilla es agregar la ordenación por ID:

```
&ID_Sort=asc
```

