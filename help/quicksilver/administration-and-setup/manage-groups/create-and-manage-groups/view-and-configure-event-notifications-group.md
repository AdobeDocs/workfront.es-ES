---
user-type: administrator
product-area: system-administration;user-management
keywords: ver,grupo,evento,notificaciones,configurar,habilitar,deshabilitar
navigation-topic: create-and-manage-groups
title: Ver y configurar notificaciones de eventos para un grupo
description: Como administrador de grupo, puede ver las notificaciones de eventos activadas para un grupo que administra. Además, si un administrador de Adobe Workfront desbloquea una notificación de eventos, puede configurarla para un grupo de nivel superior que administre. La configuración de una notificación de eventos consiste en activarla o desactivarla.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 83%

---

# Ver y configurar notificaciones de eventos para un grupo

Como administrador de grupo, puede ver las notificaciones de eventos activadas para un grupo que administra.

Además, si un administrador de Adobe Workfront desbloquea una notificación de eventos, puede configurarla para un grupo de nivel superior que administre. La configuración de una notificación de eventos consiste en activarla o desactivarla.

Un administrador de Workfront también puede hacerlo para cualquier grupo.

La configuración de una notificación de eventos para un grupo afecta a los usuarios para los que ese grupo, o uno de sus subgrupos, es su grupo de inicio. Estos usuarios verán en los perfiles de usuario las notificaciones de eventos activadas para su grupo de inicio en lugar de las notificaciones de eventos activadas en todo el sistema.

Para obtener información sobre cómo un administrador de Workfront desbloquea una notificación de eventos, consulte [Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Para obtener información acerca de la configuración de notificación predeterminada para un evento, consulte [Tipos de notificaciones de eventos](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualización y configuración de las notificaciones de eventos de un grupo

>[!TIP]
>
>Si es administrador de Workfront y ya se encuentra en la página Notificaciones por correo electrónico (Configuración > Correo electrónico > Notificaciones), puede hacer lo siguiente y pasar al paso 6: Eliminar **Notificaciones de eventos del sistema** en el cuadro situado encima de la lista, empiece a escribir el nombre del grupo en el cuadro y, a continuación, haga clic en él cuando aparezca.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

1. Haga clic en el nombre del grupo de nivel superior.
1. En el menú de la izquierda, haga clic en **Notificaciones de eventos**.

   En la lista que se muestra, la columna **Activo** de la izquierda muestra qué notificaciones están activas (azules) e inactivas (grises) para el grupo.

1. Para activar o desactivar una notificación de eventos desbloqueados: haga clic en el botón de la columna <strong>Activo</strong> para activarla <img src="assets/email-notification-enabled-unlocked.png"> o desactivarlo <img src="assets/email-notification-disabled-unlocked.png">.

   >[!INFO]
   >
   >**Ejemplo:** puede configurar las dos notificaciones de eventos de grupos de marketing principales que se muestran a continuación y que se han desbloqueado para grupos.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Si un botón de la columna <strong>Activo</strong> está atenuado y en gris <img src="assets/email-notification-disabled-locked.png">, la notificación de eventos está desactivada para todos los usuarios y los administradores del grupo no pueden activarla ni editar la línea de asunto del correo electrónico
   >* Si un botón de la columna <strong>Activo</strong> es gris y no está atenuado <img src="assets/email-notification-disabled-unlocked.png">, la notificación de eventos está <strong>desactivada para todos los usuarios y los administradores del grupo de </strong> pueden activarla para sus grupos.
   >* Si un botón de la columna <strong>Activo</strong> aparece en azul y está atenuado <img src="assets/email-notification-enabled-locked.png">, la notificación de eventos está activada para todos los usuarios y los administradores del grupo no pueden desactivarla ni editar la línea de asunto de correo electrónico para sus grupos.
   >* Si un botón de la columna <strong>Activo</strong> aparece en azul y no está atenuado <img src="assets/email-notification-enabled-unlocked.png">, la notificación de eventos está <strong>activada para todos los usuarios y </strong> los administradores del grupo pueden desactivarla para sus grupos.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

