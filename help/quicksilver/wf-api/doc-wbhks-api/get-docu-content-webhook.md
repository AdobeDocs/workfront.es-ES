---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener contenido del documento mediante webhooks
description: Devuelve los bytes sin procesar de un documento
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 13%

---

# Obtener contenido del documento mediante webhooks

Devuelve los bytes sin procesar de un documento

## URL

GET/descarga

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
   <td> ID del documento.</td> 
  </tr> 
 </tbody> 
</table>

## respuesta

Los bytes sin procesar del documento.

**Ejemplo**:  `https://www.acme.com/api/download?id=123456`
