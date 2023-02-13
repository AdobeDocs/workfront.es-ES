---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connector
navigation-topic: apps-and-their-modules
title: Calendario de Microsoft Office 365
description: En un [!DNL Adobe Workfront Fusion] en este caso, puede automatizar los flujos de trabajo que utilizan Microsoft Office 365 Calendar, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1835'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Microsoft Office 365 Calendar], así como conectarlo a varias aplicaciones y servicios de terceros.

Para usar [!DNL Office 365 Calendar] con [!DNL Adobe Workfront Fusion], es necesario tener un [!DNL Office 365 Excel] cuenta. Puede crear una en [www.office.com](http://www.office.com/).

Para obtener instrucciones sobre cómo conectar su cuenta de Office 365 a [!DNL Workfront Fusion], consulte [Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

Para usar [!DNL Microsoft Office 365 Calendar] módulos, debe tener un [!DNL Microsoft Office 365 Calendar] cuenta.

## [!DNL Microsoft Office 365 Calendar] módulos y sus campos

Al configurar [!DNL Microsoft Office 365 Calendar] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Microsoft Office 365 Calendar] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Evento](#event)
* [Calendario](#calendar)
* [Otro](#other)

### Evento

* [[!UICONTROL Eventos de Watch]](#watch-events)
* [[!UICONTROL Eventos de búsqueda]](#search-events)
* [[!UICONTROL Obtener un evento]](#get-an-event)
* [[!UICONTROL Crear un evento]](#create-an-event)
* [[!UICONTROL Actualizar un evento]](#update-an-event)
* [[!UICONTROL Eliminar un evento]](#delete-an-event)

#### [!UICONTROL Eventos de Watch]

Este módulo de déclencheur recupera los detalles de un evento cuando el evento se crea, actualiza, elimina, inicia o finaliza en el calendario seleccionado.

>[!NOTE]
>
>Para buscar ocurrencias eliminadas de una serie de eventos, seleccione [!UICONTROL Por hora de actualización] en el [!UICONTROL Ver eventos] campo . Este módulo no observa eventos individuales eliminados ni series de eventos eliminados.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch events]</td> 
   <td> <p>Seleccione cómo desea ver los eventos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Por Hora De Creación]</strong> </p> <p>Observe los nuevos eventos.</p> </li> 
     <li> <p><strong>[!UICONTROL Por Tiempo Actualizado]</strong> </p> <p>Observe los eventos actualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Seleccione el [!UICONTROL grupo de calendario] que contiene el calendario donde desea ver los eventos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendario]</td> 
   <td> <p>Seleccione el calendario específico que desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Defina las condiciones del filtro para filtrar los resultados por asunto, ID de evento o cuerpo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca el número máximo de mensajes [!DNL Workfront Fusion] debe volver durante un ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eventos de búsqueda]

Este módulo de búsqueda recupera los detalles de un evento cuando el evento se crea, actualiza, elimina, inicia o finaliza en el calendario seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Seleccione el [!UICONTROL grupo de calendario] que contiene el calendario donde desea ver los eventos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendario]</td> 
   <td> <p>Seleccione el calendario específico que desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Establezca las condiciones de filtro para filtrar los resultados. Puede filtrar por las siguientes propiedades:</p> 
    <ul> 
     <li>[!UICONTROL Asunto]</li> 
     <li>[!UICONTROL Event ID]</li> 
     <li>[!UICONTROL Fecha y hora de creación]</li> 
     <li>[!UICONTROL Fecha y hora de la última modificación]</li> 
     <li>[!UICONTROL Body Preview]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>Seleccione cómo desea ordenar los resultados.</p> 
    <ul> 
     <li><strong>[!UICONTROL Asunto]</strong>, ascendente o descendente</li> 
     <li><strong>[!UICONTROL Fecha y hora de creación]</strong>, ascendente o descendente</li> 
     <li><strong>[!UICONTROL Fecha y hora de la última modificación]</strong>, ascendente o descendente</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Especifique el número máximo de eventos [!DNL Workfront Fusion] debe volver durante un ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un evento]

Este módulo de acción recupera los detalles del evento especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Introduzca o asigne el ID del evento sobre el que desea recuperar detalles.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca o asigne un título para el evento creado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de inicio]</td> 
   <td> Introduzca un solo punto de tiempo en el que el evento se inicie en una representación de fecha y hora combinada. Usar el formato <code>({date}T{time}</code>; por ejemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de finalización]</td> 
   <td> Introduzca un solo punto de tiempo en el que el evento termine en una representación de fecha y hora combinada. Usar el formato <code>{date}T{time}</code>; por ejemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recordatorio activado]</td> 
   <td>Seleccione si desea activar un recordatorio para este evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Introduzca o asigne el número de minutos antes del inicio del evento en el que debe producirse el déclencheur del recordatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia de este evento.</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Medio]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Seleccione la sensibilidad de este evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Por favor, trate esto como personal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Privado]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Por favor, trate esto como privado]". Las reglas de la bandeja de entrada del destinatario no reenvían ni redirigen este evento.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidencial]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Por favor, trate esto como confidencial]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de contenido del cuerpo]</td> 
   <td>Seleccione si el contenido del cuerpo es texto sin formato o HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo contenido]</td> 
   <td>Introduzca o asigne el cuerpo del mensaje asociado al evento. Puede estar en formato de texto o HTML (como se especifica en el campo [!UICONTROL Body Content Type] anterior).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Introduzca los detalles de ubicación del evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Respuesta solicitada]</td> 
   <td>Select <strong>[!UICONTROL Sí]</strong> para solicitar al invitado que envíe una respuesta a la invitación del evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar como]</td> 
   <td> <p>Seleccione cómo desea que aparezca el evento para las personas que vean el calendario.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL Tentativo]</li> 
     <li>[!UICONTROL Ocupado]</li> 
     <li>[!UICONTROL Fuera de la oficina]</li> 
     <li>[!UICONTROL Trabajando en otra parte]</li> 
     <li>[!UICONTROL Desconocido]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Asistentes]</p> </td> 
   <td> <p>Agregue asistentes al evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Introduzca el nombre del asistente.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Introduzca la dirección de correo electrónico del asistente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoría]</td> 
   <td>Introduzca o asigne las categorías en las que desea que se muestre el evento en el calendario.</td> 
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
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td>Introduzca, asigne o seleccione el ID del evento que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asunto]</td> 
   <td> <p>Introduzca o asigne un título para el evento creado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de inicio]</td> 
   <td> Introduzca un solo punto de tiempo en el que el evento se inicie en una representación de fecha y hora combinada. Usar el formato <code>{date}T{time}</code>; por ejemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de finalización]</td> 
   <td> Introduzca un solo punto de tiempo en el que el evento termine en una representación de fecha y hora combinada. Usar el formato <code>({date}T{time}</code>; por ejemplo, <code>2017-08-29T04:00:00.0000000</code>. Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recordatorio activado]</td> 
   <td>Seleccione si desea activar un recordatorio para este evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Introduzca o asigne el número de minutos antes del inicio del evento en el que debe producirse el déclencheur del recordatorio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importancia]</td> 
   <td> <p>Seleccione la importancia de este evento.</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Medio]</li> 
     <li>[!UICONTROL Alto]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Seleccione la sensibilidad de este evento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Por favor, trate esto como personal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Privado]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Por favor, trate esto como privado]". Las reglas de la bandeja de entrada del destinatario no reenvían ni redirigen este evento.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidencial]</strong> </p> <p>El destinatario ve un mensaje "[!UICONTROL Por favor, trate esto como confidencial]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de contenido del cuerpo]</td> 
   <td>Seleccione si el contenido del cuerpo del mensaje asociado al evento es de texto sin formato o de HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo contenido]</td> 
   <td>Introduzca o asigne el cuerpo del mensaje asociado al evento. Puede estar en formato de texto o HTML (como se especifica en el campo [!UICONTROL Body Content Type] anterior).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Introduzca los detalles de ubicación del evento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Respuesta solicitada]</td> 
   <td>Select <strong>[!UICONTROL Sí]</strong> para solicitar al invitado que envíe una respuesta a la invitación del evento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar como]</td> 
   <td> <p>Seleccione cómo desea que aparezca el evento para las personas que vean el calendario.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL Tentativo]</li> 
     <li>[!UICONTROL Ocupado]</li> 
     <li>[!UICONTROL Fuera de la oficina]</li> 
     <li>[!UICONTROL Trabajando en otra parte]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Asistentes]</p> </td> 
   <td> <p>Agregue asistentes al evento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Introduzca el nombre del asistente.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Introduzca la dirección de correo electrónico del asistente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Categoría]</td> 
   <td>Introduzca o asigne las categorías en las que desea que se muestre el evento en el calendario.</td> 
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
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Introduzca o asigne el ID del evento que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calendario

