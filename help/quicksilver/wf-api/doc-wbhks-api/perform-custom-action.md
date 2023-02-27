---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Realizar una acción personalizada
description: Realizar una acción personalizada
author: Becky
feature: Workfront API
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 3%

---


# Realizar una acción personalizada (aún no implementada)

Este extremo permite a un usuario de Adobe Workfront (o un evento de flujo de trabajo automatizado) realizar una acción en el sistema externo. El extremo /customAction acepta un parámetro &quot;name&quot;, que permite al proveedor de enlaces web implementar varias operaciones personalizadas.

El proveedor de vínculos web registra las acciones personalizadas con Workfront al incluir las acciones en la respuesta /serviceInfo en customActions. Workfront carga esta lista al configurar o actualizar el proveedor de vínculos web en Configuración > Documentos > Integraciones personalizadas.

Los usuarios pueden almacenar en déclencheur la acción personalizada seleccionando la sección en &quot;Acciones de documento&quot;

**Dirección URL**

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
   <td> <p>Identificador que especifica el tipo de acción que se va a realizar. Este valor corresponde a uno de los valores customAction enumerados que devuelve el extremo /serviceInfo .</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>ID del documento de área de trabajo para el que se está realizando la acción.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> El ID de versión del documento de área de trabajo para el que se está realizando la acción.</td> 
  </tr> 
 </tbody> 
</table>

 

## respuesta

Una cadena JSON que indica que se ha realizado correctamente o que se ha producido un error, tal como se especifica en la sección Error Handling a continuación. En caso de error (por ejemplo, estado = &quot;error&quot;), Workfront mostrará al usuario el mensaje de error proporcionado.

**Ejemplo:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

response

```
{
status: “success”
}
```
