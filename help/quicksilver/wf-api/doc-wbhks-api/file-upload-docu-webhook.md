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
TQID: https://experienceleague.adobe.com/qLRbcWkbOxvBp5Xw1aCLjGZXHMtu2k70NgOonZsZ0lk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 266
ht-degree: 100%

---

# Carga de archivos mediante webhooks de documentos

La carga de un archivo a un proveedor de almacenamiento de documentos es un proceso de dos pasos que requiere dos puntos finales de API independientes. Adobe Workfront inicia el proceso de carga llamando a /uploadInit Este punto final devuelve un ID de documento que luego se pasa a /upload al cargar los bytes del documento. Según el sistema de almacenamiento de documentos subyacente, puede que sea necesario crear un documento de longitud cero y actualizar el contenido del documento más adelante.

Añadido a la versión 1.1 de esta especificación, el ID de documento y el ID de versión de documento se pueden utilizar para recuperar información adicional de Workfront.

**Ejemplo:** si el sistema de administración de documentos desea información adicional sobre el documento, el código de implementación del webhook podría utilizarr el ID del documento para recuperar esa información mediante la API RESTful de Workfront. Como práctica recomendada, esta información podría proceder de campos de datos personalizados del documento y contener tareas, problemas o proyectos.

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
   <td>ID de la carpeta principal, según la referencia del proveedor de webhooks.</td> 
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

## Respuesta

Los metadatos del archivo, tal como se definen en el punto final /metadata. Esto incluye el ID de documento utilizado por el proveedor.

**Ejemplo:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Método PUT

Carga los bytes de un documento en el proveedor de webhooks.

**URL**

PUT /upload

## Parámetros de consulta

| Nombre  | Descripción |
|---|---|
| id  |  El identificador documento, que se acaba de crear. |


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
