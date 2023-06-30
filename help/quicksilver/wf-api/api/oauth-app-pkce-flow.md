---
content-type: api
navigation-topic: api-navigation-topic
title: Uso del flujo PKCE para aplicaciones OAuth 2
description: Uso del flujo PKCE para aplicaciones OAuth 2
author: Becky
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo PKCE

PKCE es un flujo de autorización seguro que funciona bien con aplicaciones que se actualizan dinámicamente, como las aplicaciones móviles, pero que resulta útil en todos los clientes OAuth2. En lugar de un secreto de cliente estático, PKCE utiliza una cadena generada dinámicamente, lo que elimina el riesgo de que se filtre un secreto de cliente.

## Introducción a PKCE

Un flujo PKCE tiene los pasos siguientes. Los pasos de esta sección se presentan solo a título informativo. Para realizar estos procedimientos, consulte otras secciones de este artículo.

1. El cliente crea el `code_challenge` transformando el `code_verifier` usando `S256` cifrado.

1. El cliente dirige el explorador a la página de inicio de sesión de OAuth2, junto con el `code_challenge`. Debe registrar la aplicación (cliente) para que OAuth2 pueda aceptar la solicitud de autorización. Después del registro, la aplicación puede redirigir el explorador a OAuth2.

1. El servidor de autorización de OAuth2 redirige la solicitud de autenticación al usuario.

1. El usuario se autentica utilizando una de las opciones de inicio de sesión configuradas y puede ver una página de consentimiento en la que se enumeran los permisos que OAuth2 concederá a la aplicación.

1. OAuth2 redirige de nuevo a la aplicación con un `authorization code`.

1. La aplicación envía este código, junto con el código `code_verifier`, a OAuth2.

1. El servidor de autorización de OAuth2 transforma el `code_verifier` uso del `code_challenge_method` de la solicitud de autorización inicial, y comprueba el resultado comparándolo con el `code_challenge`. Si el valor de ambas cadenas coincide, el servidor ha comprobado que las solicitudes proceden del mismo cliente y emitirán un `access token`.

1. OAuth2 devuelve el `access token`y, opcionalmente, un `refresh token`.

1. La aplicación ahora puede utilizar estos tokens para llamar al servidor de recursos, como una API en nombre del usuario.

1. El servidor de recursos valida el token antes de responder a la solicitud.


## Configuración de la aplicación

Para poder implementar la autorización, debe registrar la aplicación en OAuth2 creando una integración de aplicaciones desde Workfront.

Para obtener instrucciones sobre la creación de la aplicación OAuth2, consulte [Creación de una aplicación web de una sola página de OAuth2 mediante PKCE](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [Creación de aplicaciones de OAuth2 para integraciones de Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## Crear la clave de revisión para el intercambio de código

De forma similar al flujo estándar del Código de autorización, la aplicación se inicia redireccionando el explorador del usuario al del Servidor de autorización `/authorize` punto final. Sin embargo, en este caso también tiene que pasar un reto de código.

El primer paso es generar un verificador de códigos y un desafío.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Verificador de códigos</td>
        <td>
          <p>Cadena URL segura aleatoria con una longitud mínima de 43 caracteres</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Desafío de código</td>
        <td>
          <p>Hash SHA-256 cifrado en URL de Base64 del verificador de códigos</p>
        </td>
      </tr>
    </tbody>
</table>


Debe agregar código en la aplicación cliente para crear el verificador de códigos y el reto de códigos.

El código del generador PKCE crea un resultado similar al siguiente:

>[!INFO]
>
>**Ejemplo:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

Su aplicación guardará `code_verifier` para más tarde, y envía el `code_challenge` junto con la solicitud de autorización al servidor de autorización `/authorize` URL.

## Solicitar un código de autorización

Si utiliza el servidor de autorización personalizado predeterminado, la dirección URL de la solicitud sería similar a la siguiente:

>[!INFO]
>
>**Ejemplo:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Tenga en cuenta los parámetros que se pasan:

* `client_id` coincide con el ID de cliente de la aplicación OAuth2 que creó en el al configurar la aplicación.

  Para obtener instrucciones, consulte Creación de una aplicación web de una sola página de OAuth2 mediante PKCE en Creación de aplicaciones de OAuth2 para integraciones de Workfront.

* `response_type` es `code`, porque la aplicación utiliza el tipo de concesión Código de autorización.

* `redirect_uri` es la ubicación de devolución de llamada a la que se dirige el agente de usuario junto con el `code`. Debe coincidir con una de las direcciones URL de redireccionamiento que especificó al crear la aplicación OAuth2.

* `code_challenge_method` es el método hash utilizado para generar el desafío, que siempre es `S256` para aplicaciones Oauth2 de Workfront que utilizan PKCE.

* `code_challenge` es el reto de código utilizado para PKCE.


## Intercambio del código por tokens

Para intercambiar el código de autorización por un token de acceso, páselo al servidor de autorización `/token` punto final junto con el `code_verifier`.

>[!INFO]
>
>**Ejemplo:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> A diferencia del flujo normal de código de autorización, esta llamada no requiere el encabezado Autorización con el ID de cliente y el secreto. Por este motivo, esta versión del flujo del código de autorización es adecuada para aplicaciones nativas como aplicaciones móviles o aplicaciones de una sola página que no tienen servidor.

Tenga en cuenta los parámetros que se pasan:

* `grant_type` es `authorization_code`, porque la aplicación utiliza el tipo de concesión Código de autorización.

* `redirect_uri` debe coincidir con el URI utilizado para obtener el código de autorización.

* `code` es el código de autorización que ha recibido del extremo /authorize.

* `code_verifier` es el verificador de código PKCE que su aplicación generó en [Crear la clave de revisión para el intercambio de código](#Create).

* `client_id` identifica a su cliente y debe coincidir con el valor preregistrado en OAuth2.


Si el código sigue siendo válido y el verificador de códigos coincide, la aplicación recibe un token de acceso.

>[!INFO]
>
>**Ejemplo:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## Validación del token de acceso

Cuando la aplicación pasa una solicitud con un token de acceso, el servidor de recursos debe validarla.

Puede validar el token de acceso con una llamada de API similar a la siguiente:

>[!INFO]
>
>**Ejemplo:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Solicitar un token de actualización

Para solicitar un token de actualización, puede realizar una llamada al POST a la API de forma similar a la siguiente:

>[!INFO]
>
>**Ejemplo:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
