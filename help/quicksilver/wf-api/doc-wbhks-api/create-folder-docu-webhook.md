---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Crear una carpeta con webhooks de documentos
description: Crear una carpeta con webhooks de documentos
author: Becky
feature: Workfront API
role: Developer
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 10%

---


# Crear una carpeta con webhooks de documentos

Crea una carpeta en un directorio determinado.

## URL

POST /createFolder

## Parámetros de consulta

| **Nombre** | **Descripción** |
|---|---|
| parentId  | ID de la carpeta en la que se debe crear la carpeta |
| name  | Nombre de la nueva carpeta |




**Respuesta**

Los metadatos de la carpeta recién creada, tal como se define en el extremo /metadata.

## Ejemplo

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

devoluciones

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"",
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
