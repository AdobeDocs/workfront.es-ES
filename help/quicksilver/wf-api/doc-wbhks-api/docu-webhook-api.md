---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: API de Document Webhooks
description: API de Document Webhooks
author: John
feature: Workfront API
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: a2f340122b22ccc57af1afffd82093e458219648
workflow-type: tm+mt
source-wordcount: '3661'
ht-degree: 3%

---


# API de Document Webhooks

Adobe Workfront Document Webhooks define un conjunto de extremos de API a través de los cuales Workfront realiza llamadas de API autorizadas a un proveedor de documentos externo. Esto permite a cualquier persona crear un complemento de middleware para cualquier proveedor de almacenamiento de documentos.

La experiencia del usuario para las integraciones basadas en weblock será similar a la de las integraciones de documentos existentes, como Google Drive, Box y Dropbox. Por ejemplo, un usuario de Workfront podrá realizar las siguientes acciones:

* Navegar por la estructura de carpetas del proveedor de documentos externo
* Buscar archivos
* Vinculación de archivos a Workfront
* Cargar archivos al proveedor de documentos externo
* Ver una miniatura del documento

## Implementación de referencia

Para ayudar a iniciar el desarrollo de una nueva implementación de enlaces web, Workfront proporciona una implementación de referencia. El código para esto se puede encontrar en [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Esta implementación se basa en Java y permite a Workfront conectar documentos en un sistema de archivos de red.

## Registro de una integración de Weblock

Los administradores de Workfront pueden agregar una integración de enlace web personalizada para su empresa navegando hasta Configuración > Documentos > Integraciones personalizadas en Workfront. Desde la página Integración personalizada de Configuración, los administradores pueden ver una lista de las integraciones de Weblock del documento existente. Desde esta página, se pueden agregar, editar, habilitar y deshabilitar integraciones. Para añadir una integración, haga clic en el botón &quot;Añadir integración&quot;.

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
   <td> <p>La ubicación de la API de devolución de llamada. Al realizar llamadas al sistema externo, Workfront simplemente adjuntará el nombre del extremo a esta dirección. Por ejemplo, si el administrador introduce la URL de la API base, " https://www.mycompany.com/api/v1 ", Workfront utilizará la siguiente URL para obtener los metadatos de un documento: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
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
   <td> <p>(Solo OAuth2) La URL completa utilizada para la autenticación de usuarios. Workfront llevará a los usuarios a esta dirección como parte del proceso de aprovisionamiento de OAuth. Nota: Workfront adjuntará un parámetro "state" a la cadena de consulta. El proveedor debe devolver esto a Workfront anexándolo al URI de redirección de Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL de punto final de token</td> 
   <td> <p>(Solo OAuth2) La URL completa de la API que se usa para recuperar tokens de OAuth2. Esto lo aloja el proveedor de enlaces web o el proveedor de documentos externos</p> <p> </p> </td> 
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
   <td>  <p>(Solo OAuth2) Se trata de un campo de solo lectura que genera Workfront. Este valor se utiliza para registrar esta integración con el proveedor de documentos externo. Nota: Como se describe anteriormente para la URL de autenticación, el proveedor debe anexar el parámetro "state" y su valor a la cadena de consulta al realizar la redirección.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(Solo ApiKey) Se utiliza para realizar llamadas de API autorizadas al proveedor de enlaces web. La clave de API emitida por el proveedor de enlaces web.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Autenticación

Los enlaces web de documentos de Workfront admiten dos formas diferentes de autenticación: OAuth2 y ApiKey. En ambos casos, Workfront pasa tokens de autenticación en el encabezado al realizar una llamada de API.

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

### Adición de encabezados de solicitud (opcional)

Además de utilizar tokens de OAuth2 o una ApiKey para la autenticación, Workfront puede enviar un conjunto predefinido de encabezados al proveedor de enlaces web por cada llamada a la API. Un administrador de Workfront puede configurarlo al registrar o editar una integración de libro web, tal como se describe en la sección anterior. Consulte Registro de una integración de Weblock.

Por ejemplo, esto se puede usar para la autenticación básica. Para ello, el administrador de Workfront agregaría la siguiente información de encabezado de solicitud en el cuadro de diálogo Integración personalizada:

   Autorización básica QWxhZGRpbjpvcGVuIHNlc2FtZQ=

donde QWxhZGRpbjpvcGVuIHNlc2FtZQ=== es una cadena codificada base-64 de &quot;username:password&quot;. Consulte Autenticación básica . Siempre que se agregue esto, Workfront pasará esto en el encabezado de solicitud HTTP, además de otros encabezados de solicitud:

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## Especificación de API

A continuación, se muestra una lista de API que el proveedor de enlaces web debe implementar para que los enlaces web de documentos funcionen.

### Obtención de tokens de OAuth2 (solo se necesita la autenticación OAuth2)

Devuelve el token de actualización de OAuth2 y el token de acceso para un usuario autenticado. Esto se invoca una vez cuando el usuario aprovisiona un proveedor de documentos. Se realizan llamadas posteriores para obtener un token de acceso actualizado.

POST de solicitud HTTP /any/url

La dirección URL se puede configurar y corresponde al valor de la dirección URL del extremo del token en la página de configuración de la integración personalizada.

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
   <td>yes</td> 
   <td> <p>Los valores incluyen "authorization_code" o "refresh_token". El valor especificado indica cuál de los dos parámetros se transferirá a esta llamada de API: code o refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>code</td> 
   <td>depends</td> 
   <td> <p>El código de autorización se envía a Workfront justo después de que el usuario haga clic en el botón "Conceder". Esto solo es necesario cuando el tipo de concesión es "authorization_code". El código de autorización debe tener una duración corta, y por lo general caduca en 10 minutos o menos.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>depends</td> 
   <td> <p>Esto solo es necesario cuando se realizan llamadas posteriores para recuperar un nuevo access_token, dado que el access_token anterior ha caducado. Al enviar este valor, establezca el parámetro grant_type en "refresh_token".</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>yes</td> 
   <td>El ID de cliente configurado en Workfront para esta integración personalizada.</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>yes</td> 
   <td> Secreto del cliente configurado en Workfront para esta integración personalizada.</td> 
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
   <th>Tipo </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>Cadena</td> 
   <td> <p>Token utilizado para realizar llamadas de API autorizadas en nombre del usuario. Esto debería caducar para evitar llamadas de API no autorizadas.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>Cadena</td> 
   <td> <p>Token de larga duración utilizado para recuperar un nuevo access_token llamando a este método de API.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>(opcional) Tiempo (en segundos) antes de que caduque el token de acceso, que generalmente es de 3.600.</p></td> 
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

### Obtener metadatos de un archivo o carpeta

Devuelve metadatos del archivo o la carpeta especificados.

**Dirección URL**

GET /metadata?id=[documento o ID de carpeta]

**Parámetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>ID del archivo o la carpeta, tal como hace referencia el proveedor de vínculos web. Es distinto al ID de documento de Workfront. Para obtener los metadatos del directorio raíz, utilice el valor '/'.</p><p>Nota: La longitud máxima del ID es de 255 caracteres.</p></td> 
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
   <th>Nombre </th> 
   <th>Tipo </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>Cadena </td> 
   <td>El nombre del documento o carpeta</td> 
  </tr> 
  <tr> 
   <td>clase </td> 
   <td>Cadena </td> 
   <td>Especifica si este elemento es un archivo o una carpeta ("archivo" o "carpeta")</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Cadena </td> 
   <td>ID del archivo o la carpeta.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Cadena </td> 
   <td> <p>Ruta de URL utilizada por un usuario para ver el documento en una ventana del explorador. La URL puede ser alojada por el proveedor de documentos o por el proveedor de almacenamiento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Cadena </td> 
   <td> <p>Ruta de URL utilizada por un usuario para descargar el documento en una ventana del explorador. La URL puede ser alojada por el proveedor de documentos o por el proveedor de almacenamiento externo nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Cadena </td> 
   <td>Tipo MIME del archivo. (opcional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Cadena </td> 
   <td>La última vez que se modificó este archivo (marca de tiempo RFC 3339 con formato)</td> 
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

**Ejemplo:** `https://www.acme.com/api/metadata?id=12345`

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
>La gestión de errores debe ser coherente en todas las llamadas a la API. Consulte la sección &quot;Gestión de errores&quot; a continuación para obtener más información.

### Obtener una lista de elementos de una carpeta

Devuelve metadatos de los archivos y carpetas de una carpeta determinada.

**Dirección URL**

GET /archivos

**Parámetros de consulta**

| Nombre  | Descripción |
|---|---|
| parentId  | El ID de la carpeta. Para obtener los metadatos del directorio raíz, utilice el valor &#39;/&#39;. |

{style=&quot;table-layout:auto&quot;}

Actualmente, la API de Document Webhooks no admite la paginación.

**Respuesta**

JSON que contiene una lista de archivos y carpetas. Los metadatos de cada elemento son los mismos que devuelve el extremo /metadata .

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

Devuelve metadatos de los archivos y carpetas devueltos por una búsqueda. Esto se puede implementar como una búsqueda de texto completo o como una consulta de base de datos normal. Workfront llama al extremo /search cuando el usuario realiza una búsqueda desde el explorador de archivos externo.

**Dirección URL**

GET /búsqueda

**Parámetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>query</td> 
   <td>Término o frase de búsqueda.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(opcional) El ID de la carpeta desde la que se ejecutó la búsqueda. Nota: Este es un marcador de posición para una función futura en Workfront. Actualmente, workfront no pasa este parámetro. </p> </td> 
  </tr> 
  </tbody> 
</table>

Actualmente, la API de Document Webhooks no admite la paginación.

 

**Respuesta**

JSON contiene una lista de metadatos para archivos y carpetas que coinciden con la consulta. Lo que constituye una &quot;coincidencia&quot; lo determina el proveedor de weblinks. Idealmente, debería hacer una búsqueda de texto completo. También funciona la búsqueda basada en nombres de archivo.

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

**Dirección URL**

GET /descarga

**Parámetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> El ID del documento.</td> 
  </tr> 
 </tbody> 
</table>

 

**Respuesta**

Los bytes sin procesar del documento.

**Ejemplo:** `https://www.acme.com/api/download?id=123456`

### Obtener una miniatura de un documento

Devuelve los bytes de miniaturas sin procesar de un documento.

**Dirección URL**

GET/miniatura

**Parámetros de consulta**

| Nombre  | Descripción |
|---|---|
| id  | El ID del documento. |
| size  |  La anchura de la miniatura |

{style=&quot;table-layout:auto&quot;}

 

**Respuesta**

Los bytes de miniaturas sin procesar.

**Ejemplo:** `https://www.acme.com/api/thumbnail?id=123456`

### Cargar un archivo: parte 1 de 2

La carga de un archivo en un proveedor de almacenamiento de documentos es un proceso de dos pasos que requiere dos puntos de conexión de API independientes. Workfront inicia el proceso de carga llamando a /uploadInit . Este extremo devuelve un ID de documento que luego se pasa a /upload al cargar los bytes del documento. Dependiendo del sistema de almacenamiento de documentos subyacente, puede ser necesario crear un documento de longitud cero y luego actualizar el contenido del documento más adelante.

Se ha añadido a la versión 1.1 de esta especificación, el ID de documento y el ID de versión de documento pueden utilizarse para recuperar información adicional de Workfront. Por ejemplo, si el sistema de administración de documentos desea información adicional sobre el documento, el código de implementación de weblock podría utilizar el ID del documento para recuperar esa información mediante la API RESTful de Workfront. Como práctica recomendada, esta información podría provenir de campos de datos personalizados del documento y contiene tareas, problemas o proyectos.

**Dirección URL**

POST /uploadInit

**Parámetros de consulta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>El ID de la carpeta principal, tal como hace referencia el proveedor de vínculos web.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>El nombre del documento</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>El ID del documento de Workfront (añadido en la versión 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>El ID de versión del documento de Workfront (añadido en la versión 1.1)</td> 
  </tr> 
 </tbody> 
</table>

 

**Respuesta**

Los metadatos del archivo, tal como se definen en el extremo /metadata .

**Ejemplo:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Respuesta**

`[file_metadata]` incluye el nuevo ID de documento utilizado por el proveedor de documentos.

### Cargar un archivo: parte 2 de 2

Carga los bytes de un documento en el proveedor de enlaces web.

**Dirección URL**

PUT /upload

**Parámetros de consulta**

| Nombre  | Descripción |
|---|---|
| id  |  El ID del documento que acaba de crearse. |


 

**Cuerpo de la solicitud**

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

**Ejemplo:** `https://www.acme.com/api/upload?id=1234` *[bytes de documento incluidos en la secuencia de actualización]*

**Respuesta**

```
{
"result":"success"
}
```

### Obtener información sobre el servicio 

(Fecha de versión - TBD) Devuelve información sobre el servicio, como funciones y capacidades. Workfront utilizará esta información para personalizar la interfaz de usuario en Workfront. Por ejemplo, si la implementación de enlace web contiene algunas acciones personalizadas, el JSON debería enumerar esas operaciones en el JSON. Los usuarios podrían invocar estas acciones desde Workfront.

**Dirección URL**

GET /serviceInfo

Parámetros de consulta

Ninguno. Además, las llamadas a este extremo no deben requerir autenticación.

**Respuesta**

JSON que contiene información sobre este servicio

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nombre</th> 
   <th>Tipo </th> 
   <th>Descripción</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>weblockVersion </td> 
   <td>Cadena </td> 
   <td>La versión del enlace web implementada por este servicio. Este es el número de versión que aparece en la parte superior de esta especificación.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Cadena </td> 
   <td>Número de versión interna de este servicio. Este número lo determina el proveedor de servicios de enlace web y se utiliza solamente con fines informativos.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher </td> 
   <td>Cadena </td> 
   <td>Nombre de la empresa que proporciona la implementación del enlace web.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Cadena </td> 
   <td>Una lista que contiene los puntos finales de API implementados por este servicio. Esto se puede utilizar para garantizar que la interfaz de usuario en Workfront refleje las capacidades ofrecidas por el proveedor de enlaces web. Cada elemento de la lista debe incluir el nombre del extremo (como "búsqueda").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Cadena</td> 
   <td>  <p>Una lista que contiene las operaciones personalizadas implementadas por este vínculo web. Cada elemento de la lista incluye un nombre y un nombre para mostrar. El nombre para mostrar aparecerá en la lista desplegable "Acciones de documento" de Workfront. Al hacer clic en el elemento de la lista desplegable, se activará la acción en el enlace web llamando al extremo /customAction .</p></td> 
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
Dirección URL

POST /createFolder

**Parámetros de consulta**

| Nombre  | Descripción |
|---|---|
| parentId  | El ID de carpeta en el que se debe crear la carpeta |
| name  | El nombre de la nueva carpeta |

{style=&quot;table-layout:auto&quot;}

 

**Respuesta**

Los metadatos de la carpeta recién creada, tal como se define en el extremo /metadata .

**Ejemplo:** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

return

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

(Fecha de versión - TBD) Elimina un documento o una carpeta con el ID dado en el sistema externo. Al eliminar una carpeta también se eliminará su contenido.

Dirección URL

PUT /delete

**Parámetros de consulta**

| Nombre  | Descripción |
|---|---|
| documentId  | El ID del documento que se va a eliminar |
| folderId  |  El ID de carpeta que se va a eliminar |

{style=&quot;table-layout:auto&quot;}

Respuesta Una cadena JSON que indica que se ha realizado correctamente o que se ha producido un error, tal como se especifica en la sección Gestión de errores más abajo.

**Ejemplo:** PUT https://www.acme.com/api/delete id=1234

return

```
{
"status": "success" 
}
```

return

```
{
"status": "failure", "error": "File not found"
}
```


### Cambiar el nombre de un documento o carpeta

(Fecha de versión - TBD) Cambia el nombre de un documento o carpeta por el ID dado en el sistema externo.

Dirección URL

PUT /cambiar nombre

**Parámetros de consulta**

| Nombre  | Descripción |
|---|---|
| id | El ID de documento o carpeta al que cambiar el nombre |
| name  | El nuevo nombre del documento o carpeta |

{style=&quot;table-layout:auto&quot;}

 

respuesta

Una cadena JSON que indica que se ha realizado correctamente o que se ha producido un error, tal como se especifica en la sección Error Handling a continuación.

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

(Fecha de versión - TBD) Este extremo permitirá que un usuario de Workfront (o quizá un evento de flujo de trabajo automatizado) realice una acción en el sistema externo. El extremo /customAction acepta un parámetro &quot;name&quot;, que permite al proveedor de enlaces web implementar varias operaciones personalizadas.

El proveedor de vínculos web registra las acciones personalizadas con Workfront al incluir las acciones en la respuesta /serviceInfo en customActions. Workfront carga esta lista al configurar o actualizar el proveedor de vínculos web en Configuración > Documentos > Integraciones personalizadas.\
![](assets/mceclip0-350x262.png)

Los usuarios pueden almacenar en déclencheur la acción personalizada seleccionando la sección en &quot;Acciones de documento&quot;\
![](assets/mceclip1-350x95.png)

**Dirección URL**

GET /customAction

**Parámetros de consulta**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>Nombre </th>
   <th>Descripción</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>Identificador que especifica el tipo de acción que se va a realizar. Este valor corresponde a uno de los valores customAction enumerados que devuelve el extremo /serviceInfo .</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>ID del documento de área de trabajo para el que se está realizando la acción.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> El ID de versión del documento de área de trabajo para el que se está realizando la acción.</td>
  </tr>
 </tbody>
</table>

 

**Respuesta**

Una cadena JSON que indica que se ha realizado correctamente o que se ha producido un error, tal como se especifica en la sección Error Handling a continuación. En caso de error (por ejemplo, estado = &quot;error&quot;), Workfront mostrará al usuario el mensaje de error proporcionado.

**Ejemplo:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

response

```
{
"status": "success" 
}
```


## Gestión de errores

Pueden surgir problemas al procesar solicitudes de API. Esto debe gestionarse de forma coherente en todos los extremos de la API. Cuando se produce un error, el proveedor de vínculos web hace lo siguiente:

* Incluya un código de error en el encabezado de respuesta. Los códigos de error incluyen:

   * 403 - Prohibido. Indica que faltan tokens de solicitud o que no son válidos, o que las credenciales asociadas con los tokens no tienen acceso al recurso especificado. Para los proveedores de vínculos web basados en OAuth, Workfront intentará recuperar nuevos tokens de acceso.
   * 404 - No encontrado. Indica que el archivo o la carpeta especificados no existen.
   * 500 - Error interno del servidor. Cualquier otro tipo de error.

* Describa el error en el cuerpo de la respuesta con el siguiente formato:


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Pruebas

Para verificar que la implementación del weblock del documento funciona correctamente, ejecute las siguientes pruebas. Estas son pruebas manuales que pasan por la interfaz web de Workfront y que llegan indirectamente a los puntos finales de su implementación de weblink.

### Requisitos previos

Para ejecutar estas pruebas necesita lo siguiente:

* Una cuenta de Workfront con la administración avanzada de documentos (ADM) habilitada
* Un usuario de Workfront para esta cuenta con derechos de administrador del sistema
* Una instancia de Document Weblock, a la que se puede acceder desde los extremos HTTP de Workfront

Estas pruebas también suponen que ya ha registrado la instancia de Document Weblock en Workfront en Configuración > Documentos > Integraciones personalizadas.

### Prueba 1: Aprovisionar el servicio Document Weblock para un usuario

Prueba la URL de autenticación y la URL del extremo del token para los proveedores de Weblock basados en OAuth.

1. En Workfront, vaya a la página principal Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Haga clic en el menú desplegable Add Documents y seleccione el servicio Document Weblock en Add Service.
1. (Solo servicios de OAuth) Después de completar el paso anterior, verá la carga de la página de autenticación OAuth2 de su servicio en una ventana emergente. (Nota: es posible que se le pida que inicie sesión en su servicio primero). En la página de autenticación, conceda a Workfront acceso a la cuenta del usuario haciendo clic en el botón Confiar o Permitir .
1. Verifique que su servicio se haya agregado a la lista desplegable Agregar documentos . Si no lo ve inicialmente, intente actualizar el explorador.

### Prueba 2: Vincular un documento a pruebas de Workfront con los siguientes extremos: /archivos, /metadatos

1. En Workfront, vaya a la página principal Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio Document Weblock en Añadir documentos.
1. Desde el modal, navegue por la estructura de carpetas.
1. Compruebe que puede navegar correctamente por la estructura de carpetas.
1. Seleccionar y vincular un documento a Workfront

### Prueba 3: Vaya a un documento del sistema de gestión de contenido

Prueba los puntos finales siguientes: /metadata (específicamente el viewLink)

1. Vinculación de un documento a Workfront
1. Seleccione el documento y haga clic en el vínculo Open .
1. Compruebe que el documento se abre en una nueva ficha.

### Prueba 4: Vaya a un documento del sistema de administración de contenido (con inicio de sesión)

Prueba los puntos finales siguientes: /metadata (específicamente el viewLink)

1. Asegúrese de haber cerrado la sesión del sistema de administración de contenido.
1. Vincular un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Open .
1. Compruebe que la pantalla de inicio de sesión del sistema de administración de contenido se carga en una pestaña nueva.
1. Inicie sesión y verifique que ha accedido al documento.

### Prueba 5: Descargue el documento desde el sistema de administración de contenido

Prueba los puntos finales siguientes: /metadata (específicamente el vínculo de descarga)

1. Vincular un documento a Workfront.
1. Seleccione el documento y haga clic en el vínculo Descargar .
1. Compruebe que la descarga comience.

### Prueba 6: Buscar contenido

Prueba los puntos finales siguientes: /search

1. En Workfront, vaya a la página principal Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Seleccione el servicio Document Weblock en Añadir documentos.
1. Desde el modal, realice una búsqueda.
1. Compruebe que los resultados de la búsqueda sean correctos.

### Prueba 7: Enviar documento desde Workfront al sistema de administración de contenido

Prueba los puntos finales siguientes: /files, /uploadInit, /upload

1. En Workfront, vaya a la página principal Documentos haciendo clic en el vínculo Documentos en la barra de navegación superior.
1. Cargar un documento a Workfront desde el equipo
1. Vaya a la página de detalles del documento
1. En el menú desplegable Acciones de documento , seleccione el servicio de Weblock de documento en Enviar a...
1. Vaya a la carpeta de destino deseada y haga clic en el botón Save .
1. Compruebe que el documento se haya cargado en la ubicación correcta del sistema de administración de contenido.

### Prueba 8: Ver miniaturas en Workfront

Prueba los puntos finales siguientes: /thumbnail

1. Vincular un documento a Workfront.
1. Seleccione el documento en la lista.
1. Compruebe que la miniatura aparece en el panel derecho.

### Prueba 9: Obtención de los bytes de contenido

Prueba los puntos finales siguientes: /download

1. Vincular un documento a Workfront.
1. Vaya a la página de detalles del documento.
1. Envíe el documento a Workfront seleccionando Acciones de documento > Enviar a... > Workfront. Esto creará una nueva versión del documento en Workfront.
1. Descargue el documento desde Workfront haciendo clic en el vínculo Descargar .

### Prueba 10: Actualizar token de acceso (solo proveedores de Weblock de OAuth2)

Prueba los puntos finales siguientes: URL del extremo del token

1. Aprovisionar un servicio de Document Weblock para un usuario
1. Invalide el token de acceso del usuario en 1 ) esperando que se agote el tiempo de espera o 2) invalidándolo manualmente en el sistema externo.
1. Actualice el token de acceso en Workfront. Puede hacerlo, por ejemplo, vinculando un documento a Workfront. Sabdrá que el token de acceso se actualizó correctamente si pudo navegar a un documento y vincularlo.

>[!NOTE]
>
>Actualmente, Send To... no está disponible para documentos vinculados. Workfront lo agregará. Puede probar el extremo /download pulsando el extremo manualmente usando un cliente REST, como Postman. Alternativamente, el extremo /download se puede probar generando una prueba digital. Para habilitarlo, póngase en contacto con Workfront.

## Versiones

* Versión 1.0 (Fecha de versión - mayo de 2015)

   * Especificación inicial

* Versión 1.1 (Fecha de versión - junio de 2015)

   * Se ha actualizado /uploadInit - Se ha añadido documentId y documentVersionId

* Versión 1.2 (Fecha de versión - octubre de 2015)

   * Se ha añadido /createFolder

