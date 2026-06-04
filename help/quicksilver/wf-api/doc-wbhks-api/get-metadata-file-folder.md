---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener metadatos para un archivo o una carpeta
description: Obtener metadatos para un archivo o una carpeta
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
TQID: https://experienceleague.adobe.com/H04UQeyhGw-FdXDwaRZs5PSXnN-YErVptHWn-78INYo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 90%

---

# Obtener metadatos para un archivo o una carpeta

Devuelve los metadatos del archivo o la carpeta especificados.

**URL**

GET /metadata?id=[identificador de documento o carpeta]

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
   <td>id</td> 
   <td>El ID del archivo o la carpeta, tal como lo hace referencia el proveedor del gancho web. Es diferente al ID del documento de Adobe Workfront. Para obtener los metadatos del directorio raíz, utilice el valor "/".
   <p>Nota: La longitud máxima del ID es de 255 caracteres.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Respuesta

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre </th> 
   <th>Tipo </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>Cadena </td> 
   <td>El nombre del documento o la carpeta</td> 
  </tr> 
  <tr> 
   <td>kind </td> 
   <td>Cadena </td> 
   <td>Especifica si este elemento es un archivo o una carpeta (“archivo” o “carpeta”)</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Cadena </td> 
   <td>El ID del archivo o carpeta.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Cadena </td> 
   <td> <p>La ruta URL utilizada por un usuario para ver el documento en una ventana del explorador. La URL puede alojarla el proveedor de documentos o el proveedor de almacenamiento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Cadena </td> 
   <td> <p>La ruta de URL utilizada por un usuario para descargar el documento en una ventana del explorador. La URL puede alojarla el proveedor de documentos o el proveedor de almacenamiento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Cadena </td> 
   <td>El tipo MIME del archivo. (opcional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Cadena </td> 
   <td>Última vez que se modificó este archivo (marca de tiempo RFC 3339 con formato)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Largo</td> 
   <td> El tamaño del archivo en bytes. (opcional)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booleano</td> 
   <td> Indica si este archivo o carpeta es de solo lectura para el usuario autenticado. (opcional) </td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"My Document",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"2014­06­05T17:39:45.251Z",<br>size: "32554694"<br>}</pre>

>[!NOTE]
>
>La gestión de errores debe ser coherente en todas las llamadas a la API. Consulte la sección “Gestión de errores” más abajo para obtener más información.
