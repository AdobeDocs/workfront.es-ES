---
title: Configurar notificaciones de eventos para todos los miembros del sistema
description: Las notificaciones de eventos déclencheur correos electrónicos a los usuarios cuando se produce un evento determinado. Como administrador de Adobe Workfront o usuario con nivel de acceso de Planificador, puede configurar una notificación de evento para todos los usuarios del sistema. La configuración de una notificación de evento consiste en activarla o desactivarla.
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Configurar notificaciones de eventos para todos los miembros del sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Las notificaciones de eventos déclencheur correos electrónicos a los usuarios cuando se produce un evento determinado. Como administrador de Adobe Workfront o usuario con nivel de acceso de Planificador, puede configurar una notificación de evento para todos los usuarios del sistema. La configuración de una notificación de evento consiste en activarla o desactivarla.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Según el evento que habilite y el usuario mantenga habilitado su propio perfil, los usuarios recibirán notificaciones por correo electrónico instantáneas, diarias o tanto instantáneas como diarias cuando se produzca un evento.

Primero debe especificar qué notificaciones desea que reciban todos los usuarios en el área de configuración de la instancia de Workfront. Una vez que activa una notificación en el área Configuración, esta se muestra como activada para cada usuario en su página de perfil.

Después de activar las notificaciones en el área Configuración y de que aparezcan en las páginas de perfil de los usuarios, los usuarios individuales u otro usuario con una licencia de Plan también pueden configurar las notificaciones activadas en un perfil de usuario para controlar qué notificaciones recibe ese usuario específico y con qué frecuencia. Para obtener más información, consulte [Activar o desactivar sus propias notificaciones de eventos](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Para obtener una lista de todas las notificaciones de eventos que puede activar y desactivar, consulte [Notificaciones de eventos disponibles en Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Para obtener información sobre cómo desbloquear una notificación de evento para que los administradores de grupos puedan configurarlo para sus grupos, consulte [Desbloquear o bloquear la configuración de las notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) y [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Planificador o superior, con acceso administrativo a las notificaciones de recordatorio</p> <p>Para obtener información sobre cómo conceder acceso administrativo a un usuario del Plan, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Configurar notificaciones de eventos para todos los usuarios

Debe activar las notificaciones en el área Configuración de Workfront para que los usuarios puedan habilitarlas o deshabilitarlas en sus perfiles.

>[!TIP]
>
>No puede activar notificaciones para objetivos de Workfront desde el área Configuración . Los usuarios pueden activar estas notificaciones solo en sus perfiles. Los usuarios con licencias de Plan pueden activarlas para otros usuarios. Para obtener información sobre cómo activar las notificaciones de objetivos de Workfront para los usuarios, consulte [Notificaciones: Objetivos](../../../workfront-basics/using-notifications/notifications-goals.md).

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Correo electrónico** > **Notificaciones**.

1. Asegúrese de que la variable **Notificaciones de eventos** está abierta.
1. Haga clic en el conmutador a la izquierda del nombre del evento para activarlo o desactivarlo.

   Para ver el estado de notificación predeterminado de un evento, consulte [Notificaciones de eventos](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Opcional) Haga clic en el nombre de una notificación de evento para personalizar la línea de asunto de la notificación por correo electrónico.

   Para obtener más información sobre la personalización de las líneas de asunto de las notificaciones por correo electrónico, consulte [Personalización de los temas de correo electrónico para las notificaciones de eventos](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Opcional) Si desea desbloquear la configuración de una notificación por correo electrónico para que los administradores de grupos puedan configurarla por separado para sus grupos, haga clic en el botón ![](assets/lock-toggle-button.png) a la derecha de la notificación para cambiar a la posición desbloqueada ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >Esta funcionalidad está disponible inicialmente solo para los clientes del Cluster 4 como parte de un despliegue por fases. Poco después estará disponible para otros grupos temáticos. Este artículo se actualizará cuando esto ocurra.

   Para obtener más información, consulte [Desbloquear o bloquear la configuración de las notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
