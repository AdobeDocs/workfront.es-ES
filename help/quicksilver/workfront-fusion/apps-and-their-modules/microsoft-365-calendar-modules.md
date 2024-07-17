---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: conector
navigation-topic: apps-and-their-modules
title: Calendario de Microsoft Office 365
description: En  [!DNL Adobe Workfront Fusion] un escenario, puede automatizar los flujos de trabajo que usan Microsoft Office 365 Calendar, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1999'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Microsoft Office 365 Calendar], así como conectarlo a varias aplicaciones y servicios de terceros.

Para usar [!DNL Office 365 Calendar] con [!DNL Adobe Workfront Fusion], es necesario tener una cuenta de [!DNL Office 365 Excel]. Puede crear uno en [www.office.com](https://www.office.com/).

Para obtener instrucciones acerca de cómo conectar su cuenta de Office 365 a [!DNL Workfront Fusion], vea [Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

Para usar módulos de [!DNL Microsoft Office 365 Calendar], debe tener una cuenta de [!DNL Microsoft Office 365 Calendar].

## Conectando el servicio [!DNL Office 365 Calendar] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar tu cuenta de [!DNL Office 365 Calendar] a [!UICONTROL Workfront Fusion], consulta [Crear una conexión a [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Algunas aplicaciones de Microsoft utilizan la misma conexión, que está vinculada a permisos de usuario individuales. Por lo tanto, al crear una conexión, la pantalla de consentimiento de permisos muestra todos los permisos que se hayan concedido anteriormente a la conexión de este usuario, además de los nuevos permisos necesarios para la aplicación actual.
>
>Por ejemplo, si un usuario tiene permisos de &quot;Leer tabla&quot; concedidos a través del conector de Excel y, a continuación, crea una conexión en el conector de Outlook para leer correos electrónicos, la pantalla de consentimiento de permisos mostrará tanto el permiso de &quot;Leer tabla&quot; ya concedido como el permiso de &quot;Escribir correo electrónico&quot; recién requerido.

## [!DNL Microsoft Office 365 Calendar] módulos y sus campos

Al configurar [!DNL Microsoft Office 365 Calendar] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Microsoft Office 365 Calendar] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Evento](#event)
* [Calendario](#calendar)
* [Otro](#other)

### Evento

* [[!UICONTROL Ver eventos]](#watch-events)
* [[!UICONTROL Buscar eventos]](#search-events)
* [[!UICONTROL Obtener un evento]](#get-an-event)
* [[!UICONTROL Crear un evento]](#create-an-event)
* [[!UICONTROL Actualizar un evento]](#update-an-event)
* [[!UICONTROL Eliminar un evento]](#delete-an-event)

#### [!UICONTROL Ver eventos]

Este módulo de déclencheur recupera los detalles de un evento cuando el evento se crea, actualiza, elimina, inicia o finaliza en el calendario seleccionado.

>[!NOTE]
>
>Para buscar ocurrencias eliminadas de una serie de eventos, seleccione [!UICONTROL Por hora de actualización] en el campo [!UICONTROL Ver eventos]. Este módulo no inspecciona los eventos únicos eliminados ni las series de eventos eliminadas.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ver eventos]</td> 
   <td> <p>Seleccione cómo desea ver los eventos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Por Hora De Creación]</strong> </p> <p>Esté atento a los nuevos eventos.</p> </li> 
     <li> <p><strong>[!UICONTROL Por Hora De Actualización]</strong> </p> <p>Vea los eventos actualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de grupo de calendario]</td> 
   <td>Seleccione el [!UICONTROL grupo de calendarios] que contiene el calendario en el que desea ver los eventos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendario]</td> 
   <td> <p>Seleccione el calendario específico que desee ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Establezca las condiciones de filtro para filtrar los resultados por asunto, ID de evento o cuerpo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca el número máximo de mensajes que [!DNL Workfront Fusion] debe devolver durante un ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar eventos]

Este módulo de búsqueda recupera los detalles de un evento cuando este se crea, actualiza, elimina, inicia o finaliza en el calendario seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de grupo de calendario]</td> 
   <td>Seleccione el [!UICONTROL grupo de calendarios] que contiene el calendario en el que desea ver los eventos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendario]</td> 
   <td> <p>Seleccione el calendario específico que desee ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Establezca las condiciones de filtro para filtrar los resultados. Puede filtrar por las siguientes propiedades:</p> 
    <ul> 
     <li>[!UICONTROL Asunto]</li> 
     <li>[!UICONTROL ID de evento]</li> 
     <li>[!UICONTROL Fecha y hora de creación]</li> 
     <li>[!UICONTROL Fecha y hora de la última modificación]</li> 
     <li>[!UICONTROL Vista previa del cuerpo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td> <p>Seleccione cómo desea ordenar los resultados.</p> 
    <ul> 
     <li><strong>[!UICONTROL Asunto]</strong>, ascendente o descendente</li> 
     <li><strong>[!UICONTROL Fecha y hora de creación]</strong>, ascendente o descendente</li> 
     <li><strong>[!UICONTROL Última fecha y hora de modificación]</strong>, ascendente o descendente</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Introduzca el número máximo de eventos que [!DNL Workfront Fusion] debe devolver durante un ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un evento]

Este módulo de acción recupera detalles del evento especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de evento]</td> 
   <td> <p>Introduzca o asigne el ID del evento del que desea obtener detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un evento]

