---
content-type: overview;reference
navigation-topic: notifications
title: Resumen de notificaciones
description: Adobe Workfront envía notificaciones por correo electrónico, notificaciones en la aplicación y notificaciones en su dispositivo móvil.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 1%

---

# Resumen de notificaciones

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] envía notificaciones por correo electrónico, notificaciones en la aplicación y notificaciones en el dispositivo móvil.

## Notificaciones por correo electrónico

[!DNL Workfront] envía notificaciones por correo electrónico para alertar a los usuarios sobre la actividad en Workfront y proporcionar información y vínculos útiles.

Para cambiar las preferencias de las notificaciones por correo electrónico, consulta [Modificar tus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Si desea recibir notificaciones por correo electrónico desde el entorno de espacio aislado, debe habilitar los correos electrónicos desde el perfil de usuario en ese entorno.

Puede recibir las siguientes notificaciones por correo electrónico de [!DNL Workfront]:

* [Notificaciones de eventos](#event-notifications)
* [Notificaciones de resumen diario](#daily-digest-notifications)
* [Notificación de comentarios publicados](#notification-of-posted-comments)
* [Recordatorios automáticos](#automatic-reminders)
* [Notificaciones de recordatorio](#reminder-notifications)
* [Notificaciones de tableros](#boards-notifications)
* [Otros [!DNL Workfront] correos electrónicos](#other-workfront-emails)

### Notificaciones de eventos

Las notificaciones de eventos generalmente se activan debido a ciertos eventos predefinidos, como tener una tarea asignada o obtener una respuesta a un comentario que ha realizado.

Una vez que el administrador de [!DNL Workfront] o el administrador del grupo hayan activado las notificaciones de eventos en su sistema [!DNL Workfront], puede seleccionar cuáles desea recibir editando las preferencias de [!UICONTROL Notificaciones] en su perfil de usuario. También puede elegir si desea recibir notificaciones cuando se produzcan eventos o si desea recibir eventos resumidos en un correo electrónico de resumen diario.

Es posible que solo vea un subconjunto de estas notificaciones en su configuración, dependiendo de cómo el administrador de [!DNL Workfront] haya configurado las notificaciones de eventos para su sistema [!DNL Workfront]. Para obtener más información, consulte [Configurar notificaciones de eventos para todos los usuarios del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

El estado predeterminado muestra qué notificaciones (diarias, instantáneas o ambas) están habilitadas de forma predeterminada para los nuevos usuarios cuando los crea.

Para obtener una lista completa de las notificaciones de eventos e información sobre cómo se habilitan y configuran en el nivel del sistema, el nivel de grupo o el nivel de usuario, consulte [Notificaciones de eventos disponibles en [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para obtener información sobre cómo elegir las notificaciones de eventos que desea recibir, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Las notificaciones de eventos son las únicas notificaciones que se pueden configurar para que se entreguen en las actualizaciones diarias de resumen.

### Notificaciones de resumen diario

Una notificación de resumen diaria es un correo electrónico que contiene todas las notificaciones de un tipo determinado que recibió en las 24 horas anteriores al correo electrónico.

Para obtener una lista completa de las notificaciones por correo electrónico que se han habilitado para una entrega de correo electrónico de resumen diario, así como información sobre todas las categorías de notificaciones por correo electrónico, consulte [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] no envía ninguna notificación de resumen diario para las categorías de eventos [!UICONTROL Miscelánea] y [!DNL Goals]. No puedes desactivar las Notificaciones diarias para estas categorías.

Al recibir notificaciones de resumen diario, hay que tener en cuenta varios aspectos:

* Cada sección [!UICONTROL notifications] del panel **[!UICONTROL Mi configuración]** genera su propio correo electrónico de resumen diario. Puede tener tantos correos electrónicos de resumen diario como ajustes de notificación habilitados para correos electrónicos de resumen diario.\
   Por ejemplo, si seleccionó recibir un correo electrónico de resumen diario de varias acciones en la **[!UICONTROL Información sobre los proyectos de mi propiedad],** recibirá una notificación por correo electrónico en la que se enumeran todos los eventos cumplidos en esta área.

* Las notificaciones de un correo electrónico de resumen diario se agrupan por varios criterios. Por ejemplo, en el caso de **[!UICONTROL Información sobre proyectos de mi propiedad]**, los eventos se agrupan por el nombre del proyecto.

  Para la categoría **[!UICONTROL Comunicación]**, las notificaciones se agrupan por el objeto donde se produjo la comunicación.

  >[!NOTE]
  >
  >En la categoría Comunicación, puede seleccionar notificaciones individuales solo para envío instantáneo. Para que las notificaciones se envíen en un resumen diario, debe seleccionarlas todas.

* El correo electrónico de resumen diario enumera los eventos que se produjeron para las acciones en un área en particular (como **Información sobre proyectos de mi propiedad**) en las 24 horas anteriores a la hora elegida para la entrega.
* La zona horaria de la hora seleccionada para la entrega de compendio diario coincide con la zona horaria, tal como está configurada en el explorador.
* Los correos electrónicos de resumen diario tienen el nombre de la sección en la línea de asunto, así como la fecha en la que se envían.
* Al menos un evento debe almacenar en déclencheur una notificación para que se envíe el compendio diario. Los resúmenes diarios no se envían si no se cumplen los eventos marcados para los correos electrónicos de resúmenes diarios.

### Notificación de comentarios publicados

Las notificaciones de la categoría [!UICONTROL Comunicación] le avisan de los comentarios que se han publicado en el flujo de [!UICONTROL Actualización] de un elemento específico.

Se han seleccionado los correos electrónicos de resumen diario de la categoría [!UICONTROL Comunicación] para todas las notificaciones disponibles.

La información se resume para el objeto donde se produjo la comunicación y se muestra un número total de mensajes de comunicación para cada objeto.

Para responder al comentario o verlo en Workfront:

1. Haga clic en el botón **[!UICONTROL Comentario]** del correo electrónico.

   Se abre el área [!UICONTROL Actualizaciones] del objeto, con el comentario específico delineado en azul.

   Hay un cuadro de respuesta abierto, que puede utilizar para responder al comentario.

Para obtener más información sobre cómo configurar las notificaciones por correo electrónico, incluida la activación de las notificaciones de resumen diario, consulte [Ver y modificar la configuración de las notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) en [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Recordatorios automáticos

El administrador de [!DNL Workfront] habilita los recordatorios automáticos para avisarle de tareas y problemas que vencen, que se retrasan o que están cerca de la fecha planificada de finalización. Para las notificaciones tardías, el correo electrónico se envía todas las noches hasta que se complete la tarea o el problema. Una vez que el administrador los ha configurado, no puede desactivarlos. Tampoco puede cambiar el contenido ni la línea de asunto de un correo electrónico activado por un recordatorio automático.

Se pueden enviar a una o más de las siguientes opciones:

* Los usuarios asignados a una tarea o un problema
* El responsable inmediato del usuario
* El gerente del gerente inmediato

Los correos electrónicos de recordatorio automático se envían desde la dirección de correo electrónico que el administrador de [!DNL Workfront] seleccionó para administrar los mensajes de correo electrónico salientes.

En función del recordatorio automático activado, los siguientes tipos de información están disponibles en el correo electrónico del recordatorio automático:

* La fecha cuando se creó la tarea o el problema
* Nombre de tarea o problema
* Nombre del proyecto en el que reside la tarea o el problema
* Descripción de tarea o problema
* Lista de usuarios asignados a la tarea o al problema
* El nombre del usuario que ingresó la tarea o el problema
* Prioridad de la tarea o el problema
* Fecha en la que venció la tarea o el problema

Para obtener información acerca de cómo habilitar los avisos automáticos, vea [Configurar avisos automáticos](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Notificaciones de recordatorio

Un administrador de [!DNL Workfront] (o un usuario con un nivel de acceso de [!UICONTROL Planificador] y acceso administrativo a las notificaciones de recordatorio) puede diseñar notificaciones de recordatorio sobre la inminencia de los plazos y asociarlas manualmente a proyectos, tareas, problemas y hojas de horas.

>[!IMPORTANT]
>
>Si la fecha límite cambia después de que un usuario reciba una notificación de recordatorio para cualquiera de los objetos mencionados anteriormente, el usuario no recibe otra notificación de recordatorio.

Las notificaciones de recordatorio se envían desde la dirección de correo electrónico que el administrador de [!DNL Workfront] seleccionó para administrar los mensajes de correo electrónico salientes.

Para obtener información sobre cómo configurar y habilitar las notificaciones de recordatorio, consulte [Configurar notificaciones de recordatorio](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Para obtener información sobre cómo obtener el acceso administrativo requerido, vea [Conceder acceso administrativo a los usuarios a ciertas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Notificaciones de tableros

[!DNL Adobe Workfront] [!UICONTROL Tableros] le envía un mensaje de correo electrónico cuando se le agrega a un tablero y cuando se le asigna una tarjeta. Puede seleccionar qué correos electrónicos desea recibir en las preferencias de sus tableros.

Para obtener más información, consulte [Notificaciones y preferencias por correo electrónico de los tableros](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Otros [!DNL Workfront] correos electrónicos

Hay otros correos electrónicos que podría recibir de [!DNL Workfront] y que no se pueden configurar.

Los siguientes correos electrónicos son enviados automáticamente por [!DNL Workfront] cuando se cumplen estas condiciones:

* Restaurar un elemento: cuando el administrador de [!DNL Workfront] restaura un objeto de la papelera [!UICONTROL Reciclar], se envía un correo electrónico al administrador de [!DNL Workfront].
* No se pudo restaurar: Cuando el administrador de [!DNL Workfront] intenta restaurar un objeto desde la Papelera de reciclaje y la restauración falla, se envía un correo electrónico al administrador de [!DNL Workfront].

Los siguientes correos electrónicos solo se pueden configurar en el nivel de perfil de usuario. No se pueden habilitar ni deshabilitar en el sistema:

* Finalización de una tarea personal: cuando se complete una tarea personal que asignó a otra persona, recibirá un correo electrónico.
* Comentario añadido al usuario: cuando alguien comente en su perfil de usuario, recibirá un correo electrónico.

## Notificaciones en la aplicación

Puede recibir notificaciones dentro de la aplicación web [!DNL Workfront] cuando se produzcan ciertos eventos.

Para obtener más información sobre las notificaciones en la aplicación, consulte [Ver y administrar notificaciones en la aplicación](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Notificaciones por correo electrónico en la aplicación de correo electrónico móvil

Puede recibir [!DNL Workfront] notificaciones por correo electrónico en su aplicación de correo electrónico móvil, en su dispositivo móvil.

Si tiene la aplicación móvil [!DNL Workfront] instalada en el teléfono, al pulsar los vínculos del correo electrónico se abrirán en la aplicación móvil [!DNL Workfront]. Esto incluye pulsar cualquiera de los siguientes botones de acción:

* [!UICONTROL Trabajar En Ello]
* [!UICONTROL Comentario]
* [!UICONTROL Tomar decisión sobre la aprobación]
* [!UICONTROL Ver todas las notificaciones]
* [!UICONTROL Agregar]
* [!UICONTROL Introducción]
* [!UICONTROL Ver más detalles]

Para obtener más información sobre la aplicación móvil [!DNL Workfront], consulte [Usar la [!DNL Adobe Workfront] aplicación móvil](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
