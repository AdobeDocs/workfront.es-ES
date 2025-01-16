---
title: Módulos de DocuSign
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2007'
ht-degree: 94%

---

# Módulos de DocuSign

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos DocuSign](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/docusign-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Los módulos [!DNL DocuSign] de [!DNL Adobe Workfront Fusion] le permiten supervisar y recuperar el estado de los sobres, buscar y recuperar sobres o descargar y enviar un documento para iniciar sesión en su cuenta de [!DNL DocuSign].

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, consulte [Módulos de  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar módulos [!DNL DocuSign], debe tener una cuenta de [!DNL DocuSign].

## Información de API de DocuSign

El conector de DocuSign utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>1.18.11</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL DocuSign] a [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

Para crear una conexión para los módulos de [!DNL DocuSign]:

1. Haga clic en **[!UICONTROL Añadir]** junto al cuadro [!UICONTROL Conexión] cuando empiece a configurar el primer módulo de [!DNL DocuSign].
1. Introduzca lo siguiente:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td>Escriba un nombre para la nueva conexión de [!DNL DocuSign]</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Account type]</td> 
      <td>Seleccione si la cuenta a la que desea conectarse es una cuenta de producción o una cuenta de demostración.</td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe tal como se describe en [Crear una conexión a [!DNL Adobe Workfront Fusion] : instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## Módulos de [!DNL DocuSign] y sus campos

Al configurar módulos de [!DNL DocuSign], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL DocuSign] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Activadores](#triggers)
* [Acciones](#actions)

### Activadores

#### [!UICONTROL Ver sobres]

Este módulo de activador inicia un escenario cuando se envía, entrega, firma, completa o rechaza un sobre.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL DocuSign] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Seleccione la cuenta que contiene los registros que desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event type]</td> 
   <td> <p> Seleccione el tipo de evento que desea ver.</p> 
    <ul> 
     <li>[!UICONTROL Document completed]</li> 
     <li>[!UICONTROL Document declined]</li> 
     <li>[!UICONTROL Document sent]</li> 
     <li>[!UICONTROL Document signed]</li> 
     <li>[!UICONTROL New document in Inbox]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Output fields]</p> </td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Introduzca o asigne el número máximo de registros con los que desea que trabaje el módulo durante cada ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Descargar un documento]](#download-a-document)
* [[!UICONTROL Leer un sobre]](#read-an-envelope)
* [[!UICONTROL Cargar un archivo en un sobre]](#upload-a-file-to-an-envelope)
* [[!UICONTROL Crear un nuevo sobre]](#create-a-new-envelope)
* [[!UICONTROL Añadir destinatario al sobre]](#add-recipient-to-envelope)
* [[!UICONTROL Añadir campo personalizado]](#add-custom-field)
* [[!UICONTROL Modificar campo personalizado]](#modify-custom-field)
* [[!UICONTROL Enviar sobre]](#send-envelope)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada de API personalizada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL DocuSign] a [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Account]</td> 
   <td>Introduzca o asigne la cuenta que desea usar para acceder a la API de [!DNL DocuSign].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>Escriba la dirección del servidor web con el que desea que interactúe el módulo.</p> <p>Puede escribir una dirección URL relativa, lo que significa que no tiene que incluir el protocolo (como <code>http://</code>) al principio. Esto sugiere al servidor web que la interacción se está produciendo en el servidor.</p> <p>Por ejemplo: <code>[!DNL /api/conversations].create</code></p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Method]</td> 
   <td> <p>Seleccione el método de petición HTTP que necesita para configurar la llamada de la API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Determina el tipo de contenido de la petición.</p> <p>Por ejemplo:<code> {"Content-type":"application/json"}</code></p> <p>Nota: Si se producen errores y es difícil determinar su origen, considere la posibilidad de modificar los encabezados basándose en la documentación de [!DNL Workfront]. Si la llamada de API personalizada devuelve un error de petición HTTP 422, intente utilizar un encabezado “Content-Type”:“text/plain”.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice instrucciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la instrucción condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Introduzca o asigne el número máximo de resultados con los que se va a trabajar durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** enumerar sobres
>
>La siguiente llamada de la API devuelve sobres a partir de la fecha especificada en su cuenta de [!DNL DocuSign]:
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**Método**: `GET`
>
>**Cadena de consulta**:
>
>* **Clave**: `from_date`
>
>* **Valor**: `YYYY-MM-DD`
>
>Especifica cuándo comienza la solicitud a comprobar los cambios de estado de los sobres de la cuenta.
>
>![](assets/example-docusign-setup-350x770.png)
>
>El resultado se puede encontrar en la salida del módulo en Paquete > Cuerpo > Sobres.
>
>En nuestro ejemplo, se devolvieron 6 sobres:
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL Descargar un documento]

Este módulo de acción descarga un solo documento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL DocuSign] a [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Seleccione la cuenta que contiene el documento que desea descargar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID del sobre que desea descargar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Document ID]</p> </td> 
   <td> <p>Introduzca o asigne el ID del documento que desea descargar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificate]</td> 
   <td>Seleccione <strong>[!UICONTROL Yes]</strong> si desea incluir el certificado de firma del sobre en la descarga.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents by User ID]</td> 
   <td>Seleccione <strong>[!UICONTROL Yes]</strong> si desea que los destinatarios puedan recuperar documentos por el ID de usuario. Por ejemplo, si un usuario se incluye en dos órdenes de enrutamiento diferentes con distintas visibilidades, al utilizar esta opción se devuelven todos los documentos de ambas rutas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encrypt]</td> 
   <td>Seleccione <strong>[!UICONTROL Yes]</strong> si desea que los bytes de PDF devueltos en la respuesta se cifren para todos los administradores de claves configurados en su cuenta de [!DNL DocuSign].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Seleccione el idioma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show Changes]</td> 
   <td>Cuando se establece en <strong>[!UICONTROL Yes]</strong>, los campos modificados para el PDF devuelto se resaltan en amarillo y las iniciales o firmas opcionales se resaltan en rojo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watermark]</td> 
   <td> <p>Seleccione <strong>[!UICONTROL No]</strong> para quitar la marca de agua de los documentos PDF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un sobre]

Este módulo de acción lee información sobre un sobre en [!DNL DocuSign] mediante el identificador del sobre.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL DocuSign] a [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Seleccione la cuenta que contiene el documento del que desea leer información.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID que contiene el documento del que desea leer información.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Seleccione las propiedades que desea que aparezcan en la salida del módulo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar un archivo en un sobre]

