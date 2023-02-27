---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Carga de archivos a través de Document Webhooks
description: Carga de archivos a través de Document Webhooks
author: Becky
feature: Workfront API
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%

---


# Carga de archivos a través de Document Webhooks

La carga de un archivo en un proveedor de almacenamiento de documentos es un proceso de dos pasos que requiere dos extremos de API independientes. Adobe Workfront inicia el proceso de carga llamando a /uploadInit . Este extremo devuelve un ID de documento que luego se pasa a /upload al cargar los bytes del documento. Dependiendo del sistema de almacenamiento de documentos subyacente, podría ser necesario crear un documento de longitud cero y luego actualizar el contenido del documento más adelante.

Se ha añadido a la versión 1.1 de esta especificación, el ID de documento y el ID de versión de documento pueden utilizarse para recuperar información adicional de Workfront.

**Ejemplo:** Si el sistema de administración de documentos desea información adicional sobre el documento, el código de implementación de weblock podría utilizar el ID del documento para recuperar esa información mediante la API RESTful de Workfront. Como práctica recomendada, esta información podría provenir de campos de datos personalizados del documento y contiene tareas, problemas o proyectos.

## Método POST

**Dirección URL**

POST /uploadInit

### Parámetros de consulta

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
   <td>parentId </td> 
   <td>El ID de la carpeta principal, tal como hace referencia el proveedor de vínculos web.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>El nombre del documento</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>El ID del documento de Workfront (añadido en la versión 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>El ID de versión del documento de Workfront (añadido en la versión 1.1) </td> 
  </tr> 
 </tbody> 
</table>

## respuesta

Los metadatos del archivo, tal como se definen en el extremo /metadata . Esto incluye el ID del documento utilizado por el proveedor.

**Ejemplo:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Método PUT

Carga los bytes de un documento en el proveedor de enlaces web.

**Dirección URL**

PUT /upload

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| id  |  El ID del documento que acaba de crearse. |


**Cuerpo de la solicitud**

Los bytes de contenido sin procesar del documento.

**Respuesta**

```
{
result: “success”
}
```

o

```
{
result: “fail”
}
```

**Ejemplo**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

response

```
{
result:"success"
}
```
