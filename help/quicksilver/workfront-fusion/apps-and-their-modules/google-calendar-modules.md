---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de calendario de Google
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan Google Calendar, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3773'
ht-degree: 0%

---

# [!DNL Google Calendar] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!UICONTROL Calendario de Google], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar [!DNL Google Calendar] módulos, debe tener un [!DNL Google] cuenta.

## [!DNL Google Calendar] módulos y sus campos

Al configurar [!DNL Google Calendar] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Google Calendar] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Eventos](#events)
* [Calendarios](#calendars)
* [Reglas de control de acceso](#access-control-rules)
* [Iteradores (obsoleto)](#iterators-deprecated)
* [Otro](#other)

### Eventos

* [[!UICONTROL Ver eventos]](#watch-events)
* [[!UICONTROL Eventos de búsqueda]](#search-events)
* [[!UICONTROL Obtener un evento]](#get-an-event)
* [[!UICONTROL Crear un evento]](#create-an-event)
* [[!UICONTROL Actualizar un evento]](#update-an-event)
* [[!UICONTROL Eliminar un evento]](#delete-an-event)


#### [!UICONTROL Ver eventos]

Este módulo de déclencheur ejecuta un escenario cuando se agrega, actualiza, elimina, inicia o finaliza un nuevo evento en el calendario especificado. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendario] </td> 
   <td> <p>Seleccione el calendario con el que desea que funcione el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch Events]</td> 
   <td> <p>Elija si desea ver eventos por Fecha de creación, Fecha de actualización, Fecha de inicio o Fecha de finalización.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar eventos eliminados]</td> 
   <td> <p>Active esta opción para incluir eventos que se hayan eliminado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] </td> 
   <td> <p>Escriba el texto que desee buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p> Establezca el número máximo de eventos que [!DNL Workfront Fusion] funciona con durante un ciclo (el número de repeticiones por ejecución de escenario). Si el valor se establece demasiado alto, la conexión se puede interrumpir en el lado del servicio de terceros dado (tiempo de espera). [!DNL Workfront Fusion] no tiene influencia en esto. Se recomienda establecer un valor inferior y definir un valor mayor para el número máximo de ciclos o ejecutar el escenario con más frecuencia.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eventos de búsqueda]

Este módulo de acción busca un evento en el calendario seleccionado.

El calendario y los parámetros de la búsqueda se especifican.

El módulo devuelve el ID del evento y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta de Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con Adobe Workfront Fusion: Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione el calendario que desee buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de inicio]</td> 
   <td> <p> Introduzca o asigne la fecha en la que se inicia el evento. Este módulo también recupera eventos que comienzan antes de esta fecha y que siguen ocurriendo en la fecha de inicio ingresada. </p> <p>Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de finalización]</td> 
   <td> <p> Introduzca o asigne la fecha en la que finaliza el evento. </p> <p> Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eventos únicos]</td> 
   <td> <p> Active esta opción para tratar eventos recurrentes como instancias únicas. Por ejemplo, si tiene una reunión semanal y esta opción está habilitada, el módulo devuelve la reunión de cada semana como un evento independiente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Escriba o asigne el término de búsqueda por el que desea buscar. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td> <p>Seleccione el orden de los eventos devueltos en el resultado.</p> 
    <ul> 
     <li><strong>[!UICONTROL Hora de inicio]</strong>: Ordenar por fecha y hora de inicio (ascendente). Esto solo está disponible cuando se consultan eventos únicos.</li> 
     <li><strong>[!UICONTROL Tiempo actualizado]</strong>: Ordenar por la última modificación (ascendente).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p>Configurar el número máximo de eventos [!DNL Workfront Fusion] vuelve durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un evento]

Este módulo de acción devuelve los metadatos de un solo evento del calendario especificado.

El calendario y el evento se especifican.

El módulo devuelve el ID del evento y todos los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendario]</td> 
   <td> <p>Introduzca o asigne el ID del calendario que contiene el evento que desea obtener.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Introduzca el ID de evento del [!DNL Google Calendar] que desee obtener.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un evento]

Este módulo de acción crea un evento.

El calendario y los parámetros del evento se especifican.

