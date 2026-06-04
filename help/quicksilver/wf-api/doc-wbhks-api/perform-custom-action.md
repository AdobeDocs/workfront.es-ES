---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Realizar una acción personalizada
description: Realizar una acción personalizada
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
TQID: https://experienceleague.adobe.com/y9RxzhalPQGx0BEMOtLVOAxwyh-OhQcxuARtBrJd8Yg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 191
ht-degree: 100%

---

# Realizar una acción personalizada (aún no se ha implementado)

Este punto final permite a un usuario de Adobe Workfront (o un evento de flujo de trabajo automatizado) realizar una acción en el sistema externo. El punto final /customAction acepta un parámetro “name”, que permite al proveedor de webhook implementar varias operaciones personalizadas.

El proveedor de webhook registra las acciones personalizadas con Workfront al incluir las acciones en la respuesta /serviceInfo en customActions. Workfront carga esta lista al configurar o actualizar el proveedor de webhook en Configuración > Documentos > Integraciones personalizadas.

Los usuarios pueden activar la acción personalizada seleccionando la sección en “Acciones de documento”

**URL**

GET /customAction

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
   <td> <p>name</p> </td> 
   <td> <p>Identificador que especifica el tipo de acción que se va a realizar. Este valor corresponde a uno de los valores customAction que devuelve el punto final /serviceInfo.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>Identificador del documento de Workfront para el cual se realiza la acción.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> Identificador de versión del documento de Workfront para el cual se realiza la acción.</td> 
  </tr> 
 </tbody> 
</table>

 

## Respuesta

Una cadena JSON que indica éxito o error, tal como se especifica en la sección Gestión de errores que viene a continuación. En caso de error (es decir, estado = &quot;error&quot;), Workfront mostrará el mensaje de error proporcionado al usuario.

**Ejemplo:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

respuesta

```
{
status: "success"
}
```
