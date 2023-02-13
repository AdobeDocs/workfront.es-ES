---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Correo electrónico de Microsoft Office 365
description: En un [!DNL Adobe Workfront Fusion] en este caso, puede automatizar los flujos de trabajo que utilizan el correo electrónico de Microsoft Office 365, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!UICONTROL Correo electrónico de Microsoft Office 365], así como conectarlo a varias aplicaciones y servicios de terceros.

Para usar [!UICONTROL Correo electrónico de Office 365] con [!DNL Adobe Workfront Fusion], es necesario tener un [!UICONTROL Cuenta de Office 365]. Puede crear una en www.office.com.

Para obtener instrucciones sobre cómo conectar su [!UICONTROL Office 365] cuenta para [!DNL Workfront Fusion], consulte [Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

Después de conceder el consentimiento, se le redirige de nuevo a la función [!UICONTROL Workfront Fusion] página de administración donde puede seguir creando su escenario.

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

Para usar [!DNL Microsoft Office 365 Email] módulos, debe tener un [!DNL Microsoft Office 365 Email] cuenta.

## [!DNL Microsoft Office 365 Email] módulos y sus campos

Al configurar [!DNL Microsoft Office 365 Email] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Microsoft Office 365 Email] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Mensaje](#message)
* [Mensaje borrador](#draft-message)
* [Datos adjuntos](#attachment)
* [Otro](#other)

### Mensaje

* [[!UICONTROL Mensajes de Watch]](#watch-messages)
* [[!UICONTROL Buscar mensajes]](#search-messages)
* [[!UICONTROL Obtener un mensaje]](#get-a-message)
* [[!UICONTROL Crear y enviar un mensaje]](#create-and-send-a-message)
* [[!UICONTROL Mover un mensaje]](#move-a-message)
* [[!UICONTROL Eliminar un mensaje]](#delete-a-message)

#### [!UICONTROL Mensajes de Watch]

Déclencheur cuando se envía o recibe un nuevo mensaje de correo electrónico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Watch Messages]</p> </td> 
   <td> <p>Seleccione los mensajes que desee ver:</p> 
    <ul> 
     <li>[!UICONTROL Solo No leído]</li> 
     <li>[!UICONTROL Sólo lectura]</li> 
     <li>[!UICONTROL Todo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Seleccione la carpeta que contiene los mensajes que desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Buscar]</td> 
   <td>Introduzca la consulta de búsqueda. Para obtener información sobre cómo escribir una consulta de búsqueda, consulte la [!DNL Microsoft] artículo de soporte <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Buscar correo y personas en [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Introduzca el número máximo de mensajes [!DNL Workfront Fusion] debe volver durante un ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar mensajes]

Busca mensajes según criterios específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Seleccione la carpeta que contiene los mensajes que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Buscar]</td> 
   <td>Introduzca la consulta de búsqueda. Para obtener información sobre cómo escribir una consulta de búsqueda, consulte la [!DNL Microsoft] artículo de soporte <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Buscar correo y personas en [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>Seleccione cómo desea ordenar los resultados:</p> 
    <ul> 
     <li>[!UICONTROL Asunto (ascendente o descendente)]</li> 
     <li>[!UICONTROL Fecha y hora de creación (ascendente o descendente)]</li> 
     <li>[!UICONTROL Última fecha de modificación (ascendente o descendente)]</li> 
     <li>[!UICONTROL Fecha y hora de recepción (ascendente o descendente)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca el número máximo de mensajes [!DNL Workfront Fusion] debe volver durante un ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un mensaje]

Obtiene los metadatos de un mensaje específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje para el que desea recuperar los metadatos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener contenido MIME]</td> 
   <td>Active esta opción para recuperar datos sobre el contenido MIME del mensaje. El contenido de [!UICONTROL MIME] puede incluir imágenes, audio, vídeo u otros tipos de archivos.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear y enviar un mensaje]

Crea y envía un mensaje de correo electrónico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca o asigne la línea de asunto del mensaje.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo de contenido del cuerpo]</td> 
   <td>Seleccione si el contenido del cuerpo del mensaje es HTML o Texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo contenido]</td> 
   <td> <p>Introduzca o asigne el texto del cuerpo del mensaje del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia del correo electrónico</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Añada la dirección de correo electrónico a la que desea enviar los mensajes:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Escriba el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Añada los destinatarios a los que desee recibir una copia del mensaje:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Escriba el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatarios Cco]</p> </td> 
   <td> <p>Añada los destinatarios que desee copiar en el mensaje, sin permitir que otros destinatarios vean sus nombres o direcciones de correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Escriba el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Añada los archivos adjuntos al correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Introduzca el nombre del archivo. Ejemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Introduzca los datos del archivo en el campo o asigne el origen del archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados de mensajes de Internet]</td> 
   <td> <p>Añada los encabezados de mensaje para el correo electrónico.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Introduzca el nombre del encabezado</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca un valor para el encabezado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un mensaje]

Mueve un mensaje de correo electrónico a una carpeta seleccionada del buzón.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje que desea mover a una carpeta diferente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder] </td> 
   <td> <p>Seleccione o asigne el ID de la carpeta a la que desea mover el mensaje.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un mensaje]

