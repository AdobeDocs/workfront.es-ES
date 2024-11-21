---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Correo electrónico de Microsoft Office 365
description: En  [!DNL Adobe Workfront Fusion] un escenario, puede automatizar los flujos de trabajo que utilizan el correo electrónico de Microsoft Office 365, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2723'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que usan el [!UICONTROL correo electrónico de Microsoft Office 365], así como conectarlo a varias aplicaciones y servicios de terceros.

Para usar [!UICONTROL Correo electrónico de Office 365] con [!DNL Adobe Workfront Fusion], es necesario tener una [!UICONTROL cuenta de Office 365]. Puede crear uno en www.office.com.

Para obtener instrucciones sobre cómo conectar tu cuenta de [!UICONTROL Office 365] a [!DNL Workfront Fusion], consulta [Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

Después de dar su consentimiento, se le redirigirá a la página de administración de [!UICONTROL Workfront Fusion], donde podrá continuar creando su escenario.

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

Para usar módulos de [!DNL Microsoft Office 365 Email], debe tener una cuenta de [!DNL Microsoft Office 365 Email].

## Información de API de correo electrónico de Microsoft Office 365

El conector de correo electrónico de Microsoft Office 365 utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> Versión 1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 2.6.5</td> 
  </tr>
 </tbody> 
 </table>



## Conectando el servicio [!DNL Office 365 Email] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar tu cuenta de [!DNL Office 365 Email] a [!UICONTROL Workfront Fusion], consulta [Crear una conexión a [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Algunas aplicaciones de Microsoft utilizan la misma conexión, que está vinculada a permisos de usuario individuales. Por lo tanto, al crear una conexión, la pantalla de consentimiento de permisos muestra todos los permisos que se hayan concedido anteriormente a la conexión de este usuario, además de los nuevos permisos necesarios para la aplicación actual.
>
>Por ejemplo, si un usuario tiene permisos de &quot;Leer tabla&quot; concedidos a través del conector de Excel y, a continuación, crea una conexión en el conector de Outlook para leer correos electrónicos, la pantalla de consentimiento de permisos mostrará tanto el permiso de &quot;Leer tabla&quot; ya concedido como el permiso de &quot;Escribir correo electrónico&quot; recién requerido.

## [!DNL Microsoft Office 365 Email] módulos y sus campos

Al configurar [!DNL Microsoft Office 365 Email] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Microsoft Office 365 Email] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Mensaje](#message)
* [Borrador de mensaje](#draft-message)
* [Archivos adjuntos](#attachment)
* [Otro](#other)

### Mensaje

* [[!UICONTROL Crear y enviar un mensaje (heredado)]](#create-and-send-a-message)
* [[!UICONTROL Eliminar un mensaje]](#delete-a-message)
* [[!UICONTROL Obtener un mensaje]](#get-a-message)
* [[!UICONTROL Mover un mensaje]](#move-a-message)
* [[!UICONTROL Buscar mensajes]](#search-messages)
* [[!UICONTROL Ver mensajes]](#watch-messages)



#### [!UICONTROL Crear y enviar un mensaje (heredado)]

Crea y envía un mensaje de correo electrónico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca o asigne la línea de asunto del mensaje.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo de contenido de cuerpo]</td> 
   <td>Seleccione si el contenido del cuerpo del mensaje es HTML o Texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido del cuerpo]</td> 
   <td> <p>Introduzca o asigne el texto del cuerpo del mensaje del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia del correo electrónico</p> 
    <ul> 
     <li>[!UICONTROL Bajo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL A Destinatarios]</p> </td> 
   <td> <p>Añada la dirección de correo electrónico a la que desea enviar los mensajes:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Destinatarios]</p> </td> 
   <td> <p>Añada los destinatarios a los que desea recibir una copia del mensaje:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatarios CCO]</p> </td> 
   <td> <p>Añada los destinatarios que desee copiar en el mensaje, sin permitir que otros destinatarios vean sus nombres o direcciones de correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archivos adjuntos]</p> </td> 
   <td> <p>Agregue los archivos adjuntos al correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre de archivo]</strong> </p> <p>Introduzca el nombre del archivo. Ejemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Datos]</strong> </p> <p>Introduzca los datos del archivo en el campo o asigne el origen del archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados de mensajes de Internet]</td> 
   <td> <p>Añada los encabezados de los mensajes de correo electrónico.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del encabezado</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca un valor para el encabezado.</p> </li> 
    </ul> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca o asigne la línea de asunto del mensaje.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo de contenido de cuerpo]</td> 
   <td>Seleccione si el contenido del cuerpo del mensaje es HTML o Texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido del cuerpo]</td> 
   <td> <p>Introduzca o asigne el texto del cuerpo del mensaje del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia del correo electrónico</p> 
    <ul> 
     <li>[!UICONTROL Bajo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL A Destinatarios]</p> </td> 
   <td> <p>Añada la dirección de correo electrónico a la que desea enviar los mensajes:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Destinatarios]</p> </td> 
   <td> <p>Añada los destinatarios a los que desea recibir una copia del mensaje:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatarios CCO]</p> </td> 
   <td> <p>Añada los destinatarios que desee copiar en el mensaje, sin permitir que otros destinatarios vean sus nombres o direcciones de correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archivos adjuntos]</p> </td> 
   <td> <p>Agregue los archivos adjuntos al correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre de archivo]</strong> </p> <p>Introduzca el nombre del archivo. Ejemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Datos]</strong> </p> <p>Introduzca los datos del archivo en el campo o asigne el origen del archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados de mensajes de Internet]</td> 
   <td> <p>Añada los encabezados de los mensajes de correo electrónico.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del encabezado</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca un valor para el encabezado.</p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL ID de mensaje]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje que desea eliminar.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un mensaje]

