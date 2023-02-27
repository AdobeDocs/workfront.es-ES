---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Crear una carpeta con Webhooks de documento
description: Crear una carpeta con Webhooks de documento
author: Becky
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 7%

---


# Crear una carpeta con Webhooks de documento

Crea una carpeta en un directorio determinado.

## Dirección URL

POST /createFolder

## Parámetros de consulta

| **Nombre** | **Descripción** |
|---|---|
| parentId  | El ID de carpeta en el que se debe crear la carpeta |
| name  | El nombre de la nueva carpeta |




**Respuesta**

Los metadatos de la carpeta recién creada, tal como se define en el extremo /metadata .

## Ejemplo

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

return

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
