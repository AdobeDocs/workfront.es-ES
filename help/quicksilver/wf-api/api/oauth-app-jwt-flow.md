---
content-type: api
navigation-topic: api-navigation-topic
title: Uso del flujo JWT para aplicaciones OAuth 2 personalizadas
description: Uso del flujo JWT para aplicaciones OAuth 2 personalizadas
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
TQID: https://experienceleague.adobe.com/uxF82lsimZlGpWRe8BEt80-9wb0rnwz7uhBHCI8nAig
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 462
ht-degree: 99%

---

# Configure y utilice las aplicaciones OAuth 2 personalizadas de la organización mediante el flujo JWT

Para integrarse con Workfront y permitir que la aplicación cliente se comunique con Workfront en nombre del usuario, debe hacer lo siguiente:

* Creación de una aplicación OAuth2
* Creación de un certificado de clave pública
* Creación de un JSON Web Token (JWT)

## Creación de una aplicación OAuth2

Para obtener instrucciones sobre cómo crear la aplicación OAuth2, consulte [Creación de una aplicación OAuth2 mediante la autenticación de servidor (flujo JWT)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) en [Creación de aplicaciones OAuth2 para integraciones de Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Puede tener hasta un total de diez aplicaciones OAuth2 a la vez.

## Creación de un certificado de clave pública

El JWT debe estar firmado y codificado en base 64 para su inclusión en la solicitud de acceso. Las bibliotecas de JWT proporcionan funciones para realizar estas tareas.

El token debe firmarse con la clave privada para un certificado de firma digital. Si lo hace, puede utilizar la clave privada de cualquier certificado asociado para firmar el JWT.

El algoritmo utilizado es RS256 (firma RSA con SHA-256). Se trata de un algoritmo asimétrico y usa un par de claves pública y privada. El proveedor de identidad tiene una clave privada (secreta) empleada para generar la firma y el consumidor del JWT obtiene una clave pública para validarla.

Para generar la clave pública, siga **una** de estas opciones.

* Abra el terminal de macOS/Linux, ejecute el siguiente comando y cargue `certificate_pub.crt` con el botón **Agregar clave pública** en la configuración de la aplicación OAuth2 en Workfront.

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Use el botón **Generar un par de claves pública y privada** en la configuración de la aplicación OAuth2 en Workfront para generar RSA.

## Creación de un token web JSON

Un token web JSON para la autenticación de cuenta de servicio requiere un conjunto particular de notificaciones y debe firmarse con un certificado de firma digital válido. Recomendamos utilizar una de las bibliotecas o herramientas disponibles de manera pública para crear el JWT.

La siguiente tabla contiene información sobre los campos que pueden ser necesarios al configurar el token JWT.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Requerido. El parámetro de caducidad es un parámetro obligatorio que mide la hora absoluta desde el 01/01/1970 GMT. Debe asegurarse de que la hora de caducidad sea posterior a la hora de emisión. Transcurrido este tiempo, el JWT deja de ser válido. </p> <p>Nota: recomendamos tener un token de corta duración (unos minutos) para que caduque poco después de cambiarlo por un token de acceso. Cada vez que se requiere un nuevo token de acceso, se firma e intercambia un JWT. Este es un enfoque más seguro. No recomendamos tókenes de mayor duración que se reutilicen para obtener tókenes de acceso según sea necesario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>necesario. El emisor es el ID de cliente de los detalles de la aplicación OAuth2.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>necesario. El asunto es el ID de usuario que creó la clave pública durante la configuración.</td> 
  </tr> 
 </tbody> 
</table>

## Intercambie el JWT para recuperar un token de acceso

1. Envíe una petición POST a:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. El cuerpo de la solicitud debe contener parámetros con codificación URL con el ID del cliente, el secreto del cliente y el JWT:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
