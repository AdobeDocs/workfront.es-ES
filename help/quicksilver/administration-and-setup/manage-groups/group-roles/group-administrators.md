---
title: Administradores de grupo
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Es posible que los administradores de Adobe Workfront de una organización grande con muchos departamentos no deseen administrar todos los departamentos y grupos de la organización dentro de esos departamentos. En su lugar, pueden crear un grupo para cada departamento y subgrupos dentro de ese grupo, cada uno administrado por un administrador de grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# Administradores de grupos

<!-- Audited: 12/2023 -->

Es posible que los administradores de Adobe Workfront de una organización grande con muchos departamentos no deseen administrar todos los departamentos y grupos de la organización dentro de esos departamentos. En su lugar, pueden crear un grupo para cada departamento y subgrupos dentro de ese grupo, cada uno administrado por un administrador de grupo.

Un administrador de grupo puede administrar las necesidades de un grupo, como la pertenencia de usuarios, plantillas de diseño, datos personalizados, estados y preferencias.

Pueden existir hasta 14 niveles de subgrupos en un grupo.

>[!NOTE]
>
>Todos los administradores de grupo de la jerarquía sobre un subgrupo tienen derechos administrativos para administrar ese subgrupo.

Para obtener información sobre cómo crear y administrar grupos, vea [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) y [Administrar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Vea también [Información general de subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Designación de administradores de grupo

Cada grupo de nivel superior debe tener al menos un administrador de grupo. Un administrador de Workfront o de un grupo puede asignar administradores de grupos a los subgrupos del grupo, pero esto no es obligatorio. Para obtener más información, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Si es administrador de Workfront, le recomendamos que haga lo siguiente antes de designar usuarios como administradores de grupo:

* Tome nota de la cantidad actual de administradores de Workfront en su sistema.
* Tome nota del número de grupos que tiene en su sistema.
* Determine si puede cambiar el nivel de acceso de algunos de los administradores de Workfront y designarlos como administradores de grupo en su lugar.

  Para obtener más información acerca de las capacidades de los administradores de grupos, consulte [Tareas realizadas por los administradores de grupos](#tasks-done-by-group-administrators) en este artículo.

* Determine si desea que los administradores de grupo puedan iniciar sesión como otros usuarios o restablecer las contraseñas de los usuarios de los grupos que administra. Se necesita acceso adicional para realizar estas tareas, como se explica a continuación en [Acceso necesario para los administradores del grupo](#access-needed-for-group-administrators).
* Para mejorar la administración de usuarios, considere la posibilidad de asignar grupos o subgrupos en lugar de usuarios a los siguientes objetos:

   * Plantillas de diseño
   * Horarios
   * Perfiles de hoja de horas

## Acceso necesario para los administradores del grupo {#access-needed-for-group-administrators}

Cada administrador de grupo debe tener

* Una licencia de planificación en el modelo actual de precios y empaquetado
* Una licencia estándar en el nuevo modelo de precios y empaquetado

Se recomienda que los administradores de grupo tengan acceso de edición a los usuarios para que puedan realizar las siguientes tareas:

* Inicie sesión como otros usuarios en los grupos y subgrupos que administran.
* Restablecer la contraseña de otro usuario en los grupos que administra.

>[!IMPORTANT]
>
>Los administradores de grupo deben tener un acceso mayor que los que administran; de lo contrario, no podrán ver ni modificar niveles de acceso menores.
>Para obtener instrucciones sobre cómo conceder este acceso, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Para un administrador de grupo que necesite asignar perfiles de plantilla de horas a usuarios de sus grupos y subgrupos, también recomendamos acceso administrativo a las plantillas de horas y a las horas. Para obtener instrucciones sobre cómo conceder este acceso, consulte [Conceder acceso administrativo a usuarios en ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Tareas realizadas por los administradores del grupo {#tasks-done-by-group-administrators}

Como administrador de grupos, puede llevar a cabo las tareas descritas a continuación para administrar los grupos que supervisa. Algunas de ellas son las mismas que las capacidades que se proporcionan a un administrador de Workfront.

>[!NOTE]
>
>En el nuevo modelo de precios y empaquetado, debe tener un plan Prime o superior para realizar lo siguiente:
>
> * Crear notificaciones de eventos de grupo
> * Configurar las preferencias del proyecto de grupo
> * Configurar las preferencias de tareas de grupo y problemas
> * Desbloquear la configuración de las preferencias del subgrupo
> * Agrupar preferencias de horas y hojas de horas
> * Desbloquear hoja de horas y preferencia de horas

### Administrar miembros del grupo {#manage-group-members}

* Cree, edite y elimine subgrupos dentro de los grupos y subgrupos que administra. Para obtener instrucciones, vea [Crear un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Añada a sus grupos y subgrupos los usuarios para los que tenga acceso de edición. O bien, puede agregar usuarios a grupos y subgrupos editando sus perfiles.

  También puede actualizar los campos del perfil de un miembro del grupo si tiene habilitado el permiso Administración de usuarios (usuarios del grupo) en su nivel de acceso.

  Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Los administradores de Workfront pueden anular los cambios realizados por un administrador de grupo en las pertenencias a grupos.

* Restablezca las contraseñas de los usuarios que sean miembros de los grupos que administre. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Inicie sesión como usuarios que sean miembros de los grupos que administra. Para obtener más información, vea [Iniciar sesión como otro usuario](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Vea el número de licencias disponibles para su grupo y los subgrupos debajo de él. Para obtener más información, consulte [Administrar licencias disponibles en el sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Administrar objetos de grupo {#manage-group-objects}

* Cree plantillas de diseño de nivel de grupo y asócielas a los grupos y subgrupos que administre. Para obtener más información, consulte [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Cree perfiles de hojas de horas a nivel de grupo, asócielos a los usuarios y grupos que administre y genere hojas de horas manualmente. Para obtener más información, consulte [Crear, editar y asignar perfiles de hojas de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Sin acceso administrativo a los procesos de aprobación, cree y edite los procesos de aprobación para los grupos y subgrupos que administra. Para obtener más información, vea [Crear un proceso de aprobación de elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Para obtener información acerca del acceso administrativo a los procesos de aprobación, vea [Conceder acceso administrativo a los usuarios a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Cree programaciones y asócielas a un grupo que administre. Para obtener más información, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Gestionar un equipo asignado a un grupo que usted gestione, sin ser miembro del equipo. Además, cree un informe de equipo basado en el campo Grupo para identificar a qué grupo está asignado un equipo determinado. Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Restaurar un proyecto que esté asociado a un grupo que usted administre, junto con cualquier tarea, problema o documento asociado con el proyecto. Para obtener más información, vea [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Administrar las herramientas y preferencias del grupo {#manage-group-preferences-and-tools}

* Cuando la preferencia de un proyecto, una preferencia de tarea o problema o la preferencia de plantillas de horas y horas estén desbloqueadas para grupos en todo el sistema, edite esa preferencia para los grupos que administre. Estas preferencias afectan al comportamiento del proyecto, la tarea y el problema. Para obtener más información, consulte lo siguiente:

   * [Configurar preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Cree y edite los estados de grupo de los grupos que administra. Para obtener más información, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configure una notificación de eventos para los grupos que administre. Esto solo se puede hacer después de que un administrador de Workfront desbloquee la capacidad de configurar notificaciones de eventos para grupos a través del sistema. Para obtener más información, vea [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
