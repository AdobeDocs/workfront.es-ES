---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos AWS S3
description: La variable [!DNL Adobe Workfront Fusion AWS] Los módulos S3 le permiten realizar operaciones en sus contenedores S3.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1381'
ht-degree: 0%

---

# Módulos AWS S3

La variable [!DNL Adobe Workfront Fusion AWS] Los módulos S3 le permiten realizar operaciones en sus contenedores S3.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar [!UICONTROL AWS S3] módulos, debe tener un [!DNL Amazon Web Service] cuenta.

## Connect [!DNL AWS] a [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Para conectar [!DNL AWS S3] a [!DNL Workfront Fusion] debe conectar su [!DNL AWS] cuenta para [!DNL Workfront Fusion]. Para ello, primero deberá crear un usuario de API en [!DNL AWS] [!UICONTROL IAM].

1. Inicie sesión en su [!DNL AWS] [!UICONTROL IAM] cuenta.
1. Vaya a **[!UICONTROL Administración de identidad y acceso]** > **[!UICONTROL Gestión de acceso]** > **[!UICONTROL Usuarios]**.

1. Haga clic en **[!UICONTROL Agregar usuario]**.
1. Introduzca el nombre del nuevo usuario y seleccione la opción **[!UICONTROL Acceso mediante programación]** en la [!UICONTROL Tipo de acceso] para obtener más información.
1. Haga clic en **[!UICONTROL Adjuntar las políticas existentes directamente]** y, a continuación, busque **[!UICONTROL AmazonS3FullAccess]** en la barra de búsqueda. Haga clic en él cuando aparezca y, a continuación, haga clic en **[!UICONTROL Siguiente]**.

1. Continúe por las otras pantallas de cuadro de diálogo y, a continuación, haga clic en **[!UICONTROL Crear usuario]**.
1. Copie el **[!UICONTROL Acceso a ID de clave]** y **[!UICONTROL Clave de acceso secreta]**.

1. Vaya a [!DNL Workfront Fusion] y abra el [!DNL AWS S3] módulo **[!UICONTROL Crear una conexión]** diálogo.
1. Introduzca la variable [!UICONTROL Acceso a ID de clave] y [!UICONTROL Clave de acceso secreta] del paso 7 a los campos respectivos y haga clic en **[!UICONTROL Continuar]** para establecer la conexión.

Se ha establecido la conexión. Puede continuar con la configuración del módulo.

## [!DNL AWS S3] módulos y sus campos

Al configurar [!DNL AWS S3] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL AWS S3] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)
* [Búsquedas](#searches)

### Acciones

* [[!UICONTROL Crear depósito]](#create-bucket)
* [[!UICONTROL Obtener archivo]](#get-file)
* [[!UICONTROL Cargar archivo]](#upload-file)
* [[!UICONTROL Realizar una llamada de API]](#make-an-api-call)

#### [!UICONTROL Crear depósito]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL AWS] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Introduzca el nombre del nuevo depósito.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la discusión de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">puntos finales regionales</a> en la documentación de AWS.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener archivo]

Descarga un archivo de un compartimento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL AWS] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la discusión de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">puntos finales regionales</a> en el [!DNL AWS] documentación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleccione el bloque desde el que desea descargar el archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>Introduzca la ruta al archivo. Ejemplo: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar archivo]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL AWS] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la discusión de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">puntos finales regionales</a> en el [!DNL AWS] documentación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder] (opcional) </p> </td> 
   <td> <p>Especifique la carpeta de destino en la que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers] (opcional)</p> </td> 
   <td> <p> Inserte encabezados de solicitud. Los encabezados disponibles se encuentran en la <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] documentación: objeto [!UICONTROL PUT]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada de API]

