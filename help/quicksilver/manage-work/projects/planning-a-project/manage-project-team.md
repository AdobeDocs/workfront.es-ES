---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Administrar el equipo del proyecto
description: El equipo del proyecto está formado por usuarios asociados al proyecto. Los miembros del equipo del proyecto se muestran en la sección Personas del proyecto o en la sección Personas de la plantilla que se puede utilizar para crear un proyecto.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 23%

---

# Administrar el equipo del proyecto

<!--take preview and production references out at production - August 7-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>

-->

El equipo del proyecto está formado por usuarios asociados al proyecto. Para más información, consulte [Información general del equipo del proyecto](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

Los miembros del equipo del proyecto se muestran en la sección Personas del proyecto.

Los usuarios que se muestran en la sección Personas de una plantilla de proyecto se convertirán en el equipo del proyecto una vez creado el proyecto a partir de la plantilla.

Los siguientes usuarios se agregan automáticamente al equipo del proyecto, tanto para proyectos como para plantillas:

* Propietario
* Patrocinador
* Usuarios asignados a tareas
* Usuarios asignados a problemas (solo para un proyecto)

Los usuarios del equipo del proyecto reciben notificaciones sobre el proyecto. Para obtener más información, consulte [Tipos de notificación de eventos](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Puede administrar los usuarios de los equipos del proyecto y de la plantilla agregándolos (solo para el proyecto), eliminándolos o enviándoles una actualización.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
    <p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos y plantillas</p> <p>Acceso de visualización o superior a los usuarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores a un proyecto o a una plantilla</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p>
    <p>Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and Templates</p> <p>View or higher access to Users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project or to a template</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Add users to a Project Team

When you add users to the project team, they gain View permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Users on the Project Team are not automatically added to the resource management tools for the project.

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following:

* Tasks
* Issues

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

If users that don't fulfill any role on the project want to be notified about certain updates or changes during the life of the project, you can manually add them to the project team. 

 For more information about what notifications can be enabled for users on the project team, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md). 

 <!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 



## Manage people on a project

1. Go to the project you want to manage the project team for.

   >[!TIP]
   >
   >You must have users assigned to tasks, issues or as stakeholders on the project to have them display in the People section.

1. Click **People** in the left panel. 

1. Click **Add users**. 

   The **Add users to Project Team** box displays.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In the **Add users** box, begin typing the name of an active Workfront user that you want to add to the project team, then click the name when it appears in the list.

   Repeat this step to add multiple users to the project team. The users must belong to the group associated with the project. 

   >[!TIP]
   >
   >* You cannot add users by adding their teams, groups, companies, or job roles.
   >* As you add the users, notice the avatar, the user's Primary Role, and their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them.
   >
   >  You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Click **Add**.

   The users gain View permissions to the project and receive notifications about the project as part of the project team.

1. (Optional) If you want a user to receive a  notification when their job role is added to a task, issue, or project approval, click inside the **Job Role** column for the user, and select a job role that will be associated with the approval. 

   The users will receive notifications related to the approvals assigned to the selected job role. 

   For more information see the "Role-based approvals" section in the article [Project Team overview](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Select one or several users in the list, then click the **Remove** icon ![Remove icon](assets/remove-icon.png) to remove them from the team. 
 
1. Click **Yes, Remove Selected Users** to confirm and remove the users.

   Users are removed and unassigned from incomplete work items.

   For more information, see the [Considerations for removing users from a project team](#considerations-for-removing-users-from-a-project-team) section in this article.
1. (Optional) To send an update for this project to users, click **Update All** to send the update to everyone on the team

   Or 

   Select one or multiple users in the list, then click **Send Update to User**.

   <!--update screen shot when they fix the bug - the text above the box needs to match the OLD box, below-->

![Enviar actualización al cuadro de usuario en el proyecto](assets/send-update-to-user-on-project-box-2025.png)

<!--Old UI for projects but the text above the comment box is right and matches the functionality):
   ![OLD Send update to user on a project](assets/send-update-to-user-on-project-box.png)-->

Se abre la casilla **Enviar actualización al usuario**.

1. Realice una de las siguientes acciones:

   * Añada una actualización para los usuarios seleccionados.
   * Haga clic en el icono de candado para que la actualización sea privada para los usuarios de su empresa.
   * Etiquete usuarios adicionales para recibir la misma actualización.
   * Haga clic en **Enviar**.

   La actualización se agrega a la sección **Actualizaciones** del proyecto y todos los usuarios seleccionados se muestran como usuarios etiquetados.

   Los usuarios pueden recibir una notificación por correo electrónico, si están habilitados para ellos, y una notificación dentro de la aplicación sobre la nueva actualización.

1. (Opcional) Haga clic en el icono **Exportar** ![Icono de exportar](assets/export-icon.png) para exportar la lista de usuarios a un archivo

   O

   Seleccione usuarios y luego haga clic en el icono **Exportar** para exportar solo usuarios específicos.

## Administrar personas en una plantilla

1. Vaya a la plantilla para la que desea administrar el equipo del proyecto.

   >[!TIP]
   >
   >Debe tener usuarios asignados a tareas o como partes interesadas en la plantilla para que se muestren en la sección Personas.

1. Haga clic en **Personas** en el panel izquierdo.

1. Seleccione uno o varios usuarios en la lista y luego haga clic en el icono **Quitar** para quitarlos del equipo.

1. Haga clic en **Sí, quitar usuarios seleccionados** para confirmar y quitar los usuarios.

   Los usuarios se eliminan y se anula su asignación de las tareas de plantilla.

   Para obtener más información, consulte la sección [Consideraciones para eliminar usuarios de un equipo de proyecto](#considerations-for-removing-users-from-a-project-team) en este artículo.

1. (Opcional) Para enviar una actualización a los usuarios, haga clic en **Actualizar todo** para enviar la actualización a todos los usuarios de la lista

   O

   Seleccione uno o varios usuarios en la lista y luego haga clic en **Enviar actualización al usuario**.

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![Enviar actualización al cuadro de usuario en la plantilla](assets/send-update-to-user-on-template-box.png)

   Se abre la casilla **Enviar actualización al usuario**.

1. Haga lo siguiente:

   * Añada una actualización para los usuarios seleccionados.
   * Haga clic en **Etiquetar personas** para etiquetar a usuarios adicionales y recibir la misma actualización.
   * Seleccione la opción **Privado para mi compañía** de para que la actualización sea privada para los usuarios de su compañía.
   * Haga clic en **Enviar**.

     >[!TIP]
     >
     >La configuración de **Privado para mi compañía** solo está disponible cuando su perfil de Workfront está asociado con una compañía.

   La actualización se agrega a la sección **Actualizaciones** del perfil de cada usuario etiquetado.

   Los usuarios pueden recibir una notificación por correo electrónico, si están habilitados para ellos, y una notificación dentro de la aplicación sobre la nueva actualización.

1. Haga clic en el icono **Exportar** ![icono Exportar](assets/export-icon.png) para exportar la lista de usuarios a un archivo

   O

   Seleccione usuarios y luego haga clic en el icono **Exportar** para exportar solo usuarios específicos.

## Consideraciones para quitar usuarios de un equipo del proyecto

Al quitar usuarios de sus funciones en el proyecto, siguen formando parte del equipo del proyecto.

Debe eliminarlos del equipo del proyecto, de la sección Personas del proyecto, para que dejen de recibir notificaciones enviadas al equipo del proyecto.

Si quita un usuario del equipo del proyecto y el usuario está asignado a tareas o problemas del proyecto, se le quita la asignación de las tareas y problemas que no se hayan completado. En este caso, las tareas y los problemas vuelven al área Trabajo no asignado del Distribuidor de cargas de trabajo.

Los usuarios asignados a tareas y problemas completados permanecen asignados a las tareas y problemas, incluso después de quitarlos del equipo del proyecto.

Los siguientes usuarios se eliminan de sus funciones en el proyecto cuando los elimina de la sección Personas de un proyecto o una plantilla:

* Usuarios asignados a tareas incompletas
* Usuarios asignados a problemas incompletos

Los siguientes usuarios no se eliminan de sus funciones en el proyecto cuando los elimina de la sección Personas de un proyecto o una plantilla:

* Propietario
* Patrocinador

Para obtener más información sobre cómo quitar usuarios del equipo del proyecto, consulte [Quitar usuarios de los proyectos](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).

