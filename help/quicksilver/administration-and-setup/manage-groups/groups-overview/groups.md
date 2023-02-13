---
title: Grupos
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un administrador de Workfront puede crear grupos de usuarios que coincidan con la estructura del departamento. Los grupos son similares pero distintos de los equipos y las empresas. El administrador de Workfront concede a los grupos el acceso a las áreas de Workfront en las que necesitan trabajar y comunicarse. Cada grupo puede mantener su información de Workfront, como usuarios, plantillas, formularios personalizados y proyectos separados de los de otros departamentos. Se requiere al menos un administrador de grupo para cada grupo. Los administradores de grupos pueden usar la página Grupos para administrar sus grupos en un solo lugar. Puede crear hasta 14 niveles de subgrupos en un grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# Información general sobre grupos

Un administrador de Workfront puede crear grupos de usuarios que coincidan con la estructura del departamento. Los grupos son similares pero distintos de los equipos y las empresas.

El administrador de Workfront concede a los grupos el acceso a las áreas de Workfront en las que necesitan trabajar y comunicarse. Cada grupo puede mantener su información de Workfront, como usuarios, plantillas, formularios personalizados y proyectos separados de los de otros departamentos.

Se requiere al menos un administrador de grupo para cada grupo. Los administradores de grupos pueden usar la página Grupos para administrar sus grupos en un solo lugar. Para obtener más información, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

Puede crear hasta 14 niveles de subgrupos en un grupo. Para obtener más información, consulte [Información general de subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) y [Crear un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Uso de grupos para organizar usuarios

Como administrador de Workfront o administrador de grupos, puede asociar usuarios a grupos y subgrupos. Si publica un grupo, los usuarios con una licencia de Planificador pueden asociar usuarios con él. Para obtener más información sobre los administradores de grupos y los grupos públicos, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Cuando cree un usuario, le recomendamos que lo agregue al grupo de inicio correspondiente y a otros grupos en los que el usuario debería trabajar. Un usuario solo puede tener un grupo de inicio, pero puede estar en varios otros grupos.

Al formar parte de un grupo, el usuario puede acceder a los objetos que se comparten con el grupo y los subgrupos. Por ejemplo, si comparte un proyecto con un grupo, los usuarios del grupo y los subgrupos del grupo tendrán acceso a él.

>[!TIP]
>
>Si los departamentos de su organización a menudo trabajan juntos para administrar proyectos y los recursos de esos proyectos, puede que no sea necesario dividir los departamentos en muchos grupos más pequeños. Algunos grupos de alto nivel podrían funcionar mejor.

Un grupo puede tener un número ilimitado de usuarios.

Para obtener más información sobre la creación de usuarios nuevos, consulte [Agregar usuarios](../../../administration-and-setup/add-users/add-users.md).

## Concesión de un acceso de grupo a objetos

Cuando comparte un objeto con un grupo, todos los miembros de ese grupo (incluidos los miembros de cualquier subgrupo) tienen acceso al objeto. Para obtener más información sobre cómo compartir en Workfront, consulte [Información general sobre cómo compartir permisos en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Asociación de un grupo con un objeto

Al crear o editar uno de los siguientes objetos de Workfront, puede asociarlo a un grupo:

* **Proyecto**: Puede asociar un solo grupo con un proyecto para indicar la propiedad del proyecto.

   Esto no concede implícitamente a cada miembro del grupo derechos al proyecto. Para tener derechos sobre el proyecto, los usuarios deben recibir derechos compartiendo el proyecto con ellos.

   Aunque los usuarios pueden ser miembros de varios grupos, un proyecto puede tener un solo grupo asociado. Los usuarios de otros grupos aún pueden trabajar en el mismo proyecto si los proyectos se han compartido con ellos o con sus grupos. El grupo asociado con el proyecto suele ser el grupo responsable de completarlo o el grupo para el que se entrega el proyecto.

   Para obtener instrucciones sobre cómo asociar un proyecto a un grupo, consulte [Administrar información en el área Información general del proyecto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, programa o empresa**: Al crear o editar un portafolio, programa o empresa, puede asignarle un solo grupo para indicar que el grupo es propietario o que tiene la responsabilidad de él. Con esta asociación, los administradores y usuarios pueden identificar fácilmente en qué carteras, programas y empresas están trabajando sus grupos.

   Por ejemplo, un administrador de grupo puede enumerar todas las carteras de la organización mediante una lista o informe y anotar en la columna Grupo qué carteras tienen asignadas a su grupo.

   >[!NOTE]
   >
   >Asignar un grupo a un portafolio, programa o empresa con un grupo no significa automáticamente que la información del grupo tenga acceso a sus datos. Debe compartir manualmente el acceso a los datos con el grupo para que puedan verlo.

   Para obtener instrucciones, consulte [Crear un portafolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Crear un programa](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)y [Crear y editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Proceso de aprobación**: Puede hacer que un proceso de aprobación esté disponible para proyectos, tareas y problemas pertenecientes a un grupo determinado. Para obtener más información, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Ruta de Milestone**: Puede permitir que los usuarios de ciertos grupos utilicen una ruta de hitos con sus proyectos. Para obtener más información, consulte [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Plantilla de diseño**: Puede conceder permiso a los administradores de un grupo para modificar una plantilla de diseño. Para obtener instrucciones, consulte [Conceder acceso administrativo a una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Perfil de hoja de horas**: Puede conceder permiso a los administradores de un grupo para modificar un perfil de parte de horas. Para obtener más información, consulte [Crear, editar y asignar perfiles de parte de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Programaciones**: Puede conceder permiso a los administradores de un grupo para modificar una programación. Para obtener más información, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Equipos**: Puede asociar un grupo con un equipo para que los administradores de los grupos y sus subgrupos puedan ver y trabajar con ellos desde el área Grupos . Para obtener más información, consulte [Crear un equipo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) o [Editar configuración de equipo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Plantilla**: Puede asignar un grupo a una plantilla de proyecto. Esto puede ayudarle a agilizar el proceso de creación de proyectos y a identificar más fácilmente qué grupos son propietarios de las plantillas de proyecto, así como a informar al respecto. Para obtener más información, consulte la sección [Información general](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) en el artículo [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Elementos eliminados y restaurados recientemente**: Puede ver y administrar los grupos que han eliminado recientemente. Para obtener más información, consulte [Ver y administrar los elementos eliminados recientemente de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) y [Ver y administrar los elementos restaurados recientemente de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
