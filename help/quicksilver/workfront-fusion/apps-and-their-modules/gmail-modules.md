---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de Gmail
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan Gmail, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1785'
ht-degree: 0%

---

# [!DNL Gmail] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Gmail], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar [!DNL Gmail] módulos, debe tener un [!DNL Gmail] cuenta.

## Connect [!DNL Gmail] a [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connect [!DNL Gmail] a [!DNL Workfront Fusion] uso de [!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connect [!DNL Gmail] a [!DNL Workfront Fusion] using [!DNL gmail.com] o [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connect [!DNL Gmail] a [!DNL Workfront Fusion] using[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

Para obtener instrucciones sobre cómo conectar su [!DNL G Suite] cuenta para [!UICONTROL Workfront Fusion], consulte [Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) en el artículo [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connect [!DNL Gmail] a [!DNL Workfront Fusion] using [!DNL gmail.com] o [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Si [!DNL @gmail.com] o [!DNL @googlemail.com] usuario debe crear un cliente de OAuth en [el [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) para obtener una [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente].

Para obtener instrucciones paso a paso sobre cómo crear el cliente OAuth y obtener un [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente], consulte [Conecte Adobe Workfront Fusion a Google Services mediante un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] módulos y sus campos

Al configurar [!DNL Gmail] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Gmail] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Iteradores](#iterators)

### Déclencheur

#### [!UICONTROL Ver correos electrónicos]

Este módulo de déclencheur ejecuta un escenario cuando se recibe un nuevo correo electrónico para ser procesado.

El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta de correo electrónico que desee ver.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de filtro] </td> 
   <td> <p>Seleccione el tipo de filtro que desea utilizar para ver los correos electrónicos</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtro simple]</strong> </p> <p>Rellene los campos [!UICONTROL Criteria], [!UICONTROL Sender Email Address], [!UICONTROL Subject] y [!UICONTROL Search Phrase]</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail filter]</strong> </p> <p>En el campo [!UICONTROL Query], introduzca la consulta que desea utilizar para filtrar correos electrónicos.</p> <p>Para obtener más información, consulte [!DNL Gmail] filtros, consulte <a href="https://support.google.com/mail/answer/7190">Operadores de búsqueda</a> en el [!DNL Gmail] documentación.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criterios]</td> 
   <td>Seleccione si desea ver los correos electrónicos de [!UICONTROL all email], [!UICONTROL only read emails] o [!UICONTROL only unread].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dirección de correo electrónico del remitente]</td> 
   <td> <p> Introduzca una dirección de correo electrónico para ver solo los correos electrónicos enviados desde esa dirección.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asunto]</td> 
   <td>Introduzca una cadena de texto para ver solo los correos electrónicos que tengan esa cadena de texto en el asunto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Palabra de búsqueda]</td> 
   <td>Introduzca una cadena de texto para ver solo los correos electrónicos que tengan esa cadena de texto en cualquier parte del correo electrónico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Marcar mensajes de correo electrónico como leídos al recuperarlos]</td> 
   <td> <p> Active esta opción para marcar los correos electrónicos recuperados como leídos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Enviar un correo electrónico]](#send-an-email)
* [[!UICONTROL Crear un borrador]](#create-a-draft)
* [[!UICONTROL Marcar un correo electrónico como leído]](#mark-an-email-as-read)
* [[!UICONTROL Marcar un correo electrónico como no leído]](#mark-an-email-as-unread)
* [[!UICONTROL Mover un correo electrónico]](#move-an-email)
* [[!UICONTROL Copiar un correo electrónico]](#copy-an-email)
* [[!UICONTROL Eliminar un correo electrónico]](#delete-an-email)
* [[!UICONTROL Modificación de las etiquetas de correo electrónico]](#modify-email-labels)

#### [!UICONTROL Enviar un correo electrónico]

Este módulo de acción envía un nuevo correo electrónico.

Usted especifica el destinatario del correo electrónico.

El módulo devuelve el ID del correo electrónico y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Desde]</td> 
   <td> <p>Introduzca o asigne una dirección de correo electrónico del remitente.</p> <p>Nota: Si introduce una dirección de correo electrónico incorrecta, puede que se produzca un error al enviar un mensaje porque es posible que su cuenta no tenga permiso para enviar correos electrónicos desde una dirección distinta a la suya.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong>y, a continuación, introduzca o asigne la dirección de correo electrónico de cada destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asunto] </td> 
   <td> <p>Introduzca o asigne el asunto del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Introduzca o asigne el contenido del correo electrónico (cuerpo del mensaje). Se permiten etiquetas de HTML.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong> para añadir un archivo adjunto. Puede asignar un archivo de los módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Agregar]</strong>, luego introduzca o asigne la dirección de correo electrónico para cada destinatario de la copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind Copy recipients]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Agregar]</strong>y, a continuación, introduzca o asigne la dirección de correo electrónico para cada destinatario de copia ciega.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un borrador]

Este módulo de acción crea un nuevo borrador de correo electrónico y lo agrega a la carpeta que especifique.

Especifique la carpeta en la que desea crear un borrador.

El módulo devuelve el ID del borrador del correo electrónico y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta en la que desea crear un borrador.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong>y, a continuación, introduzca o asigne la dirección de correo electrónico de cada destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asunto] </td> 
   <td> <p>Introduzca o asigne el asunto del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Introduzca o asigne el contenido del correo electrónico (cuerpo del mensaje). Se permiten etiquetas de HTML.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong> para añadir un archivo adjunto. Puede asignar un archivo de los módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Agregar]</strong>, luego introduzca o asigne la dirección de correo electrónico para cada destinatario de la copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind Copy recipients]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Agregar]</strong>y, a continuación, introduzca o asigne la dirección de correo electrónico para cada destinatario de copia ciega.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar un correo electrónico como leído]

