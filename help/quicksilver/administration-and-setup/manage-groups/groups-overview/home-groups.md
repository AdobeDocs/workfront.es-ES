---
title: Información general de grupos de inicio
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un grupo de inicio se asigna en el perfil del usuario. Todos los usuarios deben tener un grupo de inicio.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 92%

---

# Información general sobre los grupos de inicio

Un grupo de inicio se asigna en el perfil del usuario. Todos los usuarios deben tener un grupo de inicio. Un usuario puede pertenecer a más de un grupo, pero solo puede tener un grupo de inicio. Para obtener más información sobre los grupos, consulte [Información general sobre los grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Aunque cualquier grupo existente en el sistema puede ser asignado como grupo de inicio de un usuario, se recomienda crear y asignar nuevos grupos que representen unidades organizativas más grandes. 

Al establecer grupos de inicio, tenga en cuenta cómo divide su organización a los usuarios de Adobe Workfront. A continuación se ofrecen algunas sugerencias para determinar qué tipo de grupos se deben utilizar como grupo de inicio:

* Grupos que representan departamentos, como TI o Marketing
* Grupos gobernados por presupuestos diferentes
* Grupos ubicados en diferentes áreas o regiones
* Grupos formados por varios equipos que pertenecen al mismo centro de coste

>[!NOTE]
>
>Si necesita reorganizar los grupos de inicio en unidades organizativas, debe
>
>1. Crear el nuevo grupo, como se explica en [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. Reasignar el nuevo grupo como el grupo de inicio del usuario, como se explica en [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Administración de plantillas de diseño

Al asignar una plantilla de diseño a un grupo, todos los usuarios que tengan el grupo asignado como su grupo de inicio pueden ver la configuración especificada en la plantilla de diseño.

Si una plantilla de diseño está asignada a un grupo de inicio, solo será visible para los usuarios asignados a ese grupo de inicio.

Para obtener más información, consulte [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Administración de licencias

A cada usuario se le puede asignar un solo grupo de inicio, lo que facilita la administración del número de licencias.

Los administradores de Workfront tienen la opción de establecer un número máximo de licencias para los grupos de inicio.

La definición de un número máximo de licencias permite a los administradores de Workfront impedir que una unidad de negocio en particular utilice las licencias de Workfront adquiridas para otras unidades de negocio.

Para obtener más información, consulte [Administrar licencias disponibles en el sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
