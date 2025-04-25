---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener información sobre el servicio
description: Obtener información sobre el servicio
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 80%

---


# Obtener información sobre el servicio (aún no implementado)

>[!NOTE]
>
>La fecha de lanzamiento de esta función aún está por determinar.

Devuelve información sobre el servicio, como características y funcionalidades. Adobe Workfront utilizará esta información para personalizar la interfaz de usuario en Workfront. Por ejemplo, si la implementación del webhook contiene algunas acciones personalizadas, JSON debe enumerar esas operaciones en el JSON. Los usuarios podrían entonces invocar estas acciones desde Workfront.

**URL**

GET /serviceInfo

## Parámetros de consulta

Ninguno. Además, las llamadas a este punto final no deben requerir autenticación.

## Respuesta

JSON que contiene información sobre este servicio

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Tipo</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>Cadena</td> 
   <td>La versión del webhook implementada por este servicio. Es el número de versión que aparece en la parte superior de esta especificación.</td> 
  </tr> 
  <tr> 
   <td>version</td> 
   <td>Cadena</td> 
   <td>Número de versión interno de este servicio. Este número está determinado por el proveedor de servicios de webhook y solo se utiliza con fines informativos.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher</td> 
   <td>Cadena</td> 
   <td>El nombre de la compañía que proporciona la implementación del webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Cadena</td> 
   <td>Lista que contiene los puntos finales de la API implementados por este servicio. Se puede utilizar para garantizar que la interfaz de usuario de Workfront refleje las funciones que ofrece el proveedor del webhook. Cada elemento de la lista debe incluir el nombre del punto final (como "búsqueda").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Cadena</td> 
   <td>  <p>Una lista que contiene las operaciones personalizadas implementadas por este webhook. Cada elemento de la lista incluye un nombre y un nombre para mostrar. El nombre para mostrar aparecerá en la lista desplegable “Acciones de documento” de Workfront. Al hacer clic en el elemento de la lista desplegable, se invocará la acción en el webhook llamando al punto final /customAction.</p></td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo**`https://www.acme.com/api/serviceInfo`

devoluciones

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```