El módulo devuelve el ID del evento y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta de Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con Adobe Workfront Fusion: Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Crear un evento]</td> 
   <td> <p>Seleccione cómo desea crear el evento.</p> 
    <ul> 
     <li><b>[!UICONTROL En Detalle]</b><p>Esta opción le permite dar más detalles sobre el evento.<br></p></li> 
     <li><b>[!UICONTROL Rápido]</b><p>Solo es necesario seleccionar el calendario e introducir un nombre para el evento. Puede incluir detalles de hora y lugar en el nombre y [!DNL Google Calendar] programará el evento para ese lugar y hora.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione el calendario en el que desea que aparezca el evento.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Color]</td> 
   <td>Seleccione el color que el evento muestre en el calendario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event name]</td> 
   <td> <p> Introduzca o asigne un nombre para el evento. </p> <p>Nota: Si ha seleccionado [!UICONTROL Adición rápida] en el campo [!UICONTROL Crear un evento], puede incluir la fecha y la hora del evento y [!DNL Workfront Fusion] crea el evento para esa fecha y hora. Ejemplo: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Si ha seleccionado [!UICONTROL Adición rápida] pero no incluye una fecha y hora en el nombre del evento, el evento se crea a partir de la hora actual y dura una hora.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Evento de todo el día]</td> 
   <td>Active esta opción si el evento es de todo el día (no requiere hora de inicio y finalización).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de inicio]</td> 
   <td> <p>Si se trata de un evento de todo el día, introduzca la fecha de inicio del evento. </p> <p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de finalización]</td> 
   <td> <p> Si se trata de un evento de todo el día, introduzca la fecha de finalización del evento. </p> <p>Para obtener una lista de los formatos de fecha admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Descripción]</td> 
   <td>Introduzca o asigne una descripción para el evento. Este campo admite HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Location]</td> 
   <td>Introduzca una ubicación para el suceso en el formulario de texto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Usar la configuración de recordatorio predeterminada para este evento]</td> 
   <td>Active esta opción para utilizar la configuración predeterminada de recordatorio. Si establece un recordatorio personalizado en el campo [!UICONTROL Reminder], este valor se establece en No.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reminder] </td> 
   <td> <p>Agregue un recordatorio para el evento. Para cada recordatorio, seleccione el método con el que desea que se le recuerde y defina cuánto tiempo (en minutos) antes del evento que desea que se le recuerde.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Asistentes]</td> 
   <td>Agregue los asistentes al evento. Para cada asistente, introduzca o asigne su nombre y dirección de correo electrónico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar como]</td> 
   <td>Seleccione si desea que las personas que ven el calendario lo vean como Ocupado o Disponible durante este evento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibilidad] </td> 
   <td> <p>Seleccione la visibilidad de este evento. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Predeterminado]</b></p> <p>El evento tiene la visibilidad que ha establecido en la configuración del calendario.</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>Cualquier persona con la que se comparta el calendario puede ver este evento.</p> </li> 
     <li> <p><b>[!UICONTROL Privado]</b></p> <p>Solo los asistentes pueden ver este evento.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificación sobre la creación del evento]</td> 
   <td> <p>Seleccione si desea enviar notificaciones sobre la creación de un nuevo evento a todos los invitados, a los que no sean[!DNL Google Calendar] invitados, o a nadie.</p> <p>Sugerencia: Se recomienda utilizar la opción [!UICONTROL Ninguno] solo para casos de uso de migración.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Los invitados pueden modificar el evento]</td> 
   <td> <p>Active esta opción si desea que los invitados puedan modificar este evento.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurrence]</td> 
   <td>Agregue las reglas de periodicidad que desee aplicar a este evento. Cada regla requiere una lista de líneas [!UICONTROL RULE], [!UICONTROL EXRULE], [!UICONTROL RDATE] y [!UICONTROL EXDATE] para un evento recurrente. Tenga en cuenta que las líneas [!UICONTROL DTSTART] y [!UICONTROL DTEND] no están permitidas en este campo; las horas de inicio y finalización del evento se especifican en los campos de inicio y finalización. Este campo se omite para eventos únicos o instancias de eventos recurrentes. Para obtener más información, consulte <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un evento]

Este módulo de acción cambia un evento existente.

