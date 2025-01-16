---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de AWS S3
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1455'
ht-degree: 91%

---

# Módulos de AWS S3

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos de AWS S3](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/aws-s3-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Los módulos S3 de [!DNL Adobe Workfront Fusion AWS] le permiten realizar operaciones en los bloques de S3.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

Para usar los módulos [!UICONTROL AWS S3] debe tener una cuenta de [!DNL Amazon Web Service].

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

Para conectar [!DNL AWS S3] a [!DNL Workfront Fusion] debe conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion]. Para hacerlo, primero necesitará crear un usuario de API en [!DNL AWS] [!UICONTROL IAM].

1. Inicie sesión en su cuenta de [!DNL AWS] [!UICONTROL IAM].
1. Navegue a **[!UICONTROL Gestión de Identidad y Accesos]** > **[!UICONTROL Gestión de Accesos]** > **[!UICONTROL Usuarios]**.

1. Haga clic en **[!UICONTROL Agregar usuario]**.
1. Introduce el nombre del nuevo usuario y selecciona la opción **[!UICONTROL Acceso programático]** en la sección [!UICONTROL Tipo de acceso].
1. Haga clic en **[!UICONTROL Vincular políticas existentes directamente]**, luego busque **[!UICONTROL AmazonS3FullAccess]** en la barra de búsqueda. Haga clic en él cuando aparezca y luego haga clic en **[!UICONTROL Siguiente]**.

1. Continúe con las otras pantallas de diálogo y luego haga clic en **[!UICONTROL Crear usuario]**.
1. Copie el **[!UICONTROL ID de clave de acceso]** y la **[!UICONTROL Clave de acceso secreta]** proporcionados.

1. Vaya a [!DNL Workfront Fusion] y abre el cuadro de diálogo [!DNL AWS S3] del módulo **[!UICONTROL Crear un destino]**.
1. Introduzca el [!UICONTROL ID de clave de acceso] y la [!UICONTROL Clave de acceso secreta] del paso 7 en los campos correspondientes y haga clic en **[!UICONTROL Continuar]** para establecer la conexión.

Se ha establecido la conexión. Puede continuar con la configuración del módulo.

## [!DNL AWS S3] módulos y sus campos

