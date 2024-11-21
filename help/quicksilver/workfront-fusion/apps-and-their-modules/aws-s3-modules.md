---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de AWS S3
description: Los módulos  [!DNL Adobe Workfront Fusion AWS] S3 le permiten realizar operaciones en sus bloques de S3.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 0%

---

# Módulos de AWS S3

Los módulos S3 de [!DNL Adobe Workfront Fusion AWS] le permiten realizar operaciones en los bloques de S3.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar los módulos [!UICONTROL AWS S3], debes tener una cuenta de [!DNL Amazon Web Service].

## Información de la API de AWS S3

El conector AWS S3 utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td>https://s3.{{parameters.region}}.amazonaws.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.5.21</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL AWS] a [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Para conectar [!DNL AWS S3] a [!DNL Workfront Fusion], debe conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion]. Para ello, primero tendrá que crear un usuario de API en [!DNL AWS] [!UICONTROL IAM].

1. Inicie sesión en su cuenta de [!DNL AWS] [!UICONTROL IAM].
1. Vaya a **[!UICONTROL Administración de identidad y acceso]** > **[!UICONTROL Administración de acceso]** > **[!UICONTROL Usuarios]**.

1. Haga clic en **[!UICONTROL Agregar usuario]**.
1. Escriba el nombre del nuevo usuario y seleccione la opción **[!UICONTROL Acceso mediante programación]** en la sección [!UICONTROL Tipo de acceso].
1. Haga clic en **[!UICONTROL Adjuntar directivas existentes directamente]** y, a continuación, busque **[!UICONTROL AmazonS3FullAccess]** en la barra de búsqueda. Haga clic en él cuando aparezca y luego haga clic en **[!UICONTROL Siguiente]**.

1. Continúe con las otras pantallas de diálogo y luego haga clic en **[!UICONTROL Crear usuario]**.
1. Copie la **[!UICONTROL clave de acceso ID]** y la **[!UICONTROL clave de acceso secreta]** que se proporcionaron.

1. Vaya a [!DNL Workfront Fusion] y abra el diálogo **[!UICONTROL Crear una conexión]** del módulo [!DNL AWS S3].
1. Escriba la [!UICONTROL clave de acceso ID] y la [!UICONTROL clave de acceso secreta] del paso 7 en los campos respectivos y haga clic en **[!UICONTROL Continuar]** para establecer la conexión.

Se ha establecido la conexión. Puede continuar con la configuración del módulo.

## [!DNL AWS S3] módulos y sus campos

Al configurar [!DNL AWS S3] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL AWS S3] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)
* [Búsquedas](#searches)

### Acciones

* [[!UICONTROL Crear cubo]](#create-bucket)
* [[!UICONTROL Obtener archivo]](#get-file)
* [[!UICONTROL Cargar archivo]](#upload-file)
* [[!UICONTROL Realizar una llamada API]](#make-an-api-call)

#### [!UICONTROL Crear cubo]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], vea <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre] </td> 
   <td> <p>Introduzca el nombre del nuevo bloque.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la descripción de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">extremos regionales</a> en la documentación de AWS.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener archivo]

Descarga un archivo desde un contenedor.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], vea <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, vea la descripción de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">extremos regionales</a> en la documentación de [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleccione el contenedor desde el que desee descargar el archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ruta]</p> </td> 
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
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], vea <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, vea la descripción de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">extremos regionales</a> en la documentación de [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Carpeta] (opcional) </p> </td> 
   <td> <p>Especifique la carpeta de destino en la que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL archivo Source]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Encabezados] (opcional)</p> </td> 
   <td> <p> Insertar encabezados de solicitud. Los encabezados disponibles se encuentran en la documentación de <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3]: [!UICONTROL PUT] objeto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada API]

