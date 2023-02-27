---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Muestra metadatos de archivos o carpetas
description: Muestra metadatos de archivos o carpetas
author: Becky
feature: Workfront API
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 5%

---


# Obtener lista de elementos del contenido de la carpeta

Enumera los metadatos de los archivos y carpetas de una carpeta determinada.

**Dirección URL**

GET /archivos

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| parentId  | El ID de la carpeta. Para obtener los metadatos del directorio raíz, utilice el valor ‘/&#39;. |
| máximo de  | El número máximo de elementos que se van a devolver. Se utiliza para la paginación. |
| offset  |  El desplazamiento de página, utilizado junto con &quot;max&quot;. |


## respuesta

JSON que contiene una lista de archivos y carpetas. Los metadatos de cada elemento son los mismos que devuelve el extremo /metadata .

**Ejemplo:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ”,
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ”,
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
