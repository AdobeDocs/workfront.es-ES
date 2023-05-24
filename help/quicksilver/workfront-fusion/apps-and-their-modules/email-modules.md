---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de correo electrónico
description: En un [!DNL Adobe Workfront Fusion] En este escenario, puede conectar su cuenta de correo electrónico a varias aplicaciones y servicios de terceros. Esto le permite descargar correos electrónicos a través de IMAP, enviar correos electrónicos a través de SMTP, crear nuevos borradores, mover y copiar correos electrónicos de una carpeta a otra, marcar correos electrónicos como leídos o no leídos y eliminar correos electrónicos.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: ea19c2a58bac322c804fca3f6bb7d7147efa4d9a
workflow-type: tm+mt
source-wordcount: '2578'
ht-degree: 0%

---

# Módulos de correo electrónico

En un [!DNL Adobe Workfront Fusion] En este escenario, puede conectar su cuenta de correo electrónico a varias aplicaciones y servicios de terceros. Esto le permite descargar correos electrónicos a través de IMAP, enviar correos electrónicos a través de SMTP, crear nuevos borradores, mover y copiar correos electrónicos de una carpeta a otra, marcar correos electrónicos como leídos o no leídos y eliminar correos electrónicos.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conexión del correo electrónico a Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Conectar con Google](#connect-to-google)
* [Conexión a otros servicios de correo electrónico (SMAP)](#connect-to-other-email-services-smap)

### Conectar a [!DNL Google]

Utilice esta opción para crear escenarios con módulos de correo electrónico que requieran una conexión con su [!DNL Google] cuenta. Es una cuenta con ámbitos restringidos.

Puede crear una conexión con su [!DNL Google] directamente desde un módulo de correo electrónico.

1. En cualquier módulo de correo electrónico, haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. Seleccionar **[!DNL Google]** como el tipo de conexión.
1. Introduzca un nombre para la conexión.
1. (Opcional) Introduzca su [!UICONTROL [!DNL Google] ID de cliente] y [!UICONTROL Secreto del cliente].
1. Clic **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

### Conexión a otros servicios de correo electrónico (SMAP)

La conexión SMAP le permite acceder al buzón de forma remota y leer o manipular los mensajes del buzón. La mayoría de los módulos de correo electrónico utilizan la conexión SMAP.

1. En cualquier módulo de correo electrónico, haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. Seleccionar **[!UICONTROL Otros (SMTP)]** como el tipo de conexión.
1. Introduzca una **[!UICONTROL Nombre]** para la conexión.
1. Seleccione su **[!UICONTROL Email provider]** de la lista. Si su proveedor de correo electrónico no está en la lista, seleccione Otro.
1. Introduzca su **[!UICONTROL Correo electrónico]**, **[!UICONTROL Su nombre completo]**, su **[!UICONTROL Nombre de usuario]** y su **[!UICONTROL Contraseña]**.
1. (Condicional) Si su proveedor no está en la lista, escriba su **[!UICONTROL servidor SMTP]** y **[!UICONTROL Puerto]** y especifique si desea hacer lo siguiente **[!UICONTROL Usar una conexión segura (TLS)]**. Para encontrar esta información, consulte la [!UICONTROL Ayuda] para su buzón de correo. Si no dispone de esta información, póngase en contacto con su proveedor de servicios de correo electrónico.
1. Clic **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!UICONTROL Correo electrónico] módulos y sus campos

Al configurar [!UICONTROL Correo electrónico] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, pueden mostrarse campos adicionales en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Es posible que algunos de los campos de correo electrónico ya contengan datos porque los ha utilizado en otro módulo del escenario. Consulte la documentación de ayuda por correo electrónico si necesita información sobre ellos.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>ID único de correo electrónico conocido como[!UICONTROL ID de correo electrónico (UID)]&#39; es el identificador del correo electrónico. El ID de correo electrónico es específico para cada carpeta del correo electrónico.

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Iteradores](#iterators)

### Déclencheur

#### [!UICONTROL Ver correos electrónicos]

Déclencheur cuando se recibe un nuevo correo electrónico para su procesamiento según criterios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de correo electrónico a [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar el correo electrónico a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta que contiene los correos electrónicos que desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criterios]</p> </td> 
   <td> <p>Seleccione los criterios según los cuales quiere ver los correos electrónicos:</p> 
    <ul> 
     <li>[!UICONTROL Todos los correos electrónicos]</li> 
     <li>[!UICONTROL Sólo Leer Correos Electrónicos]</li> 
     <li>[!UICONTROL Solo Correos Electrónicos No Leídos]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dirección de correo electrónico del remitente] </td> 
   <td> <p>Introduzca la dirección de correo electrónico del remitente cuyos correos electrónicos desea ver.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Dirección de correo electrónico del destinatario]</td> 
   <td> <p> Introduzca la dirección de correo electrónico del destinatario cuyos correos electrónicos desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto] </td> 
   <td> <p>Introduzca el asunto del correo electrónico que desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Frase] </td> 
   <td> <p>Introduzca cualquier palabra clave para ver solo los correos electrónicos que contengan frases específicas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcar los mensajes como leídos cuando se recuperan]</td> 
   <td> <p>Active esta opción para marcar el correo electrónico no leído como leído después de recuperar los detalles.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> El número máximo de correos electrónicos [!DNL Workfront Fusion] debe devolverse durante un ciclo de ejecución de escenario.</p> </td> 
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
* [[!UICONTROL Obtener correos electrónicos]](#get-emails)

#### [!UICONTROL Enviar un correo electrónico]

Envía un nuevo correo electrónico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de correo electrónico a [!DNL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar el correo electrónico a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Guardar mensaje después de enviar]</td> 
   <td>Una vez enviado el mensaje de correo electrónico, se guardará en el buzón. Active esta opción si desea guardar los correos electrónicos enviados mediante [!DNL Workfront Fusion] a la <i>[!UICONTROL Correo enviado]</i> u otra carpeta del buzón. Algunos servicios de correo electrónico, como [!DNL Gmail], guarda automáticamente los mensajes enviados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL A] </td> 
   <td> <p>Añada las direcciones de correo electrónico a las que desee enviar el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto] </td> 
   <td> <p>Introduzca o asigne la línea de asunto del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de contenido]</p> </td> 
   <td> <p>Seleccione el tipo de [!UICONTROL content] para el correo electrónico:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Texto sin formato]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido] </td> 
   <td> <p>Introduzca o asigne el contenido del correo electrónico en formato de HTML mediante etiquetas de HTML o en texto sin formato, según lo que elija en el campo [!UICONTROL Content Type].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archivos adjuntos]</p> </td> 
   <td> <p>Agregar un archivo adjunto:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre de archivo]</strong> </p> <p>Introduzca el nombre del archivo. Por ejemplo, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Datos]</strong> </p> <p>Introduzca la ruta a la carpeta para cargar el archivo adjunto.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Introduzca el [!UICONTROL content ID] para insertar el archivo adjunto (imagen) en el contenido.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar destinatario] </td> 
   <td> <p>Introduzca o asigne una o varias direcciones de correo electrónico a las que desee enviar una copia de este correo electrónico. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatario de copia ciega]</td> 
   <td> <p> Introduzca o asigne una o varias direcciones de correo electrónico a las que desee enviar una copia de este correo electrónico sin que aparezcan en él.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Desde] </td> 
   <td> <p>Introduzca o asigne la dirección de correo electrónico (y el nombre, si es necesario) que aparece en el campo [!UICONTROL From] del mensaje. </p> <p>Importante: Utilice la sintaxis correcta: <code>name@email.com</code> o <code>"Name" name@email.com</code>.</p> <p>Nota: Normalmente, [!DNL Workfront Fusion] utiliza la dirección de correo electrónico que especificó al crear la conexión como dirección del remitente. Si introduce cualquier otra dirección de correo electrónico, puede producirse un error al enviar un mensaje, ya que es posible que su cuenta no tenga permiso para enviar correos electrónicos desde una dirección diferente a la suya. Por ejemplo,. <code>test@mail.com</code> o "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Remitente]</p> </td> 
   <td> <p>Escriba o asigne la dirección de correo electrónico que aparece en el campo [!UICONTROL Remitente] del correo electrónico.</p> <p>Sugerencia: Si no está seguro de si desea utilizar este campo o el campo De, le recomendamos que elija el campo De.</p> <p>Importante: Utilice la sintaxis correcta: <code>name@email.com</code> o <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Responder A]</td> 
   <td> <p> Si desea que las respuestas a este correo electrónico se envíen a una dirección diferente a la dirección "de", introduzca la dirección de correo electrónico a la que desea enviar las respuestas a este correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> Si responde a un correo electrónico específico, introduzca o asigne el ID del correo electrónico al que está respondiendo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referencias de [!UICONTROL] </td> 
   <td> <p>Introduzca los ID de mensaje de todas las respuestas del hilo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prioridad]</p> </td> 
   <td> <p>Seleccione la prioridad del correo electrónico:</p> 
    <ul> 
     <li>[!UICONTROL Alta]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Bajo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Encabezados]</p> </td> 
   <td> <p>Añada los encabezados:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Añada la clave. Por ejemplo, [!UICONTROL Remitente], [!UICONTROL Fecha], [!UICONTROL Para], etc.</p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>Introduzca el valor de la clave.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un borrador]

