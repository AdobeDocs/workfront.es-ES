---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Administrar el equipo del proyecto
description: El equipo del proyecto está formado por usuarios asociados al proyecto. Los miembros del equipo del proyecto aparecen en la sección Personas del proyecto o en la sección Personas de la plantilla que podrían usarse para crear un proyecto.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: bb2479b936a9064a4df34ac3e840dd78cae297b6
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 26%

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

Los usuarios que se muestran en la sección Personas de un proyecto plantilla se convertirán en el equipo del proyecto después de que el proyecto se cree desde el plantilla.

Los siguientes usuarios se añaden automáticamente al equipo del proyecto, tanto para proyectos como para plantillas:

* Propietario
* Patrocinador
* Usuarios asignados a tareas
* Usuarios asignados a problemas (solo para un proyecto)

Los usuarios del equipo del proyecto reciben notificaciones sobre el proyecto. Para obtener más información, consulte [Tipos de notificación de eventos](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Puede administrar los usuarios de los equipos del proyecto y de la plantilla agregándolos (solo para el proyecto), eliminándolos o enviándoles una actualización.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Estándar </p>
    <p>Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos y plantillas</p> <p>Acceso de visualización o superior a los usuarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores a un proyecto o a una plantilla</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

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

-->

## Gestionar personas en un proyecto

1. Vaya al proyecto para el que desea administrar el proyecto equipo.

   >[!TIP]
   >
   >Debe tener usuarios asignados a tareas, problemas o como partes interesadas en el proyecto para que se muestren en la sección Personas.

1. Haga clic **en Personas** en el panel izquierdo.

1. Haga clic en **Agregar usuarios**.

   Se muestra el cuadro **Agregar usuarios al equipo del proyecto**.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. En el cuadro **Agregar usuarios**, empiece a escribir el nombre de un usuario activo de Workfront que desee agregar al equipo del proyecto y, a continuación, haga clic en el nombre cuando aparezca en la lista.

   Repita este paso para agregar varios usuarios al equipo del proyecto. Los usuarios deben pertenecer al grupo asociado al proyecto.

   >[!TIP]
   >
   >* No puede agregar usuarios agregando sus equipos, grupos, compañías o funciones.
   >* A medida que añada usuarios, fíjese en su avatar, su función principal y su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.
   >
   >  Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Haga clic en **Añadir**.

   Los usuarios obtienen permisos de visualización del proyecto y reciben notificaciones sobre el proyecto como parte del equipo del proyecto.

1. (Opcional) Si desea que un usuario reciba un notificación cuando su función de trabajo se agrega a una aprobación de tarea, problema o proyecto, haga clic dentro de la columna Rol **de** trabajo para el usuario y seleccione un función de trabajo que se asociará con la aprobación.

   Los usuarios recibirán notificaciones relacionadas con las aprobaciones asignadas al función de trabajo seleccionado.

   Para obtener más información, consulte la sección &quot;Aprobaciones basadas en funciones&quot; en el artículo Información general[ del equipo del proyecto](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Seleccione uno o varios usuarios en la lista y, a continuación, haga clic en el icono **de** Quitar![ Quitar](assets/remove-icon.png) icono para eliminarlos del equipo.

1. Haga clic en **Sí, quitar usuarios seleccionados** para confirmar y quitar los usuarios.

   Los usuarios se quitan y se quitan las asignaciones de los elementos de trabajo incompletos.

   Para obtener más información, consulte la sección [Consideraciones para eliminar usuarios de un equipo de proyecto](#considerations-for-removing-users-from-a-project-team) en este artículo.
1. (Opcional) Para enviar una actualización para este proyecto a los usuarios, haga clic en **Actualizar todo** para enviar la actualización a todos los miembros del equipo

   O

   Seleccione uno o varios usuarios en la lista y luego haga clic en **Enviar actualización al usuario**.

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

   La actualización se agrega a la **sección Actualizaciones** del proyecto y todos los usuarios seleccionados se muestran como usuarios etiquetado.

   Los usuarios pueden recibir un notificación correo electrónico, si están habilitados para ellos, y recibir un notificación en la aplicación sobre la nueva actualización.

1. (Opcional) Haga clic en el **icono** Exportar![ icono Exportar](assets/export-icon.png) para exportar el lista de usuarios a un archivo

   O

   Seleccione usuarios y luego haga clic en el icono **Exportar** para exportar solo usuarios específicos.

## Administrar personas en una plantilla

1. Vaya a la plantilla desea administrar el proyecto equipo.

   >[!TIP]
   >
   >Debe tener usuarios asignados a tareas o como partes interesadas en la plantilla para que se muestren en la sección Personas.

1. Haga clic **en Personas** en el panel izquierdo.

1. Seleccione uno o varios usuarios en la lista y, a continuación, haga clic en el icono Quitar **** para eliminarlos del equipo.

1. Haga clic en **Sí, Quitar usuarios** seleccionados para confirmar y eliminar los usuarios.

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

   La actualización se agrega a la **sección Actualizaciones** de cada etiquetado perfil del usuario.

   Los usuarios pueden recibir un notificación correo electrónico, si están habilitados para ellos, y recibir un notificación en la aplicación sobre la nueva actualización.

1. Haga clic en el icono **Exportar** ![icono Exportar](assets/export-icon.png) para exportar la lista de usuarios a un archivo

   O

   Seleccione usuarios y, a continuación, haga clic en el **icono Exportar** para exportar solo usuarios específicos.

## Consideraciones para eliminar usuarios de un equipo de proyecto

Al quitar usuarios de sus funciones en el proyecto, siguen formando parte del equipo del proyecto.

Debe eliminarlos de la equipo del proyecto, de la sección Personas del proyecto, para que dejen de recibir notificaciones enviadas al equipo del proyecto.

Si quita un usuario del equipo del proyecto y el usuario está asignado a tareas o problemas del proyecto, se le quita la asignación de las tareas y problemas que no se hayan completado. En este caso, las tareas y los problemas vuelven al área Trabajo no asignado del Distribuidor de cargas de trabajo.

Los usuarios asignados a tareas y problemas completados permanecen asignados a las tareas y problemas, incluso después de quitarlos del equipo del proyecto.

Los siguientes usuarios se eliminan de sus funciones en el proyecto cuando los elimina de la sección Personas de un proyecto o una plantilla:

* Usuarios asignados a tareas incompletas
* Usuarios asignados a problemas incompletos

Los siguientes usuarios no se eliminan de sus funciones en el proyecto cuando los elimina de la sección Personas de un proyecto o una plantilla:

* Propietario
* Patrocinador

Para obtener más información sobre cómo quitar usuarios del equipo del proyecto, consulte [Quitar usuarios de los proyectos](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).

