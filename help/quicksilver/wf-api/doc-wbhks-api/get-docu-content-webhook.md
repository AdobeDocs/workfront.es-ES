---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener contenido del documento mediante webhooks
description: Devuelve los bytes sin procesar de un documento
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 9%

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

## Respuesta

Los bytes sin procesar del documento.

**Ejemplo**:  `https://www.acme.com/api/download?id=123456`