Crea y agrega un nuevo borrador a una carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de correo electrónico a [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar el correo electrónico a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
   <td>Seleccione la carpeta en la que desea crear el borrador del correo electrónico.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL A] </td> 
   <td> <p>Introduzca o asigne la dirección de correo electrónico a la que desea enviar el correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto] </td> 
   <td> <p>Introduzca o asigne la línea de asunto del correo electrónico.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de contenido]</p> </td> 
   <td> <p>Seleccione el tipo de contenido del correo electrónico:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Texto sin formato]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido] </td> 
   <td> <p>Introduzca o asigne el contenido del correo electrónico en formato de HTML mediante etiquetas de HTML o en texto sin formato, según lo que elija en el campo [!UICONTROL Content Type].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archivos adjuntos]</p> </td> 
   <td> <p>Agregar un archivo adjunto:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre de archivo]</strong> </p> <p>Introduzca el nombre del archivo. Por ejemplo, sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Datos]</strong> </p> <p>Introduzca la ruta a la carpeta para cargar el archivo adjunto.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Introduzca el ID de contenido para insertar el archivo adjunto (imagen) en el contenido.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar destinatario] </td> 
   <td> <p>Introduzca o asigne una o varias direcciones de correo electrónico a las que desee enviar una copia de este correo electrónico. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destinatario de copia ciega]</td> 
   <td> <p> Introduzca o asigne una o varias direcciones de correo electrónico a las que desee enviar una copia de este correo electrónico sin que aparezcan en él.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Desde] </td> 
   <td> <p>Introduzca o asigne la dirección de correo electrónico (y el nombre, si es necesario) que aparece en el campo [!UICONTROL From] del mensaje. </p> <p>Importante: Utilice la sintaxis correcta: <code>name@email.com</code> o <code>"Name" name@email.com</code>.</p> <p>Nota: Normalmente, [!DNL Workfront Fusion] utiliza la dirección de correo electrónico que especificó al crear la conexión como dirección del remitente. Si introduce cualquier otra dirección de correo electrónico, puede producirse un error al enviar un mensaje, ya que es posible que su cuenta no tenga permiso para enviar correos electrónicos desde una dirección diferente a la suya. Por ejemplo,. <code>test@mail.com</code> o "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Remitente]</p> </td> 
   <td> <p>Escriba o asigne la dirección de correo electrónico que aparece en el campo [!UICONTROL Remitente] del correo electrónico.</p> <p>Sugerencia: Si no está seguro de si desea utilizar este campo o el campo De, le recomendamos que elija el campo De.</p> <p>Importante: Utilice la sintaxis correcta: <code>name@email.com</code> o <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Responder A]</td> 
   <td> <p> Si desea que las respuestas a este correo electrónico se envíen a una dirección diferente a la dirección "[!UICONTROL from]", introduzca la dirección de correo electrónico a la que desea que se envíen las respuestas a este correo electrónico.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> Si responde a un correo electrónico específico, introduzca o asigne el ID del correo electrónico al que está respondiendo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Referencias de [!UICONTROL] </td> 
   <td> <p>Introduzca los ID de mensaje de todas las respuestas del hilo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Prioridad]</p> </td> 
   <td> <p>Seleccione la prioridad del correo electrónico:</p> 
    <ul> 
     <li>[!UICONTROL Alta]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Bajo]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Encabezados]</p> </td> 
   <td> <p>Añada los encabezados:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Añada la clave. Por ejemplo, Remitente, Fecha, Para, etc.</p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>Introduzca el valor de la clave.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar un correo electrónico como leído]

