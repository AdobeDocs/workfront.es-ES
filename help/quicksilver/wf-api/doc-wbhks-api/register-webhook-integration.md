---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Registro de una integración de Weblock
description: Registro de una integración de Weblock
author: Becky
feature: Workfront API
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 11%

---


# Registro de una integración de Weblock

Los administradores de Adobe Workfront pueden agregar una integración de enlace web personalizada para su empresa navegando hasta Configuración > Documentos > Integraciones personalizadas en Workfront. Desde la página Integración personalizada de Configuración, los administradores pueden ver una lista de las integraciones de Weblock del documento existente. Desde esta página, se pueden agregar, editar, habilitar y deshabilitar integraciones.

Para añadir una integración, haga clic en **Agregar integración personalizada**.

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## Campos disponibles

Al añadir una integración, el administrador introduce valores para los campos siguientes.

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
   <td> <p>La ubicación de la API de devolución de llamada. Al realizar llamadas al sistema externo, Workfront simplemente adjuntará el nombre del extremo a esta dirección. Por ejemplo, si el administrador introduce la URL de la API base, "https://www.mycompany.com/api/v1", Workfront utilizará la siguiente URL para obtener los metadatos de un documento: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
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
   <td> <p>(Solo OAuth2) La URL completa utilizada para la autenticación de usuarios. Workfront llevará a los usuarios a esta dirección como parte del proceso de aprovisionamiento de OAuth. Nota: Workfront adjuntará un parámetro "state" a la cadena de consulta. El proveedor debe devolver esto a Workfront anexándolo al URI de redirección de Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL de punto final de token</td> 
   <td> <p>(Solo OAuth2) La URL completa de la API que se usa para recuperar tokens de OAuth2. Esto lo aloja el proveedor de enlaces web o el proveedor de documentos externos</p> </td> 
  </tr> 
  <tr> 
   <td>Id. de cliente</td> 
   <td>(Solo OAuth2) El ID de cliente OAuth2 para esta integración</td> 
  </tr> 
  <tr> 
   <td>Secreto de cliente</td> 
   <td> <p>(Solo OAuth2) Secreto de cliente OAuth2 para esta integración</p> </td> 
  </tr> 
  <tr> 
   <td>URI de redireccionamiento de Workfront</td> 
   <td>(Solo OAuth2) Se trata de un campo de solo lectura que genera Workfront. Este valor se utiliza para registrar esta integración con el proveedor de documentos externo. Nota: Como se describe anteriormente para la URL de autenticación, el proveedor debe anexar el parámetro "state" y su valor a la cadena de consulta al realizar la redirección.</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>(Solo ApiKey) Se utiliza para realizar llamadas de API autorizadas al proveedor de enlaces web. La clave de API emitida por el proveedor de enlaces web.</p> </td> 
  </tr> 
 </tbody> 
</table>
