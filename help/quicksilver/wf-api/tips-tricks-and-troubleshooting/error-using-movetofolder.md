---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: La acción moveToFolder del documento no funciona
description: Al utilizar la acción moveToFolder del documento, se devuelve un error 422.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
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
source-wordcount: 121
ht-degree: 100%

---

# La acción moveToFolder del documento no funciona

## Problema

Al utilizar la acción `moveToFolder` del objeto Document, se devuelve un error 422.

O

Si se utiliza esta acción a través del módulo Adobe Authenticator en Workfront Fusion, el documento no se mueve, pero no hay indicación del error. El error es el mismo, pero el módulo de Adobe Authenticator no lo muestra.

## Solución

Una posible causa de un error 422 para esta acción es que la acción está intentando mover un documento de una carpeta vinculada a otra carpeta vinculada.

Compruebe que el documento que desea mover no esté ya en una carpeta vinculada.
