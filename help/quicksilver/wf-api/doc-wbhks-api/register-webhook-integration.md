---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Registro de una integración de webhook
description: Registro de una integración de webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 79%

---


# Registro de una integración de webhook

Los administradores de Adobe Workfront pueden añadir una integración de webhook para su empresa navegando hasta Configuración > Documentos > Integraciones personalizadas en Workfront. Desde la página Integración personalizada dentro de Configuración, los administradores pueden ver una lista de las integraciones de webhook de documentos existentes. Desde esta página, las integraciones se pueden añadir, editar, activar y desactivar.

Para agregar una integración, haga clic en **Agregar integración personalizada**.

![Agregar integración personalizada](assets/webhooks-integration-2-350x220.png)

## Campos disponibles

Al añadir una integración, el administrador introduce valores en los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre de campo</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nombre</td> 
   <td>Nombre de esta integración.</td> 
  </tr> 
  <tr> 
   <td>URL de API básica</td> 
   <td> <p>La ubicación de la API de devolución de llamada. Al realizar llamadas al sistema externo, Workfront simplemente anexará el nombre del punto final a esta dirección. Por ejemplo, si el administrador introduce la URL de API básica, https://www.mycompany.com/api/v1, Workfront utiliza la siguiente URL para obtener los metadatos de un documento: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Parámetros de solicitud</td> 
   <td> <p>Valores opciones que se agregarán a querystring en cada llamada API. Por ejemplo: access_type </p> </td> 
  </tr> 
  <tr> 
   <td>Tipo de autenticación</td> 
   <td>OAuth2 o ApiKey</td> 
  </tr> 
  <tr> 
   <td>URL de autenticación</td> 
   <td> <p>(Solo OAuth2) Dirección URL completa utilizada para la autenticación de usuarios. Workfront llevará a los usuarios a esta dirección como parte del proceso de aprovisionamiento de OAuth. Nota: Workfront anexará un parámetro “state” a la cadena de consulta. El proveedor debe devolverlo a Workfront anexándolo al URI de redireccionamiento de Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL de punto final de token</td> 
   <td> <p>(Solo para OAuth2) URL de API completa que sirve para recuperar tókenes de OAuth2. Esto lo aloja el proveedor de webhooks o el proveedor de documentos externo</p> </td> 
  </tr> 
  <tr> 
   <td>Id. de cliente</td> 
   <td>(Solo para OAuth2) ID de cliente OAuth2 para esta integración.</td> 
  </tr> 
  <tr> 
   <td>Secreto de cliente</td> 
   <td> <p>(Solo para OAuth2) Secreto de cliente Oauth2 para esta integración.</p> </td> 
  </tr> 
  <tr> 
   <td>URI de redireccionamiento de Workfront</td> 
   <td>(Solo OAuth2) Se trata de un campo de solo lectura que genera Workfront. Este valor se utiliza para registrar esta integración con el proveedor de documentos externo. Nota: Como se ha descrito anteriormente para la URL de autenticación, el proveedor debe anexar el parámetro “state” y su valor a la cadena de consulta al realizar la redirección.</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>(Solo ApiKey) Se utiliza para realizar llamadas de API autorizadas al proveedor de webhooks. Se trata de la clave API emitida por el proveedor de webhooks.</p> </td> 
  </tr> 
 </tbody> 
</table>
