---
title: Conceder a los usuarios acceso administrativo a determinadas áreas
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para otorgar a los usuarios con una licencia de planificación acceso administrativo a determinadas áreas del sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
TQID: https://experienceleague.adobe.com/1nXA0NxLQW3tiIrhCKAd5EMfqBjQW68GHNN42dQmptQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9041e7a1c1bf6f7909039fe238b4564ab204752c
workflow-type: tm+mt
source-wordcount: 714
ht-degree: 88%

---

# Conceder a los usuarios acceso administrativo a determinadas áreas

{{preview-fast-release-general}}

<!--Linked in several places, do not rename or change URL.-->

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para otorgar a los usuarios con una licencia estándar o de planificación acceso administrativo a determinadas áreas del sistema.

>[!NOTE]
>
>Esto es diferente a otorgar a un usuario acceso administrativo completo a Workfront, como se explica en [Conceder a un usuario acceso administrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).&#x200B;

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conceder a los usuarios de Standard o Plan acceso administrativo a ciertas áreas de Workfront

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que no modifique los niveles de acceso integrado para poder consultarlos después de configurar los usuarios. Para personalizar un nivel de acceso, copie el nivel de acceso predeterminado y modifique la copia. (Puede hacerlo para todos los niveles de acceso, excepto para el Administrador del sistema y el Usuario externo).

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Niveles de acceso**.
1. Haga clic en el nombre del nivel de acceso que desee utilizar para otorgar a los usuarios acceso administrativo a determinadas áreas de Workfront.
1. En la sección **Permitir acceso administrativo para**, active las casillas para conceder el acceso administrativo necesario.

   Estas opciones le permiten conceder las siguientes capacidades:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Procesos de aprobación</td> 
      <td><p>Cree y administre procesos de aprobación para su uso en todo el sistema y para grupos específicos.</p><p>Sin este acceso, los usuarios solo pueden crear procesos de aprobación ad-hoc en los elementos a los que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="preview">Historial de cambios</span></td> 
      <td><p><span class="preview">Vea los registros de historial de cambios de Workfront en Configuración &gt; Seguimiento de cambios &gt; Lista de historial de cambios.</span></p>
      <p><span class="preview">Sin este acceso, los usuarios no tienen esta opción en el área de Configuración.</span></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compañías</td> 
      <td><p>Añadir compañías nuevas y editar las existentes en Workfront</p>
      <p>Sin este acceso, los usuarios solo pueden ver las empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td><p>Cree y edite (añada, edite y elimine los campos) formularios personalizados dentro de su grupo.</p><p>Sin este acceso, los usuarios solo pueden adjuntar formularios existentes a objetos a los que tengan acceso para contribuir o administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipos de cambio</td> 
      <td> <p>Añada una nueva moneda en Workfront.</p> <p>Sin este acceso, el usuario solo puede añadir una moneda existente a un proyecto que cree.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td><p>Vea todos los gastos en objetos en Workfront.</p><p>Esto no permite al usuario crear nuevos tipos de gastos.</p><p>Sin este acceso, el usuario solo puede ver lo siguiente:</p>
       <ul>
        <li>Gastos en proyectos, tareas o problemas que administran</li>
        <li>Sus propios gastos</li>
        <li>Los gastos de sus subordinados</li>
       </ul></td> 
     </tr>
     <tr> 
      <td role="rowheader">Hitos de mi grupo</td> 
      <td>Vea todas las rutas de hitos del sistema en el menú Rutas de hitos en Configuración. Los usuarios también pueden editar o eliminar cualquier ruta de hitos que pertenezca a cualquiera de sus grupos. Los usuarios no pueden administrar (editar o eliminar) las rutas de hitos que no están asignadas a ninguno de sus grupos.<br><p>Sin este acceso, los usuarios solo pueden ver las rutas de hitos existentes y aplicarlas a los proyectos a los que tienen acceso para administrar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Crear y administrar notificaciones de recordatorio en Workfront.<br>Sin este acceso, los usuarios se limitan a recibir y ver notificaciones.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hojas de horas y horas</td> 
      <td> <p>Permite a los usuarios ver todas las horas y plantillas de horas en Workfront.</p> <p>Cuando esta opción está deshabilitada, los usuarios solo pueden ver las horas en:</p> 
       <ul> 
        <li>Proyectos, tareas o problemas que administran</li> 
        <li>Su propia plantilla de horas</li> 
        <li>Una plantilla de horas de un subordinado</li> 
        <li>Una plantilla de horas que aprueban</li> 
       </ul> <p><b>NOTA</b>:  <p>Independientemente de si esta opción está habilitada o deshabilitada, los administradores de grupos pueden crear perfiles de plantillas de horas para los grupos y subgrupos que administran y asignarlas a miembros del grupo cuyos perfiles de usuario tengan acceso para editar.</p> <p>Si se habilita esta opción, es posible que algunos administradores de grupos tengan demasiado acceso, ya que pueden ver las plantillas de horas generadas por los perfiles de la plantilla de horas (y las horas) para todos los usuarios del sistema y no solo las de los grupos que administran. Puede desactivar esta opción para los administradores de grupos que no necesiten tanto acceso.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cuando termine, haga clic en **Guardar**.
