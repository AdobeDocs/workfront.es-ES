---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Carga de archivos mediante webhooks de documentos
description: Carga de archivos mediante webhooks de documentos
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 5%

---


# Carga de archivos mediante webhooks de documentos

La carga de un archivo a un proveedor de almacenamiento de documentos es un proceso de dos pasos que requiere dos extremos de API independientes. Adobe Workfront inicia el proceso de carga llamando a /uploadInit Este extremo devuelve un ID de documento que luego se pasa a /upload al cargar los bytes del documento. Según el sistema de almacenamiento de documentos subyacente, puede ser necesario crear un documento de longitud cero y actualizar el contenido del documento más adelante.

Añadido a la versión 1.1 de esta especificación, el ID de documento y el ID de versión de documento se pueden utilizar para recuperar información adicional de Workfront.

**Ejemplo:** Si el sistema de administración de documentos desea información adicional sobre el documento, el código de implementación del gancho web podría utilizar el ID del documento para recuperar esa información mediante la API RESTful de Workfront. Como práctica recomendada, esta información podría proceder de campos de datos personalizados del documento y contener tareas, problemas o proyectos.

## Método POST

**URL**

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
   <td>ID de la carpeta principal, tal como lo hace referencia el proveedor de ganchos web.</td> 
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
   <td>El ID de la versión del documento de Workfront (añadido en la versión 1.1) </td> 
  </tr> 
 </tbody> 
</table>

## respuesta

Los metadatos del archivo, tal como se definen en el extremo /metadata. Esto incluye el ID de documento utilizado por el proveedor.

**Ejemplo:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Método PUT

Carga los bytes de un documento al proveedor de ganchos web.

**URL**

PUT /upload

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| id  |  El ID del documento, que acaba de crearse. |


**Cuerpo de solicitud**

Los bytes de contenido sin procesar del documento.

**Respuesta**

```
{
result: "success"
}
```

o

```
{
result: "fail"
}
```

**Ejemplo**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

respuesta

```
{
result:"success"
}
```
