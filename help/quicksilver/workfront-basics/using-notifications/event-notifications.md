---
content-type: overview
navigation-topic: notifications
title: Notificaciones de eventos
description: Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos como proyectos, tareas o problemas. Se envían cuando se produce algo en el proyecto que otros necesitan conocer. Según el evento, los usuarios reciben notificaciones instantáneas, diarias o instantáneas por correo electrónico.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Notificaciones de eventos

Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos como proyectos, tareas o problemas. Se envían cuando se produce algo en el proyecto que otros necesitan conocer. Según el evento, los usuarios reciben notificaciones instantáneas, diarias o instantáneas por correo electrónico.

>[!NOTE]
>
>Las notificaciones de eventos son uno de varios tipos de [!DNL Adobe Workfront] notificaciones. Para obtener información acerca de todos los [!DNL Workfront] tipos de notificación, consulte [[!DNL Adobe Workfront] notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

## Configuración de notificaciones de eventos

Los correos electrónicos de notificación de eventos se pueden configurar en los siguientes niveles enumerados a continuación. La configuración de una notificación de eventos consiste en activarla o desactivarla.

* **Nivel del sistema**: A [!DNL Workfront] El administrador de puede activar y desactivar las notificaciones de eventos en el sistema, tal como se explica en [Configurar notificaciones de eventos para todos los usuarios del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Todos los grupos heredan las notificaciones del sistema de forma predeterminada, pero es posible que los administradores de grupos puedan cambiar algunas configuraciones en el nivel de grupo, si lo permite el [!DNL Workfront] administrador, tal como se explica en el siguiente elemento de viñeta a continuación.

* **Nivel de grupo**: un administrador de grupo puede configurar una notificación de eventos para los grupos que administra después de una [!DNL Workfront] El administrador de desbloquea esta capacidad para grupos. Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo se aplica a [!DNL Workfront] administradores (para cualquier grupo). Para obtener más información, consulte [Visualización y configuración de notificaciones de eventos para un grupo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Inicialmente, esta funcionalidad solo está disponible para los clientes del clúster 4 como parte de un despliegue gradual. Poco después estará disponible para otros clústeres. Este artículo se actualizará a medida que esto ocurra.

* **Nivel de usuario**: todas las notificaciones de eventos activadas en todo el sistema se enumeran en el [!UICONTROL Notificaciones] en su perfil individual. Los usuarios pueden activar y desactivar allí sus notificaciones de eventos individuales.

  [!DNL Workfront] los administradores y usuarios con acceso para editar otros usuarios también pueden activar y desactivar notificaciones en el perfil de usuarios individuales.

  Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Las notificaciones a nivel de usuario también incluyen [!DNL Workfront Goals] notificaciones. Sin embargo, la variable [!DNL Workfront] El administrador de o el administrador del grupo no pueden configurar notificaciones para [!DNL Workfront Goals]. Cada usuario debe configurar su propio [!DNL Workfront Goals] notificaciones en su perfil. Si tiene acceso para editar usuarios, también puede modificar estas notificaciones para otros. Para activar [!DNL Workfront Goals] para las notificaciones de su perfil o de otros usuarios a los que tenga acceso para editar, consulte [Notificaciones: Objetivos](../../workfront-basics/using-notifications/notifications-goals.md).

  Para obtener más información sobre las notificaciones, consulte [!DNL Workfront] El administrador puede configurar, consulte [Configurar notificaciones de eventos para todos los usuarios del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] solo están disponibles en El nuevo [!DNL Adobe Workfront] experiencia.

## Contenido de notificación de eventos

Un correo electrónico de notificación de eventos contiene información sobre el evento que se ha producido y un vínculo a [!DNL Workfront] donde puede ver el evento en el sistema. Para obtener más información sobre la recepción de notificaciones por correo electrónico, consulte [[!DNL Adobe Workfront] notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] el administrador no puede cambiar el contenido de las notificaciones por correo electrónico, ya que están configuradas por [!DNL Workfront]. Sin embargo, pueden cambiar las líneas de asunto de los correos electrónicos de notificaciones de eventos. Para obtener más información, consulte [Personalizar temas de correo electrónico para notificaciones de eventos](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Para obtener una lista de todos los [!DNL Workfront] notificaciones de eventos, junto con una breve descripción de cada evento y si está activo o inactivo de forma predeterminada, consulte [Notificaciones de eventos disponibles en [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