Obtiene los metadatos de un mensaje específico

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de mensaje]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje para el que desea recuperar los metadatos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener contenido MIME]</td> 
   <td>Active esta opción para recuperar datos sobre el contenido MIME del mensaje. El contenido de [!UICONTROL MIME] puede incluir imágenes, audio, vídeo u otros tipos de archivos.</td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de mensaje]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje que desea mover a una carpeta diferente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta de correo] </td> 
   <td> <p>Seleccione o asigne el ID de la carpeta a la que desea mover el mensaje.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Carpeta de correo]</td> 
   <td> <p>Seleccione la carpeta que contiene los mensajes que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Buscar]</td> 
   <td>Introduzca la consulta de búsqueda. Para obtener información sobre cómo escribir una consulta de búsqueda, consulte el artículo de soporte técnico de [!DNL Microsoft] <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Buscar correo y personas en [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td> <p>Seleccione cómo desea ordenar los resultados:</p> 
    <ul> 
     <li>[!UICONTROL Asunto (ascendente o descendente)]</li> 
     <li>[!UICONTROL Fecha y hora de creación (ascendente o descendente)]</li> 
     <li>[!UICONTROL Fecha y hora de la última modificación (ascendente o descendente)]</li> 
     <li>[!UICONTROL Fecha y hora de recepción (ascendente o descendente)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca el número máximo de mensajes que [!DNL Workfront Fusion] debe devolver durante un ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver mensajes]

Déclencheur cuando se envía o recibe un nuevo mensaje de correo electrónico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ver mensajes]</p> </td> 
   <td> <p>Seleccione los mensajes que desee ver:</p> 
    <ul> 
     <li>[!UICONTROL Solo no leído]</li> 
     <li>[!UICONTROL Sólo lectura]</li> 
     <li>[!UICONTROL Todo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta de correo]</td> 
   <td> <p>Seleccione la carpeta que contiene los mensajes que desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Buscar]</td> 
   <td>Introduzca la consulta de búsqueda. Para obtener información sobre cómo escribir una consulta de búsqueda, consulte el artículo de soporte técnico de [!DNL Microsoft] <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Buscar correo y personas en [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Introduzca el número máximo de mensajes que [!DNL Workfront Fusion] debe devolver durante un ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Borrador de mensaje

* [Crear un borrador de mensaje](#create-a-draft-message)
* [Enviar un borrador de mensaje](#send-a-draft-message)
* [Actualizar un mensaje](#update-a-message)

#### [!UICONTROL Crear un borrador de mensaje]

Crea un nuevo mensaje de correo electrónico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca la línea de asunto del mensaje.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de contenido de cuerpo]</td> 
   <td>Seleccione si el contenido del cuerpo del mensaje es HTML o Texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido del cuerpo]</td> 
   <td> <p>Introduzca el texto del cuerpo del mensaje del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia del correo electrónico</p> 
    <ul> 
     <li>[!UICONTROL Bajo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL A Destinatarios]</p> </td> 
   <td> <p>Añada los destinatarios a los que desea enviar los mensajes:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Destinatarios]</p> </td> 
   <td> <p>Añada los destinatarios Cuando desee recibir una copia del mensaje:</p> 
    <ul> 
     <li> <p><strong>Nombre</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>Dirección de correo electrónico</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Destinatarios Cco</p> </td> 
   <td> <p>Añada los destinatarios que desee copiar en el mensaje, sin permitir que otros destinatarios vean sus nombres o direcciones de correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archivos adjuntos]</p> </td> 
   <td> <p>Agregue los archivos adjuntos al correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre de archivo]</strong> </p> <p>Introduzca el nombre del archivo. Ejemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Datos]</strong> </p> <p>Introduzca los datos del archivo en el campo o asigne el origen del archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enviar un mensaje de borrador]