Este módulo de acción crea un nuevo evento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca o asigne un título para el evento creado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de inicio]</td> 
   <td> Introduzca un único punto de tiempo en el que el evento se inicia en una representación combinada de fecha y hora. Use el formato <code>({date}T{time}</code>; por ejemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de finalización]</td> 
   <td> Introduzca un único punto de tiempo en el que el evento termina en una representación combinada de fecha y hora. Use el formato <code>{date}T{time}</code>; por ejemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Recordatorio de [!UICONTROL activado]</td> 
   <td>Seleccione si desea activar un recordatorio para este evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recordatorio]</td> 
   <td>Introduzca o asigne el número de minutos antes del inicio del evento en el que debe producirse el déclencheur del recordatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia de este evento.</p> 
    <ul> 
     <li>[!UICONTROL Bajo]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensibilidad] </td> 
   <td> <p>Seleccione la confidencialidad de este evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Please treatment this as Personal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Privado]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Please treatment this as Private]". Las reglas de la bandeja de entrada del destinatario no reenvían ni redirigen este evento.</p> </li> 
     <li> <p><strong>[!UICONTROL confidencial]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Please treatment this as Confidential]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de contenido de cuerpo]</td> 
   <td>Seleccione si el contenido del cuerpo es texto sin formato o HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido del cuerpo]</td> 
   <td>Introduzca o asigne el cuerpo del mensaje asociado al evento. Puede tener formato de HTML o texto (como se especifica en el campo [!UICONTROL Body Content Type] anterior).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ubicación]</td> 
   <td> <p>Introduzca los detalles de ubicación del evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Respuesta solicitada]</td> 
   <td>Seleccione <strong>[!UICONTROL Yes]</strong> para solicitar al invitado que envíe una respuesta a la invitación del evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar como]</td> 
   <td> <p>Seleccione cómo desea que aparezca el evento para las personas que vean el calendario.</p> 
    <ul> 
     <li>[!UICONTROL Gratis]</li> 
     <li>[!UICONTROL Provisional]</li> 
     <li>[!UICONTROL Ocupado]</li> 
     <li>[!UICONTROL Fuera de la oficina]</li> 
     <li>[!UICONTROL Trabajar en otra parte]</li> 
     <li>[!UICONTROL Desconocido]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Asistentes]</p> </td> 
   <td> <p>Agregue los asistentes al evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Escriba el nombre del asistente.</p> </li> 
     <li> <p><strong>[!UICONTROL Correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del asistente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoría]</td> 
   <td>Escriba o asigne las categorías que desea que el evento muestre como en el calendario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un evento]

