---
title: Administrar notificaciones de correo electrónico de Adobe Workfront Planning
description: Cuando alguien le etiqueta a usted o a sus equipos en un comentario de registro en Adobe Workfront Planning, recibe una notificación por correo electrónico de esa etiqueta.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 26%

---


# Administrar notificaciones por correo electrónico de Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede recibir notificaciones por correo electrónico de Workfront Planning cuando existan los siguientes escenarios:

* Alguien le etiqueta a usted o a sus equipos en un comentario de registro

  Para obtener información sobre cómo etiquetar a otras personas en un comentario de registro, consulte [Administrar comentarios de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* Alguien le pide permiso para acceder a una vista o a un espacio de trabajo
* Alguien confirma que se ha concedido su acceso a una vista o a un área de trabajo <!--Isk confirmed that there is nno email for denying access but did not test-->
* Envía una solicitud de Workfront Planning. Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Alguien aprueba o rechaza una solicitud de Workfront Planning que usted haya enviado. Para obtener más información, consulte [Aprobar una solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* El estado cambia a una solicitud de Workfront Planning que ha enviado.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia unificada de Adobe.</p> 
<p>Los usuarios de su organización solo reciben notificaciones de Workfront Planning cuando su organización está integrada en la experiencia unificada de Adobe. </p>
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar, Ligero o Colaborador</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de vista o superiores a un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.
   <p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
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

1. (Condicional y opcional) Después de que alguien solicite o le conceda permisos para acceder a una vista o a un espacio de trabajo, vaya al mensaje de correo electrónico que le informa de la solicitud de permiso. El remitente del correo electrónico es Adobe Experience Cloud.

1. (Opcional) Haga clic en el mensaje en el cuadro **Workfront** dentro del correo electrónico.

   Se abre la página de detalles de registro en Workfront. Puede realizar actualizaciones en el registro o responder al comentario.

1. (Condicional) Si está disponible, haga clic en **Ver todas las notificaciones**.
La página **Notificaciones** se abre en Adobe Experience Cloud. Se muestran todas las notificaciones de todas las aplicaciones de Adobe Experience Cloud.


Para obtener información sobre cómo solicitar, conceder o denegar permisos a una vista o área de trabajo, vea [Solicitar permisos a una vista o área de trabajo](/help/quicksilver/planning/access/request-permissions.md).

Para obtener información sobre cómo administrar las notificaciones de Workfront Planning, consulte [Administrar las preferencias de notificación de Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Administrar notificaciones por correo electrónico sobre el envío, la aprobación o el rechazo de solicitudes de Workfront Planning

1. (Opcional) Vaya al correo electrónico que le envía Workfront
después de enviar una solicitud, o después de que una solicitud enviada se haya aprobado o rechazado. El remitente del correo electrónico es Adobe Workfront.

1. (Opcional) Haga clic en **Abrir solicitud**. Esto abre la solicitud en Workfront Planning.

1. Haga clic en el icono **Notificaciones** ![Icono del área de notificaciones Unified Shell](assets/notifications-area-icon-unified-shell.png) en la esquina superior derecha de la pantalla para acceder a la página **Notificaciones**.

   Para obtener información sobre cómo administrar las notificaciones de Workfront Planning, consulte [Administrar las preferencias de notificación de Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
