---
title: Configurar notificaciones de eventos para todos los usuarios del sistema
description: Las notificaciones de eventos almacenan en déclencheur los correos electrónicos a los usuarios cuando se produce un evento determinado. Como administrador de Adobe Workfront o usuario con un nivel de acceso de Planificador, puede configurar una notificación de eventos para todos los usuarios del sistema. La configuración de una notificación de eventos consiste en activarla o desactivarla.
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Configurar notificaciones de eventos para todos los usuarios del sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Las notificaciones de eventos almacenan en déclencheur los correos electrónicos a los usuarios cuando se produce un evento determinado. Como administrador de Adobe Workfront o usuario con un nivel de acceso de Planificador, puede configurar una notificación de eventos para todos los usuarios del sistema. La configuración de una notificación de eventos consiste en activarla o desactivarla.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Según el evento que habilite y el usuario mantenga esta opción habilitada en su propio perfil, los usuarios recibirán notificaciones instantáneas, diarias o instantáneas y diarias por correo electrónico cuando se produzca un evento.

Primero debe especificar qué notificaciones desea que reciban todos los usuarios en el área de Configuración de la instancia de Workfront. Una vez activada una notificación en el área de Configuración, se muestra activada para cada usuario en su página de perfil.

Una vez que las notificaciones se activan en el área de Configuración y aparecen en las páginas de perfil de los usuarios, los usuarios individuales u otro usuario con una licencia de Plan también pueden configurar las notificaciones activadas en un perfil de usuario para controlar qué notificaciones recibe ese usuario específico y con qué frecuencia. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obtener una lista de todas las notificaciones de eventos que puede activar y desactivar, consulte [Notificaciones de eventos disponibles en Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para obtener información sobre cómo desbloquear una notificación de eventos para que los administradores de grupos puedan configurarla en sus grupos, consulte [Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) y [Visualización y configuración de notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Planificador o superior, con acceso administrativo a las notificaciones de recordatorio</p> <p>Para obtener información sobre cómo otorgar acceso administrativo a un usuario del Plan, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Configurar notificaciones de eventos para todos los usuarios

Debe habilitar las notificaciones en el área de Configuración de Workfront para que los usuarios puedan habilitarlas o deshabilitarlas en sus perfiles.

>[!TIP]
>
>No puede activar notificaciones para Workfront Goals desde el área de Configuración. Los usuarios solo pueden activar estas notificaciones en sus perfiles. Los usuarios con licencias de planificación pueden activarlas para otros usuarios. Para obtener información sobre cómo habilitar las notificaciones de Workfront Goals para los usuarios, consulte [Notificaciones: Objetivos](../../../workfront-basics/using-notifications/notifications-goals.md).

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Clic **Correo electrónico** > **Notificaciones**.

   ![](assets/notifications-area-under-setup-emails.png)


1. Asegúrese de que la **Notificaciones de eventos** está abierta.
1. Haga clic en el conmutador situado a la izquierda del nombre del evento para activarlo o desactivarlo.

   Para ver el estado de notificación predeterminado de un evento, consulte [Notificaciones de eventos](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Opcional) Haga clic en el nombre de una notificación de evento para personalizar la línea de asunto de la notificación por correo electrónico.

   Para obtener más información sobre la personalización de las líneas de asunto de las notificaciones por correo electrónico, consulte [Personalizar temas de correo electrónico para notificaciones de eventos](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Opcional) Si desea desbloquear la configuración de una notificación por correo electrónico para que los administradores de grupos puedan configurarla por separado para sus grupos, haga clic en el botón ![](assets/lock-toggle-button.png) a la derecha de la notificación para cambiarla a la posición desbloqueada ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >Inicialmente, esta funcionalidad solo está disponible para los clientes del clúster 4 como parte de un despliegue gradual. Poco después estará disponible para otros clústeres. Este artículo se actualizará a medida que esto ocurra.

   Para obtener más información, consulte [Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
