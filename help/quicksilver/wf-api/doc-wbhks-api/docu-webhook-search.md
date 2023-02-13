---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Buscar a través de Webhooks de documentos
description: Buscar a través de Webhooks de documentos
author: John
feature: Workfront API, Digital Content and Documents
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 4%

---

# Buscar a través de Webhooks de documentos

Devuelve metadatos de los archivos y carpetas devueltos por una búsqueda. Esto se puede implementar como una búsqueda de texto completo o como una consulta de base de datos normal. Adobe Workfront llama al extremo /search cuando el usuario realiza una búsqueda desde el explorador de archivos externo.

## Dirección URL

GET /búsqueda

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
   <td>Término o frase de búsqueda.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(opcional) El ID de la carpeta desde la que se ejecutó la búsqueda. Nota: Este es un marcador de posición para una función futura en Workfront. Actualmente, workfront no pasa este parámetro. </p> </td> 
  </tr> 
  <tr> 
   <td>máx.</td> 
   <td>El número máximo de elementos que se van a devolver. Se utiliza para la paginación.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> El desplazamiento de página, utilizado junto con "max".</td> 
  </tr> 
 </tbody> 
</table>

 

## respuesta

JSON contiene una lista de metadatos para archivos y carpetas que coinciden con la consulta. Lo que constituye una &quot;coincidencia&quot; lo determina el proveedor de weblinks. Idealmente, debería hacer una búsqueda de texto completo. También funciona la búsqueda basada en nombres de archivo.

**Ejemplo:**

Ejemplo:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
