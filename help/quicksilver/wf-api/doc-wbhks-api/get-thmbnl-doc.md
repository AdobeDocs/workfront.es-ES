---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener una miniatura de un documento
description: Obtener una miniatura de un documento
author: John
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 7%

---


# Obtener una miniatura de un documento

Devuelve los bytes de miniaturas sin procesar de un documento.

**Dirección URL**

GET/miniatura

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| id  | El ID del documento. |
| size  |  Ancho de la miniatura. |


## respuesta

Los bytes de miniaturas sin procesar.

**Ejemplo:**: https://www.acme.com/api/thumbnail?id=123456