Este módulo de acción actualiza un evento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de evento]</td> 
   <td>Introduzca, asigne o seleccione el ID del evento que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca o asigne un título para el evento creado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de inicio]</td> 
   <td> Introduzca un único punto de tiempo en el que el evento se inicia en una representación combinada de fecha y hora. Use el formato <code>{date}T{time}</code>; por ejemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de finalización]</td> 
   <td> Introduzca un único punto de tiempo en el que el evento termina en una representación combinada de fecha y hora. Use el formato <code>({date}T{time}</code>; por ejemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Recordatorio de [!UICONTROL activado]</td> 
   <td>Seleccione si desea activar un recordatorio para este evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recordatorio]</td> 
   <td>Introduzca o asigne el número de minutos antes del inicio del evento en el que debe producirse el déclencheur del recordatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia de este evento.</p> 
    <ul> 
     <li>[!UICONTROL Bajo]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL Alta]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensibilidad] </td> 
   <td> <p>Seleccione la confidencialidad de este evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Please treatment this as Personal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Privado]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Please treatment this as Private]". Las reglas de la bandeja de entrada del destinatario no reenvían ni redirigen este evento.</p> </li> 
     <li> <p><strong>[!UICONTROL confidencial]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Please treatment this as Confidential]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de contenido de cuerpo]</td> 
   <td>Seleccione si el contenido del cuerpo del mensaje asociado con el evento es texto sin formato o HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido del cuerpo]</td> 
   <td>Introduzca o asigne el cuerpo del mensaje asociado al evento. Puede tener formato de HTML o texto (como se especifica en el campo [!UICONTROL Body Content Type] anterior).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ubicación]</td> 
   <td> <p>Introduzca los detalles de ubicación del evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Respuesta solicitada]</td> 
   <td>Seleccione <strong>[!UICONTROL Yes]</strong> para solicitar al invitado que envíe una respuesta a la invitación del evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar como]</td> 
   <td> <p>Seleccione cómo desea que aparezca el evento para las personas que vean el calendario.</p> 
    <ul> 
     <li>[!UICONTROL Gratis]</li> 
     <li>[!UICONTROL Provisional]</li> 
     <li>[!UICONTROL Ocupado]</li> 
     <li>[!UICONTROL Fuera de la oficina]</li> 
     <li>[!UICONTROL Trabajar en otra parte]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Asistentes]</p> </td> 
   <td> <p>Agregue los asistentes al evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nombre]</strong> </p> <p>Escriba el nombre del asistente.</p> </li> 
     <li> <p><strong>[!UICONTROL Correo electrónico]</strong> </p> <p>Introduzca la dirección de correo electrónico del asistente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoría]</td> 
   <td>Escriba o asigne las categorías que desea que el evento muestre como en el calendario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un evento]

Este módulo de acción elimina un evento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de evento]</td> 
   <td> <p>Introduzca o asigne el ID del evento que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calendario

* [[!UICONTROL Enumerar calendarios]](#list-calendars)
* [[!UICONTROL Obtener un calendario]](#get-a-calendar)
* [[!UICONTROL Crear un calendario]](#create-a-calendar)
* [[!UICONTROL Actualizar un calendario]](#update-a-calendar)
* [[!UICONTROL Eliminar un calendario]](#delete-a-calendar)

#### [!UICONTROL Enumerar calendarios]

Este módulo de búsqueda recupera una lista de todos los calendarios del usuario autenticado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de grupo de calendario]</td> 
   <td>Seleccione el [!UICONTROL grupo de calendarios] que contiene los calendarios que desea enumerar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Introduzca el número máximo de calendarios que [!DNL Workfront Fusion] debe devolver durante un ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un calendario]

Este módulo de acción recupera detalles sobre un solo calendario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td> <p>Introduzca o asigne el ID del calendario del que desea obtener detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un calendario]

Este módulo de acción crea un nuevo calendario en su cuenta de Google.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de calendario]</td> 
   <td> <p>Escriba un nombre para el nuevo calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un calendario]

Este módulo de acción edita un calendario existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td>Escriba el [!UICONTROL Calendar ID] del calendario que desea actualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre de calendario]</td> 
   <td> <p>Escriba un nombre para el nuevo calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un calendario]

Este módulo de acción elimina un calendario existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td>Escriba el identificador de [!UICONTROL Calendario] del calendario que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

### Otro

#### [!UICONTROL Realizar una llamada API]

Este módulo le permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Escriba una ruta relativa a <code>https://graph.microsoft.com</code>. Ejemplo:<code> /v1.0/me/events</code></p> </td> 
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
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
