---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Registrar una integración de webhook
description: Registrar una integración de webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
TQID: https://experienceleague.adobe.com/gt9fGu286M-fya5XVuYfTMzJ0dHJT5J7f0uvctqbL0A
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 94f14afac621d7a0e41daceeb8eb7a5d2682f911
workflow-type: tm+mt
source-wordcount: 409
ht-degree: 70%

---

# Registrar una integración de webhook

{{highlighted-preview}}

Los administradores de Adobe Workfront pueden añadir una integración de webhook para su empresa navegando hasta Configuración > Documentos > Integraciones personalizadas en Workfront. Desde la página Integración personalizada dentro de Configuración, los administradores pueden ver una lista de las integraciones de webhook de documentos existentes. Desde esta página, las integraciones se pueden añadir, editar, habilitar y deshabilitar.

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
   <td> <p>Valores opcionales que se anexan a la cadena de consulta de cada llamada API. Por ejemplo, access_type=offline. </p> </td> 
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
  <tr class="preview"> 
   <td>Habilitar la carga interrumpida para archivos grandes</td> 
   <td> <p>Seleccione esta casilla de verificación para habilitar las cargas de varias partes (fragmentadas) para archivos de más de 25 MB. Cuando no se selecciona, los archivos se cargan en una sola solicitud independientemente de su tamaño.</p> </td> 
  </tr> 
  <tr class="preview"> 
   <td>Umbral de carga interrumpida (MB)</td> 
   <td> <p>El tamaño máximo, en MB, de cada fragmento cuando se divide un archivo grande para la carga. Acepta valores de hasta 100 MB.</p> </td> 
  </tr> 
 </tbody> 
</table>
