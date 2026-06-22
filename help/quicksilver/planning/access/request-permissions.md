---
title: Solicitar permisos a una vista o a un Workspace
description: Cuando alguien comparte un vínculo a una vista o área de trabajo a la que no tiene acceso, puede solicitar permisos para abrirlo. En este artículo se explican los pasos para solicitar acceso a una vista o área de trabajo cuando se encuentra con un vínculo compartido que no se puede abrir.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/FvXVCMMz-PfaT-QAaMq0c5qUruR1MJoMv6etcrAstXA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 567
ht-degree: 11%

---

# Solicitar permisos para una vista o un espacio de trabajo


<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después del lanzamiento en Vista previa, las mismas funciones también están disponibles mensualmente en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


<!-- 
no longer needed: 
>[!IMPORTANT]
>
>The functionality described in this article is available only when your organization has been onboarded to the Adobe Unified Experience. 
>
>For more information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md). 
-->

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
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
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
   <li><p>Ver, contribuir o administrar para un espacio de trabajo</p></li>
   <li><p>Ver, contribuir o administrar para un tipo de registro</p></li>
   <li><p><span class="preview">Ver o administrar un registro</span></p></li>
   </ul>  
   <p>Solo los usuarios con permisos de Administración de un espacio de trabajo y una vista pueden compartir una vista públicamente.</p></td> 
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
 Old:
 
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
</table>
-->


## Solicitar permisos

Solicitar permisos para una vista es similar a solicitar permisos para un área de trabajo, un tipo de registro o <span class="preview">un registro</span>.

Cuando alguien comparte con usted un vínculo a un área de trabajo, tipo de registro, <span class="preview">registro</span> o una vista a la que no tiene acceso:

1. Haga clic en el vínculo compartido con usted para la vista o el espacio de trabajo.

   Se muestra una página **No tiene acceso** para informarle de que no tiene acceso a la vista ni al área de trabajo.

   ![Solicitar acceso a la vista](assets/request-access-to-view.png)

   >[!NOTE]
   >
   >Si no tiene acceso a un tipo de registro o a <span class="preview">registro</span>, la página No tiene acceso a muestra que debe tener acceso al área de trabajo.


1. (Condicional) Si el vínculo compartido es para una vista de un área de trabajo a la que tiene acceso, haga clic en **Abrir con vista existente**. Si tiene permisos para acceder al espacio de trabajo, la página de tipo de registro se abrirá en la vista predeterminada.

1. (Opcional y condicional) Si no tiene permisos para ver el área de trabajo, agregue un mensaje personalizado en el cuadro disponible y, a continuación, haga clic en **Solicitar acceso**.

   Todos los usuarios con permisos de Administración de la vista o del espacio de trabajo reciben las siguientes notificaciones para la solicitud de acceso:
   * Una notificación en la aplicación
     ![Notificación en la aplicación para solicitud de acceso](assets/in-app-notification-for-access-request.png)
   * Una notificación por correo electrónico
     ![Notificación por correo electrónico de la solicitud de acceso](assets/email-notification-for-access-request.png)

1. (Condicional) Cuando el administrador de la vista o del espacio de trabajo le concede permisos para la vista o el espacio de trabajo, recibe una notificación por correo electrónico y una notificación en la aplicación con una confirmación de que el permiso se ha concedido. <!--check this - I was not able to test this, but Isk confirmed.-->
