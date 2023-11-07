---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Buscar mediante webhooks de documentos
description: Buscar mediante webhooks de documentos
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 5%

---

# Buscar mediante webhooks de documentos

Devuelve metadatos de los archivos y carpetas devueltos por una búsqueda. Esto se puede implementar como una búsqueda de texto completo o como una consulta de base de datos normal. Adobe Workfront llama al extremo /search cuando el usuario realiza una búsqueda desde el explorador de archivos externo.

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
   <td>Número máximo de elementos que se van a devolver. Se utiliza para la paginación.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> El desplazamiento de página, utilizado junto con "max".</td> 
  </tr> 
 </tbody> 
</table>

 

## respuesta

JSON que contiene una lista de metadatos para archivos y carpetas que coinciden con la consulta. Lo que constituye una &quot;coincidencia&quot; lo determina el proveedor del gancho web. Lo ideal es que realice una búsqueda de texto completo. También funciona la búsqueda basada en nombres de archivo.

**Ejemplo:**

Ejemplo:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
