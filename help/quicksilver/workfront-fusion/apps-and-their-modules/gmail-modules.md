---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Gmail
description: En un escenario de  [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan Gmail, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 0%

---

# [!DNL Gmail] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Gmail], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td role="rowheader">Product</td> 
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

Para usar módulos de [!DNL Gmail], debe tener una cuenta de [!DNL Gmail].

## Conectar [!DNL Gmail] a [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Conectar [!DNL Gmail] a [!DNL Workfront Fusion] usando [!DNL Google Workspace]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Conectar [!DNL Gmail] a [!DNL Workfront Fusion] usando [!DNL gmail.com] o [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Conectar [!DNL Gmail] a [!DNL Workfront Fusion] mediante [!DNL  Google Workspace] {#connect-gmail-to-workfront-fusion-using-g-suite}

Para obtener instrucciones sobre cómo conectar tu cuenta de [!DNL Google Workspace] a [!UICONTROL Workfront Fusion], consulta [Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) en el artículo [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Conectar [!DNL Gmail] a [!DNL Workfront Fusion] mediante [!DNL gmail.com] o [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Si es un usuario de [!DNL @gmail.com] o [!DNL @googlemail.com], debe crear un cliente de OAuth en [the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) para obtener un [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente].

Para obtener instrucciones paso a paso sobre cómo crear el cliente OAuth y obtener un [!UICONTROL ID de cliente] y un [!UICONTROL Secreto de cliente], consulte [Conectar Adobe Workfront Fusion a los servicios de Google mediante un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] módulos y sus campos

Al configurar [!DNL Gmail] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Gmail] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Iteradores](#iterators)

### Déclencheur

#### [!UICONTROL Ver correos electrónicos]

Este módulo de déclencheur ejecuta un escenario cuando se recibe un nuevo correo electrónico para procesarlo.

El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta de correo electrónico que desee ver.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de filtro] </td> 
   <td> <p>Seleccione el tipo de filtro que desea utilizar para ver los correos electrónicos</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtro simple]</strong> </p> <p>Rellene los campos [!UICONTROL Criterios], [!UICONTROL Dirección de correo electrónico del remitente], [!UICONTROL Asunto] y [!UICONTROL Frase de búsqueda]</p> </li> 
     <li> <p> <strong>[!UICONTROL filtro de Gmail]</strong> </p> <p>En el campo [!UICONTROL Query], introduzca la consulta que desea utilizar para filtrar correos electrónicos.</p> <p>Para obtener más información sobre los filtros de [!DNL Gmail], consulte <a href="https://support.google.com/mail/answer/7190">Operadores de búsqueda</a> en la documentación de [!DNL Gmail].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criterios]</td> 
   <td>Seleccione si desea ver [!UICONTROL todos los correos electrónicos], [!UICONTROL sólo leer correos electrónicos] o [!UICONTROL sólo no leer] correos electrónicos.</td> 
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
   <td>[!UICONTROL Frase de búsqueda]</td> 
   <td>Introduzca una cadena de texto para ver solo los correos electrónicos que tengan esa cadena de texto en cualquier parte del correo electrónico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Marcar los mensajes de correo electrónico como leídos cuando se recuperan]</td> 
   <td> <p> Active esta opción para marcar los correos electrónicos recuperados como leídos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo.</p> </td> 
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
* [[!UICONTROL Modificar etiquetas de correo electrónico]](#modify-email-labels)

#### [!UICONTROL Enviar un correo electrónico]

Este módulo de acción envía un nuevo correo electrónico.

Especifique el destinatario del correo electrónico.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Desde]</td> 
   <td> <p>Introduzca o asigne una dirección de correo electrónico de remitente.</p> <p>Nota: si introduce una dirección de correo electrónico incorrecta, puede producirse un error al enviar un mensaje, ya que es posible que la cuenta no tenga permiso para enviar correos electrónicos desde una dirección diferente a la suya.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asunto] </td> 
   <td> <p>Introduzca o asigne el asunto del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contenido] </td> 
   <td> <p>Introduzca o asigne el contenido del correo electrónico (cuerpo del mensaje). Se permiten las etiquetas de HTML.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivos adjuntos] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong> para agregar un archivo adjunto. Puede asignar un archivo de los módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copiar destinatarios]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario de la copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatarios de copia ciega]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario de la copia ciega.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un borrador]

