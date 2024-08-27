---
title: Compartir espacios de trabajo
description: Puede compartir un espacio de trabajo con otros usuarios para garantizar la colaboración al trabajar en Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 83c716dea3815ed9a2ce4c3d0598ef42b128de87
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 2%

---


# Compartir espacios de trabajo

{{planning-important-intro}}

Puede compartir un espacio de trabajo con otros usuarios para garantizar la colaboración al trabajar en Adobe Workfront Planning.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>Al conceder permisos a un espacio de trabajo, no se conceden permisos a otros usuarios para las vistas de las páginas de tipo de registro. Debe conceder permisos a vistas individuales de una página de tipo de registro para compartirlas con otros usuarios. Para obtener más información, vea [Compartir una vista](/help/quicksilver/planning/access/share-views.md).


## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

Debe tener lo siguiente para poder acceder a Workfront Planning:

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
   <td role="rowheader"><p>plan Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Plan de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre lo que se incluye en cada plan de Workfront Planning, consulte <a href="https://business.adobe.com/products/workfront/pricing.html">Precios y empaquetado de Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar </p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  <p>Administración de permisos en un espacio de trabajo</p>  </td> 
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
   <p> Adobe Workfront</p> </td>
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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->



## Compartir permisos en un espacio de trabajo

Los siguientes usuarios pueden compartir un espacio de trabajo con otros usuarios:

* Los administradores del sistema pueden compartir todos los espacios de trabajo, incluidos los que no hayan creado.
* Todos los demás usuarios solo pueden compartir espacios de trabajo para los que tengan permisos de administración.

Para compartir un espacio de trabajo con otros usuarios:

{{step1-to-planning}}

1. Abra el área de trabajo que desea compartir y haga clic en **Compartir** en la esquina superior derecha de la pantalla.

   ![](assets/share-button-on-workspace-top-right.png)

1. En el campo **Conceder acceso al área de trabajo a**, empiece a escribir el nombre de un usuario o grupo y, a continuación, haga clic en él cuando se muestre en la lista.

   ![](assets/sharing-ui-with-groups.png)

1. Seleccione uno de los siguientes niveles de permisos en el menú desplegable:
   * Ver
   * Aportar
   * Administrar

     Para obtener información acerca de los niveles de permisos y las acciones que los usuarios pueden realizar en cada nivel, vea [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Haga clic en **Copiar vínculo** para copiar un vínculo al área de trabajo en el portapapeles.
1. Compartir el vínculo copiado con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder al espacio de trabajo.
1. Haga clic en **Guardar**.

<!--
## Grant permissions to a workspace from a permission request

Users who access a link to a workspace to which they do not have permissions can request permissions to the workspace. All users with Manage permissions to the workspace receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a workspace, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![](assets/in-app-notification-for-access-request.png)
   * An email notification
      ![](assets/email-notification-for-access-request.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![](assets/notifications-list-approval-box.png)
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the workspace. 
-->


## Eliminación de permisos de un espacio de trabajo


{{step1-to-planning}}

1. Abra el área de trabajo en la que desea quitar permisos y, a continuación, haga clic en **Compartir** en la esquina superior derecha de la pantalla.
1. Haga clic en el menú desplegable situado a la derecha del nombre de un usuario o grupo y, a continuación, haga clic en **Quitar**.
1. Haga clic en **Guardar**.

   El usuario o los usuarios que pertenecen al grupo eliminado ya no tienen acceso al espacio de trabajo o a sus objetos.