Este módulo carga un archivo especificado en un sobre existente de DocuSign.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL DocuSign] a [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Seleccione la cuenta que contiene el sobre en el que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID del sobre en el que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Seleccione un archivo de origen de un módulo anterior o introduzca el nombre y los datos del archivo de origen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un nuevo sobre]

Este módulo de acción crea un nuevo sobre a partir de una plantilla. Devuelve el ID del nuevo sobre, así como el estado del nuevo sobre.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td>

<td> <p>Para obtener instrucciones sobre la conexión de su cuenta de DocuSign a Workfront Fusion, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a Workfront Fusion</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Account] </td>
   <td> <p>Seleccione la cuenta que contiene el sobre en el que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template]</td>
   <td> <p> Seleccione la plantilla a partir de la que desea crear el nuevo sobre. Las plantillas están disponibles según la [!UICONTROL Account] seleccionada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL After creation]
   </td> 
   <td> <p>Seleccione si desea guardar el sobre como borrador o enviarlo para su firma.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template recipients]</td>
    <td>Seleccione el destinatario de este sobre</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Añadir destinatario al sobre]

Este módulo de acción añade uno o más destinatarios a un sobre existente. Si el sobre ya se ha enviado, se envía un correo electrónico al destinatario. Este módulo no es válido para sobres que ya se han completado.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de DocuSign a Workfront Fusion, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a Workfront Fusion</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Account] </td>
   <td> <p>Seleccione la cuenta que contiene el sobre en el que desea añadir destinatarios.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Envelope ID]</td>
    <td>Seleccione o asigne el ID del sobre en el que desea añadir el destinatario.</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL Recipient type]</td>
   <td> <p> Seleccione el tipo de destinatario que desea añadir al sobre.</p> 
    <ul> 
     <li> <p>[!UICONTROL Agent]</p> </li> 
     <li> <p>[!UICONTROL Carbon copy]</p> </li> 
     <li> <p>[!UICONTROL Certified delivery]</p> </li> 
     <li> <p>[!UICONTROL In-person signer]</p> </li> 
     <li> <p>[!UICONTROL Intermediary]</p> </li> 
     <li> <p>[!UICONTROL Signer]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Email]</td>
   <td> <p>Introduzca o asigne la dirección de correo electrónico del destinatario que desea añadir al sobre.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Name]</td>
   <td>Introduzca o asigne el nombre del destinatario que desea añadir al sobre.</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Routing order]</td>
   <td> <p>Introduzca o asigne el número de enrutamiento del destinatario. El número de enrutamiento determina el orden en que los destinatarios reciben y firman los documentos.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Email body]</td>
   <td>Introduzca o asigne el cuerpo (contenido) del correo electrónico que se envía al destinatario.</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL Email subject]</td>
   <td>Introduzca o asigne el asunto del correo electrónico que se envía al destinatario.</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL Private message]</td>
   <td> <li> <p>Solo el destinatario seleccionado ve el mensaje privado, así como el mensaje general. El mensaje privado tiene un límite de 1000 caracteres.</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Authentication]</td> 
   <td> <p>Seleccione el método de autenticación que desee utilizar para confirmar la identidad del destinatario.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL None]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Access code]</strong> </p> <p>Introduzca o asigne el código de acceso.</p> </li> 
     <li> <p><strong>[!UICONTROL Phone]</strong> </p> <p>Introduzca o asigne el número de teléfono</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>Introduzca o asigne el número de teléfono</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add custom field]

Este módulo de acción añade un campo personalizado al documento

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL DocuSign] a [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Seleccione la cuenta que contiene el documento en el que desea añadir un campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID del sobre que contiene el documento en el que desea añadir un campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field name]</td> 
   <td>Introduzca o asigne un nombre para el nuevo campo que desea añadir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Required]</td> 
   <td>Habilite esta opción si desea que el campo añadido sea un campo obligatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show field]</td> 
   <td>Habilite esta opción si desea que el campo sea visible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>Introduzca o asigne el valor (contenido) del campo añadido. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modificar campo personalizado]

Este módulo de acción modifica un campo personalizado mediante el nombre del campo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL DocuSign] a [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Seleccione la cuenta que contiene el documento en el que desea modificar un campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID del sobre que contiene el documento en el que desea modificar un campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field ID]</td> 
   <td>Introduzca o asigne el ID del campo que desea modificar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field name]</td> 
   <td>Introduzca o asigne el nombre del campo que desea modificar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Required]</td> 
   <td>Habilite esta opción si desea que el campo modificado sea obligatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show field]</td> 
   <td>Habilite esta opción si desea que el campo sea visible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>Introduzca o asigne el valor (contenido) del campo modificado. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Send envelope]

Este módulo de acción envía un sobre borrador a sus destinatarios.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL DocuSign] a [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Conectar [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>Seleccione la cuenta que contiene el sobre borrador que desea enviar a sus destinatarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID del sobre borrador que desea enviar a sus destinatarios.</p> </td> 
  </tr> 
 </tbody> 
</table>
