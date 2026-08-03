---
title: Administrar notificaciones de correo electrónico de Adobe Workfront Planning
description: Cuando alguien le etiqueta a usted o a sus equipos en un comentario de registro en Adobe Workfront Planning, recibe una notificación por correo electrónico de esa etiqueta.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
last-update: 2026-04-01T18:23:03.000Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
TQID: https://experienceleague.adobe.com/4MvX3EX6KfcXwk5lrq6bRU7HC6gzAI1Zgi49TMZbP7M
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 347c3e87fea0289616bf1a52779c07501a8ec69d
workflow-type: tm+mt
source-wordcount: 646
ht-degree: 17%

---

# Administrar notificaciones por correo electrónico de Adobe Workfront Planning

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Puede recibir notificaciones por correo electrónico de Workfront Planning cuando existan los siguientes escenarios:

* Alguien le etiqueta a usted o a sus equipos en un comentario de registro

  Para obtener información sobre cómo etiquetar a otras personas en un comentario de registro, consulte [Administrar comentarios de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* Alguien le pide permiso para acceder a una vista, un espacio de trabajo, un tipo de registro o un registro
* Alguien confirma que se ha concedido su acceso a una vista, espacio de trabajo, tipo de registro o registro
* Envía una solicitud de Workfront Planning. Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Alguien aprueba o rechaza una solicitud de Workfront Planning que usted haya enviado. Para obtener más información, consulte [Aprobar una solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* El estado cambia a una solicitud de Workfront Planning que ha enviado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p> <p>Cualquier paquete de Planning cuando se adquiere como producto independiente</p>
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Flujo de trabajo ligero o superior</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Colaborador de Planning o superior</p>
<p><b>NOTA</b></p>
<p>No todos los clientes tienen una licencia de colaborador</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de vista o superiores a un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD: 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>

</tbody> 
</table>
-->


## Administrar notificaciones por correo electrónico cuando alguien le etiqueta en un comentario

1. (Condicional y opcional) Después de que alguien le etiquete a usted o a su equipo en un comentario de un registro, vaya a la notificación por correo electrónico que le informa de la etiqueta y del comentario. El remitente del correo electrónico es Adobe Experience Cloud.

   ![Ejemplo de notificaciones por correo electrónico](assets/email-notification-example.png)

1. (Opcional) Haga clic en el mensaje en el cuadro **Workfront** dentro del correo electrónico.

   Se abre la página de detalles de registro en Workfront. Puede realizar actualizaciones en el registro o responder al comentario.

1. (Condicional) Si está disponible, haga clic en **Ver todas las notificaciones**. <!--check with Lilit - do non-IMS users have this button??-->
La página **Notificaciones** se abre en Adobe Experience Cloud. Se muestran todas las notificaciones de todas las aplicaciones de Adobe Experience Cloud.

## Administrar notificaciones por correo electrónico al solicitar y conceder permisos

1. (Condicional y opcional) Después de que alguien solicite o le conceda permisos para acceder a un objeto de Planning, vaya al mensaje de correo electrónico que le informa de la solicitud de permiso. El remitente del correo electrónico es Adobe Experience Cloud.

1. (Opcional) Haga clic en el mensaje en el cuadro **Workfront** dentro del correo electrónico.

   El objeto para el que solicitó permisos se abre en Workfront.

1. (Condicional) Si está disponible, haga clic en **Ver todas las notificaciones**.
La página **Notificaciones** se abre en Adobe Experience Cloud. Se muestran todas las notificaciones de todas las aplicaciones de Adobe Experience Cloud.


Para obtener información sobre cómo solicitar, conceder o denegar permisos, vea [Solicitar permisos a una vista o área de trabajo](/help/quicksilver/planning/access/request-permissions.md).

Para obtener información sobre cómo administrar las notificaciones de Workfront Planning, consulte [Administrar las preferencias de notificación de Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Administrar notificaciones por correo electrónico sobre el envío, la aprobación o el rechazo de solicitudes de Workfront Planning

1. (Opcional) Vaya al correo electrónico que Workfront le envía después de enviar una solicitud, o después de que una solicitud enviada se haya aprobado o rechazado. El remitente del correo electrónico es Adobe Workfront.

1. (Opcional) Haga clic en **Abrir solicitud**. Esto abre la solicitud en Workfront Planning.

1. En la esquina superior derecha de la solicitud, haga clic en el botón **Revisar y aprobar** y, a continuación, haga clic en una de las siguientes opciones:

   * **Aprobar** para aprobar la solicitud. Se crea un registro al aprobar una solicitud de Planning.
   * **Rechazar** para rechazar la solicitud. No se crea ningún registro cuando se rechaza una solicitud en Workfront Planning. La solicitud se guardó en el área de solicitudes con el estado **Rechazada**.

   ![Botón Revisar y aprobar en la solicitud de Planning](assets/review-approval-button-with-drop-down-expanded.png)

1. Haga clic en el icono **Notificaciones** ![Icono del área de notificaciones Unified Shell](assets/notifications-area-icon-unified-shell.png) en la esquina superior derecha de la pantalla para acceder a la página **Notificaciones**.

   Para obtener información sobre cómo administrar las notificaciones de Workfront Planning, consulte [Administrar las preferencias de notificación de Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
