---
title: Agregar una aprobación a un formulario de solicitud en Adobe Workfront Planning
description: Puede agregar un proceso de aprobación a un formulario de solicitud de Adobe Workfront Planning para iniciar una aprobación para cada solicitud enviada antes de crear un registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/E9LEGJ8T822JuvIO3s8nn6UkLbX-j4ffwaKSviKxl0o
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 930
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

Este artículo describe cómo un administrador del espacio de trabajo puede agregar una aprobación a un formulario de solicitud asociado a un tipo de registro.

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
<p>Cualquier paquete Workfront y cualquier paquete Planning</p>
O
<p>Cualquier paquete de flujo de trabajo y cualquier paquete de Planning</p>

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
   <td>   <p>Administrar permisos a un espacio de trabajo y tipo de registro</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre la adición de aprobaciones a un formulario de solicitud

* Puede agregar uno o varios aprobadores a un formulario de solicitud. Puede agregar usuarios y equipos como aprobadores.
* Puede mostrar la información de aprobación de un registro creado enviando un formulario de solicitud en los campos Aprobado por y Fecha de aprobación. Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).
* Cuando se agregan varios aprobadores a un formulario de solicitud, todos los aprobadores deben aceptar la solicitud antes de crear un registro en Workfront Planning.
* Si todos los aprobadores aprueban la solicitud, se crea un registro para el tipo de registro asociado al formulario de solicitud.
* Si al menos un aprobador rechaza la solicitud y todos los demás la aprueban, se crea una solicitud para el área de Solicitudes en Workfront, pero no se crea ningún registro para el tipo de registro asociado al formulario de solicitud.
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

* Puede añadir uno o varios aprobadores a una regla de aprobación.
* Si al menos un aprobador rechaza la solicitud, esta se rechaza y no se crea el registro. La solicitud permanece en el área de solicitudes de Workfront.
* Si añade más de un aprobador y la opción Only one decision is required no está activada, todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.
* Si un equipo se establece como aprobador, solo se requiere una decisión de un miembro del equipo.

Para definir reglas de aprobación para un formulario de solicitud:

1. Comience a crear un formulario de solicitud para un tipo de registro, tal como se describe en el artículo [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Cuando se abra el formulario de solicitud, haga clic en **Configuración**.

   Se abre la ficha **Configuración**.

1. Para comenzar a configurar las reglas de aprobación, haga clic en **Aprobaciones** ![Icono de aprobaciones](assets/approvals-icon-on-form.png) en el panel izquierdo.

1. (Opcional) Si desea establecer un proceso de aprobación predeterminado, agregue al menos un usuario o equipo al campo **Aprobadores** del área **Regla de aprobación predeterminada** y, a continuación, haga clic en la casilla de verificación **Solo se requiere una decisión** si desea que el registro se cree después de que cualquiera de los aprobadores predeterminados lo haya aprobado.

   ![Área de regla de aprobación predeterminada](assets/default-approvers.png)

1. (Opcional) Empiece a añadir reglas de aprobación. Para cada regla de aprobación personalizada, haga lo siguiente:

   1. Haga clic en **Agregar regla de aprobación**
   1. Haga clic en el título del marcador de posición **Regla de aprobación sin título** e introduzca un nombre para la regla de aprobación.
   1. Haga clic en **Seleccionar un campo** y seleccione el campo que activa la regla.
   1. Seleccione el operador de la regla. Los operadores varían según el tipo de campo.
   1. Si el operador seleccionado requiere un valor, haga clic en el icono de signo más y añada uno o más valores.
   1. (Opcional) Haga clic en **Agregar condición** para agregar más condiciones y conectarlas mediante instrucciones **And** o **Or** configurando las condiciones adicionales como en los pasos C-E.
   1. En el área **Actions** de la regla de aprobación, en el campo **Aprobadores**, agregue al menos un usuario o equipo que se establecerá en el aprobador cuando se cumpla la condición.
   1. (Condicional y opcional) Si desea que el registro se cree después de que cualquiera de los aprobadores lo haya aprobado, marque la casilla **Solo se requiere una decisión**. De lo contrario, todos los aprobadores deben decidir la aprobación antes de aceptar o rechazar la solicitud.

   >[!NOTE]
   >
   >   Tenga en cuenta lo siguiente al añadir reglas de aprobación:
   >
   >   * Si solo se configura una regla predeterminada, se aplica a todas las solicitudes enviadas.
   >   * Si se cumple una regla personalizada, el valor predeterminado no se aplica al flujo de trabajo de solicitud y aprobación. Solo se aplican las reglas personalizadas coincidentes para las aprobaciones y se ignora la regla predeterminada.
   >   * Si se cumplen varias reglas personalizadas, se aplica la primera del orden. En este caso, la aprobación predeterminada no se aplica, si es que la hay.

1. Haga clic en **Guardar** para guardar las reglas de aprobación.
1. (Opcional) Haga clic en **Publicar** si nunca antes había compartido el formulario de solicitud.
