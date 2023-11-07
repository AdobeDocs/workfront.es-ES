---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener metadatos de un archivo o carpeta
description: Obtener metadatos de un archivo o carpeta
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 7%

---


# Obtener metadatos de un archivo o carpeta

Devuelve los metadatos del archivo o la carpeta especificados.

**URL**

GET /metadata?id=[ID de documento o carpeta]

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

 

## respuesta

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
   <td>bondadoso </td> 
   <td>Cadena </td> 
   <td>Especifica si este elemento es un archivo o una carpeta ("archivo" o "carpeta")</td> 
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
   <td> <p>Ruta de URL utilizada por un usuario para descargar el documento en una ventana del explorador. La URL puede alojarla el proveedor de documentos o el proveedor de almacenamiento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Cadena </td> 
   <td>Tipo MIME del archivo. (opcional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Cadena </td> 
   <td>Última vez que se modificó este archivo (marca de tiempo RFC 3339 con formato)</td> 
  </tr> 
  <tr> 
   <td>talla</td> 
   <td>Largo</td> 
   <td> El tamaño del archivo en bytes. (opcional)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booleano</td> 
   <td> Indica si este archivo o carpeta es de sólo lectura para el usuario autenticado.(opcional) </td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title: "Mi documento",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45,251",<br>tamaño: "32554694"<br>}</pre>

>[!NOTE]
>
>La gestión de errores debe ser coherente en todas las llamadas a la API. Consulte la sección &quot;Gestión de errores&quot; más abajo para obtener más información.