Este módulo de acción crea un nuevo borrador de correo electrónico y lo añade a la carpeta que especifique.

Especifique la carpeta en la que desea crear un borrador.

El módulo devuelve el ID del borrador del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta [!DNL Gmail] en la que desea crear un borrador.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asunto] </td> 
   <td> <p>Introduzca o asigne el asunto del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contenido] </td> 
   <td> <p>Introduzca o asigne el contenido del correo electrónico (cuerpo del mensaje). Se permiten las etiquetas de HTML.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivos adjuntos] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong> para agregar un archivo adjunto. Puede asignar un archivo de los módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copiar destinatarios]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario de la copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatarios de copia ciega]</td> 
   <td> <p> Haga clic en <strong>[!UICONTROL Add]</strong> y, a continuación, escriba o asigne la dirección de correo electrónico de cada destinatario de la copia ciega.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar un correo electrónico como leído]

Este módulo de acción marca un correo electrónico como leído.

Especifique el ID del correo electrónico y su carpeta.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta [!DNL Gmail] que contiene el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de correo electrónico (UID)]</td> 
   <td> <p> Introduzca o asigne el ID de correo electrónico.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar un correo electrónico como no leído]

Este módulo de acción marca un correo electrónico o borrador de correo electrónico como no leído.

Especifique el ID del correo electrónico y su carpeta.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta [!DNL Gmail] que contiene el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de correo electrónico (UID)] </td> 
   <td> <p>Introduzca o asigne el ID de correo electrónico del correo electrónico que desea marcar como no leído.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un correo electrónico]

Este módulo de acción mueve un correo electrónico o un borrador de correo electrónico a la carpeta que especifique.

Especifique la carpeta, la carpeta de destino y el ID del correo electrónico.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta de origen [!DNL Gmail] que contiene el correo electrónico que desea mover.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta de destino]</td> 
   <td> <p> Seleccione la carpeta de destino [!DNL Gmail] a la que desee mover el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de correo electrónico (UID)]</td> 
   <td> <p> Introduzca o asigne el ID de correo electrónico del correo electrónico que desea mover.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar un correo electrónico]

Este módulo de acción copia un borrador de correo electrónico o correo electrónico en la carpeta que especifique.

Especifique la carpeta, la carpeta de destino y el ID del correo electrónico.

El módulo devuelve el ID del correo electrónico y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta de origen [!DNL Gmail] que contiene el correo electrónico que desea copiar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta de destino]</td> 
   <td> <p>Seleccione la carpeta de destino [!DNL Gmail] en la que desee copiar el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de correo electrónico (UID)]</td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] ID de mensaje]</p> </td> 
   <td> <p>Introduzca o asigne el ID de correo electrónico del correo electrónico que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanentemente] </td> 
   <td> <p>Active esta opción para permitir que el módulo elimine permanentemente el correo electrónico, en lugar de moverlo a la carpeta de papelera.</p> </td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Gmail] a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] ID de mensaje]</td> 
   <td> <p> Introduzca o asigne el ID de correo electrónico del correo electrónico que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Etiquetas para agregar]</p> </td> 
   <td> <p>Seleccione o asigne la etiqueta que desea añadir al mensaje de correo electrónico seleccionado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Etiquetas que quitar]</td> 
   <td> <p> Seleccione o asigne la etiqueta que desea eliminar del mensaje de correo electrónico seleccionado.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL Etiqueta para agregar] y [!UICONTROL Etiqueta para eliminar] campos que solo cargan etiquetas creadas por el usuario.

### Iteradores

#### [!UICONTROL Iterar archivos adjuntos]

Puede repetir los archivos adjuntos del correo electrónico. Cada archivo adjunto es un paquete independiente en la salida del módulo. Para obtener más información, consulte [Módulo iterador en Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module] </td> 
   <td> <p>Seleccione el módulo desde el que desee repetir los archivos adjuntos. </p> </td> 
  </tr> 
 </tbody> 
</table>