1. Asigne el nuevo nivel de acceso a un usuario, tal como se describe en [Añadir usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Puede permitir que los usuarios tengan acceso administrativo a los usuarios. Para obtener más información sobre cómo otorgar a los usuarios acceso administrativo a usuarios para poder administrar cuentas de usuario, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


<!--     
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> <p><b>NOTE</b>: In the Preview environment, access to job roles is controlled as an object type in the access level. See <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-job-roles.md">Grant access to job roles</a>.</p>
      <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Standard or Plan user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Standard or Plan user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
     </tr>
-->

<!--
## Access of a Workfront administrator vs. access of a Standard or Plan user with administrative rights  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

The two tables below show the difference between the access rights of a user with a Workfront System Administrator access level versus those of a user with a Standard or Plan license with some administrative rights.

Workfront administrators can view all the objects in the system (regardless of who created them), create new ones, and modify or delete existing ones. They have full access to all objects in the system.

Users with a Standard or Plan license who can edit functionality in one area have full access to the functionality in that area.

>[!NOTE]
>
>Users with a Standard or Plan license who are designated as group administrators can perform some of the actions allowed for Workfront administrators. They are allowed to perform these actions only for the groups they administer, their subgroups, and the users in these groups and subgroups. For more information, see [Group administrators](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Access to the Setup area](#access-to-the-setup-area)
* [Access to objects](#access-to-objects)

### Access to the Setup area {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Standard or Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project Preferences: Projects</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Tasks &amp; Issues</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Statuses</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Priorities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Severities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Exchange Rates</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Approvals</td> 
   <td> <p>Full access</p> </td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Milestone Paths</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Custom Forms</td> 
   <td>Full access</td> 
   <td> <p>Manage custom forms they created or custom forms shared with them.</p> <p>Attach custom forms they created or custom forms shared with them to objects they have manage or contribute permissions to.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Deleted</td> 
   <td>Full access</td> 
   <td> <p>Users who are group administrators can restore projects assigned to Groups they manage, and tasks, issues, or documents associated with those projects.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Restored</td> 
   <td>Full access</td> 
   <td>Users who are group administrators can see the items they have recently restored.</td> 
  </tr> 
  <tr> 
   <td>Job Roles</td> 
   <td>Full access</td> 
   <td> <p>Modify but not delete existing job roles.</p> <p>Add new job roles.</p> </td> 
  </tr> 
  <tr> 
   <td>Teams</td> 
   <td>Full access</td> 
   <td> <p>No access to create Teams.</p> <p>Add existing teams to users when creating or editing users.</p> </td> 
  </tr> 
  <tr> 
   <td>Groups</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groups.</p> <p>Only group administrators can manage group membership, subgroups, and group-level statuses for the groups they manage. </p> </td> 
  </tr> 
  <tr> 
   <td>Companies</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Log in As</td> 
   <td>Full access </td> 
   <td> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator, they can log in as the users in the group they administer and their subgroups. They cannot log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Schedules</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Schedules.</p> <p>Access to add existing schedules to other users, at the user level. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Timesheet Profiles</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Timesheet Profiles to users, at the user level.</p> <p>Users who are group administrators can create Timesheet Profiles for the groups they administer and their subgroups. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Hour Types</td> 
   <td>Full access</td> 
   <td> <p>Access to assign Hour Types to users, at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Event Notifications</td> 
   <td>Activate/ Deactivate all</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Reminder Notifications</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Email Templates</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Templates.</p> <p>Access to add existing Email Templates to Reminder Notifications.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Automatic Reminders</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Invitations</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Invitations.</p> <p>Access to resend email invitations to unregistered users only from the People tab.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Setup</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecards</td> 
   <td>Full access</td> 
   <td> <p>Full access</p> </td> 
  </tr> 
  <tr> 
   <td>Expense Types</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Risk Types</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Access Levels</td> 
   <td> <p>Full access to modify all access levels.</p> <p>The System Administrator and External User access levels cannot be modified, by default.</p> </td> 
   <td> <p>No access to edit Access Levels.</p> <p>Assign an access level to other users which is lower or equal to theirs at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Layout Templates</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Layout Templates to other users, at the user level. </p> <p>Users designated as group administrators can create Layout Templates for groups and subgroups they manage.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Update Feeds</td> 
   <td>Full access</td> 
   <td> <p>No access to modify Update Feeds.</p> <p>Access to add fields to be tracked in the Update Feeds when editing Custom Forms.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Filters</td> 
   <td>Full access</td> 
   <td> <p>No access to create Filters in the Setup area.</p> <p>Access to create new filters in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Views</td> 
   <td>Full access</td> 
   <td> <p>No access to create Views in the Setup area.</p> <p>Access to create new views in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Groupings</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groupings in the Setup area.</p> <p>Access to create new groupings in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: List Controls</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Cloud Providers</td> 
   <td>Full access</td> 
   <td> <p>No access to configure Cloud Providers.</p> <p>Access to link documents to and from Cloud Providers from the Documents tab, after the Cloud Providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Metadata Mapping</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Documents: SharePoint Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a SharePoint integration.</p> <p>Access to link documents to and from SharePoint from the Documents tab, after the SharePoint integration with Workfront has been configured.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Custom Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a Custom Integration.</p> <p>Access to link documents to and from third-party providers from the Documents tab, after the third-party providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>System: Branding</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Customer Info</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Single Sign-On (SSO)</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Update Users for SSO</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Kick-Starts</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Diagnostics</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  <tr> 
   <td>Change Tracking: Configuration</td> 
   <td>Full access</td> 
   <td>No access</td> 
  <tr> 
   <td>Change Tracking: Change History List</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
 </tbody> 
</table>

### Access to objects {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Standard or Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendars</td> 
   <td>Full access</td> 
   <td>Manage calendars they create and calendars shared with them.</td> 
  </tr> 
  <tr> 
   <td>Dashboards</td> 
   <td>Full access</td> 
   <td>Manage dashboards they create and dashboards shared with them.</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>Full access</td> 
   <td>Manage documents they upload or documents shared with them.</td> 
  </tr> 
  <tr> 
   <td>Issues</td> 
   <td>Full access</td> 
   <td>Manage issues they create or issues shared with them.</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>Full access</td> 
   <td>Manage portfolios they create or portfolios shared with them. </td> 
  </tr> 
  <tr> 
   <td>Programs</td> 
   <td>Full access</td> 
   <td>Manage programs they create or programs shared with them.</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Full access</td> 
   <td>Manage projects they create or projects shared with them.</td> 
  </tr> 
  <tr> 
   <td>Reports</td> 
   <td>Full access</td> 
   <td>Manage reports they create or reports shared with them. View, copy and edit system reports.</td> 
  </tr> 
  <tr> 
   <td>Tasks</td> 
   <td>Full access</td> 
   <td>Manage tasks they create or tasks shared with the</td> 
  </tr> 
  <tr> 
   <td>Templates</td> 
   <td>Full access</td> 
   <td>Manage templates they create or templates shared with them</td> 
  </tr> 
  <tr> 
   <td>Timesheets</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Users</td> 
   <td>Full access</td> 
   <td> <p>Limited access</p> <p>They cannot assign groups to users for which they are not a group administrator or groups that are not public.</p> <p>They cannot assign an access level to users which is higher then their own access level.</p> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator on a group, they can reset the password of and log in as the users in the group they administer and their subgroups. They cannot reset the password of or log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->


