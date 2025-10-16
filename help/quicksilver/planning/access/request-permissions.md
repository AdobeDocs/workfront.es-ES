---
title: Solicitar permisos a una vista o a un Workspace
description: Cuando alguien comparte un vínculo a una vista o área de trabajo a la que no tiene acceso, puede solicitar permisos para abrirlo. En este artículo se explican los pasos para solicitar acceso a una vista o área de trabajo cuando se encuentra con un vínculo compartido que no se puede abrir.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 9%

---

# Solicitar permisos para una vista o un espacio de trabajo

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>La funcionalidad descrita en este artículo solo está disponible cuando su organización se ha incorporado a la experiencia unificada de Adobe.
>
>Para obtener más información, consulte [Adobe Unified Experience para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


Puede solicitar permisos para una vista o un espacio de trabajo cuando alguien comparta un vínculo con usted a la vista o al espacio de trabajo al que no tiene acceso.

Solicitar permisos a una vista es similar a solicitar permisos a un espacio de trabajo.

Este artículo describe cómo solicitar acceso a una vista o a un área de trabajo cuando alguien comparte un vínculo con usted y usted no puede tener acceso a la página compartida.

Para obtener información sobre la concesión de permisos a vistas y espacios de trabajo, consulte los siguientes artículos:

* [Compartir vistas](/help/quicksilver/planning/access/share-views.md)
* [Compartir espacios de trabajo](/help/quicksilver/planning/access/share-workspaces.md)


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
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete de Workfront y Planning</p> 
O
<p>Cualquier paquete de flujo de trabajo y planificación</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Cualquiera</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  <p>Una vez concedida la solicitud de permiso, puede obtener los siguientes permisos:</p>
   <ul><li><p>Ver o administrar para una vista</p></li>
   <li><p>Ver, contribuir o administrar para un espacio de trabajo</p></li></ul>  
   <p>Solo los usuarios con permisos de Administración de un espacio de trabajo y una vista pueden compartir una vista públicamente.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.
   <p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
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
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
 
</tbody> 
</table> -->


## Solicitar permisos para una vista o espacio de trabajo

Solicitar permisos a una vista es similar a solicitar permisos a un espacio de trabajo.

Cuando alguien comparte con usted un vínculo a un espacio de trabajo o una vista a los que no tiene acceso:

1. Haga clic en el vínculo compartido con usted para la vista o el espacio de trabajo.

   Se muestra una página **No tiene acceso** para informarle de que no tiene acceso a la vista ni al área de trabajo.

   ![Solicitar acceso a la vista](assets/request-access-to-view.png)

1. (Condicional) Si el vínculo compartido es para una vista de un área de trabajo a la que tiene acceso, haga clic en **Abrir con vista existente**. Si tiene permisos para acceder al espacio de trabajo, la página de tipo de registro se abrirá en la vista predeterminada.

1. (Opcional y condicional) Si no tiene permisos para ver el área de trabajo, agregue un mensaje personalizado en el cuadro disponible y, a continuación, haga clic en **Solicitar acceso**.

   Todos los usuarios con permisos de Administración de la vista o del espacio de trabajo reciben las siguientes notificaciones para la solicitud de acceso:
   * Una notificación en la aplicación
     ![Notificación en la aplicación para solicitud de acceso](assets/in-app-notification-for-access-request.png)
   * Una notificación por correo electrónico
     ![Notificación por correo electrónico de la solicitud de acceso](assets/email-notification-for-access-request.png)

1. (Condicional) Cuando el administrador de la vista o del espacio de trabajo le concede permisos para la vista o el espacio de trabajo, recibe una notificación por correo electrónico y una notificación en la aplicación con una confirmación de que el permiso se ha concedido. <!--check this - I was not able to test this, but Isk confirmed.-->
