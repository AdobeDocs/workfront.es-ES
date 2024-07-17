---
content-type: api
navigation-topic: api-navigation-topic
title: Uso del flujo JWT para aplicaciones OAuth 2 personalizadas
description: Uso del flujo JWT para aplicaciones OAuth 2 personalizadas
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo JWT

Para integrarse con Workfront y permitir que la aplicación cliente se comunique con Workfront en nombre del usuario, debe:

* Creación de una aplicación OAuth2
* Crear un certificado de clave pública
* Creación de un token web JSON (JWT)

## Crear una aplicación OAuth2

Para obtener instrucciones sobre cómo crear la aplicación OAuth2, consulte [Crear una aplicación OAuth2 mediante la autenticación de servidor (flujo JWT)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) en [Crear aplicaciones OAuth2 para integraciones de Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Puede tener hasta un total de diez aplicaciones OAuth2 a la vez.

## Crear un certificado de clave pública

El JWT debe estar firmado y codificado en base 64 para su inclusión en la solicitud de acceso. Las bibliotecas JWT proporcionan funciones para realizar estas tareas.

El token debe firmarse con la clave privada para un certificado de firma digital. Si lo hace, puede utilizar la clave privada de cualquier certificado asociado para firmar el JWT.

El algoritmo utilizado es RS256 (firma RSA con SHA-256). Se trata de un algoritmo asimétrico y utiliza un par de claves pública y privada. El proveedor de identidad tiene una clave privada (secreta) utilizada para generar la firma y el consumidor del JWT obtiene una clave pública para validar la firma.

Para generar la clave pública, siga **uno** de estos pasos.

* Abra el terminal de MacOS/Linux, ejecute el siguiente comando y cargue `certificate_pub.crt` con el botón **Agregar clave pública** en la configuración de la aplicación OAuth2 en Workfront.

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Use el botón **Generar un par de claves pública y privada** en la configuración de la aplicación OAuth2 en Workfront para generar RSA.

## Creación de un token web JSON

Un token web JSON para la autenticación de cuenta de servicio requiere un conjunto particular de notificaciones y debe firmarse con un certificado de firma digital válido. Le recomendamos que utilice una de las bibliotecas o herramientas disponibles públicamente para crear su JWT.

La siguiente tabla contiene información sobre los campos que pueden ser necesarios al configurar el token JWT.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Requerido. El parámetro de caducidad es un parámetro obligatorio que mide la hora absoluta desde el 01/01/1970 GMT. Debe asegurarse de que la hora de caducidad sea posterior a la hora de emisión. Transcurrido este tiempo, el JWT deja de ser válido. </p> <p>Nota: Le recomendamos que tenga un token de corta duración (unos minutos), para que caduque poco después de cambiarlo por un token de acceso. Cada vez que se requiere un nuevo token de acceso, se firma e intercambia un JWT. Este es un enfoque más seguro. No recomendamos tokens de mayor duración que se reutilicen para obtener tokens de acceso según sea necesario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">is</td> 
   <td>Requerido. El emisor es su ID de cliente de los detalles de la aplicación OAuth2.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Requerido. El asunto es el ID de usuario que creó la clave pública durante la configuración.</td> 
  </tr> 
 </tbody> 
</table>

## Intercambie el JWT para recuperar un token de acceso

1. Envíe una solicitud de POST a:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. El cuerpo de la solicitud debe contener parámetros con codificación URL con el ID del cliente, el secreto del cliente y JWT:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
