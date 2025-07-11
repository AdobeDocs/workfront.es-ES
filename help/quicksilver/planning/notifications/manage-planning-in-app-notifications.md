---
title: Administrar notificaciones en la aplicación de Adobe Workfront Planning
description: Cuando alguien le etiqueta a usted o a sus equipos en un comentario de registro, recibe una notificación por correo electrónico para esa etiqueta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: d3d4a923dddb8685a981162918f34447300136cf
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 30%

---


# Administrar notificaciones en la aplicación de Planificación de Adobe Workfront

{{planning-important-intro}}

Puede recibir notificaciones en la aplicación desde Workfront Planning cuando existan los siguientes escenarios:

* Alguien le etiqueta a usted o a sus equipos en un comentario de registro

  Para obtener información sobre cómo etiquetar a otras personas en un comentario de registro, consulte [Administrar comentarios de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* Alguien le pide permiso para acceder a una vista o a un espacio de trabajo
* Alguien confirma que se ha concedido su acceso a una vista o a un área de trabajo <!--Isk confirmed there is no notification for denying permissions - did not test-->

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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

Recibirá notificaciones en la aplicación cuando alguien solicite o le conceda permisos para una vista o un espacio de trabajo.

Para obtener información sobre cómo solicitar, conceder o denegar permisos a una vista o área de trabajo, vea [Solicitar permisos a una vista o área de trabajo](/help/quicksilver/planning/access/request-permissions.md).

Para obtener información sobre cómo administrar las notificaciones de Workfront Planning, consulte [Administrar las preferencias de notificación de Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
