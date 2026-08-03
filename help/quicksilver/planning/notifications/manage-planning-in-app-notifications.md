---
title: Administrar notificaciones en la aplicación de Adobe Workfront Planning
description: Cuando alguien le etiqueta a usted o a sus equipos en un comentario de registro, recibe una notificación por correo electrónico para esa etiqueta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
last-update: 2026-04-01T18:23:03.000Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
TQID: https://experienceleague.adobe.com/1RARIfclq-MB5bDLbn0m9zziFvuz1ugOyRsGpeKIpM0
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
source-wordcount: 430
ht-degree: 15%

---

# Administrar notificaciones en la aplicación de Planificación de Adobe Workfront

{{planning-important-intro}}

Puede recibir notificaciones en la aplicación desde Workfront Planning cuando existan los siguientes escenarios:

* Alguien le etiqueta a usted o a sus equipos en un comentario de registro

  Para obtener información sobre cómo etiquetar a otras personas en un comentario de registro, consulte [Administrar comentarios de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* Alguien le pide permiso para acceder a una vista, un espacio de trabajo o un registro
* Alguien confirma que se ha concedido su acceso a una vista, un espacio de trabajo o un registro

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

+++ Expand to view access requirements. 

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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> 

+++
-->

## Administrar notificaciones en la aplicación cuando alguien te etiqueta en un comentario

1. (Condicional) Después de que alguien lo etiquete a usted o a sus equipos en un comentario de un registro, vaya al icono de **Notificaciones** de la aplicación ![Icono de notificaciones de Experience Cloud](assets/experience-cloud-notifications-icon.png) en Adobe Experience Cloud.

   ![Ejemplo de notificación en la aplicación](assets/in-app-notification-example.png)

1. Haga clic en la notificación.

   Se abre la página de detalles de registro en Workfront Planning. Puede realizar actualizaciones en el registro o responder al comentario.

1. (Opcional) Haga clic en **Marcar todo como leído** para indicar que ha leído todas las notificaciones.
1. (Opcional) Haga clic en **Ver todo** para ir a la página **Notificaciones** en Adobe Experience Cloud.

## Administración de notificaciones en la aplicación al solicitar y conceder permisos

Recibirá notificaciones en la aplicación cuando alguien solicite o le conceda permisos para una vista, un espacio de trabajo o un tipo de registro. <!--<span class="preview">or record</span>-->

Para obtener información sobre cómo solicitar, conceder o denegar permisos, vea [Solicitar permisos a una vista o área de trabajo](/help/quicksilver/planning/access/request-permissions.md).

Para obtener información sobre cómo administrar las notificaciones de Workfront Planning, consulte [Administrar las preferencias de notificación de Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Administrar notificaciones en la aplicación al aprobar o rechazar solicitudes de Planning

Recibirá una notificación en la aplicación cuando alguien envíe una solicitud de aprobación o cuando alguien apruebe una solicitud que usted haya enviado.

Para obtener información sobre cómo enviar solicitudes, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

Para obtener información acerca de cómo aprobar solicitudes, vea [Aprobar una solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md).
