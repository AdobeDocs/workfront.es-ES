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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 4%

---


# Realizar una acción personalizada (aún no implementada)

Este punto de conexión permite a un usuario de Adobe Workfront (o un evento de flujo de trabajo automatizado) realizar una acción en el sistema externo. El extremo /customAction acepta un parámetro &quot;name&quot;, que permite al proveedor de ganchos web implementar varias operaciones personalizadas.

El proveedor de ganchos web registra las acciones personalizadas con Workfront al incluir las acciones en la respuesta /serviceInfo en customActions. Workfront carga esta lista al configurar o actualizar el proveedor de ganchos web en Configuración > Documentos > Integraciones personalizadas.

Los usuarios pueden almacenar en déclencheur la acción personalizada seleccionando la sección en &quot;Acciones de documento&quot;

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
   <td> <p>Identificador que especifica el tipo de acción que se va a realizar. Este valor corresponde a uno de los valores customAction que devuelve el extremo /serviceInfo.</p> </td> 
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

 

## respuesta

Una cadena JSON que indica éxito o error, como se especifica en la sección Gestión de errores a continuación. En caso de error (es decir, estado = &quot;error&quot;), Workfront mostrará el mensaje de error proporcionado al usuario.

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