Envía un mensaje de correo electrónico que está actualmente en borrador.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de mensaje de borrador]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un ID de mensaje]</td> 
   <td> <p>Seleccione cómo desea identificar el mensaje que se va a actualizar:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Escribir manualmente]</strong> </p> <p>Introduzca o asigne el ID del mensaje.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione la carpeta que contiene el mensaje que desea actualizar y, a continuación, seleccione el mensaje</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca la línea de asunto del mensaje.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido del cuerpo]</td> 
   <td> <p>Introduzca el texto del cuerpo del mensaje del correo electrónico.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia del correo electrónico</p> 
    <ul> 
     <li>[!UICONTROL Bajo]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL A Destinatarios]</p> </td> 
   <td> <p>Añada la dirección de correo electrónico a la que desea enviar los mensajes:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Destinatarios]</p> </td> 
   <td> <p>Añada los destinatarios Cuando desee recibir una copia del mensaje:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Destinatarios CCO]</p> </td> 
   <td> <p>Añada los destinatarios que desee copiar en el mensaje, sin permitir que otros destinatarios vean sus nombres o direcciones de correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Introduzca el nombre del contacto</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección de correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del contacto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archivos adjuntos]</p> </td> 
   <td> <p>Agregue los archivos adjuntos al correo electrónico:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre de archivo]</strong> </p> <p>Introduzca el nombre del archivo. Ejemplo: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Datos]</strong> </p> <p>Introduzca los datos del archivo en el campo o asigne el origen del archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Marcarlo como leído]</td> 
   <td>Active esta opción para marcar el mensaje actualizado como leído.</td> 
  </tr> 
 </tbody> 
</table>

### Archivos adjuntos

* [[!UICONTROL Descargar datos adjuntos]](#download-an-attachment)
* [[!UICONTROL Archivos adjuntos de lista]](#list-attachments)

#### [!UICONTROL Descargar datos adjuntos]

Este módulo descarga el archivo adjunto especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL ID de mensaje]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje que contiene el archivo adjunto que desea descargar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de datos adjuntos]</td> 
   <td> <p>Introduzca o asigne el ID del archivo adjunto que desea descargar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Archivos adjuntos de lista]

Este módulo recupera una lista de archivos adjuntos que pertenecen al mensaje especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de mensaje]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje del que desea recuperar los archivos adjuntos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de archivos adjuntos que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

* [[!UICONTROL Agregar datos adjuntos]](#add-an-attachment)
  <!--Create and send a message-->
* [[!UICONTROL Realizar una llamada API]](#make-an-api-call)

#### [!UICONTROL Agregar datos adjuntos]

Este módulo agrega un archivo adjunto grande a un mensaje.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desde dirección de correo electrónico]</td> 
   <td> <p> Para utilizar una dirección de correo electrónico compartida, introduzca la dirección aquí. El usuario cuyas credenciales se utilizan en la conexión utilizada para este módulo debe tener acceso a la carpeta compartida.<p>Deje este campo en blanco para utilizar la dirección de correo electrónico propia del propietario de la conexión.</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de mensaje]</td> 
   <td> <p> Seleccione o asigne el ID del mensaje al que desea agregar un archivo adjunto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL archivo Source]</td> 
   <td> <p>Seleccione un archivo de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada API]

Este módulo le permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Escriba una ruta relativa a <code>https://graph.microsoft.com</code>. Ejemplo:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Agregue los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] agrega los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
