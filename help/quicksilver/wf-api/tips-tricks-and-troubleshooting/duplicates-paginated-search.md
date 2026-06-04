---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Se devolvieron duplicados durante una búsqueda paginada grande
description: Se devolvieron duplicados durante una búsqueda paginada grande
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 100%

---

# Se devolvieron duplicados durante una búsqueda paginada grande

## Problema

Al realizar una búsqueda paginada de gran tamaño en la API para un objeto, el cliente recibe entradas duplicadas y registros faltantes.

## Solución

Cuando el orden no se define formalmente, nos basamos en el orden de las filas devueltas por la base de datos Oracle, lo que no garantiza ningún orden determinista. Por ejemplo, dos llamadas consecutivas con la misma consulta podrían devolver filas en un orden diferente. Del mismo modo, al realizar la paginación, las filas podrían asignarse aleatoriamente a distintas “páginas”, provocando duplicados. La solución más sencilla es añadir la ordenación por ID:

```
&ID_Sort=asc
```

