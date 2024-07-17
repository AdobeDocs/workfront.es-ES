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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 1%

---


# Obtener información sobre el servicio (aún no implementado)

>[!NOTE]
>
>La fecha de lanzamiento de esta función aún está por determinar.

Devuelve información sobre el servicio, como características y funcionalidades. Adobe Workfront utilizará esta información para personalizar la interfaz de usuario en Workfront. Por ejemplo, si la implementación del gancho web contiene algunas acciones personalizadas, el JSON debe enumerar esas operaciones en el JSON. Los usuarios podrían entonces invocar estas acciones desde Workfront.

**URL**

GET /serviceInfo

## Parámetros de consulta

Ninguna. Además, las llamadas a este extremo no deben requerir autenticación.

## Respuesta

JSON que contiene información sobre este servicio

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Tipo </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>Cadena </td> 
   <td>La versión del webhook implementada por este servicio. Este es el número de versión que aparece en la parte superior de esta especificación.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Cadena </td> 
   <td>Número de versión interno de este servicio. Este número está determinado por el proveedor de servicios de webhook y se utiliza solo con fines informativos.<br><br></td> 
  </tr> 
  <tr> 
   <td>editor </td> 
   <td>Cadena </td> 
   <td>El nombre de la empresa que proporciona la implementación del webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Cadena </td> 
   <td>Lista que contiene los puntos finales de API implementados por este servicio. Esto puede utilizarse para garantizar que la interfaz de usuario de Workfront refleje las funciones que ofrece el proveedor de ganchos web. Cada elemento de la lista debe incluir el nombre del extremo (como "búsqueda").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Cadena</td> 
   <td>  <p>Lista que contiene las operaciones personalizadas implementadas por este webhook. Cada elemento de la lista incluye un nombre y un nombre para mostrar. El nombre para mostrar aparecerá en la lista desplegable "Acciones de documento" de Workfront. Al hacer clic en el elemento de la lista desplegable, se invocará la acción en el webhook llamando al extremo /customAction.</p></td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** `https://www.acme.com/api/serviceInfo`

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
