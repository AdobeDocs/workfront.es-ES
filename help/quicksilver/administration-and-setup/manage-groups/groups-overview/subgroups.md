---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Información general sobre subgrupos
description: Puede crear hasta 14 niveles de subgrupos en un grupo. En cualquiera de estos niveles, puede crear un número ilimitado de subgrupos paralelos.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 99%

---

# Información general de subgrupos

Puede crear hasta 14 niveles de subgrupos en un grupo. En cualquiera de estos niveles, puede crear un número ilimitado de subgrupos paralelos. Para obtener instrucciones, consulte [Crear un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Para obtener información acerca de los grupos, consulte [Información general de grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## ¿Qué heredan los subgrupos?

Los subgrupos heredan la pertenencia de su grupo principal. Por lo tanto, los usuarios y grupos en un subgrupo tienen la misma visibilidad, permisos y acceso a todos los objetos que los usuarios y grupos que pertenecen al grupo principal que comparten.

Además, un subgrupo hereda automáticamente los administradores de grupo de su grupo de nivel superior, pero también puede asignar miembros de un subgrupo para que actúen como administradores de grupo.

>[!TIP]
>
>A veces, es posible que desee utilizar subgrupos para añadir varios usuarios a un grupo existente con el fin de darles acceso a un objeto que necesitan.
>
>Por ejemplo, suponga que tiene un grupo de técnicos de soporte técnico y un grupo separado de directores de TI. El grupo del servicio de asistencia tiene permisos para una cola de solicitudes determinada. Desea añadir los directores de TI al grupo del servicio de asistencia para que también tengan permisos para la cola de solicitudes. Sin la funcionalidad de subgrupos, tendría que añadir manualmente a los directores de TI al grupo de soporte técnico, lo cual podría ser ineficiente y difícil de gestionar. Si añade el grupo de directores de TI al grupo de soporte técnico como un subgrupo, realiza esta tarea de manera más rápida con solo un cambio.

>[!NOTE]
>
>Si un usuario fue añadido tanto a un subgrupo como a su grupo principal por separado, eliminar al usuario de uno no lo eliminará del otro. Si no desea que el usuario tenga el acceso permitido para el grupo principal, debe eliminar al usuario tanto del subgrupo como del grupo principal.

## Subgrupos públicos y privados

En el caso de los grupos públicos, cualquier usuario (dentro o fuera del grupo) que tenga acceso de usuario de edición puede añadir el grupo al perfil de otros usuarios. No pueden hacerlo para un grupo privado.

Solo puede editar esta opción en el grupo principal superior de una jerarquía de grupos que tenga más de un nivel. Todos los subgrupos del grupo principal heredan su configuración.

Si crea un subgrupo en un grupo que es público, el subgrupo también es público de forma predeterminada. Para obtener más información sobre cómo crear un grupo y hacerlo público, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Para obtener más información sobre el acceso necesario para editar usuarios, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Cualquier grupo que añade a un grupo existente se convierte automáticamente en un subgrupo y deja de ser un grupo principal. Sin embargo, el subgrupo conserva a sus usuarios existentes, así como cualquier asociación con proyectos, problemas y tareas, además de todos los estados de proyectos, tareas y problemas que pertenecen al nuevo grupo principal.

## Administradores de grupos para subgrupos

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

Puede asignar a los miembros del subgrupo como administradores del grupo para el subgrupo cuando lo cree o lo edite. Para obtener instrucciones, consulte [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) en el artículo [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Como alternativa, puede dejar la administración del subgrupo en manos de los administradores de grupo asignados a los grupos por encima de él. Cuando crea un subgrupo, los administradores de grupo de los grupos por encima de él tienen acceso automático para administrar el subgrupo.

>[!NOTE]
>
>Si añade a un usuario a un subgrupo y ese usuario es administrador de un grupo en cualquier nivel superior al subgrupo, dicho usuario tendrá derechos administrativos para gestionar el subgrupo, incluso sin ser asignado como administrador del grupo.

Para saber qué acciones están disponibles para un administrador de Adobe Workfront que gestiona el sistema Workfront, un administrador de grupo que gestiona un grupo de nivel superior y un administrador de grupo que gestiona un subgrupo, consulte [Acciones permitidas para los diferentes tipos de administradores](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
