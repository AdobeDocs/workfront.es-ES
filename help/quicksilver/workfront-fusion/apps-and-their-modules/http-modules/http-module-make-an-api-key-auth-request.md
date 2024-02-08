---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: http-modules
title: HTTP &gt; Realizar una solicitud de autorización de clave API
description: Esta [!DNL Adobe Workfront Fusion] El módulo de acción envía una solicitud HTTPS a una dirección URL especificada que requiere una autorización de autenticación de clave de API y procesa la respuesta.
author: Becky
feature: Workfront Fusion
exl-id: 70bf87c7-6d51-4ef4-9dce-80ad004e613f
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 0%

---

# HTTP >[!UICONTROL Realizar una solicitud de autorización de clave API]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere un [!DNL Adobe Workfront Fusion] además de una licencia de Adobe Workfront.

Esta [!DNL Adobe Workfront Fusion] El módulo de acción envía una solicitud HTTPS a una dirección URL especificada que requiere una autorización de autenticación de clave de API y procesa la respuesta.

>[!NOTE]
>
>Si se está conectando a un producto de Adobe que actualmente no tiene un conector dedicado, le recomendamos que utilice el módulo de Adobe Authenticator.
>
>Para obtener más información, consulte [módulo de Adobe Authenticator](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

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
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!UICONTROL Adobe Workfront Fusion] licencias, consulte [Licencias de Adobe Workfront Fusion](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de autorización de clave API] configuración del módulo

Al configurar la variable [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de autorización de clave API] módulo, [!DNL Adobe Workfront Fusion] muestra los campos que se indican a continuación. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Credenciales]</td> 
   <td> <p>Seleccione la clave que contiene las credenciales de autenticación de la clave de API. Para añadir una clave nueva, haga clic en <strong>[!UICONTROL Agregar]</strong> y configure la siguiente información:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre de clave]</strong></p> <p>Introduzca un nombre para este conjunto de credenciales de API.</p> </li> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Introduzca la clave de API.</p> </li> 
     <li> <p><strong>Ubicación de la clave API de [!UICONTROL]</strong> </p> <p>Seleccione si desea colocar la clave de API en el encabezado o en la consulta de la llamada de API.</p> </li> 
     <li> <p><strong>[!UICONTROL Nombre de parámetro de clave de API]</strong> </p> <p>Introduzca el nombre mediante el cual la llamada de API identifica la clave de API, como "apiKey" o "X-API-Key". Puede encontrar esta información en la documentación del servicio web al que se conecta el módulo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evaluar todos los estados como errores (excepto 2xx y 3xx)] </td> 
   <td> <p>Utilice esta opción para configurar la gestión de errores.</p> <p>Para obtener más información, consulte <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Tratamiento de errores en Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Introduzca la dirección URL a la que desea enviar una solicitud, como un punto final de API, un sitio web, etc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados] </td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Introduzca los pares de clave-valor de consulta deseados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de cuerpo]</p> </td> 
   <td> <p>El cuerpo HTTP son los bytes de datos transmitidos en un mensaje de transacción HTTP inmediatamente después de los encabezados si hay alguno que utilizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>El tipo de cuerpo sin procesar suele ser adecuado para la mayoría de las solicitudes de cuerpo HTTP incluso en situaciones en las que la documentación para desarrolladores no especifica datos para enviar.</p> <p>Especifique una forma de analizar los datos en el campo [!UICONTROL Content type].</p> <p>A pesar del tipo de contenido seleccionado, el módulo introduce los datos en cualquier formato estipulado o requerido por la documentación del desarrollador.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Este tipo de cuerpo es para [!UICONTROL POST] datos usando <code>application/x-www-form-urlencoded</code>.</p> <p>Para <code>[!UICONTROL application/x-www-form-urlencoded]</code>, el cuerpo del mensaje HTTP enviado al servidor es esencialmente una cadena de consulta. Las claves y los valores se codifican en pares clave-valor separados por <code>&amp;</code> y con una <code>=</code> entre la clave y el valor. </p> <p>Para datos binarios, utilice <code>[!UICONTROL multipart/form-data]</code> en su lugar.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Ejemplo: </b></span></span> 
       <p>Ejemplo del formato de solicitud HTTP resultante:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] es una solicitud HTTP multipart que se utiliza para enviar archivos y datos. Normalmente se utiliza para cargar archivos en el servidor.</p> <p>Añada campos para enviarlos en la solicitud. Cada campo debe contener un par clave-valor.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Texto]</strong> </p> <p>Introduzca la clave y el valor que se enviarán dentro del cuerpo de la solicitud.</p> </li> 
       <li> <p><strong>[!UICONTROL Archivo]</strong> </p> <p>Introduzca la clave y especifique el archivo de origen que desea enviar en el cuerpo de la solicitud.</p> <p>Asigne el archivo que desea cargar desde el módulo anterior (como [!UICONTROL HTTP] &gt;[!UICONTROL Obtener un archivo] o [!UICONTROL Google Drive] &gt;[!UICONTROL Descargar un archivo)], o bien introduzca el nombre de archivo y los datos de archivo manualmente.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Respuesta de análisis]</p> </td> 
   <td> <p>Active esta opción para analizar automáticamente las respuestas y convertir las respuestas JSON y XML, de modo que no necesite utilizar los módulos [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] o [!UICONTROL XML] &gt; [!UICONTROL Parse XML].</p> <p>Antes de poder utilizar contenido JSON o XML analizado, ejecute el módulo una vez manualmente para que el módulo pueda reconocer el contenido de la respuesta y le permita asignarlo en módulos posteriores.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tiempo de espera] </td> 
   <td> <p>Especifique el tiempo de espera de la solicitud en segundos (1-300). El valor predeterminado es 40 segundos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartir cookies con otros módulos HTTP]</td> 
   <td> <p> Active esta opción para compartir cookies del servidor con todos los módulos HTTP de su escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificado autofirmado]</td> 
   <td> <p> Cargue el certificado si desea utilizar TLS con el certificado autofirmado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rechazar conexiones que utilizan certificados no verificados (autofirmados)] </td> 
   <td> <p>Active esta opción para rechazar conexiones que utilicen certificados TLS no verificados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seguir redirección]</td> 
   <td> <p> Active esta opción para seguir las redirecciones de URL con respuestas 3xx.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seguir todas las redirecciones] </td> 
   <td> <p>Active esta opción para seguir las redirecciones URL con todos los códigos de respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Deshabilitar la serialización de varias claves de cadena de consulta iguales que matrices]</p> </td> 
   <td> <p>De forma predeterminada, [!DNL Workfront Fusion] administra varios valores para la misma clave de parámetro de cadena de consulta de URL que las matrices. Por ejemplo, <code>www.test.com?foo=bar&amp;foo=baz</code> se convertirá en <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Active esta opción para deshabilitar esta función. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Solicitar contenido comprimido]</td> 
   <td> <p> Active esta opción para solicitar una versión comprimida del sitio web.</p> <p>Agrega un <code>[!UICONTROL Accept-Encoding]</code> encabezado para solicitar contenido comprimido.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Utilizar TLS mutuo]</td> 
   <td> <p>Active esta opción para utilizar TLS mutuo en la solicitud HTTP.</p> <p>Para obtener más información sobre TLS mutuo, consulte <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Usar TLS mutuo en módulos HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
