---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener contenido del documento a través de Webhooks
description: Devuelve los bytes sin procesar de un documento
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '53'
ht-degree: 7%

---

# Obtener contenido del documento a través de Webhooks

Devuelve los bytes sin procesar de un documento

## Dirección URL

GET /descarga

## Parámetros de consulta

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> El ID del documento.</td> 
  </tr> 
 </tbody> 
</table>

## respuesta

Los bytes sin procesar del documento.

**Ejemplo:**:  [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
