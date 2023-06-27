---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Gmail
description: En un [!DNL Adobe Workfront Fusion] En este escenario, puede automatizar los flujos de trabajo que utilizan Gmail, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1833'
ht-degree: 0%

---

# [!DNL Gmail] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Gmail], así como conectarlo a múltiples aplicaciones y servicios de terceros.

Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar [!DNL Gmail] módulos, debe tener un [!DNL Gmail] cuenta.

## Connect [!DNL Gmail] hasta [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connect [!DNL Gmail] hasta [!DNL Workfront Fusion] usar [!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connect [!DNL Gmail] hasta [!DNL Workfront Fusion] usando [!DNL gmail.com] o [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connect [!DNL Gmail] hasta [!DNL Workfront Fusion] usando[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

Para obtener instrucciones acerca de cómo conectar su [!DNL G Suite] cuenta a [!UICONTROL Workfront Fusion], consulte [Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) en el artículo [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connect [!DNL Gmail] hasta [!DNL Workfront Fusion] usando [!DNL gmail.com] o [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Si es usted [!DNL @gmail.com] o [!DNL @googlemail.com] usuario en el que debe crear un cliente OAuth [el [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) con el fin de obtener una [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente].

Para obtener instrucciones paso a paso sobre cómo crear el cliente de OAuth y obtener una [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente], consulte [Conexión de Adobe Workfront Fusion a Google Services con un cliente de OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] módulos y sus campos

Al configurar [!DNL Gmail] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Gmail] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
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
     <li> <p> <strong>[!UICONTROL Filtro de Gmail]</strong> </p> <p>En el campo [!UICONTROL Query], introduzca la consulta que desea utilizar para filtrar correos electrónicos.</p> <p>Para obtener más información sobre [!DNL Gmail] filtros, consulte <a href="https://support.google.com/mail/answer/7190">Operadores de búsqueda</a> en el [!DNL Gmail] documentación.</p> </li> 
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
   <td> <p> Establezca el número máximo de resultados que [!DNL Workfront Fusion] trabajará con durante un ciclo.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Desde]</td> 
   <td> <p>Introduzca o asigne una dirección de correo electrónico de remitente.</p> <p>Nota: si introduce una dirección de correo electrónico incorrecta, puede producirse un error al enviar un mensaje, ya que es posible que la cuenta no tenga permiso para enviar correos electrónicos desde una dirección diferente a la suya.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Clic <strong>[!UICONTROL Agregar]</strong>y, a continuación, introduzca o asigne la dirección de correo electrónico de cada destinatario.</p> </td> 
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
   <td> <p>Clic <strong>[!UICONTROL Agregar]</strong> para agregar un archivo adjunto. Puede asignar un archivo de los módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copiar destinatarios]</td> 
   <td> <p> Clic <strong>[!UICONTROL Agregar]</strong>, luego introduzca o asigne la dirección de correo electrónico de cada destinatario de la copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatarios de copia ciega]</td> 
   <td> <p> Clic <strong>[!UICONTROL Agregar]</strong>A continuación, introduzca o asigne la dirección de correo electrónico de cada destinatario de copia oculta.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta en la que desea crear un borrador.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL A] </td> 
   <td> <p>Clic <strong>[!UICONTROL Agregar]</strong>y, a continuación, introduzca o asigne la dirección de correo electrónico de cada destinatario.</p> </td> 
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
   <td> <p>Clic <strong>[!UICONTROL Agregar]</strong> para agregar un archivo adjunto. Puede asignar un archivo de los módulos anteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copiar destinatarios]</td> 
   <td> <p> Clic <strong>[!UICONTROL Agregar]</strong>, luego introduzca o asigne la dirección de correo electrónico de cada destinatario de la copia.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatarios de copia ciega]</td> 
   <td> <p> Clic <strong>[!UICONTROL Agregar]</strong>A continuación, introduzca o asigne la dirección de correo electrónico de cada destinatario de copia oculta.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione el [!DNL Gmail] que contiene el correo electrónico.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione el [!DNL Gmail] que contiene el correo electrónico.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta de origen que contiene el correo electrónico que desea mover.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta de destino]</td> 
   <td> <p> Seleccione el [!DNL Gmail] carpeta de destino a la que desea mover el correo electrónico.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta de origen que contiene el correo electrónico que desea copiar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta de destino]</td> 
   <td> <p>Seleccione el [!DNL Gmail] carpeta de destino en la que desea copiar el correo electrónico.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Gmail] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
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
>[!UICONTROL Etiqueta para añadir] y [!UICONTROL Etiqueta para eliminar] los campos solo cargan etiquetas creadas por el usuario.

### Iteradores

#### [!UICONTROL Repetir archivos adjuntos]

Puede repetir los archivos adjuntos del correo electrónico. Cada archivo adjunto es un paquete independiente en la salida del módulo. Para obtener más información, consulte [Módulo iterador en Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Módulo de origen] </td> 
   <td> <p>Seleccione el módulo desde el que desee repetir los archivos adjuntos. </p> </td> 
  </tr> 
 </tbody> 
</table>
