---
product-area: workfront-integrations
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Administrar [!DNL Adobe Workfront] detalles de notificación de G Suite
description: En G Suite, al abrir un Adobe de correo electrónico de notificación [!DNL Workfront] se ha enviado, puede ver los detalles del elemento de trabajo asociado y responder sin salir de la bandeja de entrada. Si hay acciones disponibles, como aprobar una solicitud, puede realizar dichas acciones directamente desde Workfront para G Suite.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 0934ae23a8e80dd18872efef7d274bd57d227647
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Administrar [!DNL Adobe Workfront] detalles de notificaciones de [!DNL G Suite]

>[!NOTE]
>
>Hay un [problema conocido](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) con la versión actual de [!DNL Workfront for G Suite] no funciona como se esperaba. Estamos trabajando en una nueva versión y esperamos que se publique en el [!DNL Google Marketplace] en un futuro próximo.

En [!DNL G Suite], al abrir un correo electrónico de notificación [!DNL Adobe Workfront] se ha enviado, puede ver los detalles del elemento de trabajo asociado y responder sin dejar su [!UICONTROL Bandeja de entrada]. Si hay acciones disponibles, como aprobar una solicitud, puede realizar dichas acciones directamente desde [!DNL Workfront for G Suite].

>[!NOTE]
>
> [!DNL Workfront for G Suite] admite casi todos los tipos de notificación por correo electrónico desde los que puede recibir [!DNL Workfront] (unos 120 tipos diferentes). [!UICONTROL Resumen diario] correos electrónicos enviados desde [!DNL Workfront] no aparecen en [!DNL Workfront for G Suite]. Para obtener información sobre la variable [!DNL Workfront] tipos de notificación de correo electrónico, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Antes de administrar los detalles de las notificaciones desde [!DNL G Suite], debe

* Instalar [!DNL Workfront for G suite]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Administrar [!DNL Adobe Workfront] detalles de notificaciones de [!DNL G Suite]

1. Si la variable [!DNL Workfront for G Suite] no se muestra el panel, haga clic en el botón [!DNL Workfront] icono ![](assets/wf-lion-icon.png) en el [!DNL G Suite] barra lateral de complementos en el extremo derecho de la página.
1. En [!DNL G Suite], abra un [!DNL Workfront] correo electrónico de notificación.
1. Haga clic en **[!UICONTROL Ver todas las actualizaciones]** si se muestra cerca de la parte superior del panel.
1. Haga clic en **[!UICONTROL Detalles]**.
1. Haga clic en las opciones disponibles.

   Las opciones que se pueden mostrar están relacionadas con el tipo de notificación de correo electrónico que ha abierto. Por ejemplo, si se trata de una notificación por correo electrónico en la que se le pide que apruebe una tarea, verá **[!UICONTROL Aprobar]** y **[!UICONTROL Rechazar]** en lugar de opciones como **[!UICONTROL Trabajar en él]** o **[!UICONTROL Listo]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo de notificación por correo electrónico</th> 
      <th>Acción</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Tarea o problema</td> 
      <td><strong>[!UICONTROL Aprobar]</strong> it, <strong>[!UICONTROL Rechazar]</strong> it, <strong>[!UICONTROL Grant]</strong> acceso a él, <strong>[!UICONTROL Ignorar]</strong> una solicitud de acceso a ella, <strong>[!UICONTROL Trabajar en él]</strong>o haga clic en una opción para indicar que <strong>[!UICONTROL Listo]</strong> con</td> 
     </tr> 
     <tr> 
      <td>Proyecto</td> 
      <td><strong>[!UICONTROL Aprobar]</strong> it, <strong>[!UICONTROL Rechazar]</strong> it, <strong>[!UICONTROL Grant]</strong> acceso a él, o <strong>[!UICONTROL Ignorar]</strong> una solicitud de acceso a ella</td> 
     </tr> 
     <tr> 
      <td>Documento</td> 
      <td><strong>[!UICONTROL Aprobar]</strong> it, <strong>[!UICONTROL Rechazar]</strong> it, <strong>[!UICONTROL Grant]</strong> acceso a él, o <strong>[!UICONTROL Ignorar]</strong> una solicitud de acceso a ella</td> 
     </tr> 
     <tr> 
      <td>Actualizar </td> 
      <td> <p>Ver cualquier parte de la lista completa de actualizaciones para el elemento, de modo que tenga el contexto que necesita <strong>[!UICONTROL Post]</strong> una actualización nueva o una <strong>[!UICONTROL Respuesta]</strong>. Puede hacer clic en <strong>[!UICONTROL Notificar]</strong> para alertar a usuarios concretos sobre su respuesta. </p> <p>Para obtener más información, consulte <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Responder a un [!DNL Adobe Workfront] actualizar notificación desde [!DNL G Suite]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Solicitud de aprobación</td> 
      <td><strong>[!UICONTROL Aprobar]</strong> o <strong>[!UICONTROL Rechazar]</strong> (puede cambiar de opinión haciendo clic en la otra opción), descargarla, ver a su propietario o ver su número de referencia</td> 
     </tr> 
     <tr> 
      <td>Un cambio en el estado de un proyecto</td> 
      <td> Vea toda la información actual sobre el proyecto, incluidos los formularios personalizados. </td> 
     </tr> 
    </tbody> 
   </table>
