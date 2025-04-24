---
content-type: overview
navigation-topic: notifications
title: Notificaciones de eventos
description: Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos como proyectos, tareas o problemas. Se envían cuando se produce algo en el proyecto que otros necesitan conocer. Según el evento, los usuarios reciben notificaciones instantáneas, diarias o instantáneas y diarias por correo electrónico.
author: Courtney
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 67%

---

# Notificaciones de eventos

<!-- Audited: 4/2025 -->

Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos como proyectos, tareas o problemas. Se envían cuando se produce algo en el proyecto que otros necesitan conocer. Según el evento, los usuarios reciben notificaciones instantáneas, diarias o instantáneas y diarias por correo electrónico.

>[!NOTE]
>
>Las notificaciones de eventos son uno de los diversos tipos de notificaciones de [!DNL Adobe Workfront]. Para obtener información acerca de todos los tipos de notificación de [!DNL Workfront], consulte [Información general sobre notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

## Configuración de las notificaciones de eventos

Los correos electrónicos de notificación de eventos se pueden configurar en los siguientes niveles:

* **Nivel del sistema**: un administrador de [!DNL Workfront] puede activar y desactivar las notificaciones de eventos en el nivel del sistema, como se explica en [Configurar notificaciones de los eventos para todos los usuarios del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Todos los grupos heredan las notificaciones del sistema de forma predeterminada, pero es posible que los administradores de grupos puedan cambiar algunas configuraciones en el nivel de grupo si el administrador [!DNL Workfront] lo permite.

* **Nivel de grupo**: un administrador de grupos puede configurar una notificación de eventos para los grupos que administra después de que un administrador de [!DNL Workfront] desbloquee esta capacidad para los grupos. Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo se aplica a los administradores de [!DNL Workfront] (para cualquier grupo). Para obtener más información, vea [Ver y configurar notificaciones de eventos para un grupo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

* **Nivel de usuario**: todas las notificaciones de eventos activadas en todo el sistema se enumeran en la sección [!UICONTROL Notificaciones] de cada usuario en su perfil individual. Los usuarios pueden activar y desactivar allí sus notificaciones de los eventos individuales.

  [!DNL Workfront] administradores y usuarios con acceso para editar otros usuarios también pueden activar y desactivar notificaciones en el perfil de un usuario individual.

  Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Las notificaciones a nivel de usuario también incluyen notificaciones de [!DNL Workfront Goals]. Sin embargo, el administrador de [!DNL Workfront] o el administrador de grupos no pueden configurar las notificaciones de [!DNL Workfront Goals]. Cada usuario debe configurar sus propias notificaciones de [!DNL Workfront Goals] en su perfil. Si tiene acceso para editar usuarios, también puede modificar estas notificaciones para otros. Para habilitar notificaciones de [!DNL Workfront Goals] para su perfil o para otros usuarios a los que tiene acceso para editar, consulte [Notificaciones: Goals](../../workfront-basics/using-notifications/notifications-goals.md).

  Para obtener más información sobre las notificaciones que puede configurar el administrador de [!DNL Workfront], consulte [Configurar notificaciones de eventos para todos los usuarios del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Contenido de las notificaciones de eventos

Un mensaje de correo electrónico de notificación de eventos contiene información sobre el evento que se ha producido y un vínculo a [!DNL Workfront], en donde se puede ver el evento en el sistema. Para obtener más información sobre cómo recibir notificaciones por correo electrónico, consulte [Resumen de notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

Un administrador de [!DNL Workfront] no puede cambiar el contenido de las notificaciones por correo electrónico tal como lo ha configurado [!DNL Workfront], pero puede cambiar las líneas de asunto de las notificaciones por correo electrónico de eventos. Para obtener más información, consulte [Personalizar asuntos de correo electrónico para las notificaciones de eventos](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Para obtener una lista de todas las [!DNL Workfront] notificaciones de eventos, junto con una breve descripción de cada evento y si está activo o inactivo de forma predeterminada, consulte [Tipos de notificaciones de eventos](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
