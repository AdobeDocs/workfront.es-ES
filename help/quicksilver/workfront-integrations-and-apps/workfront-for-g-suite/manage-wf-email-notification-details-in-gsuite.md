---
product-area: workfront-integrations
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Administración de detalles de notificación de  [!DNL Adobe Workfront]  de Google Workspace
description: En Google Workspace, al abrir notificaciones por correo electrónico enviadas por Adobe  [!DNL Workfront] , es posible ver los detalles del elemento de trabajo asociado y responder sin salir de la bandeja de entrada. Si hubiera acciones disponibles, como aprobar una solicitud, será posible realizarlas directamente desde Workfront para Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 76%

---

# Administrar detalles de notificación de [!DNL Adobe Workfront] de [!DNL Google Workspace]

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la siguiente funcionalidad de Workfront para Google Workspace no estará disponible después del **28 de febrero de 2026**:
>
>* Acceso a la funcionalidad de Google Workspace desde Workfront
>
>* Visualización y administración de tareas de Workfront desde Gmail o el panel de sitio Calendario de Google
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Google Workspace.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Google Workspace, consulte [Módulos de Gmail](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) y [Módulos de Google Calendar](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

En [!DNL Google Workspace], al abrir notificaciones por correo electrónico enviadas por [!DNL Adobe Workfront], es posible ver los detalles del elemento de trabajo asociado y responder sin salir de la [!UICONTROL bandeja de entrada]. Si hubiera acciones disponibles, como aprobar una solicitud, será posible realizar esas acciones directamente desde [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] admite casi todos los tipos de notificaciones por correo electrónico que se pueden recibir de [!DNL Workfront] (unos 120 tipos diferentes). Los correos electrónicos de [!UICONTROL resumen diario] enviados desde [!DNL Workfront] no aparecen en [!DNL Workfront for Google Workspace]. Para obtener información sobre los tipos de notificación por correo electrónico de [!DNL Workfront], consulte [Modificar las propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

Para poder administrar los detalles de notificaciones de [!DNL Google Workspace], es necesario

* Instalar [!DNL Workfront for Google Workspace]\
   Para obtener instrucciones, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Administrar los detalles de notificaciones de [!DNL Adobe Workfront] de [!DNL Google Workspace]

1. Si no se muestra el panel [!DNL Workfront for Google Workspace], haga clic en el icono [!DNL Workfront] ![Workfront icon](assets/wf-lion-icon.png) en la barra lateral de complementos de [!DNL Google Workspace], en el extremo derecho de la página.
1. En [!DNL Google Workspace], abra una notificación por correo electrónico de [!DNL Workfront].
1. Haga clic en **[!UICONTROL Ver todas las actualizaciones]** si se mostrase cerca de la parte superior del panel.
1. Haga clic en **[!UICONTROL Detalles]**.
1. Haga clic en cualquier opción disponible.

   Las opciones que se mostrarán se relacionan con el tipo de notificación por correo electrónico que se abrió. Por ejemplo, si se tratase de una notificación por correo electrónico en la que se le pidiera la aprobación de una tarea, vería **[!UICONTROL Aprobar]** y **[!UICONTROL Rechazar]**, en lugar de opciones como **[!UICONTROL En proceso]** o **[!UICONTROL Listo]**:

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
      <td><strong>[!UICONTROL Approve]</strong>, <strong>[!UICONTROL Reject]</strong>, <strong>[!UICONTROL Grant]</strong> el acceso, <strong>[!UICONTROL Ignore]</strong> una solicitud de acceso, <strong>[!UICONTROL Work on it]</strong> o haga clic en una opción para indicar que está <strong>[!UICONTROL Done]</strong></td> 
     </tr> 
     <tr> 
      <td>Proyecto</td> 
      <td><strong>[!UICONTROL Approve]</strong>, <strong>[!UICONTROL Reject]</strong>, <strong>[!UICONTROL Grant]</strong> el acceso o <strong>[!UICONTROL Ignore]</strong> una solicitud de acceso</td> 
     </tr> 
     <tr> 
      <td>Documento</td> 
      <td><strong>[!UICONTROL Approve]</strong>, <strong>[!UICONTROL Reject]</strong>, <strong>[!UICONTROL Grant]</strong> el acceso o <strong>[!UICONTROL Ignore]</strong> una solicitud de acceso</td> 
     </tr> 
     <tr> 
      <td>Actualizar </td> 
      <td> <p>Consulte cualquier parte de la lista completa de actualizaciones del elemento para obtener el contexto necesario para <strong>[!UICONTROL Post]</strong> una nueva actualización o una <strong>[!UICONTROL Reply]</strong>. Haga clic en <strong>[!UICONTROL Notify]</strong> para alertar a usuarios concretos sobre la respuesta. </p> <p>Para obtener más información, consulte <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Responder a una notificación de actualización de [!DNL Adobe Workfront] de [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Solicitud de aprobación</td> 
      <td><strong>[!UICONTROL Approve]</strong> o <strong>[!UICONTROL Reject]</strong> (es posible cambiar de opinión haciendo clic en la otra opción), descargar, consultar el propietario o consultar el número de referencia</td> 
     </tr> 
     <tr> 
      <td>Cambio en el estado de un proyecto</td> 
      <td> Permite ver toda la información actual del proyecto, incluyendo los formularios personalizados. </td> 
     </tr> 
    </tbody> 
   </table>
