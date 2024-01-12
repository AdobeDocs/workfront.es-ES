---
title: Información general sobre los permisos de uso compartido en Adobe Maestro
description: Puede compartir o quitar permisos en un área de trabajo o vista de Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 8%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Información general sobre los permisos de uso compartido en Adobe Maestro

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Debe ser cliente de Workfront para tener acceso a Maestro.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede compartir o quitar permisos en un área de trabajo o vista de Adobe Maestro.

Este artículo describe los niveles de permisos para los objetos Maestro.

Para obtener información sobre cómo compartir espacios de trabajo o vistas, consulte los siguientes artículos:

* [Compartir espacios de trabajo](/help/quicksilver/maestro/access/share-workspaces.md)

* [Compartir vistas](/help/quicksilver/maestro/access/share-views.md)

## Objetos que puede compartir en Adobe Maestro

Puede compartir los siguientes objetos en Maestro:

* Espacios de trabajo

  Al compartir un espacio de trabajo, también se comparten todos los tipos de registros, registros y campos asociados a los espacios de trabajo. Las vistas no se comparten.

* Vistas

## Consideraciones acerca de compartir objetos en Maestro

* Debe tener la siguiente licencia para crear espacios de trabajo en Maestro:

   * Nuevo modelo de precios: licencia estándar
   * Modelo de precios actual: licencia de planificación.

  Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* Los administradores del sistema pueden administrar y compartir espacios de trabajo creados por otros usuarios.
* Si no es administrador del sistema, puede contribuir a los espacios de trabajo creados por otros usuarios si los comparten con usted.
* No puede compartir espacios de trabajo de forma masiva.
* Puede compartir un espacio de trabajo con las siguientes entidades:
   * Usuarios
   * Grupos
* Otros usuarios, incluidos los administradores del sistema, solo pueden acceder a las vistas que han creado o que se han compartido con ellos.

## Permisos de uso compartido para objetos Maestro

Las tablas de las secciones siguientes ilustran el nivel de permisos que puede seleccionar al compartir un área de trabajo o vista de Maestro y la funcionalidad que permite cada nivel.

### Permisos de Workspace

|        | Administrar | Contribuir | Ver |
|--------|--------|------------|-------|
| Editar | ✓ |            |       |
| Compartir | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de tipo de registro

Los permisos de Tipo de registro se heredan al conceder permisos al espacio de trabajo.

|        | Administrar | Contribuir | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Editar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de registro

Los permisos de registro se heredan al conceder permisos al espacio de trabajo.

|        | Administrar | Contribuir | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ | ✓ |       |
| Editar | ✓ | ✓ |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de campo

Los permisos de campo se heredan al conceder permisos al espacio de trabajo.
Los siguientes permisos hacen referencia a los propios campos y no a los valores asociados a cada campo. Para editar valores de campo, debe tener permisos para editar registros.

|        | Administrar | Contribuir | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Editar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |


### Ver permisos

Debe conceder permisos independientes a las vistas de registros. La concesión de permisos al espacio de trabajo no concede permisos a las vistas de registros del espacio de trabajo.

|        | Administrar | Ver |
|--------|--------|-------|
| Editar | ✓ |       |
| Eliminar | ✓ |       |
| Ver | ✓ | ✓ |
| Aplicar | ✓ | ✓ |