Marca un correo electrónico o un borrador de una carpeta seleccionada como leído configurando la variable [!UICONTROL Leer] Indicador.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de correo electrónico a [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar el correo electrónico a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
   <td>Seleccione la carpeta del correo electrónico que desea marcar como leído. Ejemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de correo electrónico (UID)]</p> </td> 
   <td> <p>Introduzca el UID de correo electrónico del correo electrónico que desea marcar como leído.</p> <p>Puede obtener el UID del correo electrónico mediante el módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o el módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Marcar un correo electrónico como no leído]

Marca un correo electrónico o un borrador de una carpeta seleccionada como no leído al establecer el indicador No leído.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de correo electrónico a [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar el correo electrónico a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
   <td>Seleccione la carpeta del correo electrónico que desea marcar como no leído. Ejemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de correo electrónico (UID)]</p> </td> 
   <td> <p>Introduzca el UID de correo electrónico del correo electrónico que desea marcar como no leído.</p> <p>Puede obtener el UID del correo electrónico mediante el módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o el módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un correo electrónico]

Mueve un correo electrónico o borrador seleccionado a una carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de correo electrónico a [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar el correo electrónico a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta de origen]</td> 
   <td>Seleccione la carpeta que contiene el correo electrónico desde el que desea mover el correo electrónico. Ejemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta de destino]</td> 
   <td> <p> Seleccione la carpeta a la que desea añadir el correo electrónico. Ejemplo: Trabajo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de correo electrónico (UID)]</p> </td> 
   <td> <p>Introduzca el UID de correo electrónico del correo electrónico que desea mover a la carpeta de destino.</p> <p>Puede obtener el UID del correo electrónico mediante el módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o el módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar un correo electrónico]

