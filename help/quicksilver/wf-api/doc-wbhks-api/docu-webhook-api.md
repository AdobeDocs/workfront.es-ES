---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: API de webhooks de documentos
description: API de webhooks de documentos
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '3627'
ht-degree: 99%

---


# API de webhooks de documentos

Adobe Workfront Document Webhooks define un conjunto de puntos finales de API a través de los cuales Workfront realiza llamadas de API autorizadas a un proveedor de documentos externo. Esto permite a cualquier usuario crear un complemento de middleware para cualquier proveedor de almacenamiento de documentos.

La experiencia del usuario para integraciones basadas en webhooks será similar a la de integraciones de documentos existentes, como Google Drive, Box y Dropbox. Por ejemplo, un usuario de Workfront podrá realizar las siguientes acciones:

* Navegar por la estructura de carpetas del proveedor de documentos externo
* Buscar archivos
* Vincular archivos a Workfront
* Cargar archivos al proveedor de documentos externo
* Ver una miniatura del documento

## Implementación de referencia

Para ayudar a impulsar el desarrollo de una nueva implementación de webhooks, Workfront proporciona una implementación de referencia. El código para ello se encuentra en [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Esta implementación está basada en Java y permite a Workfront conectar documentos en un sistema de archivos de red.

## Registrar una integración de webhook

Los administradores de Workfront pueden añadir una integración de webhook para su compañía navegando hasta Configuración > Documentos > Integraciones personalizadas en Workfront. Desde la página Integración personalizada dentro de Configuración, los administradores pueden ver una lista de las integraciones de webhook de documentos existentes. Desde esta página, las integraciones se pueden añadir, editar, habilitar y deshabilitar. Para añadir una integración, haga clic en el botón “Añadir integración”.

### Campos disponibles

Al añadir una integración, el administrador introduce valores para los campos siguientes:

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
   <td> <p>Valores opciones que se agregarán a querystring en cada llamada API. Por ejemplo: access_type</p> <p> </p> </td> 
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
   <td> <p>(Solo para OAuth2) URL de API completa que sirve para recuperar tókenes de OAuth2. Esto lo aloja el proveedor de webhooks o el proveedor de documentos externo</p> <p> </p> </td> 
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
   <td>  <p>(Solo OAuth2) Se trata de un campo de solo lectura que genera Workfront. Este valor se utiliza para registrar esta integración con el proveedor de documentos externo. Nota: Como se ha descrito anteriormente para la URL de autenticación, el proveedor debe anexar el parámetro “state” y su valor a la cadena de consulta al realizar la redirección.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(Solo ApiKey) Se utiliza para realizar llamadas de API autorizadas al proveedor de webhooks. Se trata de la clave API emitida por el proveedor de webhooks.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Autenticación

Los webhooks de documentos de Workfront admiten dos formas diferentes de autenticación: OAuth2 y ApiKey. En ambos casos, Workfront transfiere tokens de autenticación en el encabezado al realizar una llamada de API.

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

### Añadir encabezados de solicitud (opcional)

Además de utilizar tokens de OAuth2 o una ApiKey para la autenticación, Workfront puede enviar un conjunto predefinido de encabezados al proveedor de webhooks para cada llamada de API. Una persona con la función de administrador de Workfront puede configurarlo al registrar o editar una integración de webhook, tal como se describe en la sección anterior. Consulte Registro de una integración de webhook.

Por ejemplo, esto se puede utilizar para la autenticación básica. Para ello, la persona con la función de administrador de Workfront añadiría la siguiente información de encabezado de solicitud en el diálogo Integración personalizada:

   Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==

en que QWxhZGRpbjpvcGVuIHNlc2FtZQ== es una cadena codificada en base 64 de “username:password”. Consulte Autenticación básica. Siempre que se añada, Workfront lo transferirá en el encabezado de petición HTTP, además de en otros encabezados de solicitud:

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## Especificación de API

A continuación se muestra una lista de las API que el proveedor de webhooks debe implementar para que los webhooks de documentos funcionen.

### Obtención de tokens de OAuth2 (solo se necesita autenticación de OAuth2)

Devuelve el token de actualización de OAuth2 y el token de acceso de un usuario autenticado. Se invoca una vez cuando el usuario aprovisiona un proveedor de documentos. Se realizan llamadas posteriores para obtener un token de acceso actualizado.

POST de solicitudes HTTP /any/url

La dirección URL es configurable y corresponde al valor URL del punto final de token en la página Configuración de integración personalizada.

**Parámetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Requerido</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>sí</td> 
   <td> <p>Los valores incluyen “authorization_code” o “refresh_token”. El valor especificado indica cuál de los dos parámetros se pasará a esta llamada de API: code o refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>code</td> 
   <td>depende</td> 
   <td> <p>El código de autorización se envía a Workfront justo después de que el usuario haga clic en el botón Conceder. Solo es necesario cuando el tipo de concesión es “authorization_code”. El código de autorización debe ser de corta duración y normalmente caduca en 10 minutos o menos.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>depende</td> 
   <td> <p>Solo es necesario cuando se realizan llamadas subsiguientes para recuperar un nuevo access_token, dado que el access_token anterior ha caducado. Al enviar este valor, establezca el parámetro grant_type en "refresh_token".</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>sí</td> 
   <td>El ID de cliente configurado en Workfront para esta integración personalizada.</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>sí</td> 
   <td> El secreto de cliente configurado en Workfront para esta integración personalizada.</td> 
  </tr> 
 </tbody> 
</table>

 

**Respuesta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Tipo</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>Cadena</td> 
   <td> <p>Un token utilizado para hacer llamadas de API autorizadas en nombre del usuario. Debería caducar para evitar llamadas de API no autorizadas.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>Cadena</td> 
   <td> <p>Un token de larga duración que se utiliza para recuperar un nuevo access_token llamando a este método de API.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>(opcional) El tiempo (en segundos) antes de que access_token caduque, por lo general, 3.600.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Ejemplo**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```


**Respuesta**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### Obtener metadatos para archivo o carpeta

Devuelve los metadatos del archivo o la carpeta especificados.

**URL**

GET /metadata?id=[ID de documento o carpeta]

**Parámetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>El ID del archivo o la carpeta, tal como le hace referencia el proveedor del webhook. Es diferente al ID del documento de Workfront. Para obtener los metadatos del directorio raíz, utilice el valor "/".</p><p>Nota: La longitud máxima del ID es de 255 caracteres.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Respuesta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Tipo</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>Cadena</td> 
   <td>El nombre del documento o la carpeta</td> 
  </tr> 
  <tr> 
   <td>kind </td> 
   <td>Cadena</td> 
   <td>Especifica si este elemento es un archivo o una carpeta (“archivo” o “carpeta”)</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Cadena</td> 
   <td>El ID del archivo o carpeta.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Cadena</td> 
   <td> <p>La ruta URL utilizada por un usuario para ver el documento en una ventana del explorador. La URL puede alojarla el proveedor de documentos o el proveedor de almacenamiento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Cadena</td> 
   <td> <p>La ruta de URL utilizada por un usuario para descargar el documento en una ventana del explorador. La URL puede alojarla el proveedor de documentos o el proveedor de almacenamiento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Cadena</td> 
   <td>El tipo MIME del archivo. (opcional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Cadena</td> 
   <td>Última vez que se modificó este archivo (marca de tiempo RFC 3339 con formato)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Largo</td> 
   <td>  El tamaño del archivo en bytes. (opcional)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booleano</td> 
   <td>  <p> Indica si este archivo o carpeta es de solo lectura para el usuario autenticado.(opcional)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo**`https://www.acme.com/api/metadata?id=12345`

**Respuesta**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>La gestión de errores debe ser coherente en todas las llamadas a la API. Consulte la sección “Gestión de errores” más abajo para obtener más información.

### Obtener una lista de elementos de una carpeta

Devuelve los metadatos de los archivos y carpetas de una carpeta determinada.

**URL**

GET /files

**Parámetros de consulta**

| Nombre | Descripción |
|---|---|
| parentId  | El ID de la carpeta. Para obtener los metadatos del directorio raíz, utilice el valor &quot;/&quot;. |

{style="table-layout:auto"}

Actualmente, la API de webhooks de documentos no admite la paginación.

**Respuesta**

JSON que contiene una lista de archivos y carpetas. Los metadatos de cada elemento son los mismos que los devueltos por el/punto final de los metadatos.

**Ejemplo:** `https://www.acme.com/api/files?parentId=123456`

**Respuesta**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### Realizar una búsqueda

Devuelve metadatos de los archivos y carpetas devueltos por una búsqueda. Esto se puede implementar como una búsqueda de texto completo o como una consulta de base de datos normal. Workfront llama al punto final /search cuando el usuario realiza una búsqueda desde el explorador de archivos externo.

**URL**

GET /search

**Parámetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>query</td> 
   <td>El término o frase de búsqueda.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(opcional) ID de carpeta desde el que se ejecutó la búsqueda. Nota: Este es un marcador de posición para una función futura de Workfront. Actualmente, Workfront no pasa este parámetro. </p> </td> 
  </tr> 
  </tbody> 
</table>

Actualmente, la API de webhooks de documentos no admite la paginación.

 

**Respuesta**

JSON que contiene una lista de metadatos para archivos y carpetas que coinciden con la consulta. Lo que constituye una “coincidencia” lo determina el proveedor del webhook Lo ideal es que realice una búsqueda de texto completo. También funciona la búsqueda basada en nombres de archivo.

**Ejemplo:** `https://www.acme.com/api/search?query=test-query`

**Respuesta**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### Obtener el contenido de un documento

Devuelve los bytes sin procesar de un documento

**URL**

GET /download

**Parámetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td>El identificador del documento.</td> 
  </tr> 
 </tbody> 
</table>

 

**Respuesta**

Los bytes sin procesar del documento.

**Ejemplo:** `https://www.acme.com/api/download?id=123456`

### Obtener una miniatura de un documento

Devuelve los bytes de la miniatura sin procesar de un documento.

**URL**

GET /thumbnail

**Parámetros de consulta**

| Nombre | Descripción |
|---|---|
| id | El identificador del documento. |
| size | El ancho de la miniatura |

{style="table-layout:auto"}

 

**Respuesta**

Los bytes de la miniatura sin procesar.

**Ejemplo** `https://www.acme.com/api/thumbnail?id=123456`

### Cargar un archivo: parte 1 de 2

La carga de un archivo a un proveedor de almacenamiento de documentos es un proceso de dos pasos que requiere dos puntos finales de API independientes. Workfront inicia el proceso de carga llamando a /uploadInit Este punto final devuelve un ID de documento que luego se pasa a /upload al cargar los bytes del documento. Según el sistema de almacenamiento de documentos subyacente, puede ser necesario crear un documento de longitud cero y actualizar el contenido del documento más adelante.

Añadido a la versión 1.1 de esta especificación, el ID de documento y el ID de versión de documento se pueden utilizar para recuperar información adicional de Workfront. Por ejemplo, si el sistema de administración de documentos desea información adicional sobre el documento, el código de implementación del webhook podría utilizar el ID del documento para recuperar esa información mediante la API RESTful de Workfront. Como práctica recomendada, esta información podría proceder de campos de datos personalizados del documento y contener tareas, problemas o proyectos.

**URL**

POST /uploadInit

**Parámetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>ID de la carpeta principal, según la referencia del proveedor de webhooks.</td> 
  </tr> 
  <tr> 
   <td>filename</td> 
   <td>El nombre del documento</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>El ID del documento de Workfront (añadido en la versión 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>El ID de la versión del documento de Workfront (añadido en la versión 1.1)</td> 
  </tr> 
 </tbody> 
</table>

 

**Respuesta**

Los metadatos del archivo, tal como se definen en el punto final /metadata.

**Ejemplo:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Respuesta**

`[file_metadata]` incluye el nuevo identificador de documento utilizado por el proveedor de documentos.

### Cargar un archivo: parte 2 de 2

Carga los bytes de un documento en el proveedor de webhooks.

 **URL**

PUT /upload

**Parámetros de consulta**

| Nombre | Descripción |
|---|---|
| id | El identificador documento, que se acaba de crear. |


 

**Cuerpo de solicitud**

Los bytes de contenido sin procesar del documento.

**Respuesta**

```
{
"result": "success"
}
```

o

```
{
"result": "fail"
}
```

**Ejemplo:** `https://www.acme.com/api/upload?id=1234` *[bytes de documento incluidos en el flujo de actualización]*

**Respuesta**

```
{
"result":"success"
}
```

### Obtener información sobre el servicio 

(Fecha de publicación: por determinar) Devuelve información sobre el servicio, como las características y funcionalidades. Workfront utilizará esta información para personalizar la interfaz de usuario en Workfront. Por ejemplo, si la implementación del webhook contiene algunas acciones personalizadas, JSON debe enumerar esas operaciones en el JSON. Los usuarios podrían entonces invocar estas acciones desde Workfront.

**URL**

GET /serviceInfo

Parámetros de consulta

Ninguno. Además, las llamadas a este punto final no deben requerir autenticación.

**Respuesta**

JSON que contiene información sobre este servicio

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Tipo</th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>Cadena</td> 
   <td>La versión del webhook implementada por este servicio. Es el número de versión que aparece en la parte superior de esta especificación.</td> 
  </tr> 
  <tr> 
   <td>version</td> 
   <td>Cadena</td> 
   <td>Número de versión interno de este servicio. Este número está determinado por el proveedor de servicios de webhook y solo se utiliza con fines informativos.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher</td> 
   <td>Cadena</td> 
   <td>El nombre de la compañía que proporciona la implementación del webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Cadena</td> 
   <td>Lista que contiene los puntos finales de la API implementados por este servicio. Se puede utilizar para garantizar que la interfaz de usuario de Workfront refleje las funciones que ofrece el proveedor del webhook. Cada elemento de la lista debe incluir el nombre del punto final (como "búsqueda").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Cadena</td> 
   <td>  <p>Una lista que contiene las operaciones personalizadas implementadas por este webhook. Cada elemento de la lista incluye un nombre y un nombre para mostrar. El nombre para mostrar aparecerá en la lista desplegable “Acciones de documento” de Workfront. Al hacer clic en el elemento de la lista desplegable, se invocará la acción en el webhook llamando al punto final /customAction.</p></td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** https://www.acme.com/api/serviceInfo

**Devuelve**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### Crear una carpeta

(Añadido en la versión 1.2) Crea una carpeta en un directorio determinado.
URL

POST /createFolder

**Parámetros de consulta**

| Nombre | Descripción |
|---|---|
| parentId  | ID de la carpeta en la que debe crearse la carpeta |
| name | Nombre de la nueva carpeta |

{style="table-layout:auto"}

 

**Respuesta**

Los metadatos de la carpeta recién creada, tal como se definen en el punto final /metadata.

**Ejemplo**`POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

devoluciones

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### Eliminar un documento o una carpeta

(Fecha de lanzamiento: por determinar) Elimina un documento o una carpeta con el ID proporcionado en el sistema externo. Al eliminar una carpeta, también se elimina su contenido.

URL

PUT /delete

**Parámetros de consulta**

| Nombre | Descripción |
|---|---|
| documentId  | El identificador de documento que se va a eliminar |
| folderId  | El identificador de carpeta que se va a eliminar |

{style="table-layout:auto"}

Cadena de respuesta A JSON que indica éxito o error, como se especifica a continuación en la sección Gestión de errores.

**Ejemplo:** PUT https://www.acme.com/api/delete id=1234

devoluciones

```
{
"status": "success" 
}
```

devoluciones

```
{
"status": "failure", "error": "File not found"
}
```


### Cambiar el nombre de un documento o carpeta

(Fecha de lanzamiento: por determinar) Cambia el nombre de un documento o una carpeta con el ID proporcionado en el sistema externo.

URL

PUT /rename

**Parámetros de consulta**

| Nombre | Descripción |
|---|---|
| id | El identificador de documento o carpeta cuyo nombre se va a cambiar |
| name | El nuevo nombre del documento o la carpeta |

{style="table-layout:auto"}

 

Respuesta

Una cadena JSON que indica éxito o error, tal como se especifica en la sección Gestión de errores que viene a continuación.

**Ejemplo:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### Realizar una acción personalizada

(Fecha de publicación: por determinar) Este punto final permite a un usuario de Workfront (o quizás un evento de flujo de trabajo automatizado) realizar una acción en el sistema externo. El punto final /customAction acepta un parámetro “name”, que permite al proveedor de webhook implementar varias operaciones personalizadas.

El proveedor de webhook registra las acciones personalizadas con Workfront al incluir las acciones en la respuesta /serviceInfo en customActions. Workfront carga esta lista al configurar o actualizar el proveedor de webhook en Configuración > Documentos > Integraciones personalizadas.\
![Realizar una acción personalizada](assets/mceclip0-350x262.png)

Los usuarios pueden activar la acción personalizada seleccionando la sección en “Acciones de documento”\
![acciones personalizadas de Déclencheur](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**Parámetros de consulta**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>Nombre</th>
   <th>Descripción</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>Identificador que especifica el tipo de acción que se va a realizar. Este valor corresponde a uno de los valores customAction que devuelve el punto final /serviceInfo.</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>Identificador del documento de Workfront para el cual se realiza la acción.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td>Identificador de versión del documento de Workfront para el cual se realiza la acción.</td>
  </tr>
 </tbody>
</table>

 

**Respuesta**

Una cadena JSON que indica éxito o error, tal como se especifica en la sección Gestión de errores que viene a continuación. En caso de error (es decir, estado = &quot;error&quot;), Workfront mostrará el mensaje de error proporcionado al usuario.

**Ejemplo:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

respuesta

```
{
"status": "success" 
}
```


## Gestión de errores

Pueden surgir problemas a la hora de procesar solicitudes de API. Esto debe gestionarse de forma coherente en todos los puntos finales de la API. Cuando se produce un error, el proveedor del webhook hace lo siguiente:

* Incluye un código de error en el encabezado de la respuesta. Los códigos de error incluyen los siguientes:

   * 403 - Prohibido. Indica que faltan los tókenes de solicitud o que no son válidos, o bien que las credenciales asociadas con los tókenes no tienen acceso al recurso especificado. Para los proveedores de webhook basados en OAuth, Workfront intentará recuperar nuevos tokens de acceso.
   * 404 - No se encuentra. Indica que el archivo o la carpeta especificados no existen.
   * 500 - Error de servidor interno. Cualquier otro tipo de error.

* Describe el error en el cuerpo de la respuesta con el siguiente formato:


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Pruebas

Para comprobar que la implementación del webhook de documentos funciona correctamente, ejecute las siguientes pruebas. Son pruebas manuales que pasan por la interfaz web de Workfront e indirectamente llegan a los puntos finales de la implementación del webhook.

### Requisitos previos

Para ejecutar estas pruebas, necesitará lo siguiente:

* Una cuenta de Workfront con la administración avanzada de documentos (ADM) habilitada
* Un usuario de Workfront para esta cuenta con derechos de administrador del sistema
* Una instancia de Document Webhook, a cuyos puntos finales HTTP puede acceder Workfront

Estas pruebas también presuponen que ya se ha registrado la instancia de webhook de documentos en Workfront, en Configuración > Documentos > Integraciones personalizadas.

### Prueba 1: Aprovisionar el servicio de webhook de documentos para un usuario

Comprueba la URL de autenticación y la URL del punto final del token para proveedores de webhook basados en OAuth.

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Haga clic en el menú desplegable Añadir documentos y seleccione el servicio de webhook de documentos en Añadir servicio.
1. (Solo servicios de OAuth) Después de completar el paso anterior, verá cómo se carga la página de autenticación OAuth2 del servicio en una ventana emergente. (Nota: es posible que se le pida que inicie sesión en su servicio primero). En la página de autenticación, conceda acceso a Workfront a la cuenta del usuario haciendo clic en el botón Confiar o Permitir.
1. Verifique que el servicio se haya añadido a la lista desplegable Añadir documentos. Si no lo ve al principio, intente actualizar el explorador.

### Prueba 2: Vincular un documento en Workfront prueba los siguientes puntos finales: /files, /metadata

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio de webhook de documentos en Añadir documentos.
1. En el modal, navegue por la estructura de carpetas.
1. Verifique que puede desplazarse correctamente por la estructura de carpetas.
1. Seleccionar y vincular un documento a Workfront

### Prueba 3: Desplazarse hasta un documento en el sistema de administración de contenido

Comprueba los siguientes puntos finales: /metadata (específicamente viewLink)

1. Vincular un documento a Workfront
1. Seleccione el documento y haga clic en el vínculo Abrir.
1. Compruebe que el documento se abra en una nueva pestaña.

### Prueba 4: Desplazarse hasta un documento en el sistema de administración de contenido (con inicio de sesión)

Comprueba los siguientes puntos finales: /metadata (específicamente viewLink)

1. Asegúrese de haber cerrado la sesión del sistema de administración de contenido.
1. Vincule un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Abrir.
1. Compruebe que la pantalla de inicio de sesión del sistema de administración de contenido se cargue en una nueva pestaña.
1. Inicie sesión y compruebe que haya accedido al documento

### Prueba 5: Descargar el documento desde el sistema de administración de contenido

Prueba los siguientes puntos finales: /metadata (específicamente el downloadLink)

1. Vincule un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Descargar.
1. Compruebe que se inicie la descarga.

### Prueba 6: Buscar contenido

Comprueba los siguientes puntos finales: /search

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio de webhook de documentos en Añadir documentos.
1. En el modal, realice una búsqueda.
1. Compruebe que los resultados de la búsqueda sean correctos.

### Prueba 7: Enviar documento desde Workfront al sistema de administración de contenido

Comprueba los siguientes puntos finales: /files, /uploadInit, /upload

1. En Workfront, vaya a la página principal de Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Cargar un documento a Workfront desde el equipo
1. Vaya a la página de detalles del documento
1. En el menú desplegable Acciones del documento, seleccione el servicio de webhook de documentos en Enviar a…
1. Vaya a la carpeta de destino deseada y haga clic en el botón Guardar.
1. Compruebe que el documento se haya cargado en la ubicación correcta del sistema de administración de contenido.

### Prueba 8: Ver miniaturas en Workfront

Comprueba los siguientes puntos finales: /thumbnail

1. Vincule un documento a Workfront.
1. Seleccione el documento en la lista.
1. Compruebe que la miniatura aparezca en el panel derecho.

### Prueba 9: obtener los bytes de contenido

Comprueba los siguientes puntos finales: /download

1. Vincule un documento a Workfront.
1. Vaya a la página de detalles del documento.
1. Envíe el documento a Workfront seleccionando Acciones del documento > Enviar a… > Workfront. Se crea una nueva versión del documento en Workfront.
1. Descargue el documento desde Workfront haciendo clic en el vínculo Descargar.

### Prueba 10: actualizar el token de acceso (solo proveedores de webhook de OAuth2)

Comprueba los siguientes puntos finales: URL de punto final del token

1. Aprovisionamiento del servicio de webhook de documentos para un usuario
1. Invalide el token de acceso del usuario (1 ) esperando a que se agote el tiempo de espera o (2) invalidándolo manualmente en el sistema externo.
1. Actualice el token de acceso en Workfront. Para ello, por ejemplo, puede vincular un documento a Workfront. Sabrá que el token de acceso se actualizó correctamente si pudo desplazarse a un documento y vincularlo.

>[!NOTE]
>
>Actualmente, Enviar a... no está disponible para documentos vinculados. Esta se añadirá mediante Workfront. Puede comprobar el punto final /descarga presionando el punto final manualmente con un cliente REST, como Postman. Como alternativa, el punto final /download se puede probar generando una revisión digital. Para habilitar la revisión digital, póngase en contacto con Workfront.

## Versiones

* Versión 1.0 (Fecha de lanzamiento: mayo de 2015)

   * Especificación inicial

* Versión 1.1 (Fecha de lanzamiento: junio de 2015)

   * Se ha actualizado /uploadInit: se han añadido el ID de documento y el ID de versión de documento

* Versión 1.2 (Fecha de lanzamiento: octubre de 2015)

   * Se ha añadido /createFolder

