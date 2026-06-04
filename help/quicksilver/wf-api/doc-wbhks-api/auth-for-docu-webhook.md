---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Autenticación para webhooks de documentos
description: Autenticación para webhooks de documentos
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
TQID: https://experienceleague.adobe.com/cRJbyPxBa-US0cV1cHsi43qvV59-AwhPgFjEhWsC1ME
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 439
ht-degree: 97%

---

# Autenticación para webhooks de documentos

## Autenticación

Los webhooks de documentos de Adobe Workfront admiten dos formas diferentes de autenticación: OAuth2 y ApiKey. En ambos casos, Workfront transfiere tokens de autenticación en el encabezado al realizar una llamada de API.

### OAuth2

OAuth2 permite a Workfront realizar llamadas de API autorizadas a un proveedor de webhooks en nombre de un usuario. Antes de hacerlo, el usuario debe conectar su cuenta de proveedor de documentos externo a Workfront y conceder a Workfront

acceso para actuar en su nombre. Este proceso de establecimiento de comunicación solo se produce una vez por cada usuario. Funciona de la siguiente manera:

1. El usuario comienza a conectar la integración del webhook a su cuenta. Actualmente, esto se lleva a cabo haciendo clic en el menú desplegable “Añadir documento” > “Añadir servicio” > Nombre de la integración personalizada.
1. Workfront dirige al usuario a la URL de autenticación, que puede pedirle que inicie sesión en el proveedor de documentos externo. Esta página está alojada por el proveedor de webhooks o por el sistema de administración de documentos externo. Al hacerlo, Workfront añade un parámetro “state”a la URL de autenticación. Este valor debe devolverse a Workfront añadiendo el mismo valor al URI de retorno de Workfront en el paso siguiente.
1. Después de iniciar sesión en el sistema externo (o si el usuario ya ha iniciado sesión), se le redirige a una página “Autenticación”, que indica que Workfront está solicitando acceso para realizar un conjunto de acciones en su nombre.
1. Si el usuario hace clic en el botón “Permitir”, el explorador redireccionará al URI de redireccionamiento de Workfront y añadirá “code=`<code>`” a la cadena de consulta. Según la especificación de OAuth2, este token es de corta duración. La cadena de consulta también debe tener lo siguiente: “state=`<sent_by_workfront>`”.
1. Workfront procesa esta solicitud y realiza una llamada de API a la URL de punto final de token con el código de autorización.
1. La URL de punto final de token devuelve un token de actualización y uno de acceso.
1. Workfront almacena estos tokens y aprovisiona completamente la integración de webhooks para este usuario.
1. A partir de este momento, Workfront podrá realizar llamadas de API autorizadas al proveedor de webhooks. Al realizar estas llamadas, Workfront enviará el token de acceso en el encabezado de petición HTTP como se muestra a continuación:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Si el token de acceso ha caducado, Workfront realizará una llamada a la URL de punto final de token para recuperar un nuevo token de acceso e intentará de nuevo la llamada a la API autorizada con el nuevo token de acceso.

### ApiKey

Realizar llamadas de API autorizadas a un proveedor de webhooks mediante una ApiKey es mucho más sencillo que mediante OAuth2. Al realizar una llamada de API, Workfront simplemente transfiere la ApiKey y el nombre de usuario de Workfront en el encabezado de la petición HTTP: 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

El proveedor de webhooks puede utilizar el nombre de usuario para aplicar permisos específicos del usuario. Esto funciona mejor cuando ambos sistemas se conectan a LDAP mediante el inicio de sesión único (SSO).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