* [[!UICONTROL Calendarios de lista]](#list-calendars)
* [[!UICONTROL Obtener un calendario]](#get-a-calendar)
* [[!UICONTROL Crear un calendario]](#create-a-calendar)
* [[!UICONTROL Actualizar un calendario]](#update-a-calendar)
* [[!UICONTROL Eliminar un calendario]](#delete-a-calendar)

#### [!UICONTROL Calendarios de lista]

Este módulo de búsqueda recupera una lista de todos los calendarios del usuario autenticado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Seleccione el [!UICONTROL grupo de calendario] que contiene los calendarios que desea enumerar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Especifique el número máximo de calendarios [!DNL Workfront Fusion] debe volver durante un ciclo de ejecución de escenario.</td> 
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
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td> <p>Introduzca o asigne el ID del calendario del que desea recuperar los detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un calendario]

Este módulo de acción crea un nuevo calendario en la cuenta de Google.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre del calendario]</td> 
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
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td>Introduzca el [!UICONTROL Calendar ID] del calendario que desea actualizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre del calendario]</td> 
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
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td>Introduzca el ID de [!UICONTROL Calendar] del calendario que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

### Otro

#### [!UICONTROL Realizar una llamada de API]

Este módulo le permite realizar una llamada API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Office 365] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Especifique una ruta relativa a <code>https://graph.microsoft.com</code>. Ejemplo:<code> /v1.0/me/events</code></p> </td> 
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
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
