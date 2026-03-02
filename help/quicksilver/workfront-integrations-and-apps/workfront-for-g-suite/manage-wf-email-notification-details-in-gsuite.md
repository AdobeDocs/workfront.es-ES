---
product-area: workfront-integrations
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Administración de detalles de notificación de  [!DNL Adobe Workfront]  de Google Workspace
description: En Google Workspace, al abrir notificaciones por correo electrónico enviadas por Adobe  [!DNL Workfront] , es posible ver los detalles del elemento de trabajo asociado y responder sin salir de la bandeja de entrada. Si hubiera acciones disponibles, como aprobar una solicitud, será posible realizarlas directamente desde Workfront para Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: ddd1c964c4c885f71dfa30d1790cfbc6e26d6781
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 42%

---

# Administrar detalles de notificación de [!DNL Adobe Workfront] de [!DNL Google Workspace]

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, hemos optado por un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la siguiente funcionalidad de Workfront para Google Workspace **ya no está disponible**:
>
>* Acceso a la funcionalidad de Google Workspace desde Workfront
>
>* Visualización y administración de tareas de Workfront desde Gmail o el panel de sitio Calendario de Google
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Google Workspace.
>
>Para obtener información general sobre la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Google Workspace, consulte [Módulos de Gmail](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) y [Módulos de Google Calendar](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

<!--

In [!DNL Google Workspace], when you open a notification email [!DNL Adobe Workfront] has sent, you can view the associated work item details and respond without leaving your [!UICONTROL Inbox]. If actions are available, such as approving a request, you can perform those actions directly from [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] supports almost every type of email notification you can receive from [!DNL Workfront] (about 120 different types). [!UICONTROL Daily digest] emails sent from [!DNL Workfront] do not appear in [!DNL Workfront for Google Workspace]. For information about the [!DNL Workfront] email notification types, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p><p>Work or higher</p>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you can manage notification details from [!DNL Google Workspace], you must

* Install [!DNL Workfront for Google Workspace]\
   For instructions, see [Install [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Manage [!DNL Adobe Workfront] notification details from [!DNL Google Workspace]

1. If the [!DNL Workfront for Google Workspace] panel is not displayed, click the [!DNL Workfront] icon ![Workfront icon](assets/wf-lion-icon.png) in the [!DNL Google Workspace] add-ons sidebar at the far-right of the page.
1. In [!DNL Google Workspace], open a [!DNL Workfront] notification email.
1. Click **[!UICONTROL View all updates]** if it is displayed near the top of the panel.
1. Click **[!UICONTROL Details]**.
1. Click any available options.

   The options that might display relate to the type of email notification you have opened. For example, if it's an email notification asking you to approve a task, you see **[!UICONTROL Approve]** and **[!UICONTROL Reject]** instead of options such as **[!UICONTROL Work on It]** or **[!UICONTROL Done]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type of email notification</th> 
      <th>Action</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Task or issue</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, <strong>[!UICONTROL Ignore]</strong> a request for access to it, <strong>[!UICONTROL Work on it]</strong>, or click an option to indicate that you are <strong>[!UICONTROL Done]</strong> with it</td> 
     </tr> 
     <tr> 
      <td>Project</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, or <strong>[!UICONTROL Ignore]</strong> a request for access to it</td> 
     </tr> 
     <tr> 
      <td>Document</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, or <strong>[!UICONTROL Ignore]</strong> a request for access to it</td> 
     </tr> 
     <tr> 
      <td>Update </td> 
      <td> <p>View any part of the entire list of updates for the item so that you have the context you need to <strong>[!UICONTROL Post]</strong> a new update or a <strong>[!UICONTROL Reply]</strong>. You can click <strong>[!UICONTROL Notify]</strong> to alert particular users about your reply. </p> <p>For more information, see <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Reply to a [!DNL Adobe Workfront] update notification from [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Approval request</td> 
      <td><strong>[!UICONTROL Approve]</strong> or <strong>[!UICONTROL Reject]</strong> it (you can change your mind by clicking the other option), download it, view its owner, or view its reference number</td> 
     </tr> 
     <tr> 
      <td>A change in a project's status</td> 
      <td> View all the current information about the project, including any custom forms. </td> 
     </tr> 
    </tbody> 
   </table>

   -->
