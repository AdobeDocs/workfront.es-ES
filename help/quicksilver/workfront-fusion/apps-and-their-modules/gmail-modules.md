---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Gmail
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1873'
ht-degree: 94%

---

# Módulos de [!DNL Gmail]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos de Gmail](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Gmail], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar los módulos de [!DNL Gmail], debe tener una cuenta de [!DNL Gmail].

## Conectar [!DNL Gmail] a [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Conectar [!DNL Gmail] a [!DNL Workfront Fusion] mediante [!DNL Google Workspace]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Conectar [!DNL Gmail] a [!DNL Workfront Fusion] mediante [!DNL gmail.com] o [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Conectar [!DNL Gmail] a [!DNL Workfront Fusion] mediante [!DNL  Google Workspace] {#connect-gmail-to-workfront-fusion-using-g-suite}

Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Google Workspace] a [!UICONTROL Workfront Fusion], consulte [Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) en el artículo [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Conectar [!DNL Gmail] a [!DNL Workfront Fusion] mediante [!DNL gmail.com] o [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Si es usuario de [!DNL @gmail.com] o [!DNL @googlemail.com], debe crear un cliente de OAuth en [ [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) para obtener un [!UICONTROL ID de cliente] y un [!UICONTROL Secreto de cliente].

Para obtener instrucciones paso a paso sobre cómo crear el cliente OAuth y obtener un [!UICONTROL ID de cliente] y un [!UICONTROL Secreto de cliente], consulte [Conectar Adobe Workfront Fusion a los servicios de Google mediante un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Módulos de [!DNL Gmail] y sus campos

Al configurar módulos de [!DNL Gmail], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Gmail] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Activadores](#triggers)
* [Acciones](#actions)
* [Iteradores](#iterators)

### Activadores

#### [!UICONTROL Ver correos electrónicos]

Este módulo de activación ejecuta un escenario cuando se recibe un nuevo correo electrónico para procesarlo.

El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta de correo electrónico que desee ver.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filter type] </td> 
   <td> <p>Seleccione el tipo de filtro que desea utilizar para ver los correos electrónicos</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Simple filter]</strong> </p> <p>Rellene los campos [!UICONTROL Criteria], [!UICONTROL Sender Email Address], [!UICONTROL Subject] y [!UICONTROL Search Phase]</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail filter]</strong> </p> <p>En el campo [!UICONTROL Query], introduzca la consulta que desea utilizar para filtrar correos electrónicos.</p> <p>Para obtener más información sobre los filtros de [!DNL Gmail], consulte <a href="https://support.google.com/mail/answer/7190">Operadores de búsqueda</a> en la documentación de [!DNL Gmail].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criteria]</td> 
   <td>Seleccione si desea ver [!UICONTROL all email], [!UICONTROL only read emails] o [!UICONTROL only unread] correos electrónicos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sender email address]</td> 
   <td> <p> Introduzca una dirección de correo electrónico para ver solo los correos electrónicos enviados desde esa dirección.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Introduzca una cadena de texto para ver solo los correos electrónicos que tengan esa cadena de texto en el asunto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search phrase]</td> 
   <td>Introduzca una cadena de texto para ver solo los correos electrónicos que tengan esa cadena de texto en cualquier parte del correo electrónico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mark email message(s) as read when fetched]</td> 
   <td> <p> Active esta opción para marcar los correos electrónicos recuperados como leídos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of results]</td> 
   <td> <p> Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Send an email]](#send-an-email)
* [[!UICONTROL Create a draft]](#create-a-draft)
* [[!UICONTROL Mark an email as read]](#mark-an-email-as-read)
* [[!UICONTROL Mark an email as unread]](#mark-an-email-as-unread)
* [[!UICONTROL Move an email]](#move-an-email)
* [[!UICONTROL Copy an email]](#copy-an-email)
* [[!UICONTROL Delete an email]](#delete-an-email)
* [[!UICONTROL Modify email labels]](#modify-email-labels)

#### [!UICONTROL Send an email]

Este módulo de acción envía un nuevo correo electrónico.

Especifique el destinatario del correo electrónico.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL From]</td> 
   <td> <p>Introduzca o asigne una dirección de correo electrónico de remitente.</p> <p>Nota: Si introduce una dirección de correo electrónico incorrecta, puede producirse un error al enviar un mensaje, ya que es posible que la cuenta no tenga permiso para enviar correos electrónicos desde una dirección diferente a la suya.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Introduzca o asigne el asunto del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Introduzca o asigne el contenido del correo electrónico (cuerpo del mensaje). Se permiten las etiquetas HTML.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Add]</strong> para añadir un archivo adjunto. Puede asignar un archivo de los módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario de la copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind copy recipients]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario de la copia oculta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a draft]

Este módulo de acción crea un nuevo borrador de correo electrónico y lo añade a la carpeta que especifique.

Especifique la carpeta en la que desea crear un borrador.

El módulo devuelve el ID del borrador del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta [!DNL Gmail] en la que desea crear un borrador.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Introduzca o asigne el asunto del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Introduzca o asigne el contenido del correo electrónico (cuerpo del mensaje). Se permiten las etiquetas HTML.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Add]</strong> para añadir un archivo adjunto. Puede asignar un archivo de los módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario de la copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind copy recipients]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario de la copia oculta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mark an email as read]

Este módulo de acción marca un correo electrónico como leído.

Especifique el ID del correo electrónico y su carpeta.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta [!DNL Gmail] que contiene el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> Introduzca o asigne el ID de correo electrónico.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mark an email as unread]

