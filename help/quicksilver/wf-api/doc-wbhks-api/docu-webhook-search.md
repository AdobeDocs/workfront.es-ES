---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Búsqueda mediante webhooks de documentos
description: Búsqueda mediante webhooks de documentos
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
TQID: https://experienceleague.adobe.com/flRrmTOPVSGP83tVYfKG9AZOT7CNZN4IeWZNsVwcOO4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 139
ht-degree: 93%

---

# Búsqueda mediante webhooks de documentos

Devuelve metadatos de los archivos y carpetas devueltos por una búsqueda. Esto se puede implementar como una búsqueda de texto completo o como una consulta de base de datos normal. Adobe Workfront llama al punto final /search cuando el usuario realiza una búsqueda desde el explorador de archivos externo.

## URL

GET /search

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
   <td>query</td> 
   <td>El término o frase de búsqueda.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(opcional) ID de carpeta desde el que se ejecutó la búsqueda. Nota: Este es un marcador de posición para una función futura de Workfront. Actualmente, Workfront no pasa este parámetro. </p> </td> 
  </tr> 
  <tr> 
   <td>máx.</td> 
   <td>Número máximo de elementos que se devolverán. Se utiliza para la paginación.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> El desplazamiento de página, utilizado junto con “max”.</td> 
  </tr> 
 </tbody> 
</table>

 

## Respuesta

JSON que contiene una lista de metadatos para archivos y carpetas que coinciden con la consulta. Lo que constituye una “coincidencia” lo determina el proveedor del webhook Lo ideal es que realice una búsqueda de texto completo. También funciona la búsqueda basada en nombres de archivo.

**Ejemplo:**

Ejemplo:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
