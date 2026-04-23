---
title: Agregar una aprobación a un formulario de solicitud en Adobe Workfront Planning
description: Puede agregar un proceso de aprobación a un formulario de solicitud de Adobe Workfront Planning para iniciar una aprobación para cada solicitud enviada antes de crear un registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 5%

---

# Agregar una aprobación a un formulario de solicitud en Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Puede agregar un proceso de aprobación a un formulario de solicitud de Adobe Workfront Planning para iniciar una aprobación para cada solicitud enviada antes de crear un registro.

This article describes how a workspace manager can add an approval to a request form associated with a record type.

Para obtener información acerca de cómo crear un formulario de solicitud en Workfront Planning, vea [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Para obtener información sobre cómo enviar una solicitud a un tipo de registro para crear un registro, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquetes de Adobe Workfront</p></td> 
   <td> 
<p>Any Workfront package and any Planning package</p>
O
<p>Any Workflow package and any Planning package</p>

<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Manage permissions to a workspace and  record type</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations about adding approvals to a request form

* Puede agregar uno o varios aprobadores a un formulario de solicitud. Puede agregar usuarios y equipos como aprobadores.
* Puede mostrar la información de aprobación de un registro creado enviando un formulario de solicitud en los campos Aprobado por y Fecha de aprobación. Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).
* Cuando se agregan varios aprobadores a un formulario de solicitud, todos los aprobadores deben aceptar la solicitud antes de crear un registro en Workfront Planning.
* Si todos los aprobadores aprueban la solicitud, se crea un registro para el tipo de registro asociado al formulario de solicitud.
* If at least one approver rejects the request, and all others approve it, a request is created for the Requests area in Workfront, but no record is created for the record type associated with the request form.
* Añadir aprobaciones a un formulario de solicitud es opcional. Workfront Planning crea inmediatamente un registro cuando se envía una solicitud, si el formulario de solicitud no está asociado a una aprobación.

<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->

## Adición de reglas de aprobación a un formulario de solicitud

Las reglas de aprobación definen el proceso de aprobación en función de los valores de los campos de las solicitudes enviadas.

Por ejemplo, si un formulario de solicitud tiene el campo &quot;Tipo de campaña&quot;, se puede crear una regla que envíe la solicitud a una persona cuando el campo tenga el valor &quot;Digital&quot; y a una persona diferente cuando tenga el valor &quot;Imprimir&quot;.

Tenga en cuenta lo siguiente al añadir reglas de aprobación:

* You can add one or several approvers to an approval rule.
* If at least one approver rejects the request, the request is rejected and the record is not created. La solicitud permanece en el área de solicitudes de Workfront.
* Si añade más de un aprobador y la opción Only one decision is required no está activada, todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.
* Si un equipo se establece como aprobador, solo se requiere una decisión de un miembro del equipo.

Para definir reglas de aprobación para un formulario de solicitud:

1. Start creating a request form for a record type, as described in the article [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. When the request form opens, click **Settings**.

   The **Settings** tab opens.

1. To begin configuring approval rules, click **Approvals** ![Approvals icon](assets/approvals-icon-on-form.png) in the left panel.

1. (Optional) If you want to set a default approval process, add at least one user or team to the **Approvers** field of the **Default approval rule** area, then click the **Only one decision is required** checkbox if you want the record to be created after any one of the default approvers has approved it.

   ![Área de regla de aprobación predeterminada](assets/default-approvers.png)

1. (Opcional) Empiece a añadir reglas de aprobación. Para cada regla de aprobación personalizada, haga lo siguiente:

   1. Haga clic en **Agregar regla de aprobación**
   1. Haga clic en el título del marcador de posición **Regla de aprobación sin título** e introduzca un nombre para la regla de aprobación.
   1. Click **Select a field** and select the field that activates the rule.
   1. Seleccione el operador de la regla. Operators vary based on the type of field.
   1. If the selected operator requires a value, click the plus icon and add one or more values.
   1. (Optional) Click **Add condition** to add more conditions and connect them by **And** or **Or** statements by configuring the additional conditions as in steps C-E.
   1. In the **Actions** area of the approval rule, in the **Approvers** field, add at least one user or team to be set at the approver when the condition is met.
   1. (Condicional y opcional) Si desea que el registro se cree después de que cualquiera de los aprobadores lo haya aprobado, marque la casilla **Solo se requiere una decisión**. De lo contrario, todos los aprobadores deben decidir la aprobación antes de aceptar o rechazar la solicitud.

   >[!NOTE]
   >
   >   Consider the following when adding approval rules:
   >
   >   * If only a default rule is set up, it applies to every submitted request.
   >   * If a custom rule is met, the default is not applied to the request approval workflow. Only the matched custom rules apply for approvals and the default rule is ignored.
   >   * If multiple custom rules are met, the first one in the order applies. In this case, the default approval does not apply, if there is one.

1. Haga clic en **Guardar** para guardar las reglas de aprobación.
1. (Opcional) Haga clic en **Publicar** si nunca antes había compartido el formulario de solicitud.