Este módulo de acción marca un correo electrónico o borrador de correo electrónico como no leído.

Especifique el ID del correo electrónico y su carpeta.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta [!DNL Gmail] que contiene el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)] </td> 
   <td> <p>Introduzca o asigne el ID de correo electrónico del correo electrónico que desea marcar como no leído.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un correo electrónico]

Este módulo de acción mueve un correo electrónico o un borrador de correo electrónico a la carpeta que especifique.

Usted especifica la carpeta, la carpeta de destino y el ID del correo electrónico.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta de origen [!DNL Gmail] que contiene el correo electrónico que desea mover.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination folder]</td> 
   <td> <p> Seleccione la carpeta de destino [!DNL Gmail] a la que desea mover el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> Introduzca o asigne el ID de correo electrónico del correo electrónico que desea mover.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar un correo electrónico]

Este módulo de acción copia un correo electrónico o un borrador de correo electrónico a la carpeta que especifique.

Usted especifica la carpeta, la carpeta de destino y el ID del correo electrónico.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta de origen [!DNL Gmail] que contiene el correo electrónico que desea copiar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination folder]</td> 
   <td> <p>Seleccione la carpeta de destino [!DNL Gmail] a la que desea copiar el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p>Introduzca o asigne el ID de correo electrónico del correo electrónico que desea copiar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un correo electrónico]

Este módulo de acción elimina un correo electrónico o un borrador de correo electrónico de la carpeta que especifique.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] Message ID]</p> </td> 
   <td> <p>Introduzca o asigne el ID de correo electrónico del correo electrónico que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanently] </td> 
   <td> <p>Habilite esta opción para permitir que el módulo elimine permanentemente el correo electrónico, en lugar de moverlo a la carpeta de papelera.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modificar etiquetas de correo electrónico]

Este módulo de acción modifica la etiqueta de un mensaje de correo electrónico que especifique.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] Message ID]</td> 
   <td> <p> Introduzca o asigne el ID de correo electrónico del correo electrónico que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Labels to add]</p> </td> 
   <td> <p>Seleccione o asigne la etiqueta que desea añadir al mensaje de correo electrónico seleccionado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Labels to remove]</td> 
   <td> <p> Seleccione o asigne la etiqueta que desea eliminar del mensaje de correo electrónico seleccionado.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Los campos [!UICONTROL Etiqueta a añadir] y [!UICONTROL Etiqueta a eliminar] solo cargan etiquetas creadas por el usuario.

### Iteradores

#### [!UICONTROL Iterar archivos adjuntos]

Puede repetir los archivos adjuntos del correo electrónico. Cada archivo adjunto es un paquete independiente en la salida del módulo. Para obtener más información, consulte [Módulo del iterador en Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module] </td> 
   <td> <p>Seleccione el módulo desde el que desee iterar los archivos adjuntos. </p> </td> 
  </tr> 
 </tbody> 
</table>