Elimina un mensaje de correo electrónico existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Mensaje borrador

* [Crear un mensaje de borrador](#create-a-draft-message)
* [Enviar un mensaje de borrador](#send-a-draft-message)
* [Actualizar un mensaje](#update-a-message)

#### [!UICONTROL Crear un mensaje de borrador]

Crea un nuevo mensaje de correo electrónico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca la línea de asunto del mensaje.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de contenido del cuerpo]</td> 
   <td>Seleccione si el contenido del cuerpo del mensaje es HTML o Texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo contenido]</td> 
   <td> <p>Introduzca el texto del cuerpo del mensaje del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia del correo electrónico</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Añada los destinatarios a los que desee enviar los mensajes:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Escriba el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Añadir los destinatarios El que desea que reciba una copia del mensaje:</p> 
    <ul> 
     <li> <p><strong>Nombre</strong> </p> <p>Escriba el nombre del contacto</p> </li> 
     <li> <p><strong>Dirección de correo electrónico</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Destinatarios De Cco</p> </td> 
   <td> <p>Añada los destinatarios que desee copiar en el mensaje, sin permitir que otros destinatarios vean sus nombres o direcciones de correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Escriba el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Añada los archivos adjuntos al correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Introduzca el nombre del archivo. Ejemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Introduzca los datos del archivo en el campo o asigne el origen del archivo.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enviar un mensaje de borrador]

Envía un mensaje de correo electrónico que está en borrador.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de mensaje borrador]</td> 
   <td> <p> Seleccione o asigne el ID de mensaje del borrador que desea enviar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un mensaje]

Actualiza un mensaje existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir un ID de mensaje]</td> 
   <td> <p>Seleccione cómo desea identificar el mensaje que desea actualizar:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>Introduzca o asigne el ID del mensaje.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionar de la lista]</strong> </p> <p>Seleccione la carpeta que contiene el mensaje que desea actualizar y, a continuación, seleccione el mensaje</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca la línea de asunto del mensaje.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo contenido]</td> 
   <td> <p>Introduzca el texto del cuerpo del mensaje del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia del correo electrónico</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Añada la dirección de correo electrónico a la que desea enviar los mensajes:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Escriba el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Añadir los destinatarios El que desea que reciba una copia del mensaje:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Escriba el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatarios Cco]</p> </td> 
   <td> <p>Añada los destinatarios que desee copiar en el mensaje, sin permitir que otros destinatarios vean sus nombres o direcciones de correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Escriba el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Añada los archivos adjuntos al correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Introduzca el nombre del archivo. Ejemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Introduzca los datos del archivo en el campo o asigne el origen del archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcarlo como leído]</td> 
   <td>Active esta opción para marcar el mensaje actualizado como leído.</td> 
  </tr> 
 </tbody> 
</table>

### Datos adjuntos

* [[!UICONTROL Archivos adjuntos de lista]](#list-attachments)
* [[!UICONTROL Descargar un archivo adjunto]](#download-an-attachment)

#### [!UICONTROL Archivos adjuntos de lista]

Este módulo recupera una lista de archivos adjuntos pertenecientes al mensaje especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje desde el que desea recuperar los archivos adjuntos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de archivos adjuntos que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un archivo adjunto]

Este módulo descarga el archivo adjunto especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje que contiene el archivo adjunto que desea descargar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de archivo adjunto]</td> 
   <td> <p>Introduzca o asigne el ID del archivo adjunto que desea descargar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

* [[!UICONTROL Realizar una llamada de API]](#make-an-api-call)
* [[!UICONTROL Añadir un archivo adjunto]](#add-an-attachment)

#### [!UICONTROL Realizar una llamada de API]

Este módulo le permite realizar una llamada API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Especifique una ruta relativa a <code>https://graph.microsoft.com</code>. Ejemplo:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de un objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Añadir un archivo adjunto]

Este módulo añade un archivo adjunto grande a un mensaje.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje al que desea añadir un archivo adjunto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>