Para un análisis detallado de la [!DNL Amazon S3] API, consulte [[!DNL Amazon S3] [!UICONTROL REST] Introducción a la API](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL AWS] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la discusión de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">puntos finales regionales</a> en el [!DNL AWS] documentación.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Introduzca una dirección URL de host. La ruta debe ser relativa a<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud [!UICONTROL HTTP] que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud [!UICONTROL HTTP] en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Encabezados]</td> 
   <td> <p>Añada un encabezado de solicitud. Puede utilizar los siguientes encabezados de solicitud comunes. Para obtener más información, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] Documentación de API</a>.</p> <p>[!DNL Workfront Fusion] añade encabezados de autorización automáticamente.</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>Nombre del encabezado</th> 
       <th> <p> Descripción</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>Longitud del mensaje (sin los encabezados) según RFC 2616. Este encabezado es necesario para [!UICONTROL PUT] y operaciones que cargan XML, como el registro y las ACL.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>El tipo de contenido del recurso, en caso de que el contenido de la solicitud esté en el cuerpo. Ejemplo: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>El compendio MD5 del mensaje codificado base64 de 128 bits (sin los encabezados) de acuerdo con RFC 1864. Este encabezado se puede utilizar como comprobación de integridad del mensaje para verificar que los datos son los mismos datos que se enviaron originalmente. Aunque es opcional, se recomienda utilizar el mecanismo [!UICONTROL Content-MD5] como comprobación de integridad de extremo a extremo. Para obtener más información sobre la autenticación de solicitud de [!UICONTROL REST], vaya a <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">Autenticación [!UICONTROL REST]</a> en el <i>[!DNL Amazon] Guía para desarrolladores de Simple Storage Service</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Date]</p> </td> 
       <td> <p>La fecha y hora actuales según el solicitante. Ejemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Al especificar la variable <code>Authorization </code>, debe especificar <code>x-amz-date</code> o <code>Date </code>encabezado.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Expect]</p> </td> 
       <td> <p>Cuando la aplicación utiliza [!UICONTROL 100-continue], no envía el cuerpo de la solicitud hasta que recibe un acuse de recibo. Si el mensaje se rechaza en función de los encabezados, no se envía el cuerpo del mensaje. Este encabezado solo se puede utilizar si está enviando un cuerpo.</p> <p>Valores válidos: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Para las solicitudes de estilo de ruta, el valor es <code>s3.amazonaws.com</code>. Para las solicitudes de estilo virtual, el valor es <code>BucketName.s3.amazonaws.com</code>. Para obtener más información, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Alojamiento virtual</a> en el <i>[!DNL Amazon] Guía para desarrolladores de Simple Storage Service</i>.</p> <p>Este encabezado es necesario para HTTP 1.1 (la mayoría de los conjuntos de herramientas agregan este encabezado automáticamente); opcional para solicitudes HTTP/1.0.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Cuando se utiliza la versión 4 de la firma para autenticar la solicitud, este encabezado proporciona un hash de la carga útil de la solicitud. Al cargar un objeto en trozos, establezca el valor en <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> para indicar que la firma solo cubre encabezados y que no hay carga útil. Para obtener más información, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Cálculos de firma para el encabezado de autorización: Transferencia de carga útil en varios fragmentos (carga interrumpida) ([!DNL AWS] Firma versión 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>La fecha y hora actuales según el solicitante. Ejemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Al especificar la variable <code>Authorization </code>, debe especificar <code>x-amz-date</code> o <code>Date </code>encabezado. Si especifica ambos, el valor especificado para la variable <code>x-amz-date</code> el encabezado tiene prioridad.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Este encabezado se puede utilizar en los siguientes casos:</p> 
        <ul> 
         <li>Proporcionar tokens de seguridad para [!DNL Amazon DevPay] operaciones. Cada solicitud que utilice [!DNL Amazon DevPay] requiere dos <code>x-amz-security-token</code> encabezados: uno para el token de producto y otro para el token de usuario. When [!DNL Amazon S3] recibe una solicitud autenticada, compara la firma calculada con la firma proporcionada. Los encabezados de varios valores con formato incorrecto que se usan para calcular una firma pueden causar problemas de autenticación.</li> 
         <li>Proporcione un token de seguridad cuando utilice credenciales de seguridad temporales. Al realizar solicitudes utilizando credenciales de seguridad temporales obtenidas de IAM, debe proporcionar un token de seguridad mediante este encabezado. Para obtener más información sobre las credenciales de seguridad temporales, vaya a Realizar solicitudes.</li> 
        </ul> <p>Este encabezado es necesario para las solicitudes que utilizan [!DNL Amazon DevPay] y solicitudes que se firman con credenciales de seguridad temporales.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada las cadenas de consulta deseadas, como parámetros o campos de formulario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Archivos de lista]](#list-files)
* [[!UICONTROL Carpetas de lista]](#list-folders)

#### [!UICONTROL Archivos de lista]

Devuelve una lista de archivos de una ubicación especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL AWS] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la discusión de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">puntos finales regionales</a> en el [!DNL AWS] documentación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleccione el [!DNL Amazon S3] paquete que desea buscar archivos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (opcional)</p> </td> 
   <td> <p> Ruta a una carpeta en la que buscar archivos, por ejemplo <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carpetas de lista]

Devuelve una lista de carpetas de una ubicación especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL AWS] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la discusión de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">puntos finales regionales</a> en la documentación de AWS.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleccione el [!DNL Amazon S3] paquete que desea buscar carpetas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (opcional)</p> </td> 
   <td> <p> Ruta a una carpeta en la que buscar carpetas, por ejemplo <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
