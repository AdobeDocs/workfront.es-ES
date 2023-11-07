---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener una miniatura de un documento
description: Obtener una miniatura de un documento
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 11%

---


# Obtener una miniatura de un documento

Devuelve los bytes de miniatura sin procesar de un documento.

**URL**

GET/miniatura

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| id  | ID del documento. |
| talla  |  Ancho de la miniatura. |


## respuesta

Los bytes de miniatura sin procesar.

**Ejemplo:**: https://www.acme.com/api/thumbnail?id=123456
