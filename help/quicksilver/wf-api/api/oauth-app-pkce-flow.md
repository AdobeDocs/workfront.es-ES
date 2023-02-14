---
content-type: api
navigation-topic: api-navigation-topic
title: Uso del flujo PKCE para aplicaciones OAuth 2
description: Uso del flujo PKCE para aplicaciones OAuth 2
author: John
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 03df0ad329255e86780c03bbb4541e0a0a526381
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo PKCE

PKCE es un flujo de autorización seguro que funciona bien con aplicaciones que se actualizan dinámicamente, como aplicaciones móviles, pero que es valioso en todos los clientes de OAuth2. En lugar de un secreto de cliente estático, PKCE utiliza una cadena generada dinámicamente, eliminando el riesgo de que se filtre un secreto de cliente.

## Información general de PKCE

Un flujo PKCE tiene los siguientes pasos. Los pasos de esta sección se presentan solo para obtener información. Para realizar estos procedimientos, consulte otras secciones de este artículo.

1. El cliente crea la variable `code_challenge` transformando la variable `code_verifier` using `S256` cifrado.

1. El cliente dirige el explorador a la página de inicio de sesión de OAuth2, junto con el `code_challenge`. Debe registrar la aplicación (cliente) para que OAuth2 pueda aceptar la solicitud de autorización. Después del registro, la aplicación puede redirigir el navegador a OAuth2.

1. El servidor de autorización OAuth2 redirige el mensaje de autenticación al usuario.

1. El usuario se autentica mediante una de las opciones de inicio de sesión configuradas y puede ver una página de consentimiento que enumera los permisos que OAuth2 otorga a la aplicación.

1. OAuth2 redirige de nuevo a su aplicación con un `authorization code`.

1. La aplicación envía este código junto con la variable `code_verifier`, a OAuth2.

1. El servidor de autorización de OAuth2 transforma el `code_verifier` usando la variable `code_challenge_method` de la solicitud de autorización inicial, y comprueba el resultado en relación con el `code_challenge`. Si el valor de ambas cadenas coincide, el servidor ha verificado que las solicitudes provenían del mismo cliente y emitirá un `access token`.

1. OAuth2 devuelve la variable `access token`y opcionalmente a `refresh token`.

1. La aplicación ahora puede utilizar estos tokens para llamar al servidor de recursos como una API en nombre del usuario.

1. El servidor de recursos valida el token antes de responder a la solicitud.


## Configurar la aplicación

Para poder implementar la autorización, debe registrar la aplicación en OAuth2 creando una integración de aplicación desde Workfront.

Para obtener instrucciones sobre la creación de la aplicación OAuth2, consulte [Creación de una aplicación web de una sola página de OAuth2 mediante PKCE ](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) en [Creación de aplicaciones OAuth2 para integraciones de Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## Creación de la clave de prueba para el intercambio de código

Al igual que el flujo de código de autorización estándar, la aplicación se inicia redireccionando el explorador del usuario al del servidor de autorización `/authorize` punto final. Sin embargo, en este caso también tiene que pasar un desafío de código.

El primer paso es generar un verificador de código y un desafío.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Verificador de código</td>
        <td>
          <p>Cadena aleatoria segura para URL con una longitud mínima de 43 caracteres</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Desafío del código</td>
        <td>
          <p>hash SHA-256 con codificación de URL base64 del verificador de código</p>
        </td>
      </tr>
    </tbody>
</table>


Debe añadir código en la aplicación de cliente para crear el verificador de código y el desafío de código.

El código del generador PKCE crea una salida similar a la siguiente:

>[!INFO]
>
>**Ejemplo:**
>
>```
>{
>
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>
>}
>```

La aplicación guarda los `code_verifier` para más adelante, y envía la variable `code_challenge` junto con la solicitud de autorización a la `/authorize` URL.

## Solicitar un código de autorización

Si utiliza el servidor de autorización personalizado predeterminado, la dirección URL de solicitud sería similar a la siguiente:

>[!INFO]
>
>**Ejemplo:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Tenga en cuenta los parámetros que se están pasando:

* `client_id` coincide con el ID de cliente de la aplicación OAuth2 que creó en al configurar la aplicación.

   Para obtener instrucciones, consulte Creación de una aplicación web de una sola página de OAuth2 utilizando PKCE en Creación de aplicaciones OAuth2 para integraciones de Workfront.

* `response_type` es `code`, ya que la aplicación utiliza el tipo de concesión Código de autorización .

* `redirect_uri` es la ubicación de rellamada a la que se dirige el agente de usuario junto con la variable `code`. Debe coincidir con una de las direcciones URL de redireccionamiento que especificó al crear la aplicación OAuth2.

* `code_challenge_method` es el método hash utilizado para generar el desafío, que siempre es `S256` para aplicaciones Workfront Oauth2 que utilizan PKCE.

* `code_challenge` es el desafío de código utilizado para PKCE.


## Intercambiar el código para tokens

Para intercambiar el código de autorización de un token de acceso, páselo al servidor de autorización `/token` junto con la variable `code_verifier`.

>[!INFO]
>
>**Ejemplo:**
>
>```
>/token \\
>
>  --header 'accept: application/json' \\
>
>  --header 'cache-control: no-cache' \\
>
>  --header 'content-type: application/x-www-form-urlencoded' \\
>
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> A diferencia del flujo regular de código de autorización, esta llamada no requiere el encabezado Autorización con el ID de cliente y el secreto. Por este motivo, esta versión del flujo del código de autorización es apropiada para aplicaciones nativas como aplicaciones móviles o aplicaciones de una sola página que no tienen un servidor.

Tenga en cuenta los parámetros que se están pasando:

* `grant_type` es `authorization_code`, ya que la aplicación utiliza el tipo de concesión Código de autorización .

* `redirect_uri` debe coincidir con el URI utilizado para obtener el código de autorización.

* `code` es el código de autorización que recibió del extremo /authorization .

* `code_verifier` es el verificador de código PKCE en el que la aplicación ha generado [Creación de la clave de prueba para el intercambio de código](#Create).

* `client_id` identifica al cliente y debe coincidir con el valor preregistrado en OAuth2.


Si el código sigue siendo válido y el verificador de código coincide, la aplicación recibe un token de acceso.

>[!INFO]
>
>**Ejemplo:**
>
>```
>{
>
>    "access\_token": "eyJhd\[...\]Yozv",
>
>    "expires\_in": 3600,
>
>    "token\_type": "Bearer"
>
>}
>```

## Validación del token de acceso

Cuando la aplicación pasa una solicitud con un token de acceso, el servidor de recursos debe validarla.

Puede validar el token de acceso con una llamada a la API similar a la siguiente:

>[!INFO]
>
>**Ejemplo:**
>
>```
>/attask/api/<api version>/proj/search \\
>
>  --header 'sessionID: <access\_token>' \\
>```

## Solicitar un token de actualización

Para solicitar un token de actualización, puede realizar una llamada de POST a la API, similar a la siguiente:

>[!INFO]
>
>**Ejemplo:**
>
>```
>/token \\
>
>  --header 'accept: application/json' \\
>
>  --header 'cache-control: no-cache' \\
>
>  --header 'content-type: application/x-www-form-urlencoded' \\
>
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
