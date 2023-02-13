---
title: Módulos de ArchiveSign
description: La variable [!DNL Adobe Workfront Fusion DocuSign] los módulos le permiten supervisar y recuperar el estado del sobre, buscar y recuperar sobres, o descargar y enviar un documento para iniciar sesión en su [!DNL DocuSign] cuenta.
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1911'
ht-degree: 0%

---

# Módulos de ArchiveSign

La variable [!DNL Adobe Workfront Fusion] [!DNL DocuSign] los módulos le permiten supervisar y recuperar el estado del sobre, buscar y recuperar sobres, o descargar y enviar un documento para iniciar sesión en su [!DNL DocuSign] cuenta.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar [!DNL DocuSign] módulos, debe tener un [!DNL DocuSign] cuenta.

## Connect [!DNL DocuSign] a [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

Para crear una conexión para su [!DNL DocuSign] módulos:

1. Haga clic en **[!UICONTROL Agregar]** junto a la variable [!UICONTROL Conexión] cuando comience a configurar la primera [!DNL DocuSign] módulo.
1. Introduzca lo siguiente:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td>Escriba un nombre para la nueva [!DNL DocuSign] connection</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de cuenta]</td> 
      <td>Seleccione si la cuenta a la que desea conectarse es una cuenta de producción o una cuenta de demostración.</td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe tal como se describe en [Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] módulos y sus campos

Al configurar [!DNL DocuSign] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL DocuSign] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)

### Déclencheur

#### [!UICONTROL Sobres para observar]

Este módulo de déclencheur inicia un escenario cuando se envía, envía, firma, completa o rechaza un sobre.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL DocuSign] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuenta] </td> 
   <td> <p>Seleccione la cuenta que contiene los registros que desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de evento]</td> 
   <td> <p> Seleccione el tipo de evento que desea ver.</p> 
    <ul> 
     <li>[!UICONTROL Documento completado]</li> 
     <li>[!UICONTROL Documento rechazado]</li> 
     <li>[!UICONTROL Documento enviado]</li> 
     <li>[!UICONTROL Documento firmado]</li> 
     <li>[!UICONTROL Nuevo documento en la bandeja de entrada]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Campos de salida]</p> </td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de registros con los que desea que funcione el módulo durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Descargar un documento]](#download-a-document)
* [[!UICONTROL Leer un sobre]](#read-an-envelope)
* [[!UICONTROL Cargar un archivo a un sobre]](#upload-a-file-to-an-envelope)
* [[!UICONTROL Crear un sobre nuevo]](#create-a-new-envelope)
* [[!UICONTROL Agregar destinatario a sobre]](#add-recipient-to-envelope)
* [[!UICONTROL Añadir campo personalizado]](#add-custom-field)
* [[!UICONTROL Modificar campo personalizado]](#modify-custom-field)
* [[!UICONTROL Enviar sobre]](#send-envelope)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada API personalizada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL DocuSign] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cuenta]</td> 
   <td>Introduzca o asigne la cuenta que desea utilizar para acceder a la [!DNL DocuSign] API.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>Escriba la dirección en el servidor web con el que desea que interactúe el módulo.</p> <p>Puede escribir una dirección URL relativa, lo que significa que no tiene que incluir el protocolo (por ejemplo, <code>http://</code>) al principio. Esto sugiere al servidor web que la interacción se está produciendo en el servidor.</p> <p>Por ejemplo: <code>[!DNL /api/conversations].create</code></p> <p>Sugerencia: Para obtener una lista de los extremos disponibles, consulte la <a href="https://developers.docusign.com/esign-rest-api/reference">[!DNL DocuSign] Referencia de API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Esto determina el tipo de contenido de la solicitud.</p> <p>Por ejemplo,<code> {"Content-type":"application/json"}</code></p> <p>Nota: Si está obteniendo errores y es difícil determinar su origen, considere la posibilidad de modificar los encabezados en función del [!DNL Workfront] documentación. Si su llamada de API personalizada devuelve un error de solicitud HTTP 422, intente utilizar un encabezado "Content-Type":"text/plain".</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de resultados con los que trabajar durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** Sobres de lista
>
>La siguiente llamada de API devuelve sobres a partir de la fecha especificada en el [!DNL DocuSign] cuenta:
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**Método**: `GET`
>
>**Cadena de consulta**:
>
>* **Clave**: `from_date`
>
>* **Valor**: `YYYY-MM-DD`
>
>Especifica cuándo la solicitud comienza a comprobar los cambios de estado para los sobres de la cuenta.
>
>![](assets/example-docusign-setup-350x770.png)
>
>El resultado se puede encontrar en la Salida del módulo en Paquete > Cuerpo > Sobres.
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL DocuSign] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuenta] </td> 
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
   <td>Select <strong>[!UICONTROL Sí]</strong> si desea incluir el certificado de firma de sobre en la descarga.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documentos por ID de usuario]</td> 
   <td>Select <strong>[!UICONTROL Sí]</strong> si desea permitir que los destinatarios recuperen documentos por ID de usuario. Por ejemplo, si un usuario se incluye en dos pedidos de enrutamiento diferentes con distintas visibilidades, el uso de esta opción devuelve todos los documentos de ambas rutas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cifrado]</td> 
   <td>Select <strong>[!UICONTROL Sí]</strong> si desea que los bytes del PDF devueltos en la respuesta se cifren para todos los administradores de claves configurados en su [!DNL DocuSign] cuenta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Seleccione el idioma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar cambios]</td> 
   <td>Cuando se configura como <strong>[!UICONTROL Sí]</strong>, los campos modificados para el PDF devuelto se resaltan en amarillo y las firmas o iniciales opcionales se describen en rojo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marca de agua]</td> 
   <td> <p>Select <strong>[!UICONTROL No]</strong> para quitar la marca de agua de los documentos del PDF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un sobre]

Este módulo de acción lee información sobre un sobre [!DNL DocuSign] uso del ID del sobre.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL DocuSign] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuenta] </td> 
   <td> <p>Seleccione la cuenta que contiene el documento desde el que desea leer la información.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID que contiene el documento del que desea leer la información.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione las propiedades que desee que aparezcan en la salida del módulo. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar un archivo a un sobre]

