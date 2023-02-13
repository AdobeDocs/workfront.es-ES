---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Recibir [!DNL Adobe Workfront] notificaciones en [!DNL Slack]
description: Recibir [!DNL Adobe Workfront] notificaciones en [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 6%

---

# Recibir [!DNL Adobe Workfront] notificaciones en [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Una vez instalado [!DNL Adobe Workfront for Slack], puede recibir [!DNL Workfront] notificaciones en [!DNL Slack].\
Para obtener información sobre la instalación [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Puede habilitar un número determinado de [!UICONTROL notificaciones] que aparecen en la burbuja de notificaciones de la sección [!DNL Workfront] interfaz, que también se enviará en [!DNL Slack].

Las notificaciones por correo electrónico funcionan de forma independiente [!DNL Workfront] notificaciones de la interfaz. Usted o su [!DNL Workfront] el administrador puede desactivar las notificaciones por correo electrónico, mientras que las notificaciones de la interfaz no pueden desactivarse en [!DNL Workfront].\
Sin embargo, puede desactivar [!DNL Workfront] notificaciones que podría recibir en [!DNL Slack], si desea centrarse en esas notificaciones solo dentro del [!DNL Workfront] interfaz.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.\

## Requisitos previos

Antes de recibir [!DNL Workfront] notificaciones en [!DNL Slack], debe

* Configurar [!DNL Workfront for Slack]\
   Para obtener instrucciones sobre la configuración [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configurar [!DNL Workfront] notificaciones para [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Condicional) Después [!DNL Workfront] se ha añadido a [!DNL Slack] instancia, iniciar sesión [!DNL Workfront] from [!DNL Slack].\
   Para obtener información sobre cómo iniciar sesión [!DNL Workfront] from [!DNL Slack], consulte [Acceso [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir uno de los siguientes comandos en el campo del mensaje:

   `/workfront settings`

   O

   `/wf settings`

   <img src="assets/slack-configuring-settings-350x302.png" style="width: 350;height: 302;">

1. De forma predeterminada, todas las notificaciones están habilitadas.\
   Desactive cualquiera de las siguientes notificaciones:

   * [!UICONTROL Estoy asignado a una nueva tarea o problema]
   * [!UICONTROL Mi equipo está asignado a una nueva tarea o problema]
   * [!UICONTROL Recibo una nueva aprobación o solicitud de acceso]
   * [!UICONTROL Alguien me incluye en una actualización dirigida]
   * [!UICONTROL Alguien agrega un comentario a un hilo en el cual participo]
   * [!UICONTROL Se hace una actualización a una tarea, un problema o un proyecto al cual me he suscrito]
   * [!UICONTROL Alguien agrega comentarios a uno de mis elementos de trabajo]
   * [!UICONTROL Alguien comenta sobre mi solicitud de ayuda]

   Los cambios que realice en la variable [!UICONTROL notificaciones] las opciones se aplican inmediatamente.\
   Las notificaciones habilitadas se entregan en la [!DNL Workfront] [!DNL Slack] canal. Cuando desactiva las notificaciones aquí, solo se desactivan para [!DNL Slack]y no para la variable [!DNL Workfront] interfaz. Continúe recibiéndolos en el [!DNL Workfront] las notificaciones se propagan en la parte superior derecha de la interfaz.

## Administrar [!DNL Workfront] notificaciones de [!DNL Slack]

Puede recibir y responder a [!DNL Workfront] notificaciones de [!DNL Slack].

Puede desactivar las notificaciones por correo electrónico para las notificaciones que active en [!DNL Slack], para asegurarse de que no reciba notificaciones duplicadas.\
Para obtener información sobre la configuración de las notificaciones por correo electrónico, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Activación o desactivación [!DNL Workfront] notificaciones en [!DNL Slack] no afecta a las notificaciones que reciba dentro del [!DNL Workfront] interfaz.\
Notificaciones dentro del [!DNL Workfront] no se puede deshabilitar la interfaz.

Para administrar su [!DNL Workfront] notificaciones para [!DNL Slack]:

1. Iniciar sesión en [!UICONTROL Slack].
1. Iniciar sesión en [!DNL Workfront] from [!DNL Slack].\
   Para obtener información sobre cómo iniciar sesión en [!DNL Workfront] from [!DNL Slack], consulte &quot;Inicio de sesión en [!DNL Workfront] from [!DNL Slack]&quot; en [Acceso [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Asegúrese de que su [!DNL Workfront] notificaciones para [!DNL Slack] están activados.\
   Para obtener más información, consulte [!DNL Workfront] las notificaciones se pueden configurar para que también se envíen a [!DNL Slack], consulte [Configurar [!DNL Workfront] notificaciones para [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Vaya a la **[!DNL Workfront]** canal para encontrar el [!DNL Workfront] notificaciones.
1. (Condicional y opcional) Realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Trabaje en él]** aceptar para trabajar en una tarea.

      <!--   
     <img src="assets/slack-assigned-to-a-task-notification-350x198.png" alt="slack_assigned_to_a_task_notification.png" style="width: 350;height: 198;" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * (Condicional y opcional) Haga clic en **[!UICONTROL Responder en[!DNL Workfront]]** para responder a un comentario, escriba su respuesta y haga clic en **[!UICONTROL Responder]**.\

      ![slack_tagged_in_a_comment_notification.png](assets/slack-tagged-in-a-comment-notification.png)

   * (Condicional y opcional) Haga clic en **[!UICONTROL Aprobar]** o **[!UICONTROL Rechazar]** para aprobar o rechazar una tarea, un problema o un proyecto que estén pendientes de aprobación.\

      ![slack_approve_task_notification_png](assets/slack-approve-task-notification-350x105.png)

   * (Condicional y opcional) Haga clic en **[!UICONTROL Aprobar]**, **[!UICONTROL Cambios]** o **[!UICONTROL Rechazar]**, para aprobar, aprobar con cambios o rechazar un documento.\

      ![slack_approve_a_document.png](assets/slack-approve-a-document-350x362.png)\
      También puede pasar el ratón sobre la miniatura del documento y hacer clic en el icono de lupa para ver una previsualización más grande del documento, antes de aprobarlo.\
      Solo el Slack aprobado [tipos de archivo](https://api.slack.com/types/file) se puede obtener una vista previa.

   * (Condicional y opcional) Haga clic en **[!UICONTROL Concesión]** o **[!UICONTROL Ignorar]** para conceder o ignorar la solicitud de más acceso de otro usuario.\

      ![](assets/slack-access-approvals-list-350x213.png)\
      Recibirá una confirmación de que su acción se ha completado en [!DNL Workfront], para cada decisión que tome dentro de sus notificaciones.
