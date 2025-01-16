---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Google Calendar
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '3889'
ht-degree: 96%

---

# Módulos de [!DNL Google Calendar]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos de calendario de Google](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que usan [!UICONTROL Google Calendar], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, consulte [Módulos de  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar módulos [!DNL Google Calendar], debe tener una cuenta de [!DNL Google].

## Información de API de Google Calendar

El conector Google Calendar utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://www.googleapis.com/calendar/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 5.4.5</td> 
  </tr>
 </tbody> 
 </table>

## Módulos de [!DNL Google Calendar] y sus campos

Al configurar módulos de [!DNL Google Calendar], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Google Calendar] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Eventos](#events)
* [Calendarios](#calendars)
* [Reglas de control de acceso](#access-control-rules)
* [Iteradores (obsoletos)](#iterators-deprecated)
* [Otro](#other)

### Eventos

* [[!UICONTROL Ver eventos]](#watch-events)
* [[!UICONTROL Buscar eventos]](#search-events)
* [[!UICONTROL Obtener un evento]](#get-an-event)
* [[!UICONTROL Crear un evento]](#create-an-event)
* [[!UICONTROL Actualizar un evento]](#update-an-event)
* [[!UICONTROL Eliminar un evento]](#delete-an-event)


#### [!UICONTROL Ver eventos]

Este módulo de activador ejecuta un escenario cuando se añade, actualiza, elimina, inicia o finaliza un nuevo evento en el calendario que especifique. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones acerca de la conexión de la cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>Seleccione el calendario con el que desea que funcione el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch Events]</td> 
   <td> <p>Elija si desea observar eventos por fecha de creación, fecha de actualización, fecha de inicio o fecha de finalización.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show deleted events]</td> 
   <td> <p>Habilite esta opción para incluir eventos que se hayan eliminado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] </td> 
   <td> <p>Introduzca el texto que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Establezca el número máximo de eventos con los que trabaja [!DNL Workfront Fusion] durante un ciclo (el número de repeticiones por escenario ejecutado). Si el valor se establece demasiado alto, la conexión se puede interrumpir en el lado del servicio de terceros proporcionado (tiempo de espera). [!DNL Workfront Fusion] no tiene ninguna influencia en esto. Le recomendamos que establezca un valor menor y defina un valor mayor para el número máximo de ciclos o que ejecute el escenario con más frecuencia.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar eventos]

Este módulo de acción busca un evento en el calendario seleccionado.

Especifique el calendario y los parámetros de la búsqueda.

El módulo devuelve el ID del evento y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obtener instrucciones sobre la conexión de la cuenta de [!DNL Google Calendar] a Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe Workfront Fusion: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione el calendario que desee buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start date]</td> 
   <td> <p> Introduzca o asigne la fecha en la que se inicia el evento. Este módulo también recupera eventos que comienzan antes de esta fecha y que aún se producen en la fecha de inicio introducida. </p> <p>Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End date]</td> 
   <td> <p> Introduzca o asigne la fecha en la que termina el evento. </p> <p> Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Single events]</td> 
   <td> <p> Habilite esta opción para tratar los eventos recurrentes como instancias únicas. Por ejemplo, si tiene una reunión semanal y esta opción está habilitada, el módulo devolverá la reunión de cada semana como un evento independiente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Introduzca o asigne el término de búsqueda por el que desea buscar. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td> <p>Seleccione el orden de los eventos devueltos en el resultado.</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Time]</strong>: ordene por fecha y hora de inicio (orden ascendente). Esto solo está disponible cuando se consultan eventos únicos.</li> 
     <li><strong>[!UICONTROL Updated Time]</strong>: ordene por hora de última modificación (orden ascendente).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Establezca el número máximo de eventos que devuelve [!DNL Workfront Fusion] durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un evento]

Este módulo de acción devuelve los metadatos de un solo evento del calendario especificado.

Especifique el calendario y el evento.

El módulo devuelve el ID del evento y todos los campos asociados, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Introduzca o asigne el ID del calendario que contiene el evento que desea obtener.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Escriba el identificador de evento del evento de [!DNL Google Calendar] existente que desea obtener.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un evento]

Este módulo de acción crea un evento.

Especifique el calendario y los parámetros del evento.

El módulo devuelve el ID del evento y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe Workfront Fusion: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Create an Event]</td> 
   <td> <p>Seleccione cómo desea crear el evento.</p> 
    <ul> 
     <li><b>[!UICONTROL In Detail]</b><p>Esta opción le permite añadir más detalles sobre el evento.<br></p></li> 
     <li><b>[!UICONTROL Quickly]</b><p>Solo es necesario que seleccione el calendario e introduzca un nombre para el evento. Puede incluir detalles de la hora y el lugar en el nombre, y [!DNL Google Calendar] programará el evento para ese lugar y hora.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione el calendario donde desea que aparezca el evento.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Color]</td> 
   <td>Seleccione el color que el evento muestra en el calendario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event name]</td> 
   <td> <p> Introduzca o asigne un nombre para el evento. </p> <p>Nota: Si ha seleccionado [!UICONTROL Quick add] en el campo [!UICONTROL Create an event], puede incluir la fecha y la hora del evento, y [!DNL Workfront Fusion] crea el evento para esa fecha y hora. Ejemplo: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Si seleccionó [!UICONTROL Quick add] pero no incluye una fecha y hora en el nombre del evento, el evento se creará a partir de la hora actual y durará una hora.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL All day event]</td> 
   <td>Active esta opción si el evento dura todo el día (no requiere horas de inicio y finalización).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start date]</td> 
   <td> <p>Si se trata de un evento que dura todo el día, introduzca la fecha de inicio del evento. </p> <p>Para obtener una lista de formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End date]</td> 
   <td> <p> Si se trata de un evento que dura todo el día, introduzca la fecha de finalización del evento. </p> <p>Para obtener una lista de formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Description]</td> 
   <td>Introduzca o asigne una descripción para el evento. Este campo admite HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Location]</td> 
   <td>Introduzca una ubicación para el evento en forma de texto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Use the default reminder settings for this event]</td> 
   <td>Active esta opción para utilizar la configuración de recordatorio predeterminada. Si establece un aviso personalizado en el campo [!UICONTROL Reminder], este valor se establece en No.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reminder] </td> 
   <td> <p>Añada un recordatorio para el evento. Para cada recordatorio, seleccione el método con el que desea que se le recuerde y defina con cuánto tiempo (en minutos) de antelación al evento desea que se le recuerde.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attendees]</td> 
   <td>Añada los asistentes al evento. Para cada asistente, escriba o asigne su nombre y dirección de correo electrónico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show me as]</td> 
   <td>Seleccione si desea que las personas que ven el calendario lo vean como Ocupado o Disponible durante este evento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibility] </td> 
   <td> <p>Seleccione la visibilidad de este evento. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Default]</b></p> <p>El evento tiene la visibilidad que ha establecido en la configuración del calendario.</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>Cualquier persona con la que se comparta el calendario puede ver este evento.</p> </li> 
     <li> <p><b>[!UICONTROL Private]</b></p> <p>Solo los asistentes pueden ver este evento.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notification about the event creation]</td> 
   <td> <p>Seleccione si desea enviar notificaciones sobre la creación de un nuevo evento a todos los invitados, a invitados que no sean de [!DNL Google Calendar] o a nadie.</p> <p>Sugerencia: Recomendamos utilizar la opción [!UICONTROL None] solo en los casos de uso de migración.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Guests can modify the event]</td> 
   <td> <p>Active esta opción si desea que los invitados puedan modificar este evento.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurrence]</td> 
   <td>Añada las reglas de periodicidad que desee aplicar a este evento. Cada regla requiere una lista de líneas [!UICONTROL RRULE], [!UICONTROL EXRULE], [!UICONTROL RDATE] y [!UICONTROL EXDATE] para un evento recurrente. Tenga en cuenta que las líneas [!UICONTROL DTSTART] y [!UICONTROL DTEND] no están permitidas en este campo; las horas de inicio y finalización de los eventos se especifican en los campos de inicio y finalización. Este campo se omite para eventos únicos o instancias de eventos recurrentes. Para obtener más información, consulte <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un evento]

