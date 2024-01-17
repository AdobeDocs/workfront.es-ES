---
title: Información general de grupos
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un administrador de Workfront puede crear grupos de usuarios que coincidan con la estructura del departamento. Los grupos son similares a los equipos y las empresas, pero distintos de ellos.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: b5e0a590d258df4510a0bb6a44b57099f32ae6b9
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Información general de grupos

<!-- Audited: 01/2024 -->

Un administrador de Workfront puede crear grupos de usuarios que coincidan con la estructura del departamento. Los grupos son similares a los equipos y las empresas, pero distintos de ellos.

El administrador de Workfront concede a los grupos acceso a las áreas de Workfront donde necesitan trabajar y comunicarse. A continuación, cada grupo puede mantener su información de Workfront, como usuarios, plantillas y formularios y proyectos personalizados, separada de la de otros departamentos.

Se requiere al menos un administrador de grupo para cada grupo. Los administradores de grupos pueden utilizar la página Grupos para administrar sus grupos en un solo lugar. Para obtener más información, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

Puede crear hasta 14 niveles de subgrupos en un grupo. Para obtener más información, consulte [Información general sobre subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) y [Creación de un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Uso de grupos para organizar usuarios

Como administrador de Workfront o de un grupo, puede asociar usuarios con grupos y subgrupos. Si hace público un grupo, los usuarios con una licencia Standard (nueva) o Plan (actual) pueden asociar usuarios con él. Para obtener más información sobre los administradores de grupos y los grupos públicos, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Cuando cree un usuario, le recomendamos que lo añada al grupo de inicio correspondiente y a otros grupos en los que el usuario debe trabajar. Un usuario solo puede tener un grupo de inicio, pero puede estar en varios grupos más.

Formar parte de un grupo proporciona al usuario acceso a los objetos compartidos con el grupo y los subgrupos. Por ejemplo, si comparte un proyecto con un grupo, los usuarios del grupo y de sus subgrupos tienen acceso a él.

>[!TIP]
>
>Si los departamentos de la organización trabajan a menudo juntos para administrar proyectos y los recursos de esos proyectos, puede que no sea necesario dividir los departamentos en muchos grupos más pequeños. Algunos grupos de alto nivel podrían funcionar mejor.

Un grupo puede tener un número ilimitado de usuarios.

Para obtener más información sobre la creación de usuarios nuevos, consulte [Adición de usuarios](../../../administration-and-setup/add-users/add-users.md).

## Concesión de acceso de grupo a objetos

Cuando comparte un objeto con un grupo, todos los miembros de ese grupo (incluidos los miembros de cualquier subgrupo) tienen acceso al objeto. Para obtener más información sobre cómo compartir en Workfront, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Asociación de un grupo a un objeto

Al crear o editar uno de los siguientes objetos de Workfront, puede asociarlo a un grupo:

* **Proyecto**: puede asociar un solo grupo a un proyecto para indicar que es el propietario del proyecto.

  Esto no otorga implícitamente a cada miembro del grupo derechos sobre el proyecto. Para tener derechos sobre el proyecto, los usuarios deben compartir el proyecto con ellos.

  Aunque los usuarios pueden ser miembros de varios grupos, un proyecto puede tener un solo grupo asociado. Los usuarios de otros grupos pueden seguir trabajando en el mismo proyecto si este se ha compartido con ellos o con sus grupos. El grupo asociado con el proyecto suele ser el responsable de completar el proyecto o el grupo para el que se entrega el proyecto.

  Para obtener instrucciones sobre cómo asociar un proyecto a un grupo, consulte [Administrar información en el área de Información general del proyecto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, programa o empresa**: cuando crea o edita un portafolio, programa o compañía, puede asignarle un solo grupo para indicar que el grupo es propietario o tiene responsabilidad sobre él. Con esta asociación realizada, los administradores y usuarios pueden identificar fácilmente en qué portafolios, programas y empresas están trabajando sus grupos.

  Por ejemplo, un administrador de grupo puede enumerar todos los portafolios de la organización mediante una lista o un informe y anotar en la columna Grupo qué portafolios están asignados a su grupo.

  >[!NOTE]
  >
  >Asignar un grupo a un portafolio, programa o empresa con un grupo no significa automáticamente que la información en la que el grupo tiene acceso a sus datos. Debe compartir manualmente el acceso a los datos con el grupo para que puedan verlo.

  Para obtener instrucciones, consulte [Crear un portafolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Creación de un programa](../../../manage-work/portfolios/create-and-manage-programs/create-program.md), y [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Proceso de aprobación**: puede hacer que un proceso de aprobación esté disponible para proyectos, tareas y problemas que pertenezcan a un grupo determinado. Para obtener más información, consulte [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Ruta de hitos**: puede permitir que los usuarios de determinados grupos utilicen una trayectoria del hito con sus proyectos. Para obtener más información, consulte [Creación de una trayectoria del hito](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Plantilla de diseño**: puede conceder permiso a los administradores de un grupo para modificar una plantilla de diseño. Para obtener instrucciones, consulte [Concesión de acceso administrativo a una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Perfil de hoja de horas**: Puede conceder permiso a los administradores de un grupo para modificar un perfil de plantilla de horas. Para obtener más información, consulte [Crear, editar y asignar perfiles de hojas de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Horarios**: Puede conceder permiso a los administradores de un grupo para modificar una programación. Para obtener más información, consulte [Creación de una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Equipos**: puede asociar un grupo a un equipo para que los administradores de los grupos y sus subgrupos puedan ver y trabajar con esos equipos desde el área de Grupos. Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) o [Editar configuración del equipo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Plantilla**: puede asignar un grupo a una plantilla de proyecto. Esto puede ayudarle a optimizar el proceso de creación de proyectos y a identificar e informar más fácilmente sobre los grupos que poseen las plantillas de proyecto. Para obtener más información, consulte la sección [Información general](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) en el artículo [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Elementos eliminados y restaurados recientemente**: puede ver y administrar los grupos de elementos eliminados recientemente. Para obtener más información, consulte [Ver y administrar los elementos eliminados recientemente de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) y [Ver y administrar los elementos restaurados recientemente de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