Especifique el ID de calendario y de evento.

El módulo devuelve el ID del evento y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendario] </td> 
   <td> <p>Seleccione el calendario con el que desee trabajar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Introduzca el ID de evento a partir del [!DNL Google Calendar] que desea actualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

Puede actualizar la información del evento introduciendo nuevos valores en el campo deseado. Para obtener más información sobre los campos individuales, consulte [[!UICONTROL Crear un evento]](#create-an-event).

#### [!UICONTROL Eliminar un evento]

Este módulo de acción elimina un evento.

Especifique el ID de calendario y de evento.

El módulo devuelve el ID del evento y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione el calendario que contiene el evento que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID]</td> 
   <td> <p> Introduzca el ID de evento de un [!DNL Google Calendar] que desee eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificación sobre la eliminación del evento]</td> 
   <td>Seleccione si desea enviar notificaciones sobre la eliminación del evento a todos los invitados que no utilicen [!DNL Google Calendar], o nadie.</td> 
  </tr> 
 </tbody> 
</table>

### Calendarios

* [[!UICONTROL Enumerar calendarios]](#list-calendars)
* [[!UICONTROL Obtener un calendario]](#get-a-calendar)
* [[!UICONTROL Crear un calendario]](#create-a-calendar)
* [[!UICONTROL Actualizar un calendario]](#update-a-calendar)
* [[!UICONTROL Eliminar un calendario]](#delete-a-calendar)
* [[!UICONTROL Borrar un calendario]](#clear-a-calendar)

#### [!UICONTROL Enumerar calendarios]

Este módulo de acción devuelve los calendarios de la lista de calendario de un usuario.

El módulo devuelve el ID del calendario y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Función de acceso mínimo]</td> 
   <td> <p>Seleccione la función de acceso mínimo para el usuario. El módulo devuelve calendarios basados en esta función de acceso mínimo.</p> 
    <ul> 
     <li><strong>[!UICONTROL Reader ocupado libre]</strong>: El usuario puede leer información de disponibilidad. </li> 
     <li><strong>[!UICONTROL Propietario]</strong>: El usuario puede leer y modificar eventos y acceder a listas de control. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: El usuario puede leer eventos que no sean privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: El usuario puede leer y modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar calendarios ocultos]</td> 
   <td>Active esta opción para incluir calendarios ocultos en la lista que devuelve el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Configurar el número máximo de calendarios [!DNL Workfront Fusion] vuelve durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un calendario]

Este módulo de acción recupera un calendario.

Especifique el ID del calendario que desea recuperar.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione el calendario que desee recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un calendario]

Este módulo de acción crea un nuevo calendario.

Especifique un nombre para el calendario.

El módulo devuelve el ID del calendario y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre del calendario]</td> 
   <td> <p> Escriba un nombre para el nuevo calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un calendario]

Este módulo de acción actualiza un calendario.

Especifique el ID del calendario que desea actualizar.

El módulo devuelve el ID del calendario y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione el calendario que desee actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre del calendario]</td> 
   <td> <p> Escriba un nuevo nombre para el calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un calendario]

Este módulo de acción elimina un calendario.

Especifique el ID del calendario que desea eliminar.

El módulo devuelve el ID del calendario y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td> <p>Introduzca o asigne el ID del calendario que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Borrar un calendario]

Este módulo de acción elimina todos los eventos del calendario principal de una cuenta.

Especifique la conexión que se conecta a la cuenta que contiene el calendario que desea borrar.

El módulo devuelve el ID del calendario y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### Reglas de control de acceso

