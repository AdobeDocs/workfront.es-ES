---
title: Administrar las preferencias de las notificaciones para Adobe Workfront Planning
description: Es posible que pueda administrar las preferencias de las notificaciones para Adobe Workfront Planning. En este artículo se describe cómo configurar las preferencias de las notificaciones.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 34%

---


# Administrar las preferencias de las notificaciones para Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede recibir notificaciones en la aplicación o por correo electrónico cuando se produzcan las siguientes acciones en Workfront Planning:

* Alguien agrega usted o sus equipos a un comentario en la página de registro
* Alguien solicita permiso para acceder a una vista o a un espacio de trabajo
* Alguien le concede permiso para obtener acceso a una vista o a un área de trabajo <!--I could not test this but Isk confirmed-->
* Envía una solicitud de Workfront Planning.
* Alguien aprueba o rechaza una solicitud de Workfront Planning que usted haya enviado.
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
   <td><p><p>Estándar, Ligero o Colaborador
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

Para obtener más información sobre las notificaciones de Workfront Planning, consulte también los siguientes artículos:

* Para obtener información acerca de los comentarios en los registros, consulte [Administrar comentarios de registro](/help/quicksilver/planning/records/manage-record-comments.md).
* Para obtener información sobre las notificaciones en la aplicación de Workfront Planning, consulte [Administrar notificaciones en la aplicación para Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Para obtener información sobre las notificaciones por correo electrónico de Workfront Planning, consulte [Administrar notificaciones por correo electrónico para Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).


## Administrar preferencias de las notificaciones

1. Inicie sesión en Workfront con sus credenciales de Adobe Experience Cloud.
1. Haga clic en el icono **menú de cuenta** ![icono de menú de cuenta en Experience Cloud](assets/account-menu-icon-on-experience-cloud.png) en la parte superior derecha de la pantalla y, a continuación, haga clic en **Preferencias**.
1. En la sección **Notificaciones**, haga clic en **Workfront**.
1. Seleccione las notificaciones que desee recibir.
O
Anule la selección de las notificaciones que quiera dejar de recibir.

   ![Panel de notificaciones de Adobe Experience Cloud para Workfront Planning](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Las siguientes notificaciones están disponibles para Workfront:

   * **Menciones**: Recibes una notificación cuando alguien te etiqueta a ti o a tu equipo en un comentario en Workfront Planning
   * **Solicitudes**: recibe una notificación cuando alguien realiza una de las siguientes acciones:

      * Solicita o concede permiso para un objeto de Workfront Planning
      * Ha enviado una solicitud de Workfront Planning
      * El estado de una solicitud de Workfront Planning que ha enviado cambios
      * Solicita, concede o rechaza una aprobación para una solicitud de Workfront Planning

   Para obtener más información sobre cómo administrar las notificaciones, consulte [Preferencias y notificaciones de la cuenta](https://experienceleague.adobe.com/es/docs/core-services/interface/features/account-preferences).

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/es/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
