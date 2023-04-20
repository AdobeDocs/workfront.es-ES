---
content-type: overview;reference
navigation-topic: notifications
title: Notificaciones de Adobe Workfront
description: Adobe Workfront envía notificaciones por correo electrónico, notificaciones en la aplicación y notificaciones en el dispositivo móvil.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: bfe45a29290631420c3a60d7dcbe470619094ca1
workflow-type: tm+mt
source-wordcount: '1301'
ht-degree: 1%

---

# [!DNL Adobe Workfront] notificaciones

[!DNL Adobe Workfront] envía notificaciones por correo electrónico, notificaciones en la aplicación y notificaciones en el dispositivo móvil.

## Notificaciones por correo electrónico

[!DNL Workfront] envía una serie de notificaciones por correo electrónico para alertar a los usuarios sobre la actividad en Workfront y proporcionar información y vínculos útiles.

>[!NOTE]
>
>Si desea recibir notificaciones por correo electrónico del entorno de espacio aislado, debe habilitar los correos electrónicos del perfil de usuario en ese entorno.

Puede recibir las siguientes notificaciones por correo electrónico desde [!DNL Workfront]:

* [Notificaciones de eventos](#event-notifications)
* [Notificaciones diarias de resumen](#daily-digest-notifications)
* [Notificación de los comentarios publicados](#notification-of-posted-comments)
* [Avisos automáticos](#automatic-reminders)
* [Notificaciones de recordatorio](#reminder-notifications)
* [Notificaciones del tablero](#boards-notifications)
* [Otro [!DNL Workfront] correos electrónicos](#other-workfront-emails)

### Notificaciones de eventos

Las notificaciones de eventos están predefinidas en [!DNL Workfront]. Normalmente se activan mediante determinados eventos.

Una vez que el [!DNL Workfront] administrador o administrador de grupo, puede seleccionar los que desea recibir editando su [!UICONTROL Notificaciones] en su perfil de usuario. También puede elegir si desea recibir notificaciones a medida que ocurran los eventos o si desea recibir eventos resumidos en un resumen diario por correo electrónico.

Dependiendo de cómo [!DNL Workfront] el administrador ha configurado las notificaciones de eventos para su [!DNL Workfront] sistema (tal como se describe en [Configurar notificaciones de eventos para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)), es posible que solo vea un subconjunto de estas notificaciones en la configuración.

El estado predeterminado muestra qué notificaciones (diarias, instantáneas o ambas) están habilitadas de forma predeterminada para los usuarios nuevos al crear los usuarios nuevos.

Para obtener una lista completa de las notificaciones de eventos e información sobre cómo se habilitan y configuran a nivel de sistema, de grupo o de usuario, consulte [Notificaciones de eventos disponibles en [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para obtener información sobre cómo elegir qué notificaciones de eventos desea recibir, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Las notificaciones de eventos son las únicas notificaciones que se pueden configurar para enviarse en actualizaciones diarias del compendio.

### Notificaciones diarias de resumen

Para obtener una lista completa de las notificaciones por correo electrónico habilitadas para un envío de correo electrónico con compendio diario, así como información sobre todas las categorías de notificaciones por correo electrónico, consulte [Notificaciones de eventos](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] no envía ninguna notificación de resumen diario para la variable [!UICONTROL Varios] y [!DNL Goals] categorías de eventos. No puede desactivar las notificaciones diarias para estas categorías.

Hay varias cosas que hay que tener en cuenta al recibir notificaciones diarias del compendio:

* Cada [!UICONTROL notificaciones] en la sección **[!UICONTROL Mis ajustes]** el panel genera su propio correo electrónico de compendio diario. Puede tener todos los días tantos correos electrónicos recopilados diariamente como ajustes de notificación habilitados para los correos electrónicos recopilados diariamente.\
   Por ejemplo, si ha seleccionado recibir un correo electrónico de compendio diario para varias acciones en la sección **[!UICONTROL Información sobre Proyectos I] Propio,** recibe una notificación por correo electrónico que enumera todos los eventos que se han producido en esta área.

* Las notificaciones en un correo electrónico de resumen diario se agrupan según varios criterios. Por ejemplo, en el caso de **[!UICONTROL Información sobre proyectos propios]**, los eventos se agrupan por el nombre del proyecto.

   Para la variable **[!UICONTROL Comunicación]** , las notificaciones se agrupan por el objeto en el que se produjo la comunicación.

* El compendio diario de correo electrónico enumera los eventos que se produjeron para las acciones en un área en particular (como **Información sobre los proyectos que tengo**) dentro de las 24 horas previas al tiempo elegido para la entrega.
* La zona horaria de la hora seleccionada para la entrega de compendios diarios coincide con su zona horaria, ya que está configurada en su explorador.
* Los correos electrónicos de resumen diarios tienen el nombre de la sección en la línea de asunto, así como la fecha en la que se entregan.
* Al menos un evento debe almacenar en déclencheur una notificación para poder enviar el compendio diario. Los compendios diarios no se envían si no se cumple ningún evento marcado para los correos electrónicos de compendio diarios.

### Notificación de los comentarios publicados

Las notificaciones de la variable [!UICONTROL Comunicación] alerta de categoría a los comentarios que se han publicado en la [!UICONTROL Actualizar] flujo de un elemento específico.

Correos electrónicos de resumen diarios para la variable [!UICONTROL Comunicación] para todas las notificaciones disponibles.

La información se resume para el objeto en el que se produjo la comunicación y se muestra un número total de mensajes de comunicación para cada objeto.

Para obtener más información sobre la configuración de las notificaciones por correo electrónico, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obtener instrucciones sobre cómo comentar [!UICONTROL Comunicación] correos electrónicos, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Para obtener más información sobre [!UICONTROL Comunicación] correos electrónicos, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obtener más información sobre cómo activar las notificaciones de compendio diarias, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Avisos automáticos

Los recordatorios automáticos son activados por su [!DNL Workfront] administrador para avisarle de las tareas y los problemas que venzan, retrasan o se acercan a la fecha de finalización planificada. Para las notificaciones atrasadas, el correo electrónico se envía todas las noches hasta que se complete la tarea o el problema. Una vez que el administrador los haya configurado, no podrá desactivarlos. Además, no se puede cambiar el contenido ni la línea de asunto de un correo electrónico activado por un recordatorio automático.

Se pueden enviar a una o más de las siguientes opciones:

* Los usuarios asignados a una tarea o problema
* El administrador inmediato del usuario
* El administrador del administrador inmediato

Los correos electrónicos de recordatorio automático se envían desde la dirección de correo electrónico en la que [!DNL Workfront] administrador seleccionado para gestionar correos electrónicos salientes.

Dependiendo de qué recordatorio automático esté activado, los siguientes tipos de información están disponibles en el correo electrónico de recordatorio automático:

* La fecha en la que se creó la tarea o el problema
* Tarea o nombre de problema
* Nombre del proyecto en el que reside la tarea o el problema
* Descripción de la tarea o el problema
* Una lista de usuarios asignados a la tarea o el problema
* Nombre del usuario que ha introducido la tarea o el problema
* La prioridad de la tarea o el problema
* Fecha en la que la tarea o el problema vencieron

Para obtener información sobre cómo habilitar los recordatorios automáticos, consulte [Configurar recordatorios automáticos](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Notificaciones de recordatorio

A [!DNL Workfront] administrador (o un usuario con un [!UICONTROL Planificador] nivel de acceso y acceso administrativo a las notificaciones de recordatorio) puede diseñar notificaciones recordatorias sobre cómo aproximarse a los plazos y adjuntarlas a proyectos, tareas, problemas y partes de horas. Para obtener más información sobre cómo obtener el acceso administrativo necesario, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>Si la fecha límite cambia después de que un usuario reciba una notificación recordatoria para cualquiera de los objetos mencionados anteriormente, el usuario no recibe otra notificación recordatoria.

Las notificaciones del recordatorio se envían desde la dirección de correo electrónico de que la variable [!DNL Workfront] administrador seleccionado para gestionar correos electrónicos salientes.

Para obtener información sobre la configuración y activación de notificaciones de recordatorio, consulte [Configuración de notificaciones de recordatorio](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### Notificaciones del tablero

[!DNL Adobe Workfront] [!UICONTROL Tableros] le envía un correo electrónico cuando se le agrega a un tablero y cuando se le asigna una tarjeta.

Puede seleccionar qué correos electrónicos desea recibir en las preferencias de tableros. Para obtener más información, consulte [Notificaciones y preferencias de correo electrónico de tableros](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Otro [!DNL Workfront] correos electrónicos

Hay otros correos electrónicos de los que podría recibir [!DNL Workfront] que no se pueden configurar. Los siguientes correos electrónicos los envía automáticamente [!DNL Workfront] cuando se cumplan estas condiciones:

* Restaurar un elemento: Cuando la variable [!DNL Workfront] el administrador restaura un objeto del [!UICONTROL Reciclar] Bin, se envía un correo electrónico a la [!DNL Workfront] administrador.
* No se pudo restaurar: Cuando la variable [!DNL Workfront] el administrador intenta restaurar un objeto desde la Papelera de reciclaje y la restauración falla, se envía un correo electrónico al [!DNL Workfront] administrador.

Los siguientes correos electrónicos solo se pueden configurar en el nivel de perfil de usuario. No se pueden habilitar ni deshabilitar en el sistema:

* Finalización de la tarea personal: cuando se complete una tarea personal asignada a otra persona, recibirá un correo electrónico.
* Comentario añadido al usuario: cuando alguien comente en su perfil de usuario, recibirá un correo electrónico.

## Notificaciones en la aplicación

Puede recibir notificaciones dentro del [!DNL Workfront] aplicación web, cuando se producen determinados eventos.

Para obtener más información sobre las notificaciones en la aplicación, consulte [Ver y administrar notificaciones en la aplicación](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Notificaciones por correo electrónico en la aplicación de correo electrónico móvil

Puede recibir [!DNL Workfront] notificaciones por correo electrónico en la aplicación de correo electrónico móvil, en el dispositivo móvil.

Si tiene la variable [!DNL Workfront] Aplicación móvil instalada en el teléfono, al pulsar los vínculos del correo electrónico, se abren en el [!DNL Workfront] Aplicación móvil. Esto incluye pulsar cualquiera de los siguientes botones de acción:

* [!UICONTROL Trabajar en ello]
* [!UICONTROL Comentario]
* [!UICONTROL Tomar decisión de aprobación]
* [!UICONTROL Ver todas las notificaciones]
* [!UICONTROL Agregar]
* [!UICONTROL Comenzar]
* [!UICONTROL Mostrar más detalles]

Para obtener más información sobre la variable [!DNL Workfront] Aplicación móvil, consulte [Utilice la variable [!DNL Adobe Workfront] aplicación móvil](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
