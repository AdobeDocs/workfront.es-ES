---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurar tipos de solicitud
description: Mientras trabaja en un proyecto, es posible que descubra que surgen eventos inesperados. Puede registrar esos eventos inesperados como problemas para un proyecto o tarea en particular. También puede enviar solicitudes, que se registran como problemas en un proyecto designado como Cola de solicitudes. Los problemas y las solicitudes se consideran intercambiables en Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 21%

---

# Configuración de tipos de solicitud

Mientras trabaja en un proyecto, es posible que descubra que surgen eventos inesperados. Puede registrar esos eventos inesperados como problemas para un proyecto o tarea en particular. También puede enviar solicitudes, que se registran como problemas en un proyecto designado como Cola de solicitudes. Los problemas y las solicitudes se consideran intercambiables en Adobe Workfront.

Para obtener información acerca de cómo crear problemas en [!DNL Workfront], vea [Crear problemas](../../../manage-work/issues/manage-issues/create-issues.md). Para obtener información acerca de cómo crear solicitudes en [!DNL Workfront], vea [Crear y enviar [!DNL Adobe Workfront] solicitudes](../../../manage-work/requests/create-requests/create-submit-requests.md). Para obtener información acerca de cómo asociar tipos de solicitud con proyectos, vea [Definir tipos de solicitud para un proyecto](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   O
   <p>Actual: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## Personalizar los nombres de los tipos de solicitud

Como administrador de [!DNL Workfront], puede configurar los nombres de los tipos de solicitud en su sistema. Los nuevos nombres son visibles en cualquier área de [!DNL Workfront] donde se muestren los campos **[!UICONTROL Tipo de problema]** o **[!UICONTROL Tipo de solicitud]**:

* En el área **[!UICONTROL Detalles de cola]** de un proyecto que recibirá los problemas o solicitudes.
* Si se selecciona más de un tipo de solicitud para una cola de solicitudes, en el formulario **[!UICONTROL Nuevo problema]** del campo **[!UICONTROL Tipo de problema]**, cuando cree un nuevo problema o envíe una nueva solicitud.

  Para obtener más información sobre la creación de problemas en [!DNL Workfront], consulte [Crear problemas](../../../manage-work/issues/manage-issues/create-issues.md)

  Para obtener más información sobre la creación de solicitudes en [!DNL Workfront], vea [Crear y enviar [!DNL Adobe Workfront] solicitudes](../../../manage-work/requests/create-requests/create-submit-requests.md).

* En el formulario **[!UICONTROL Detalle de tema de cola]**, al configurar el tema de cola.\
   Para obtener más información sobre cómo crear temas de colas, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Para personalizar los nombres de los tipos de solicitud:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Preferencias del proyecto]** > **[!UICONTROL Estados]**.

1. Haga clic en la pestaña **[!UICONTROL Problemas]**.
1. En la parte superior de la pestaña **[!UICONTROL Problemas]**, pase el ratón sobre el nombre de un tipo de solicitud y luego haga clic en el icono **[!UICONTROL Editar]** que aparece.

   ![Editar nombre de tipo de solicitud](assets/edit-request-type-name-nwe.png)

1. En el cuadro que aparece, escriba un nombre nuevo y presione **[!UICONTROL Entrar]**.

## Configuración de estados de problemas dentro de diferentes tipos de solicitudes

Puede asociar cada tipo de solicitud con diferentes estados de problemas. También puede cambiar el orden en que se muestran los estados de un problema, según el tipo de problema.

Para obtener más información sobre cómo cambiar el orden predeterminado de los estados de problema y configurar los estados de problema, consulte la sección [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) en [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
