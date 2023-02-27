---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Autenticación para Webhooks de documentos
description: Autenticación para Webhooks de documentos
author: Becky
feature: Workfront API
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Autenticación para Webhooks de documentos

## Autenticación

Los enlaces web de documentos de Adobe Workfront admiten dos formas diferentes de autenticación: OAuth2 y ApiKey. En ambos casos, Workfront pasa tokens de autenticación en el encabezado al realizar una llamada de API.

### OAuth2

OAuth2 permite a Workfront realizar llamadas de API autorizadas a un proveedor de weblock en nombre de un usuario. Antes de hacerlo, el usuario debe conectar su cuenta de proveedor de documentos externa a Workfront y conceder Workfront

acceso para actuar en su nombre. Este proceso de enlace solo ocurre una vez para cada usuario. Así funciona:

1. El usuario comienza a conectar la integración de weblock a su cuenta. Actualmente, esto se hace haciendo clic en el menú desplegable &quot;Agregar documento&quot; > &quot;Añadir servicio&quot; > Nombre de integración personalizado.
1. Workfront navega por el usuario en la dirección URL de autenticación, lo que puede pedir al usuario que inicie sesión en el proveedor de documentos externo. Esta página está alojada por el proveedor de enlaces web o el sistema externo de administración de documentos. Al hacerlo, Workfront agrega un parámetro &quot;state&quot; a la URL de autenticación. Este valor debe devolverse a Workfront anexando el mismo valor al URI de retorno de Workfront en el paso siguiente.
1. Después de iniciar sesión en el sistema externo (o si el usuario ya ha iniciado sesión), se accede al usuario a una página de &quot;autenticación&quot;, en la que se explica que Workfront solicita el acceso para realizar un conjunto de acciones en nombre del usuario.
1. Si el usuario hace clic en el botón &quot;Permitir&quot;, el explorador redireccionará al URI de redireccionamiento de Workfront y agregará &quot;code=`<code>`&quot; a la cadena de consulta. Según la especificación OAuth2, este token tiene una duración corta. La cadena de consulta también debe tener lo siguiente: &quot;state=`<sent_by_workfront>`&quot;.
1. Workfront procesa esta solicitud y realiza una llamada API a la URL del extremo del token con el código de autorización.
1. La dirección URL del extremo del token devuelve un token de actualización y un token de acceso.
1. Workfront almacena estos tokens y proporciona al usuario la integración de weblock.
1. A partir de este punto, Workfront podrá realizar llamadas de API autorizadas al proveedor de weblock. Al realizar estas llamadas, Workfront enviará el token de acceso en el encabezado de solicitud HTTP como se muestra a continuación:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Si el token de acceso ha caducado, Workfront realizará una llamada a la URL del extremo del token para recuperar un nuevo token de acceso e intentará de nuevo la llamada de API autorizada con el nuevo token de acceso.

### ApiKey

Realizar llamadas de API autorizadas a un proveedor de weblock mediante una ApiKey es mucho más sencillo que OAuth2. Al realizar una llamada de API, Workfront simplemente pasará el nombre de usuario ApiKey y Workfront en el encabezado de solicitud HTTP: 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

El proveedor de Weblock puede utilizar el nombre de usuario para aplicar permisos específicos del usuario. Esto funciona mejor cuando ambos sistemas se conectan a LDAP mediante el inicio de sesión único (SSO).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of “username:password”. See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