Para obtener un análisis detallado de la API [!DNL Amazon S3], consulte [[!DNL Amazon S3] [!UICONTROL Introducción a la API REST]](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], vea <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, vea la descripción de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">extremos regionales</a> en la documentación de [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Introduzca una URL de host. La ruta debe ser relativa a <code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud [!UICONTROL HTTP] que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!UICONTROL HTTP] métodos de solicitud en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Encabezados]</td> 
   <td> <p>Añada un encabezado de solicitud. Puede utilizar los siguientes encabezados de solicitud comunes. Para obtener más encabezados de solicitud, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] Documentación de la API </a>.</p> <p>[!DNL Workfront Fusion] agrega encabezados de autorización automáticamente.</p> 
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
       <td> <p>Longitud del mensaje (sin encabezados) según RFC 2616. Este encabezado es necesario para [!UICONTROL PUT] y las operaciones que cargan XML, como el registro y las ACL.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>El tipo de contenido del recurso, en caso de que el contenido de la solicitud esté en el cuerpo. Ejemplo: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>Resumen MD5 de 128 bits codificado en base64 del mensaje (sin los encabezados) según RFC 1864. Este encabezado se puede utilizar como comprobación de integridad de mensajes para comprobar que los datos son los mismos que se enviaron originalmente. Aunque es opcional, se recomienda utilizar el mecanismo [!UICONTROL Content-MD5] como comprobación de integridad de extremo a extremo. Para obtener más información acerca de la autenticación de solicitudes de [!UICONTROL REST], vaya a Autenticación <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST]</a> en la <i>[!DNL Amazon] Guía para desarrolladores de Simple Storage Service</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Fecha]</p> </td> 
       <td> <p>La fecha y hora actuales según el solicitante. Ejemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Cuando especifique el encabezado <code>Authorization </code>, debe especificar el encabezado <code>x-amz-date</code> o <code>Date </code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Esperar]</p> </td> 
       <td> <p>Cuando la aplicación utiliza [!UICONTROL 100-continue], no envía el cuerpo de la solicitud hasta que recibe una confirmación. Si el mensaje se rechaza en función de los encabezados, no se envía el cuerpo del mensaje. Este encabezado solo se puede utilizar si envía un cuerpo.</p> <p>Valores válidos: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Para solicitudes de estilo de ruta, el valor es <code>s3.amazonaws.com</code>. Para solicitudes de estilo virtual, el valor es <code>BucketName.s3.amazonaws.com</code>. Para obtener más información, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Alojamiento virtual</a> en la <i>[!DNL Amazon] Guía para desarrolladores de Simple Storage Service</i>.</p> <p>Este encabezado es necesario para HTTP 1.1 (la mayoría de los kits de herramientas lo añaden automáticamente); opcional para las solicitudes HTTP/1.0.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Cuando se utiliza la versión de firma 4 para autenticar la solicitud, este encabezado proporciona un hash de la carga útil de la solicitud. Al cargar un objeto en fragmentos, establezca el valor en <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> para indicar que la firma cubre solo los encabezados y que no hay carga útil. Para obtener más información, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Cálculos de firma para el encabezado de autorización: transferencia de carga útil en varios fragmentos (carga interrumpida) ([!DNL AWS] versión de firma 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>La fecha y hora actuales según el solicitante. Ejemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Cuando especifique el encabezado <code>Authorization </code>, debe especificar el encabezado <code>x-amz-date</code> o <code>Date </code>. Si especifica ambos, el valor especificado para el encabezado <code>x-amz-date</code> tiene prioridad.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Este encabezado se puede utilizar en los siguientes casos:</p> 
        <ul> 
         <li>Proporcione tokens de seguridad para [!DNL Amazon DevPay] operaciones. Cada solicitud que usa [!DNL Amazon DevPay] requiere dos encabezados <code>x-amz-security-token</code>: uno para el token de producto y otro para el token de usuario. Cuando [!DNL Amazon S3] recibe una solicitud autenticada, compara la firma calculada con la firma proporcionada. El uso de encabezados de varios valores con un formato incorrecto para calcular una firma puede causar problemas de autenticación.</li> 
         <li>Proporcione un token de seguridad cuando utilice credenciales de seguridad temporales. Al realizar solicitudes con credenciales de seguridad temporales obtenidas de IAM, debe proporcionar un token de seguridad mediante este encabezado. Para obtener más información sobre las credenciales de seguridad temporales, vaya a Creación de solicitudes.</li> 
        </ul> <p>Este encabezado es necesario para las solicitudes que usan [!DNL Amazon DevPay] y las solicitudes que se firmaron con credenciales de seguridad temporales.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Agregue las cadenas de consulta deseadas, como parámetros o campos de formulario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
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
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], vea <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, vea la descripción de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">extremos regionales</a> en la documentación de [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleccione el bloque [!DNL Amazon S3] en el que desea buscar archivos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (opcional)</p> </td> 
   <td> <p> Ruta a una carpeta en la que buscar archivos, p. ej. <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carpetas de lista]

Devuelve una lista de carpetas desde una ubicación especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], vea <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Región] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la descripción de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">extremos regionales</a> en la documentación de AWS.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleccione el bloque [!DNL Amazon S3] en el que desea buscar carpetas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (opcional)</p> </td> 
   <td> <p> Ruta a una carpeta en la que buscar carpetas, p. ej. <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