Este módulo de acción marca un correo electrónico como leído.

Especifique el ID del correo electrónico y su carpeta.

El módulo devuelve el ID del correo electrónico y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta que contiene el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> Introduzca o asigne el ID de correo electrónico.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar un correo electrónico como no leído]

Este módulo de acción marca un borrador de correo electrónico o de correo electrónico como no leído.

Especifique el ID del correo electrónico y su carpeta.

El módulo devuelve el ID del correo electrónico y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta que contiene el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)] </td> 
   <td> <p>Introduzca o asigne el ID de correo electrónico del correo electrónico que desea marcar como no leído.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un correo electrónico]

Este módulo de acción mueve un borrador de correo electrónico o correo electrónico a la carpeta que especifique.

Especifique la carpeta, la carpeta de destino y el ID del correo electrónico.

El módulo devuelve el ID del correo electrónico y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta de origen que contiene el correo electrónico que desea mover.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta de destino]</td> 
   <td> <p> Seleccione el [!DNL Gmail] carpeta de destino a la que desea mover el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> Introduzca o asigne el ID de correo electrónico del correo electrónico que desea mover.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar un correo electrónico]

Este módulo de acción copia un borrador de correo electrónico o correo electrónico en una carpeta especificada.

Especifique la carpeta, la carpeta de destino y el ID del correo electrónico.

El módulo devuelve el ID del correo electrónico y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta de origen que contiene el correo electrónico que desea copiar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta de destino]</td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta de destino a la que desea copiar el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p>Introduzca o asigne el ID de correo electrónico del correo electrónico que desea copiar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un correo electrónico]

Este módulo de acción elimina un borrador de correo electrónico o correo electrónico de una carpeta especificada.

El módulo devuelve el ID del correo electrónico y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] ID del mensaje]</p> </td> 
   <td> <p>Introduzca o asigne el ID de correo electrónico del correo electrónico que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanentemente] </td> 
   <td> <p>Active esta opción para permitir que el módulo elimine permanentemente el correo electrónico, en lugar de moverlo a la carpeta de la papelera.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modificación de las etiquetas de correo electrónico]

Este módulo de acción modifica la etiqueta de un mensaje de correo electrónico que especifique.

El módulo devuelve el ID del correo electrónico y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] ID del mensaje]</td> 
   <td> <p> Introduzca o asigne el ID de correo electrónico del correo electrónico que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Etiquetas que añadir]</p> </td> 
   <td> <p>Seleccione o asigne la etiqueta que desee añadir al mensaje de correo electrónico seleccionado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Etiquetas que quitar]</td> 
   <td> <p> Seleccione o asigne la etiqueta que desee eliminar del mensaje de correo electrónico seleccionado.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL Etiqueta para agregar] y [!UICONTROL Etiqueta que se va a quitar] los campos solo cargan etiquetas creadas por el usuario.

### Iteradores

#### [!UICONTROL Iteración de archivos adjuntos]

Puede iterar los archivos adjuntos de los correos electrónicos. Cada archivo adjunto es un paquete separado en la salida del módulo. Para obtener más información, consulte [Módulo de iteración en Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module] </td> 
   <td> <p>Seleccione el módulo desde el que desea iterar los archivos adjuntos. </p> </td> 
  </tr> 
 </tbody> 
</table>
