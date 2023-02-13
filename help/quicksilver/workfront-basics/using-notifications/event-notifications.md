---
content-type: overview
navigation-topic: notifications
title: Notificaciones de eventos
description: Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos como proyectos, tareas o problemas. Se envían cuando se produce algo en el proyecto que otros necesitan saber. Según el evento, los usuarios reciben notificaciones de correo electrónico instantáneas, diarias o instantáneas y diarias sobre el evento.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Notificaciones de eventos

Las notificaciones de eventos son correos electrónicos activados por varios tipos de eventos en objetos como proyectos, tareas o problemas. Se envían cuando se produce algo en el proyecto que otros necesitan saber. Según el evento, los usuarios reciben notificaciones de correo electrónico instantáneas, diarias o instantáneas y diarias sobre el evento.

>[!NOTE]
>
>Las notificaciones de eventos son uno de varios tipos [!DNL Adobe Workfront] notificaciones. Para obtener información sobre todos los [!DNL Workfront] tipos de notificación, consulte [[!DNL Adobe Workfront] notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

## Configuración de notificaciones de eventos

Los correos electrónicos de notificación de eventos se pueden configurar en los siguientes niveles enumerados a continuación. La configuración de una notificación de evento consiste en activarla o desactivarla.

* **Nivel del sistema**: A [!DNL Workfront] el administrador puede activar y desactivar las notificaciones de eventos en el sistema, tal como se explica en [Configurar notificaciones de eventos para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   De forma predeterminada, todos los grupos heredan las notificaciones del sistema, pero es posible que los administradores de grupos puedan cambiar algunas configuraciones a nivel de grupo si lo permite el [!DNL Workfront] administrador, tal como se explica en el siguiente elemento de viñeta a continuación.

* **Nivel de grupo**: Un administrador de grupo puede configurar una notificación de evento para los grupos que administra después de una [!DNL Workfront] administrador desbloquea esta capacidad para grupos. Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con [!DNL Workfront] administradores (para cualquier grupo). Para obtener más información, consulte [Ver y configurar notificaciones de eventos para un grupo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

   >[!NOTE]
   >
   >Esta funcionalidad está disponible inicialmente solo para los clientes del Cluster 4 como parte de un despliegue por fases. Poco después estará disponible para otros grupos temáticos. Este artículo se actualizará cuando esto ocurra.

* **Nivel de usuario**: Todas las notificaciones de eventos activadas en todo el sistema se enumeran en el informe de cada usuario [!UICONTROL Notificaciones] en su perfil individual. Los usuarios pueden activar y desactivar allí las notificaciones de eventos individuales.

   [!DNL Workfront] los administradores y usuarios con acceso para editar otros usuarios también pueden activar y desactivar notificaciones en el perfil de usuarios individuales.

   Para obtener más información, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

   >[!NOTE]
   >
   >Las notificaciones a nivel de usuario también incluyen [!DNL Workfront Goals] notificaciones. Sin embargo, la variable [!DNL Workfront] el administrador o el administrador del grupo no pueden configurar las notificaciones para [!DNL Workfront Goals]. Cada usuario debe configurar su propio [!DNL Workfront Goals] notificaciones en su perfil. Si tiene acceso para editar usuarios, también puede modificar estas notificaciones para otros usuarios. Para habilitar [!DNL Workfront Goals] notificaciones para su perfil o para otros usuarios a los que tiene acceso para editar, consulte [Notificaciones: Objetivos](../../workfront-basics/using-notifications/notifications-goals.md).

   Para obtener más información sobre las notificaciones, la variable [!DNL Workfront] administrador puede configurar, consulte [Configurar notificaciones de eventos para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] solo están disponibles en el [!DNL Adobe Workfront] experiencia.

## Contenido de la notificación de eventos

Un correo electrónico de notificación de evento contiene información sobre el evento que se produjo y contiene un vínculo a [!DNL Workfront] donde puede ver el evento en el sistema. Para obtener más información sobre la recepción de notificaciones por correo electrónico, consulte [[!DNL Adobe Workfront] notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] El administrador no puede cambiar el contenido de las notificaciones por correo electrónico, ya que están configuradas por [!DNL Workfront]. Sin embargo, pueden cambiar las líneas de asunto de los correos electrónicos de notificaciones de eventos. Para obtener más información, consulte [Personalización de los temas de correo electrónico para las notificaciones de eventos](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Para obtener una lista, todas las [!DNL Workfront] notificaciones de eventos, junto con una breve descripción de cada evento, y si está activo o inactivo de forma predeterminada, consulte [Notificaciones de eventos disponibles en [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
