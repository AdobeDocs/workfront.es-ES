---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Muestra los metadatos de archivos o carpetas
description: Muestra los metadatos de archivos o carpetas
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
TQID: https://experienceleague.adobe.com/nZv42xMbDRJbkwR-lFKI6dAbeszSzGWAwn--qkKhVVM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 101
ht-degree: 70%

---

# Obtener una lista de elementos del contenido de la carpeta

Enumera los metadatos de los archivos y carpetas de una carpeta determinada.

**URL**

GET /files

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| parentId  | El ID de la carpeta. Para obtener los metadatos del directorio raíz, utilice el valor &quot;/&quot;. |
| máx.  | Número máximo de elementos que se devolverán. Se utiliza para la paginación. |
| offset  |  El desplazamiento de página, utilizado junto con “max”. |


## Respuesta

JSON que contiene una lista de archivos y carpetas. Los metadatos de cada elemento son los mismos que los devueltos por el/punto final de los metadatos.

**Ejemplo:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