* [[!UICONTROL Enumerar reglas de control de acceso]](#list-access-control-rules)
* [[!UICONTROL Obtener una regla de control de acceso]](#get-an-access-control-rule)
* [[!UICONTROL Creación de una regla de control de acceso]](#create-an-access-control-rule)
* [[!UICONTROL Actualizar una regla de control de acceso]](#update-an-access-control-rule)
* [[!UICONTROL Eliminar una regla de control de acceso]](#delete-an-access-control-rule)

#### [!UICONTROL Enumerar reglas de control de acceso]

Este módulo de acción devuelve las reglas de la lista de control de acceso de un calendario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione el calendario que contiene las reglas de control de acceso que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td>Configurar el número máximo de resultados [!DNL Workfront Fusion] vuelve durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener una regla de control de acceso]

Este módulo de acción devuelve los metadatos de una regla de control de acceso.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione el calendario que contiene la regla de control de acceso que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Access control rule ID]</td> 
   <td>Seleccione la regla de control de acceso que desee recuperar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creación de una regla de control de acceso]

Este módulo de acción crea una nueva regla de control de acceso.

Especifique un nombre para el calendario.

El módulo devuelve el ID de la regla de control de acceso y de los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione el calendario en el que desea crear una regla de control de acceso.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rol]</td> 
   <td> <p>Seleccione la función que desea asignar a la regla de acceso. </p> 
    <ul> 
     <li><strong>[!UICONTROL Reader ocupado libre]</strong>: El usuario puede leer información de disponibilidad. </li> 
     <li><strong>[!UICONTROL Propietario]</strong>: El usuario puede leer y modificar eventos y acceder a listas de control. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: El usuario puede leer eventos que no sean privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: El usuario puede leer y modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td> <p>Seleccione el tipo de ámbito. </p> 
    <ul> 
     <li><strong>[!UICONTROL Predeterminado]</strong>: El ámbito público. Este es el valor predeterminado. </li> 
     <li><strong>[!UICONTROL Usuario]</strong>: Limita el ámbito a un solo usuario. </li> 
     <li><strong>[!UICONTROL Group]</strong>: Limita el ámbito a un grupo. </li> 
     <li><strong>[!UICONTROL Domain]</strong>: Limita el ámbito a un dominio. </li> 
    </ul> <p>Nota: Los permisos otorgados al ámbito [!UICONTROL Default], o al público, se aplican a cualquier usuario, autenticado o no.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor]</td> 
   <td>Introduzca la dirección de correo electrónico de un usuario o grupo, o el nombre de un dominio, según el tipo de ámbito.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificaciones]</td> 
   <td> <p>Active esta opción para enviar notificaciones sobre el cambio de acceso. </p> <p>Nota: No hay notificaciones sobre la eliminación del acceso. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar una regla de control de acceso]

Este módulo de acción actualiza una regla de control de acceso.

Especifique un nombre para el calendario.

El módulo devuelve el ID de la regla de control de acceso y de los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione el calendario que contiene la regla de control de acceso que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>Seleccione la regla de control de acceso que desee actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rol]</td> 
   <td> <p>Seleccione la función que desea asignar a la regla de acceso. </p> 
    <ul> 
     <li><strong>[!UICONTROL Ninguno]</strong>: Esta función no proporciona acceso.</li> 
     <li><strong>[!UICONTROL Reader ocupado libre]</strong>: El usuario puede leer información de disponibilidad. </li> 
     <li><strong>[!UICONTROL Propietario]</strong>: El usuario puede leer y modificar eventos y acceder a listas de control. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: El usuario puede leer eventos que no sean privados. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: El usuario puede leer y modificar eventos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enviar notificaciones]</td> 
   <td> <p>Active esta opción para enviar notificaciones sobre el cambio de acceso. </p> <p>Nota: No hay notificaciones sobre la eliminación del acceso. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar una regla de control de acceso]

Este módulo de acción elimina una regla de control de acceso.

Especifique un nombre para el calendario.

El módulo devuelve el ID de la regla de control de acceso y de los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendario]</td> 
   <td> <p>Seleccione o asigne el ID del calendario que contiene la regla de control de acceso que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>Seleccione o asigne el ID de la regla de control de acceso que desee eliminar.</td> 
  </tr> 
 </tbody> 
</table>

### Iteradores (obsoleto)

