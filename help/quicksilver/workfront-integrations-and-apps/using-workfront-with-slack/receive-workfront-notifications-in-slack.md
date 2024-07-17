---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Recibir [!DNL Adobe Workfront] notificaciones en [!DNL Slack]
description: Recibir [!DNL Adobe Workfront] notificaciones en [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 1%

---

# Recibir [!DNL Adobe Workfront] notificaciones en [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Después de instalar [!DNL Adobe Workfront for Slack], puede recibir [!DNL Workfront] notificaciones en [!DNL Slack].\
Para obtener información acerca de la instalación de [!DNL Workfront for Slack], vea [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Puede habilitar un número seleccionado de [!UICONTROL notificaciones] que aparecen en la burbuja de notificaciones de la interfaz [!DNL Workfront], para que también se entreguen en [!DNL Slack].

Las notificaciones por correo electrónico funcionan de forma independiente de las notificaciones de la interfaz [!DNL Workfront]. Usted o su administrador de [!DNL Workfront] pueden deshabilitar las notificaciones por correo electrónico, mientras que las notificaciones de interfaz no se pueden deshabilitar en [!DNL Workfront].\
Sin embargo, puede deshabilitar [!DNL Workfront] notificaciones que podría recibir en [!DNL Slack] si desea centrarse en esas notificaciones únicamente dentro de la interfaz [!DNL Workfront].

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].\

## Requisitos previos

Para poder recibir [!DNL Workfront] notificaciones en [!DNL Slack], debe

* Configurar [!DNL Workfront for Slack]\
   Para obtener instrucciones sobre cómo configurar [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configurar [!DNL Workfront] notificaciones para [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Condicional) Después de que [!DNL Workfront] se haya agregado a su instancia [!DNL Slack], inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener información sobre cómo iniciar sesión en [!DNL Workfront] desde [!DNL Slack], consulte [Acceso [!DNL Adobe Workfront] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir uno de los siguientes comandos en el campo de mensaje:

   `/workfront settings`

   O

   `/wf settings`

1. De forma predeterminada, todas las notificaciones están habilitadas.\
   Deshabilite cualquiera de las siguientes notificaciones:

   * [!UICONTROL Se me ha asignado una nueva tarea o problema]
   * [!UICONTROL Mi equipo está asignado a una nueva tarea o problema]
   * [!UICONTROL Recibo una nueva aprobación o solicitud de acceso]
   * [!UICONTROL Alguien me incluye en una actualización dirigida]
   * [!UICONTROL Alguien agrega comentarios a un hilo en el que participo]
   * [!UICONTROL Se ha realizado una actualización en una tarea, un problema o un proyecto al cual me he suscrito]
   * [!UICONTROL Alguien agrega comentarios a uno de mis elementos de trabajo]
   * [!UICONTROL Alguien agrega comentarios a mi solicitud de ayuda]

   Los cambios que realice en las opciones [!UICONTROL notifications] se aplicarán inmediatamente.\
   Las notificaciones que ha habilitado se entregan en el canal [!DNL Workfront] [!DNL Slack]. Cuando deshabilita las notificaciones aquí, solo se deshabilitan para [!DNL Slack] y no para la interfaz [!DNL Workfront]. Sigue recibiéndolos en la burbuja de notificaciones [!DNL Workfront] en la parte superior derecha de la interfaz.

## Administrar [!DNL Workfront] notificaciones de [!DNL Slack]

Puede recibir y responder a [!DNL Workfront] notificaciones de [!DNL Slack].

Puede deshabilitar las notificaciones por correo electrónico para las notificaciones que habilita en [!DNL Slack], a fin de asegurarse de que no recibe notificaciones duplicadas.\
Para obtener información sobre cómo configurar las notificaciones por correo electrónico, consulte [Modificar las notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Habilitar o deshabilitar [!DNL Workfront] notificaciones en [!DNL Slack] no afecta a las notificaciones que reciba dentro de la interfaz [!DNL Workfront].\
No se pueden deshabilitar las notificaciones dentro de la interfaz [!DNL Workfront].

Para administrar las notificaciones de [!DNL Workfront] para [!DNL Slack]:

1. Inicie sesión en [!UICONTROL Slack].
1. Iniciar sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener información sobre cómo iniciar sesión en [!DNL Workfront] desde [!DNL Slack], consulte la sección &quot;Iniciar sesión en [!DNL Workfront] desde [!DNL Slack]&quot; en [Acceso [!DNL Adobe Workfront] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Asegúrese de que las notificaciones de [!DNL Workfront] para [!DNL Slack] estén habilitadas.\
   Para obtener más información sobre qué [!DNL Workfront] notificaciones se pueden configurar para enviarlas también a [!DNL Slack], consulte [Configurar [!DNL Workfront] notificaciones para [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Vaya al canal **[!DNL Workfront]** para encontrar las notificaciones de [!DNL Workfront].
1. (Condicional y opcional) Realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Trabajar en ello]** para aceptar que se trabaje en una tarea.

   * (Condicional y opcional) Haga clic en **[!UICONTROL Responder en[!DNL Workfront]]** para responder a un comentario, escriba su respuesta y haga clic en **[!UICONTROL Responder]**.

   * (Condicional y opcional) Haga clic en **[!UICONTROL Aprobar]** o **[!UICONTROL Rechazar]** para aprobar o rechazar una tarea, problema o proyecto que esté pendiente de su aprobación.

   * (Condicional y opcional) Haga clic en **[!UICONTROL Aprobar]**, **[!UICONTROL Cambios]** o **[!UICONTROL Rechazar]** para aprobar, aprobar con cambios o rechazar un documento.

     También puede pasar el ratón sobre la miniatura del documento y hacer clic en el icono de lupa para ver una vista previa más grande del documento antes de aprobarlo.\
      Solo se puede obtener una vista previa de los [tipos de archivo](https://api.slack.com/types/file) del Slack aprobado.

   * (Condicional y opcional) Haga clic en **[!UICONTROL Conceder]** o **[!UICONTROL Ignorar]** para conceder o ignorar la solicitud de más acceso de otro usuario.\

     Recibirá una confirmación de que su acción se completó en [!DNL Workfront], por cada decisión que tome dentro de sus notificaciones.