Copia un correo electrónico o un borrador en una carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de correo electrónico a [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar el correo electrónico a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta de origen]</td> 
   <td>Seleccione la carpeta desde la que desea copiar el correo electrónico. Ejemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta de destino]</td> 
   <td> <p> Seleccione la carpeta en la que desea copiar el correo electrónico. Ejemplo: Trabajo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de correo electrónico (UID)]</p> </td> 
   <td> <p>Introduzca el UID de correo electrónico del correo electrónico que desea copiar en la carpeta de destino.</p> <p>Puede obtener el UID del correo electrónico mediante el módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o el módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un correo electrónico]

Quita un correo electrónico o un borrador de la carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de correo electrónico a [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar el correo electrónico a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
   <td>Seleccione la carpeta del correo electrónico que desea eliminar. Ejemplo: Principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de correo electrónico (UID)]</p> </td> 
   <td> <p>Introduzca el UID de correo electrónico del correo electrónico que desea eliminar.</p> <p>Puede obtener el UID del correo electrónico mediante el módulo [!UICONTROL Email] &gt;[!UICONTROL Watch Email] o el módulo [!UICONTROL Search Email].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expurgar]</td> 
   <td> <p>Active esta opción para permitir que el módulo quite permanentemente todos los mensajes marcados como [!UICONTROL Eliminado] en el buzón abierto actualmente.</p> <p>Nota: En [!DNL Gmail], este comportamiento se basa en la configuración de la sección [!UICONTROL Settings] &gt;[!UICONTROL Forwarding POP/IMAP in IMAP access].</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener correos electrónicos]

