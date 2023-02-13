---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Información general de subgrupos
description: Puede crear hasta 14 niveles de subgrupos en un grupo. En cualquiera de estos niveles, puede crear un número ilimitado de subgrupos paralelos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Información general de subgrupos

Puede crear hasta 14 niveles de subgrupos en un grupo. En cualquiera de estos niveles, puede crear un número ilimitado de subgrupos paralelos. Para obtener instrucciones, consulte [Crear un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Para obtener información sobre los grupos, consulte [Información general sobre grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## ¿Qué heredan los subgrupos?

Los subgrupos heredan la pertenencia a su grupo principal. Por lo tanto, los usuarios y grupos de un subgrupo tienen la misma visibilidad, permisos y acceso a todos los objetos que los usuarios y grupos que pertenecen al grupo principal que comparten.

Además, un subgrupo hereda automáticamente los administradores de grupo de su grupo de nivel superior, pero también puede asignar miembros de un subgrupo para que actúen como administradores de grupo.

>[!TIP]
>
>A veces, es posible que desee utilizar subgrupos para agregar varios usuarios a un grupo existente a fin de darles acceso a un objeto que necesiten.
>
>Por ejemplo, supongamos que tiene un grupo de técnicos de asistencia técnica y un grupo separado de directores de TI. El grupo del servicio de asistencia tiene permisos para una cola de solicitud determinada. Desea agregar los directores de TI al grupo de asistencia para que también tengan permisos en la cola de solicitud. Sin la funcionalidad de los subgrupos, tendría que añadir los directores de TI al grupo de asistencia manualmente, lo que podría ser ineficiente y difícil de administrar. Si agrega el grupo Directores de TI al grupo de asistencia técnica como subgrupo, realizará esta tarea más rápido con solo un cambio.

>[!NOTE]
>
>Si un usuario se agregó a un subgrupo y a su grupo principal por separado, al eliminarlo de uno no se elimina al usuario del otro. Si no desea que el usuario tenga el acceso permitido para el grupo principal, debe quitar el usuario del subgrupo y del grupo principal.

## Subgrupos públicos y privados

Para un grupo público, cualquier usuario (dentro o fuera del grupo) que tenga acceso de usuario de edición puede agregar el grupo al perfil de otros usuarios. No pueden hacerlo para un grupo privado.

Esta opción solo se puede editar en el grupo principal superior de una jerarquía de grupos que tenga más de un nivel. Todos los subgrupos del grupo principal heredan su configuración.

Si crea un subgrupo en un grupo que sea público, el subgrupo también será público de forma predeterminada. Para obtener más información sobre la creación de un grupo y su publicación, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Para obtener más información sobre el acceso necesario para editar usuarios, consulte [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Cualquier grupo que agregue a un grupo existente se convertirá automáticamente en un subgrupo y ya no será un grupo principal. Sin embargo, el subgrupo conserva sus usuarios existentes, así como cualquier asociación con proyectos, problemas y tareas, además de todos los estados de proyectos, tareas y problemas que pertenecen al nuevo grupo principal.

## Administradores de grupo para subgrupos

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

Puede asignar miembros de subgrupo como administradores de grupo al subgrupo cuando lo cree o lo edite. Para obtener instrucciones, consulte [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) en el artículo [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Como alternativa, puede dejar la administración del subgrupo en manos de los administradores del grupo que estén asignados a los grupos superiores. Cuando crea un subgrupo, los administradores de grupo sobre los grupos superiores tienen acceso automático para administrar el subgrupo.

>[!NOTE]
>
>Si agrega un usuario a un subgrupo y este es un administrador de grupo para un grupo en cualquier parte superior al subgrupo, ese usuario tendrá derechos administrativos para administrar el subgrupo, incluso sin que se le asigne como administrador de grupo.

Para saber qué acciones están disponibles para un administrador de Adobe Workfront que administra el sistema Workfront, un administrador de grupo que administra un grupo de nivel superior y un administrador de grupo que administra un subgrupo, consulte [Acciones permitidas para diferentes tipos de administradores](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