Este módulo de acción cambia un evento existente.

Especifique el calendario y el ID de evento.

El módulo devuelve el ID del evento y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones acerca de la conexión de la cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>Seleccione el calendario con el que desea trabajar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Introduzca el ID de evento del evento de [!DNL Google Calendar] creado anteriormente que desee actualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Puede actualizar la información del evento introduciendo nuevos valores en el campo deseado. Para obtener más información sobre los campos individuales, consulte [[!UICONTROL Crear un evento]](#create-an-event).

#### [!UICONTROL Eliminar un evento]

Este módulo de acción elimina un evento.

Especifique el calendario y el ID de evento.

El módulo devuelve el ID del evento y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione el calendario que contiene el evento que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID]</td> 
   <td> <p> Introduzca el ID de evento de un evento de [!DNL Google Calendar] creado anteriormente que desee eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notification about the event deletion]</td> 
   <td>Seleccione si desea enviar notificaciones sobre la eliminación del evento a todos los invitados, a invitados que no usen [!DNL Google Calendar] o a nadie.</td> 
  </tr> 
 </tbody> 
</table>

### Calendarios

* [[!UICONTROL Lista de calendarios]](#list-calendars)
* [[!UICONTROL Obtener un calendario]](#get-a-calendar)
* [[!UICONTROL Crear un calendario]](#create-a-calendar)
* [[!UICONTROL Actualizar un calendario]](#update-a-calendar)
* [[!UICONTROL Eliminar un calendario]](#delete-a-calendar)
* [[!UICONTROL Borrar un calendario]](#clear-a-calendar)

#### [!UICONTROL Lista de calendarios]

Este módulo de acción devuelve los calendarios de la lista de calendarios de un usuario.

El módulo devuelve el ID del calendario y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Minimum access role]</td> 
   <td> <p>Seleccione la función de acceso mínimo del usuario. El módulo devuelve calendarios basados en esta función de acceso mínimo.</p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: el usuario puede leer información de libre/ocupado. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: el usuario puede leer y modificar eventos y puede acceder a listas de control. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: el usuario puede leer eventos que no son privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: el usuario puede leer y modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show hidden calendars]</td> 
   <td>Active esta opción para incluir los calendarios ocultos en la lista que devuelve el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Establezca el número máximo de calendarios que devuelve [!DNL Workfront Fusion] durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un calendario]

Este módulo de acción recupera un calendario.

Especifique el identificador del calendario que desea recuperar.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione el calendario que desea recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un calendario]

Este módulo de acción crea un nuevo calendario.

Especifique un nombre para el calendario.

El módulo devuelve el ID del calendario y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar name]</td> 
   <td> <p> Introduzca un nombre para el nuevo calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un calendario]

