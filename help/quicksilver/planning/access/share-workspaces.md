---
title: Compartir espacios de trabajo
description: Puede compartir un espacio de trabajo con otros usuarios para garantizar la colaboración al trabajar en Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 54a6e633e903c73a78b36e90fb27edb445dc8d47
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 12%

---

# Compartir espacios de trabajo

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede compartir un espacio de trabajo con otros usuarios para garantizar la colaboración al trabajar en Adobe Workfront Planning.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>La concesión de permisos a un espacio de trabajo no significa que se conceden permisos a otros usuarios para ver las páginas de tipo de registro. Debe conceder permisos a vistas individuales de una página de tipo de registro para compartirlas con otros usuarios. Para obtener más información, vea [Compartir una vista](/help/quicksilver/planning/access/share-views.md).


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete de Workfront y Planning</p> 
O
<p>Cualquier paquete de flujo de trabajo y planificación</p> 
 </tr>
<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p> 
  </td> 
  </tr>

<td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  <p>Administración de permisos en un espacio de trabajo</p>  </td> 
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
<p>Your organization must be onboarded to the Adobe Unified Experience for users to be able to request and grant permissions to a workspace from a permission request. </p> 
<p>Users must be added to the Adobe Admin Console in order to gain permissions to Workfront Planning workspaces.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Manage permissions to a workspace</p>  </td> 
  </tr> 

</tbody> 
</table> -->

## Consideraciones sobre compartir espacios de trabajo

* Para obtener información general sobre cómo compartir objetos en Workfront Planning, consulte también [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Puede compartir espacios de trabajo con usuarios, equipos, funciones, grupos o empresas de su organización.
* Además de los equipos, grupos, empresas y funciones del puesto, solo puede compartir con los usuarios que se han añadido a Adobe Admin Console.
* No puede compartir espacios de trabajo con usuarios que no pertenezcan a su organización.
* Al compartir un espacio de trabajo, también se comparten todos los tipos de registros, registros y campos asociados a los espacios de trabajo.
* Al compartir un espacio de trabajo, las vistas no se comparten. Debe compartir vistas por separado.
* Los permisos de Workspace se muestran como Permisos heredados en los tipos de registro.

## Compartir permisos en un espacio de trabajo

Los siguientes usuarios pueden compartir un espacio de trabajo con otros usuarios:

* Los administradores del sistema pueden compartir todos los espacios de trabajo, incluidos los que no hayan creado.
* Todos los demás usuarios solo pueden compartir espacios de trabajo para los que tengan permisos de administración.

Para compartir un espacio de trabajo con otros usuarios:

{{step1-to-planning}}

1. Abra el área de trabajo que desea compartir y haga clic en **Compartir** en la esquina superior derecha de la pantalla.

   ![Botón Compartir en la parte superior derecha del espacio de trabajo](assets/share-button-on-workspace-top-right.png)

1. En el campo **Conceder acceso a este área de trabajo**, empiece a escribir el nombre de un usuario, grupo, equipo, empresa o rol y, a continuación, haga clic en él cuando se muestre en la lista.

   ![IU para compartir con grupos](assets/sharing-ui-with-groups.png)

   >[!NOTE]
   >
   >* Además de los equipos, grupos, empresas y funciones del puesto, solo puede compartir con los usuarios que se han añadido a Adobe Admin Console. No puede agregar usuarios solo de Workfront. Para obtener más información, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
   >
   >* Cuando comparte un área de trabajo con un usuario, su rol de trabajo principal <span class="preview">y su correo electrónico</span> también se muestran en el campo. Debe tener activada la configuración Ver información de contacto para el objeto Usuarios en su nivel de acceso para poder ver el correo electrónico del usuario.


1. Seleccione uno de los siguientes niveles de permisos en el menú desplegable:
   * Ver
   * Aportar
   * Administrar

     Para obtener información acerca de los niveles de permisos y las acciones que los usuarios pueden realizar en cada nivel, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Haga clic en **Copiar vínculo** para copiar un vínculo al área de trabajo en el portapapeles.
1. Comparta el vínculo copiado con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder al espacio de trabajo.
1. Haga clic en **Guardar**.

   Los usuarios con los que ha compartido el espacio de trabajo reciben una notificación en la aplicación y por correo electrónico sobre si tienen permisos para él.

## Conceder permisos a un espacio de trabajo desde una solicitud de permiso

Los usuarios que accedan a un vínculo a un espacio de trabajo para el que no tengan permisos pueden solicitar permisos. Todos los usuarios con permisos de Administrar en el espacio de trabajo reciben la solicitud de permiso y pueden concederlos o denegarlos.

1. (Condicional) Si usted es el administrador de un espacio de trabajo, es posible que otro usuario le solicite el acceso a la vista en las áreas siguientes:

   * Una notificación en la aplicación
     ![Notificación en la aplicación para solicitud de acceso](assets/in-app-notification-for-access-request.png)
   * Una notificación por correo electrónico
     ![Notificación por correo electrónico de la solicitud de acceso](assets/email-notification-for-access-request.png)
1. (Condicional) En el área de notificación de Workfront, haga clic en la notificación dentro de la aplicación
O
En la notificación por correo electrónico, haga clic en **Ver todas las notificaciones** y, a continuación, haga clic en la notificación en la lista.

   Se muestra el cuadro **Solicitudes de acceso pendientes**.

   ![Cuadro de aprobación de lista de notificaciones](assets/notifications-list-approval-box.png)

1. (Opcional) Para el usuario cuyos permisos desea aprobar, seleccione una de las siguientes opciones en el menú desplegable situado a la derecha del nombre del usuario:
   * **Vista**
   * **Aportar**
   * **Administrar**
1. Seleccione el usuario para el que desea aprobar o denegar el permiso y, a continuación, haga clic en **Aprobar todo** o **Denegar todo**.
1. Haga clic en la flecha que señala a la izquierda de **Solicitudes de acceso pendientes** y, a continuación, haga clic en **Guardar**.

   Si ha aprobado la solicitud, los usuarios se agregan al cuadro para compartir del área de trabajo. El usuario que solicita el permiso recibe un correo electrónico de confirmación de que su solicitud se ha aprobado. <!--will they also get an in-app notification??-->


## Eliminación de permisos de un espacio de trabajo


{{step1-to-planning}}

1. Abra el área de trabajo en la que desea quitar permisos y, a continuación, haga clic en **Compartir** en la esquina superior derecha de la pantalla.
1. Haga clic en el menú desplegable situado a la derecha del nombre de la entidad con la que comparte el área de trabajo y, a continuación, haga clic en **Quitar**.
1. Haga clic en **Guardar**.

   Los usuarios eliminados ya no tendrán acceso al espacio de trabajo ni a sus objetos.

   No hay ninguna notificación para los usuarios que se han eliminado del espacio de trabajo de que ya no tienen estos permisos.