---
title: Información general sobre los grupos de inicio
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Se asigna un grupo de inicio en el perfil del usuario. Se requiere que todos los usuarios tengan un grupo en el hogar. Un usuario puede pertenecer a más de un grupo, pero solo puede tener un grupo de inicio. Aunque cualquier grupo existente en el sistema se puede asignar como grupo de inicio de un usuario, se recomienda crear y asignar nuevos grupos que representen unidades organizativas más grandes. Al establecer los grupos principales, tenga en cuenta cómo su organización divide a los usuarios de Adobe Workfront.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Información general sobre los grupos de inicio

Se asigna un grupo de inicio en el perfil del usuario. Se requiere que todos los usuarios tengan un grupo en el hogar. Un usuario puede pertenecer a más de un grupo, pero solo puede tener un grupo de inicio. Para obtener más información sobre Grupos, consulte [Información general sobre grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Aunque cualquier grupo existente en el sistema se puede asignar como grupo de inicio de un usuario, se recomienda crear y asignar nuevos grupos que representen unidades organizativas más grandes.

Al establecer los grupos principales, tenga en cuenta cómo su organización divide a los usuarios de Adobe Workfront. Estas son algunas sugerencias para determinar qué tipo de grupos deben utilizarse como grupo de inicio:

* Grupos que representan departamentos, como TI o Marketing
* Grupos regidos por diferentes presupuestos
* Grupos ubicados en diferentes áreas o regiones
* Grupos formados por varios equipos que pertenecen al mismo centro de costes

>[!NOTE]
>
>Si necesita reorganizar los grupos de inicio en unidades organizativas, debe hacer clic en
>1. Cree el nuevo grupo, tal como se explica en [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. Reasigne el nuevo grupo como grupo de inicio del usuario, tal como se explica en [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>


## Administración de plantillas de diseño

Cuando asigna una plantilla de diseño a un grupo, todos los usuarios que tengan el grupo asignado como su grupo principal pueden ver la configuración especificada en la plantilla de diseño.

Si se asigna una plantilla de diseño a un grupo de inicio, solo será visible para los usuarios asignados a ese grupo de inicio.

Para obtener más información, consulte [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) en [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Administración de licencias

Cada usuario puede asignarse a un solo grupo de inicio, lo que facilita la administración de recuentos de licencias.

Los administradores de Workfront tienen la opción de establecer el máximo de recuentos de licencias para los grupos principales.

La configuración de un recuento máximo de licencias permite a los administradores de Workfront impedir que una unidad empresarial utilice las licencias de Workfront adquiridas para otras unidades empresariales.

Para obtener más información, consulte [Administre las licencias disponibles en su sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
