---
title: Configurar notificaciones de eventos para todos en el sistema
description: Las notificaciones de eventos activan correos electrónicos a los usuarios cuando se produce un evento determinado. Como administrador de Adobe Workfront o usuario con un nivel de acceso al Planificador, puede configurar una notificación de eventos para todos los usuarios del sistema. La configuración de una notificación de eventos consiste en activarla o desactivarla.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 85%

---

# Configurar notificaciones de los eventos para todos los usuarios del sistema

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Las notificaciones de eventos activan correos electrónicos a los usuarios cuando se produce un evento determinado. Como administrador de Adobe Workfront o usuario con un nivel de acceso al Planificador, puede configurar una notificación de eventos para todos los usuarios del sistema. La configuración de una notificación de eventos consiste en activarla o desactivarla.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Según el evento que habilite y si los usuarios mantienen esta opción habilitada en su perfil, estos recibirán notificaciones instantáneas, diarias o instantáneas y diarias por correo electrónico cuando se produzca un evento.

Primero debe especificar qué notificaciones desea que reciban todos los usuarios en el área Configuración de la instancia de su Workfront. Una vez activada una notificación en el área de Configuración, se muestra activada para cada usuario en su página de perfil.

Una vez que las notificaciones se activan en el área Configuración y aparecen en las páginas de perfil de los usuarios, los usuarios individuales u otro usuario con una licencia de Plan también pueden configurar las notificaciones activadas en un perfil de usuario para controlar qué notificaciones recibe ese usuario específico y con qué frecuencia. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obtener una lista de todas las notificaciones de eventos que puede activar y desactivar, consulte [Tipos de notificaciones de eventos](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para obtener información acerca de cómo desbloquear una notificación de eventos para que los administradores de grupos puedan configurarla en sus grupos, consulte [Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) y [Visualización y configuración de notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
<p>Plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Planificador o superior con acceso administrativo a las notificaciones de recordatorio</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Configurar notificaciones de eventos para todos los usuarios

Debe habilitar las notificaciones en el área Configuración de Workfront para que los usuarios puedan habilitarlas o deshabilitarlas en sus perfiles individuales.

>[!TIP]
>
>No puede activar notificaciones para Workfront Goals desde el área Configuración. Los usuarios solo pueden activar estas notificaciones en sus perfiles. Los usuarios con licencias de Plan pueden activarlas para otros usuarios. Para obtener más información acerca de cómo habilitar las notificaciones de Workfront Goals para los usuarios, vea [Notificaciones: Goals](../../../workfront-basics/using-notifications/notifications-goals.md).

{{step-1-to-setup}}

1. Haga clic en **Correo electrónico** > **Notificaciones**.

   ![Área de notificaciones en correos electrónicos de configuración](assets/notifications-area-under-setup-emails.png)


1. Asegúrese de que la pestaña **Notificaciones de eventos** esté abierta.
1. Cambie el conmutador a la izquierda del nombre del evento para activarlo o desactivarlo.

   Para ver el estado de la notificación predeterminado de un evento, consulte [Notificaciones de eventos](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Opcional) Haga clic en el nombre de una notificación de evento para personalizar la línea del asunto de la notificación por correo electrónico.

   Para obtener más información sobre cómo personalizar las líneas del asunto de las notificaciones por correo electrónico, consulte [Personalizar asuntos de correo electrónico para notificaciones de eventos](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Opcional) Si desea desbloquear la configuración de una notificación por correo electrónico para que los administradores del grupo puedan configurarla por separado para sus grupos, haga clic en el botón ![Bloquear conmutador](assets/lock-toggle-button.png) a la derecha de la notificación para cambiarla a la posición desbloqueada ![Desbloquear conmutador](assets/unlock-toggle-button.png).

   Para obtener más información, consulte [Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Los usuarios pueden personalizar la frecuencia de estas notificaciones en su perfil de usuario.
