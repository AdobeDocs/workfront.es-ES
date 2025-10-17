---
title: Información general de grupos
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un administrador de Workfront puede crear grupos de usuarios que coincidan con la estructura del departamento. Los grupos son similares a los equipos y las empresas, pero distintos de ellos.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 99%

---

# Información general sobre grupos

<!-- Audited: 01/2024 -->

Un administrador de Workfront puede crear grupos de usuarios que coincidan con la estructura del departamento. Los grupos son similares a los equipos y las empresas, pero distintos de ellos.

El administrador de Workfront concede a los grupos acceso a las áreas de Workfront donde necesitan trabajar y comunicarse. A continuación, cada grupo puede mantener su información de Workfront, como usuarios, plantillas y formularios y proyectos personalizados, separada de la de otros departamentos.

Se requiere al menos un administrador de grupos para cada grupo. Los administradores de grupos pueden utilizar la página Grupos para administrar sus grupos en un solo lugar. Para obtener más información, consulte [Administradores de grupos](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

Puede crear hasta 14 niveles de subgrupos en un grupo. Para obtener más información, consulte [Información general sobre subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) y [Crear un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Uso de grupos para organizar usuarios

Como administrador de Workfront o de grupos, puede asociar usuarios a grupos y subgrupos. Si hace público un grupo, los usuarios con una licencia Standard (nueva) o Plan (actual) pueden asociar usuarios a él. Para obtener más información sobre los administradores de grupos y los grupos públicos, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Cuando cree un usuario, le recomendamos que lo añada al grupo de inicio correspondiente y a otros grupos en los que el usuario debe trabajar. Un usuario solo puede tener un grupo de inicio, pero puede estar en varios grupos más.

Formar parte de un grupo proporciona al usuario acceso a los objetos compartidos con el grupo y los subgrupos. Por ejemplo, si comparte un proyecto con un grupo, los usuarios del grupo y sus subgrupos tienen acceso a él.

>[!TIP]
>
>Si los departamentos de la organización trabajan a menudo juntos para administrar proyectos y los recursos de esos proyectos, puede que no sea necesario dividir los departamentos en muchos grupos más pequeños. Algunos grupos de alto nivel podrían funcionar mejor.

Un grupo puede tener un número ilimitado de usuarios.

Para obtener más información sobre la creación de usuarios nuevos, consulte [Añadir usuarios](../../../administration-and-setup/add-users/add-users.md).

## Concesión a un grupo del acceso a objetos

Cuando comparte un objeto con un grupo, todos los miembros de ese grupo (incluidos los miembros de cualquier subgrupo) tienen acceso al objeto. Para obtener más información sobre el uso compartido en Workfront, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Asociación de un grupo a un objeto

Al crear o editar uno de los siguientes objetos de Workfront, puede asociarlo a un grupo:

* **Proyecto**: puede asociar un solo grupo a un proyecto para indicar que es el propietario del proyecto.

  Esto no otorga implícitamente a cada miembro del grupo derechos sobre el proyecto. Para tener derechos sobre el proyecto, los usuarios deben compartir el proyecto con ellos.

  Los usuarios pueden ser miembros de varios grupos, pero un proyecto puede tener un solo grupo asociado. Los usuarios de otros grupos pueden seguir trabajando en el mismo proyecto si éste se ha compartido con ellos o sus grupos. El grupo asociado al proyecto suele ser el responsable de completar el proyecto o el grupo a quien se entrega el proyecto.

  Para obtener instrucciones sobre la asociación de un proyecto a un grupo, consulte [Administrar información en el área Información general del proyecto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portafolio, programa o compañía**: cuando va a crear o editar un portafolio, programa o compañía, puede asignarle un solo grupo para indicar que el grupo es propietario o tiene responsabilidad sobre él. Con esta asociación realizada, los administradores y usuarios pueden identificar fácilmente en qué portafolios, programas y empresas están trabajando sus grupos.

  Por ejemplo, un administrador de grupos puede enumerar todos los portafolios de la organización mediante una lista o un informe y anotar en la columna Grupo qué portafolios están asignados a su grupo.

  >[!NOTE]
  >
  >Asignar un grupo a un portafolio, programa o compañía con un grupo no significa automáticamente que la información de dicho grupo tenga acceso a sus datos. Debe compartir manualmente el acceso a los datos con el grupo para que puedan verlos.

  Para obtener instrucciones, consulte [Crear un portafolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Crear un programa](../../../manage-work/portfolios/create-and-manage-programs/create-program.md) y [Crear y editar compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Proceso de aprobación**: puede hacer que un proceso de aprobación esté disponible para proyectos, tareas y problemas que pertenezcan a un grupo determinado. Para obtener más información, consulte [Crear un proceso de aprobación de elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Ruta de hitos**: puede permitir que los usuarios de determinados grupos utilicen una ruta de hitos con sus proyectos. Para obtener más información, consulte [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Plantilla de diseño**: puede conceder permiso a los administradores de un grupo para modificar una plantilla de diseño. Para obtener instrucciones, consulte [Conceder acceso administrativo a una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Perfil de plantilla de horas**: puede conceder permiso a los administradores de un grupo para modificar un perfil de plantilla de horas. Para obtener más información, consulte [Crear, editar y asignar perfiles de hojas de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Horarios**: puede conceder permiso a los administradores de un grupo para modificar una programación. Para obtener más información, consulte [Crear programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Equipos**: puede asociar un grupo con un equipo para que los administradores de los grupos y sus subgrupos puedan ver y trabajar con esos equipos desde el área de grupos. Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) o [Editar configuración de equipos](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Plantilla**: puede asignar un grupo a una plantilla de proyecto. Esto puede ayudarle a agilizar el proceso de creación de proyectos y a identificar e informar más fácilmente sobre qué grupos poseen qué plantillas de proyecto. Para obtener más información, consulte la sección [Información general](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) en el artículo [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Elementos eliminados y restaurados recientemente**: puede ver y administrar los grupos que han eliminado elementos borrados recientes. Para obtener más información, consulte [Ver y administrar los elementos eliminados recientemente de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) y [Ver y administrar los elementos restaurados de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