Este módulo de acción actualiza un calendario.

Especifique el identificador del calendario que desea actualizar.

El módulo devuelve el ID del calendario y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione el calendario que desee actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar name]</td> 
   <td> <p> Introduzca un nuevo nombre para el calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un calendario]

Este módulo de acción elimina un calendario.

Especifique el identificador del calendario que desea eliminar.

El módulo devuelve el ID del calendario y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Introduzca o asigne el ID del calendario que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Borrar un calendario]

Este módulo de acción elimina todos los eventos del calendario principal de una cuenta.

Especifique la conexión que se conecta a la cuenta que contiene el calendario que desea borrar.

El módulo devuelve el ID del calendario y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### Reglas de control de acceso

* [[!UICONTROL Lista de reglas de control de acceso]](#list-access-control-rules)
* [[!UICONTROL Obtener una regla de control de acceso]](#get-an-access-control-rule)
* [[!UICONTROL Crear una regla de control de acceso]](#create-an-access-control-rule)
* [[!UICONTROL Actualizar una regla de control de acceso]](#update-an-access-control-rule)
* [[!UICONTROL Eliminar una regla de control de acceso]](#delete-an-access-control-rule)

#### [!UICONTROL Lista de reglas de control de acceso]

Este módulo de acción devuelve las reglas de la lista de control de acceso de un calendario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione el calendario que contiene las reglas de control de acceso que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Establezca el número máximo de resultados que devuelve [!DNL Workfront Fusion] durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener una regla de control de acceso]

Este módulo de acción devuelve los metadatos de una regla de control de acceso.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione el calendario que contiene la regla de control de acceso que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Access control rule ID]</td> 
   <td>Seleccione la regla de control de acceso que desea recuperar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear una regla de control de acceso]

Este módulo de acción crea una nueva regla de control de acceso.

Especifique un nombre para el calendario.

El módulo devuelve el ID de la regla de control de acceso y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione el calendario en que desea crear una regla de control de acceso.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Seleccione la función que desea asignar a la regla de acceso. </p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: el usuario puede leer información de disponibilidad. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: el usuario puede leer y modificar eventos y puede acceder a listas de control. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: el usuario puede leer eventos que no son privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: el usuario puede leer y modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td> <p>Seleccione el tipo de ámbito.  </p> 
    <ul> 
     <li><strong>[!UICONTROL Default]</strong>: el ámbito público. Este es el valor predeterminado. </li> 
     <li><strong>[!UICONTROL User]</strong>: limita el ámbito a un solo usuario. </li> 
     <li><strong>[!UICONTROL Group]</strong>: limita el ámbito a un grupo. </li> 
     <li><strong>[!UICONTROL Domain]</strong>: limita el ámbito a un dominio. </li> 
    </ul> <p>Nota: Los permisos concedidos al ámbito [!UICONTROL Default] o público se aplican a cualquier usuario, autenticado o no.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td>Introduzca la dirección de correo electrónico de un usuario o grupo, o el nombre de un dominio, según el tipo de ámbito.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notifications]</td> 
   <td> <p>Habilite esta opción para enviar notificaciones sobre el cambio de acceso. </p> <p>Nota: No hay notificaciones sobre la eliminación de acceso. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar una regla de control de acceso]