Devuelve correos electrónicos que coinciden con los criterios especificados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de correo electrónico a [!UICONTROL Workfront Fusion], consulte <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Conectar el correo electrónico a [!UICONTROL Workfront Fusion]</a> en este artículo.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta que contiene los correos electrónicos que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcar los mensajes como leídos cuando se recuperan] </td> 
   <td> <p>Active esta opción si desea marcar el correo electrónico no leído como leído después de recuperar los detalles.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criterios]</p> </td> 
   <td> <p>Seleccione los criterios de los correos electrónicos que desea recuperar:</p> 
    <ul> 
     <li>[!UICONTROL Todos los correos electrónicos]</li> 
     <li>[!UICONTROL Sólo Leer Correos Electrónicos]</li> 
     <li>[!UICONTROL Solo Correos Electrónicos No Leídos]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dirección de correo electrónico del remitente] </td> 
   <td> <p>Introduzca o asigne la dirección de correo electrónico del remitente cuyos correos electrónicos desea recuperar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Dirección de correo electrónico del destinatario]</td> 
   <td> <p> Introduzca o asigne la dirección de correo electrónico del destinatario cuyos correos electrónicos desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde la fecha] </td> 
   <td> <p>Introduzca o asigne la fecha para recuperar los correos electrónicos procesados en la fecha especificada o posteriormente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antes de la fecha]</td> 
   <td> <p> Introduzca o asigne la fecha para recuperar los correos electrónicos procesados en la fecha especificada o antes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto] </td> 
   <td> <p>Introduzca o asigne el asunto del correo electrónico que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Frase] </td> 
   <td> <p>Introduzca o asigne cualquier palabra clave para recuperar solo los correos electrónicos que contengan frases específicas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de correo electrónico (UID)]</td> 
   <td> <p> Introduzca el ID de correo electrónico (UID) del correo electrónico cuyos detalles desee recuperar.</p> <p>Puede obtener el UID del correo electrónico utilizando [!DNL Workfront Fusion]Módulo 's[!UICONTROL Ver correo electrónico] o módulo [!UICONTROL Buscar correo electrónico].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Número máximo de resultados]</td> 
   <td> <p> El número máximo de correos electrónicos [!DNL Workfront Fusion] debe devolverse durante un ciclo de ejecución de escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Continuar la ejecución de la ruta aunque el módulo no devuelva resultados]</td> 
   <td> <p> Seleccione si desea continuar ejecutando el módulo aunque no se devuelvan resultados.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Iteradores

#### [!UICONTROL Iterar archivos adjuntos]

Itera los archivos adjuntos recibidos uno a uno.

El módulo iterador de correo electrónico permite administrar los archivos adjuntos de los correos electrónicos por separado. Por ejemplo, puede configurar para ver correos electrónicos para repetir los correos electrónicos con archivos adjuntos y recibir alertas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origen]</td> 
   <td> <p>Seleccione el módulo que genera el correo electrónico con los archivos adjuntos por los que desea iterar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre los iteradores, consulte [Módulo iterador en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
