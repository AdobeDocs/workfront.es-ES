---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtener información sobre el servicio
description: Obtener información sobre el servicio
author: Becky
feature: Workfront API
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 4%

---


# Obtener información sobre el servicio (aún no implementado)

>[!NOTE]
>
>Aún no se ha determinado la fecha de lanzamiento de esta función.

Devuelve información sobre el servicio, como características y capacidades. Adobe Workfront utilizará esta información para personalizar la interfaz de usuario en Workfront. Por ejemplo, si la implementación de enlace web contiene algunas acciones personalizadas, el JSON debería enumerar esas operaciones en el JSON. Los usuarios podrían invocar estas acciones desde Workfront.

**Dirección URL**

GET /serviceInfo

## Parámetros de consulta

Ninguno. Además, las llamadas a este extremo no deben requerir autenticación.

## respuesta

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
   <td>weblockVersion </td> 
   <td>Cadena </td> 
   <td>La versión del enlace web implementada por este servicio. Este es el número de versión que aparece en la parte superior de esta especificación.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Cadena </td> 
   <td>Número de versión interna de este servicio. Este número lo determina el proveedor de servicios de enlace web y se utiliza solamente con fines informativos.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher </td> 
   <td>Cadena </td> 
   <td>Nombre de la empresa que proporciona la implementación del enlace web.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Cadena </td> 
   <td>Una lista que contiene los puntos finales de API implementados por este servicio. Esto se puede utilizar para garantizar que la interfaz de usuario en Workfront refleje las capacidades ofrecidas por el proveedor de enlaces web. Cada elemento de la lista debe incluir el nombre del extremo (como "búsqueda").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Cadena</td> 
   <td>  <p>Una lista que contiene las operaciones personalizadas implementadas por este vínculo web. Cada elemento de la lista incluye un nombre y un nombre para mostrar. El nombre para mostrar aparecerá en la lista desplegable "Acciones de documento" de Workfront. Al hacer clic en el elemento de la lista desplegable, se activará la acción en el enlace web llamando al extremo /customAction .</p></td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** `https://www.acme.com/api/serviceInfo`

return

```
{
webhook version: “1.2”, version: “1.0”, publisher: “Acme, LLC”, availableEndpoints: [“files”, “metadata”, “search”, “download”
“thumbnail”, “uploadInit”, “upload” ], customActions [
{
name: “archive”, displayName: “Archive” 
}, 
{name: “doSomethingElse”, displayName: “Do Something” }, 
] 
}
```