Este módulo de acción actualiza una regla de control de acceso.

Especifique un nombre para el calendario.

El módulo devuelve el ID de la regla de control de acceso y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione el calendario que contiene la regla de control de acceso que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>Seleccione la regla de control de acceso que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Seleccione la función que desea asignar a la regla de acceso. </p> 
    <ul> 
     <li><strong>[!UICONTROL None]</strong>: esta función no proporciona acceso.</li> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: el usuario puede leer información de disponibilidad. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: el usuario puede leer y modificar eventos y puede acceder a listas de control. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: el usuario puede leer eventos que no son privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: el usuario puede leer y modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notifications]</td> 
   <td> <p>Habilite esta opción para enviar notificaciones sobre el cambio de acceso. </p> <p>Nota: No hay notificaciones sobre la eliminación de acceso. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar una regla de control de acceso]

Este módulo de acción elimina una regla de control de acceso.

Especifique un nombre para el calendario.

El módulo devuelve el ID de la regla de control de acceso y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Seleccione o asigne el ID del calendario que contiene la regla de control de acceso que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>Seleccione o asigne el ID de la regla de control de acceso que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

### Iteradores (obsoletos)

Los módulos [!UICONTROL Iterar archivos adjuntos] e [!UICONTROL Iterar asistentes] han quedado obsoletos. Para iterar archivos adjuntos o asistentes, use el módulo [!UICONTROL Control de flujo] > [!UICONTROL Iterador]. Para obtener más información, consulte [Módulo iterador en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### Otro

* [[!UICONTROL Realizar una llamada de API]](#make-an-api-call)
* [[!UICONTROL Información de disponibilidad]](#get-freebusy-information)

#### [!UICONTROL Realizar una llamada API]

Este módulo le permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de la conexión de la cuenta de [!DNL Google Calendar] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe [!DNL Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Introduzca una ruta relativa a <code>https://www.googleapis.com/calendar</code>. Ejemplo: <code>/v3/users/me/calendarList</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Seleccione el método de petición HTTP que necesita para configurar la llamada de la API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] añade los encabezados de autorización en su lugar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Cuando utilice afirmaciones condicionales como <code>if</code> en el JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Información de disponibilidad]

Este módulo de acción devuelve información de disponibilidad para un conjunto de calendarios.

El módulo devuelve el ID del calendario y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obtener instrucciones sobre la conexión de la cuenta de [!DNL Google Calendar] a Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe Workfront Fusion: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minimum time]</td> 
   <td> <p> Introduzca el inicio del intervalo del que desea recuperar información.</p> <p> Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum time]</td> 
   <td> <p> Introduzca el final del intervalo para el que desea recuperar información. </p> <p>Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendars]</td> 
   <td> <p>Para cada calendario del que desee recuperar información, haga clic en <strong>Añadir</strong> y escriba o asigne el identificador de calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Activador de un escenario antes de un evento

Puede activar un escenario en un tiempo especificado antes de un evento con la ayuda de [!DNL Google Calendar] recordatorios de correo electrónico estándar y el módulo [!UICONTROL Webhooks] >[!UICONTROL mailhook personalizado].

1. Use el módulo [!UICONTROL Calendario de Google] >[!UICONTROL Actualizar un evento] para añadir un recordatorio por correo electrónico al evento:

   ![](assets/trigger-scen-before-event-350x209.png)

1. Cree un nuevo escenario a partir del módulo [!UICONTROL Webhooks] >[!UICONTROL mailhook personalizado].

   1. Copie la dirección de correo electrónico del mailhook.
   1. Guarde el escenario y ejecútelo.

1. En [!DNL Gmail], redirija los recordatorios de correo electrónico de [!DNL Google Calendar] a la dirección de correo electrónico del mailhook:

   1. Abra la configuración de **[!UICONTROL [!DNL Gmail]]**.
   1. Abra la pestaña **[!UICONTROL Reenvío y POP/IMAP]**.
   1. Haga clic en **[!UICONTROL Añadir una dirección de reenvío].**
   1. Pegue la dirección de correo electrónico de los mailhooks copiados, haga clic en&#x200B;**[!UICONTROL Siguiente]**, confirme pulsando **[!UICONTROL Continuar]** en la ventana emergente y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

   1. En [!DNL Workfront Fusion], cambie al nuevo escenario que debería finalizar su ejecución al recibir el correo electrónico de confirmación.
   1. Haga clic en la burbuja situada encima del módulo para inspeccionar su salida.
   1. Expanda el elemento `Text` y copie el código de confirmación:

      ![](assets/confirmation-code-350x252.png)

   1. En Gmail, pegue el código de confirmación en el cuadro de edición y haga clic en&#x200B;**[!UICONTROL Verificar]**:

      ![](assets/paste-code-350x46.png)

   1. Abra la pestaña **[!UICONTROL Filtros y direcciones bloqueadas]**.
   1. Haga clic en **[!UICONTROL Crear un nuevo filtro]**.
   1. Configure un filtro para todos los correos electrónicos que provengan de `     calendar-notification@google.com` y haga clic en&#x200B;**[!UICONTROL Crear un filtro]**:
   1. Seleccione **[!UICONTROL Reenviarlo a]** y elija la dirección de correo electrónico de los mailhooks de la lista.
   1. Haga clic en **[!UICONTROL Crear filtro]** para crear el filtro.

1. (Opcional) En [!DNL Workfront Fusion], añada el módulo [!UICONTROL Analizador de texto] > [!UICONTROL Patrón de coincidencia] después del módulo [!UICONTROL Webhooks] >[!UICONTROL Mailhook personalizado] para analizar el código de HTML del correo electrónico y obtener la información que necesite.

   Por ejemplo, puede configurar el módulo de la siguiente manera para obtener el ID del evento:

   *Patrón*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Texto*: el elemento `HTML content` se ha extraído del módulo [!UICONTROL Webhooks] >[!UICONTROL Mailhook personalizado].