Al configurar módulos de [!DNL AWS S3], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL AWS S3] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)
* [Búsquedas](#searches)

### Acciones

* [[!UICONTROL Crear cubo]](#create-bucket)
* [[!UICONTROL Obtener archivo]](#get-file)
* [[!UICONTROL Cargar archivo]](#upload-file)
* [[!UICONTROL Realizar una llamada de API]](#make-an-api-call)

#### [!UICONTROL Crear cubo]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Introduzca el nombre del cubo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la explicación sobre <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html?lang?=es">puntos finales regionales</a> en la documentación de AWS.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener archivo]

Descargue un archivo de un cubo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la explicación sobre <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html?lang?=es">Puntos finales regionales</a> en la documentación de [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleccione el cubo desde el que desee descargar el archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>Introduzca la ruta al archivo. Ejemplo: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la explicación sobre <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html?lang?=es">puntos finales regionales</a> en la documentación de [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder] (opcional) </p> </td> 
   <td> <p>Especifique la carpeta de destino en la que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers] (opcional)</p> </td> 
   <td> <p> Insertar encabezados de solicitud. Los encabezados disponibles se encuentran en la documentación de <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html?lang=es">[!DNL AWS S3]: objeto de [!UICONTROL PUT</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada de API]

Para obtener una explicación sobre la API de [!DNL Amazon S3], consulte Introducción a la API REST de [[!DNL Amazon S3] ](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Region] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la explicación sobre <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html?lang?=es">puntos finales regionales</a> en la documentación de [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>Introduzca una URL de host. La ruta debe ser relativa a <code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Method]</td> 
   <td> <p>Seleccione el método de petición [!UICONTROL HTTP] que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de petición [!UICONTROL HTTP] en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Añada un encabezado de solicitud. Puede utilizar los siguientes encabezados de solicitud comunes. Para obtener más encabezados de solicitud, consulte la documentación de la API de <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html?lang=es">[!DNL AWS S3]</a>.</p> <p>[!DNL Workfront Fusion] añade encabezados de autorización automáticamente.</p> 
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
       <td> <p>El tipo de contenido del recurso, en caso de que el contenido de la solicitud esté en el cuerpo. Ejemplo: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>Resumen MD5 de 128 bits codificado en base64 del mensaje (sin los encabezados) según RFC 1864. Este encabezado se puede utilizar como comprobación de integridad de mensajes para comprobar que los datos son los mismos que se enviaron originalmente. Aunque es opcional, se recomienda utilizar el mecanismo [!UICONTROL Content-MD5] como comprobación de integridad de extremo a extremo. Para obtener más información acerca de la autenticación de solicitud de [!UICONTROL REST], vaya a Autenticación <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST]</a> en la guía para desarrolladores de <i>[!DNL Amazon] Simple Storage Service</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Date]</p> </td> 
       <td> <p>La fecha y hora actuales según el solicitante. Ejemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>.  Cuando especifique el encabezado <code>Authorization </code>, debe especificar el encabezado <code>x-amz-date</code> o <code>Date </code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Expect]</p> </td> 
       <td> <p>Cuando la aplicación utiliza [!UICONTROL 100-continue], no envía el cuerpo de la solicitud hasta que reciba una confirmación. Si el mensaje se rechaza en función de los encabezados, no se envía el cuerpo del mensaje. Este encabezado solo se puede utilizar si envía un cuerpo.</p> <p>Valores válidos: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Para solicitudes path-style, el valor es <code>s3.amazonaws.com</code>. Para solicitudes de estilo virtual, el valor es <code>BucketName.s3.amazonaws.com</code>. Para obtener más información, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html?lang=es">Virtual Hosting</a> en la publicación <i>[!DNL Amazon] Simple Storage Service Developer Guide</i>.</p> <p>Este encabezado es necesario para HTTP 1.1 (la mayoría de los kits de herramientas lo añaden automáticamente); opcional para las solicitudes HTTP/1.0.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Cuando se utiliza la versión de firma 4 para autenticar la solicitud, este encabezado proporciona un hash de la carga útil de la solicitud. Al cargar un objeto en fragmentos, establezca el valor en <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> para indicar que la firma cubre solo los encabezados y que no hay carga útil. Para obtener más información, consulte <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html?lang=es">Cálculos de firma para el encabezado de autorización: transferencia de la carga útil en varios fragmentos (carga interrumpida) ([!DNL AWS] versión de firma 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>La fecha y hora actuales según el solicitante. Ejemplo: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>.  Cuando especifique el encabezado <code>Authorization </code>, debe especificar el encabezado <code>x-amz-date</code> o <code>Date </code>. Si especifica ambos, el valor especificado del encabezado <code>x-amz-date</code> tiene prioridad.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Este encabezado se puede utilizar en los siguientes casos:</p> 
        <ul> 
         <li>Debe proporcionar tokens de seguridad para las operaciones de [!DNL Amazon DevPay]. Cada solicitud que usa [!DNL Amazon DevPay] requiere dos encabezados <code>x-amz-security-token</code>: uno para el token de producto y otro para el token de usuario. Cuando [!DNL Amazon S3] recibe una solicitud autenticada, compara la firma calculada con la firma proporcionada. El uso de encabezados de varios valores con un formato incorrecto para calcular una firma puede causar problemas de autenticación.</li> 
         <li>Debe proporcionar un token de seguridad cuando utilice credenciales de seguridad temporales. Al realizar solicitudes con credenciales de seguridad temporales obtenidas de IAM, debe proporcionar un token de seguridad mediante este encabezado. Para obtener más información sobre las credenciales de seguridad temporales, vaya a Creación de solicitudes.</li> 
        </ul> <p>Este encabezado es necesario para las solicitudes que usan [!DNL Amazon DevPay] y las solicitudes que se firman con credenciales de seguridad temporales.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Añada las cadenas de consulta deseadas, como parámetros o campos de formulario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Cuando utilice instrucciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la instrucción condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Listar archivos]](#list-files)
* [[!UICONTROL Listar carpetas]](#list-folders)

#### [!UICONTROL Listar archivos]

Devuelve una lista de archivos de una ubicación especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la explicación sobre <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html?lang?=es">Puntos finales regionales</a> en la documentación de [!DNL AWS].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleccione el grupo [!DNL Amazon S3] en el que desea buscar archivos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (opcional)</p> </td> 
   <td> <p> Ruta a una carpeta en la que se buscan archivos, por ejemplo, <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listar carpetas]

Devuelve una lista de carpetas desde una ubicación especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL AWS] a [!DNL Workfront Fusion], consulte <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Conectar [!DNL AWS] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleccione el punto final regional. Para obtener más información, consulte la descripción de <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html?lang?=es">puntos finales regionales</a> en la documentación de AWS.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleccione el cubo de [!DNL Amazon S3] en el que desea buscar carpetas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (opcional)</p> </td> 
   <td> <p> Ruta a una carpeta en la que se buscan carpetas, por ejemplo, <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