La variable [!UICONTROL iterar archivos adjuntos] y [!UICONTROL repetir asistentes] Los módulos de se han quedado obsoletos. Para iterar archivos adjuntos o asistentes, utilice el [!UICONTROL Control de flujo] > [!UICONTROL Iterador] módulo. Para obtener más información, consulte [Módulo de iteración en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### Otro

* [[!UICONTROL Realizar una llamada de API]](#make-an-api-call)
* [[!UICONTROL Obtener información disponible/ocupada]](#get-freebusy-information)

#### [!UICONTROL Realizar una llamada de API]

Este módulo le permite realizar una llamada API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con el Adobe [!DNL Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Especifique una ruta relativa a <code>https://www.googleapis.com/calendar</code>. Ejemplo: <code>/v3/users/me/calendarList</code></td> 
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

#### [!UICONTROL Obtener información disponible/ocupada]

Este módulo de acción devuelve información de disponibilidad para un conjunto de calendarios.

El módulo devuelve el ID del calendario y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL Google Calendar] cuenta de Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con Adobe Workfront Fusion: Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mínimo de tiempo]</td> 
   <td> <p> Introduzca el inicio del intervalo para el que desea recuperar información.</p> <p> Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tiempo máximo]</td> 
   <td> <p> Introduzca el final del intervalo para el que desea recuperar información. </p> <p>Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendarios]</td> 
   <td> <p>Para cada calendario desde el que desee recuperar información, haga clic en <strong>Agregar</strong> e introduzca o asigne el ID de calendario.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Déclencheur de un escenario antes de un evento

Se puede almacenar en déclencheur un escenario en un tiempo especificado antes de un evento con la ayuda de [!DNL Google Calendar] los recordatorios de correo electrónico y la variable [!UICONTROL Enlaces web] >[!UICONTROL Buzón personalizado] módulo.

1. Utilice la variable [!UICONTROL Calendario de Google] >[!UICONTROL Actualizar un evento] para agregar un recordatorio de correo electrónico al evento:

   ![](assets/trigger-scen-before-event-350x209.png)

1. Cree un nuevo escenario a partir de la variable [!UICONTROL Enlaces web] >[!UICONTROL Buzón personalizado] módulo.

   1. Copie la dirección de correo electrónico del vínculo de correo.
   1. Guarde el escenario y ejecútelo.

1. En [!DNL Gmail], redirija el [!DNL Google Calendar] recordatorios de correo electrónico para la dirección de correo electrónico del maillock:

   1. Abra su **[!UICONTROL [!DNL Gmail]configuración]**.
   1. Abra el **[!UICONTROL Reenvío y POP/IMAP]** pestaña .
   1. Haga clic en **[!UICONTROL Agregar una dirección de reenvío].**
   1. Pegue la dirección de correo electrónico de los buzones copiados, haga clic en &#x200B;**[!UICONTROL Siguiente]**, confirme pulsando **[!UICONTROL Continuar]** en la ventana emergente, haga clic en **[!UICONTROL OK]**.

   1. En [!DNL Workfront Fusion], cambie al nuevo escenario que debe finalizar su ejecución recibiendo el correo electrónico de confirmación.
   1. Haga clic en la burbuja situada encima del módulo para inspeccionar la salida del módulo.
   1. Expanda el `Text` y copie el código de confirmación:

      ![](assets/confirmation-code-350x252.png)

   1. En Gmail, pegue el código de confirmación en el cuadro de edición y haga clic en &#x200B;**[!UICONTROL Verificar]**:

      ![](assets/paste-code-350x46.png)

   1. Abra el **[!UICONTROL Filtros y direcciones bloqueadas]** pestaña .
   1. Haga clic en **[!UICONTROL Crear un nuevo filtro]**.
   1. Configuración de un filtro para todos los correos electrónicos procedentes de `     calendar-notification@google.com` y haga clic en &#x200B;**[!UICONTROL Crear un filtro]**:
   1. Select **[!UICONTROL Reenviar para]** y seleccione la dirección de correo electrónico de los buzones de la lista.
   1. Haga clic en **[!UICONTROL Crear filtro]** para crear el filtro.

1. (Opcional) En [!DNL Workfront Fusion], añada la variable [!UICONTROL Analizador de texto] > [!UICONTROL Patrón de coincidencia] después del [!UICONTROL Enlaces web] >[!UICONTROL Buzón personalizado] para analizar el código de HTML del correo electrónico y obtener la información que necesite.

   Por ejemplo, puede configurar el módulo de la siguiente manera para obtener el ID del evento:

   *Patrón*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Texto*: La variable `HTML content` elemento generado desde el [!UICONTROL Enlaces web] >[!UICONTROL Buzón personalizado] módulo.
