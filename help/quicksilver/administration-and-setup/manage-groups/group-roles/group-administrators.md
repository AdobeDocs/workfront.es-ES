---
title: Administradores de grupo
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Es posible que los administradores de Adobe Workfront de una organización grande con muchos departamentos no deseen administrar todos los departamentos y grupos de la organización dentro de esos departamentos. En su lugar, pueden crear un grupo para cada departamento y subgrupos dentro de ese grupo, cada uno administrado por un administrador de grupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 03667fbdd1b0d68b9ad2d2db4a1ed85b8136062b
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# Administradores de grupo

Es posible que los administradores de Adobe Workfront de una organización grande con muchos departamentos no deseen administrar todos los departamentos y grupos de la organización dentro de esos departamentos. En su lugar, pueden crear un grupo para cada departamento y subgrupos dentro de ese grupo, cada uno administrado por un administrador de grupos.

Un administrador de grupos puede administrar las necesidades de un grupo, como la pertenencia de un usuario, las plantillas de diseño, los datos personalizados, los estados y las preferencias.

Pueden existir hasta 14 niveles de subgrupos bajo un grupo.

>[!NOTE]
>
>Todos los administradores de grupo de la jerarquía superior a un subgrupo tienen derechos administrativos para administrar ese subgrupo.

Para obtener información sobre cómo crear y administrar grupos, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) y [Administrar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Consulte también [Información general de subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Designación de administradores de grupos

Cada grupo de nivel superior debe tener al menos un administrador de grupo. Un administrador de Workfront o un administrador de un grupo pueden asignar administradores de grupo a los subgrupos del grupo, pero esto no es necesario. Para obtener más información, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Si es administrador de Workfront, le recomendamos que haga lo siguiente antes de designar a los usuarios como administradores de grupos:

* Tenga en cuenta el número actual de administradores de Workfront en su sistema.
* Anote el número de grupos que tiene en su sistema.
* Determine si puede cambiar el nivel de acceso de algunos de los administradores de Workfront y designarlos como administradores de grupo.

   Para obtener más información sobre las capacidades de los administradores de grupos, consulte [Tareas realizadas por los administradores de grupos](#tasks-done-by-group-administrators).

* Determine si desea que los administradores de grupos puedan iniciar sesión como otros usuarios o restablecer las contraseñas de los usuarios de los grupos que administra. Se necesita acceso adicional para realizar estas tareas, como se explica en [Acceso necesario para administradores de grupos](#access-needed-for-group-administrators).
* Para una mejor administración de usuarios, considere la posibilidad de asignar grupos o subgrupos en lugar de usuarios a los siguientes objetos:

   * Plantillas de diseño
   * Horarios
   * Perfiles de hoja de horas

## Acceso necesario para administradores de grupos {#access-needed-for-group-administrators}

Todos los administradores de grupos deben tener una licencia de Plan.

Se recomienda que los administradores de grupos tengan acceso de edición a los usuarios para que puedan realizar las siguientes tareas:

* Inicie sesión como otros usuarios en los grupos y subgrupos que administran.
* Restablezca la contraseña de otro usuario en los grupos que administra.

>[!IMPORTANT]
>
>Los administradores de grupos deben tener un acceso mayor que los que administran; de lo contrario, no podrán ver ni modificar los niveles de acceso inferiores.
>Para obtener instrucciones sobre la concesión de este acceso, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Para un administrador de grupo que necesite asignar perfiles de parte de horas a usuarios de sus grupos y subgrupos, también recomendamos Acceso administrativo a partes de horas y horas. Para obtener instrucciones sobre la concesión de este acceso, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Tareas realizadas por los administradores de grupos {#tasks-done-by-group-administrators}

Como administrador de grupos, puede llevar a cabo las tareas siguientes para administrar los grupos que supervisa. Algunas son iguales a las capacidades que se ofrecen a un administrador de Workfront.

* [Administrar miembros del grupo](#manage-group-members)
* [Administrar objetos de grupo](#manage-group-objects)
* [Administrar las preferencias y herramientas del grupo](#manage-group-preferences-and-tools)

### Administrar miembros del grupo {#manage-group-members}

* Cree, edite y elimine subgrupos dentro de los grupos y subgrupos que administra. Para obtener instrucciones, consulte [Crear un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Agregue a los usuarios para los que tenga acceso de edición a sus grupos y subgrupos. O agregue usuarios a grupos y subgrupos editando sus perfiles.

   También puede actualizar los campos del perfil de un miembro del grupo si tiene habilitado el permiso Administración de usuarios (Usuarios del grupo) en su nivel de acceso.

   Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Los administradores de Workfront pueden anular los cambios realizados por un administrador de grupos en las suscripciones a grupos.

* Restablezca contraseñas para los usuarios que sean miembros de los grupos que administra. Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Inicie sesión como usuarios que sean miembros de los grupos que administra. Para obtener más información, consulte [Iniciar sesión como otro usuario](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Vea el número de licencias disponibles para su grupo y los subgrupos que se encuentran debajo. Para obtener más información, consulte [Administre las licencias disponibles en su sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Administrar objetos de grupo {#manage-group-objects}

* Cree plantillas de diseño de nivel de grupo y asócielas a los grupos y subgrupos que administre. Para obtener más información, consulte [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Cree perfiles de hojas de horas de nivel de grupo, asócielos a los usuarios y grupos que administre y genere hojas de horas manualmente. Para obtener más información, consulte [Crear, editar y asignar perfiles de parte de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Sin acceso administrativo a los procesos de aprobación, cree y edite procesos de aprobación para los grupos y subgrupos que administra. Para obtener más información, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   Para obtener información sobre el acceso administrativo a los procesos de aprobación, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Cree programaciones y asócielas a un grupo que administre. Para obtener más información, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Administre un equipo asignado a un grupo que administra, sin ser miembro del equipo. Además, cree un informe de equipo basado en el campo Grupo para identificar al grupo al que se asigna un determinado equipo. Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Restaure un proyecto que esté asociado con un grupo que administra, junto con cualquier tarea, problema o documento asociado al proyecto. Para obtener más información, consulte [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Administrar las preferencias y herramientas del grupo {#manage-group-preferences-and-tools}

* Cuando una preferencia de proyecto, tarea o preferencia de problema, o hojas de horas y preferencias de horas se desbloqueen para grupos en todo el sistema, edite esa preferencia para los grupos que administra. Estas preferencias afectan al comportamiento del proyecto, la tarea y el problema. Para obtener más información, consulte lo siguiente:

   * [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Cree y edite estados de grupo para los grupos que administra. Para obtener más información, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configure una notificación de evento para los grupos que administra. Solo puede hacerlo después de que un administrador de Workfront desbloquee la capacidad de configurar notificaciones de eventos para grupos a través del sistema. Para obtener más información, consulte [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
