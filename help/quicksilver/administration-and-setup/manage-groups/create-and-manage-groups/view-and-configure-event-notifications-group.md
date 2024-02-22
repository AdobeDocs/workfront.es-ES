---
user-type: administrator
product-area: system-administration;user-management
keywords: ver, grupo, evento, notificaciones, configurar, habilitar, deshabilitar
navigation-topic: create-and-manage-groups
title: Visualización y configuración de notificaciones de eventos para un grupo
description: Como administrador de grupo, puede ver las notificaciones de eventos activadas para un grupo que administra. Además, si un administrador de Adobe Workfront desbloquea una notificación de eventos, puede configurarla para un grupo de nivel superior que administre. La configuración de una notificación de eventos consiste en activarla o desactivarla.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Visualización y configuración de notificaciones de eventos para un grupo

Como administrador de grupo, puede ver las notificaciones de eventos activadas para un grupo que administra.

Además, si un administrador de Adobe Workfront desbloquea una notificación de eventos, puede configurarla para un grupo de nivel superior que administre. La configuración de una notificación de eventos consiste en activarla o desactivarla.

Un administrador de Workfront también puede hacer esto para cualquier grupo.

La configuración de una notificación de eventos para un grupo afecta a los usuarios para los que ese grupo, o uno de sus subgrupos, es su grupo de inicio. En sus perfiles de usuario, estos usuarios ven las notificaciones de eventos activadas para su grupo de inicio en lugar de las notificaciones de eventos activadas en todo el sistema.

Para obtener información sobre cómo un administrador de Workfront desbloquea una notificación de eventos, consulte [Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Para obtener información sobre la configuración de notificación predeterminada para un evento, consulte [Tipos de notificación de eventos](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Visualización y configuración de las notificaciones de eventos de un grupo

1. (Condicional y opcional) Si es administrador de Workfront y ya se encuentra en la página Notificaciones por correo electrónico (Configuración > Correo electrónico > Notificaciones), puede hacer lo siguiente y pasar al paso 6: Eliminar **Notificaciones de eventos del sistema** en el cuadro situado encima de la lista, empiece a escribir el nombre del grupo en el cuadro y, a continuación, haga clic en él cuando aparezca.
1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo de nivel superior.
1. En el menú izquierdo, haga clic en **Notificaciones de eventos**.

   En la lista que se muestra, la variable **Activo** La columna de la izquierda muestra qué notificaciones están activas (azul) e inactivas (gris) para el grupo.

1. Para activar o desactivar una notificación de evento desbloqueado: haga clic en el botón del <strong>Activo</strong> columna para activar <img src="assets/email-notification-enabled-unlocked.png"> o desactivar <img src="assets/email-notification-disabled-unlocked.png"> it.

   >[!INFO]
   >
   >**Ejemplo:** Puede configurar las dos notificaciones de eventos de grupos de marketing principales que se muestran a continuación y que se han desbloqueado para grupos.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Si aparece un botón en <strong>Activo</strong> columna gris y atenuada <img src="assets/email-notification-disabled-locked.png">, la notificación de eventos se desactiva para todos los usuarios y los administradores de grupos no pueden activarla ni editar la línea de asunto de su correo electrónico
   >* Si aparece un botón en <strong>Activo</strong> la columna es gris y no está atenuada <img src="assets/email-notification-disabled-unlocked.png">, la notificación de eventos es <strong>desactivado para todos los usuarios y</strong> los administradores de grupos pueden activarlo para sus grupos.
   >* Si aparece un botón en <strong>Activo</strong> la columna está en azul y atenuada <img src="assets/email-notification-enabled-locked.png">Además, la notificación de eventos se activa para todos los usuarios y los administradores de grupos no pueden desactivarla ni editar la línea de asunto de correo electrónico para sus grupos.
   >* Si aparece un botón en <strong>Activo</strong> la columna es azul y no está atenuada <img src="assets/email-notification-enabled-unlocked.png">, la notificación de eventos es <strong>activado para todos los usuarios y</strong> los administradores de grupos pueden desactivarlo para sus grupos.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