Este módulo carga un archivo especificado en un sobre existente en Sign.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL DocuSign] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuenta] </td> 
   <td> <p>Seleccione la cuenta que contiene el sobre en el que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID del sobre en el que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td>Seleccione un archivo de origen de un módulo anterior o introduzca el nombre y los datos del archivo de origen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un sobre nuevo]

Este módulo de acción crea un nuevo sobre a partir de una plantilla. Devuelve el ID del nuevo sobre, así como el estado del nuevo sobre.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td>

<td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de Sign a Workfront Fusion, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a Workfront Fusion</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Cuenta] </td>
   <td> <p>Seleccione la cuenta que contiene el sobre en el que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template]</td>
   <td> <p> Seleccione la plantilla desde la que desea crear el nuevo sobre. Las plantillas están disponibles en función de la [!UICONTROL Account] seleccionada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL Después de la creación]
   </td> 
   <td> <p>Seleccione si desea guardar el sobre como borrador o enviarlo para firmarlo.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template recipients]</td>
    <td>Seleccione el destinatario de este sobre</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar destinatario a sobre]

Este módulo de acción agrega uno o más destinatarios a un sobre existente. Si el sobre ya se ha enviado, el destinatario recibe un correo electrónico. Este módulo no es válido para sobres que ya se han completado.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de Sign a Workfront Fusion, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a Workfront Fusion</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Cuenta] </td>
   <td> <p>Seleccione la cuenta que contiene el sobre donde desea agregar destinatarios.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Envelope ID]</td>
    <td>Seleccione o asigne el ID del sobre donde desea añadir el destinatario.</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL Tipo de destinatario]</td>
   <td> <p> Seleccione el tipo de destinatario que desea añadir al sobre.</p> 
    <ul> 
     <li> <p>[!UICONTROL Agent]</p> </li> 
     <li> <p>[!UICONTROL Carbon copy]</p> </li> 
     <li> <p>[!UICONTROL Envío certificado]</p> </li> 
     <li> <p>[!UICONTROL Firmante]</p> </li> 
     <li> <p>[!UICONTROL Intermediario]</p> </li> 
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
    <td>[!UICONTROL Orden de enrutamiento]</td>
   <td> <p>Introduzca o asigne el número de enrutamiento para el destinatario. El número de enrutamiento determina el orden en que los destinatarios reciben y firman los documentos.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Email body]</td>
   <td>Introduzca o asigne el cuerpo (contenido) del correo electrónico que se envía al destinatario.</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL Asunto del correo electrónico]</td>
   <td>Introduzca o asigne el asunto del correo electrónico que se envía al destinatario.</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL Mensaje privado]</td>
   <td> <li> <p>Solo el destinatario seleccionado ve el mensaje privado, así como el mensaje general. El mensaje privado está limitado a 1000 caracteres.</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Autenticación]</td> 
   <td> <p>Seleccione el método de autenticación que desea utilizar para confirmar la identidad del destinatario.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ninguno]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Código de acceso]</strong> </p> <p>Introduzca o asigne el código de acceso.</p> </li> 
     <li> <p><strong>[!UICONTROL Phone]</strong> </p> <p>Escriba o asigne el número de teléfono</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>Escriba o asigne el número de teléfono</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Añadir campo personalizado]

Este módulo de acción agrega un campo personalizado al documento

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL DocuSign] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuenta] </td> 
   <td> <p>Seleccione la cuenta que contiene el documento al que desea agregar un campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID del sobre que contiene el documento al que desea agregar un campo personalizado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field name]</td> 
   <td>Introduzca o asigne un nombre para el nuevo campo que desea agregar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Requerido]</td> 
   <td>Active esta opción si desea que el campo añadido sea obligatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar campo]</td> 
   <td>Active esta opción si desea que el campo esté visible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valor]</td> 
   <td>Introduzca o asigne el valor (contenido) del campo añadido. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modificar campo personalizado]

Este módulo de acción modifica un campo personalizado con el nombre del campo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL DocuSign] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuenta] </td> 
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
   <td role="rowheader">[!UICONTROL Requerido]</td> 
   <td>Active esta opción si desea que el campo modificado sea obligatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar campo]</td> 
   <td>Active esta opción si desea que el campo esté visible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valor]</td> 
   <td>Introduzca o asigne el valor (contenido) del campo modificado. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enviar sobre]

Este módulo de acción envía un sobre borrador a sus destinatarios.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL DocuSign] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuenta] </td> 
   <td> <p>Seleccione la cuenta que contiene el sobre borrador que desea enviar a sus destinatarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> Introduzca o asigne el ID del sobre borrador que desea enviar a sus destinatarios.</p> </td> 
  </tr> 
 </tbody> 
</table>
