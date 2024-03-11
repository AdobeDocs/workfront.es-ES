---
title: Información general sobre los permisos de uso compartido en Adobe Maestro
description: Puede compartir o quitar permisos en un área de trabajo o vista de Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 7%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Información general sobre los permisos de uso compartido en Adobe Maestro

{{maestro-important-intro}}

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

* El tipo de licencia de Adobe Workfront funciona junto con los permisos de Maestro para proporcionarle acceso para ver, contribuir o administrar objetos de Maestro.

  Para obtener información acerca de cómo afectan los tipos de licencia a los niveles de permisos de los objetos Maestro, vea [Información general sobre el tipo de licencia al utilizar las funciones de planificación de Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).
* Los administradores del sistema pueden administrar y compartir espacios de trabajo creados por otros usuarios.
* Si no es administrador del sistema, puede contribuir a los espacios de trabajo creados por otros usuarios si los comparten con usted.
* No puede compartir espacios de trabajo de forma masiva.
* Puede compartir un espacio de trabajo con las siguientes entidades:
   * Usuarios
   * Grupos
* Otros usuarios, incluidos los administradores del sistema, solo pueden acceder a las vistas que han creado o que se han compartido con ellos.
* Puede compartir un vínculo a un espacio de trabajo o a una vista desde una página de tipo de registro con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder al espacio de trabajo o a la página de tipo de registro que se muestra en la vista seleccionada.

## Permisos de uso compartido para objetos Maestro

Las tablas de las secciones siguientes ilustran el nivel de permisos que puede seleccionar al compartir un área de trabajo o vista de Maestro y la funcionalidad que permite cada nivel.

>[!IMPORTANT]
>
>No todos los usuarios pueden tener los niveles de permisos que se describen a continuación. La licencia individual de los usuarios determina el nivel de permisos que pueden recibir para los objetos de Maestro.
>
>Para obtener más información, consulte [Información general sobre el tipo de licencia al utilizar las funciones de planificación de Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).


### Permisos de Workspace

|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Editar | ✓ |            |       |
| Compartir | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de tipo de registro

Los permisos de Tipo de registro se heredan al conceder permisos al espacio de trabajo.

|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Editar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de registro

Los permisos de registro se heredan al conceder permisos al espacio de trabajo.

|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ | ✓ |       |
| Editar | ✓ | ✓ |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de campo

Los permisos de campo se heredan al conceder permisos al espacio de trabajo.
Los siguientes permisos hacen referencia a los propios campos y no a los valores asociados a cada campo. Para editar valores de campo, debe tener permisos para editar registros.

|        | Administrar | Aportar | Ver |
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






