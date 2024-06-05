---
title: Información general sobre los permisos de uso compartido en Adobe Workfront Planning
description: Puede compartir o quitar permisos en un espacio de trabajo o vista de Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 3856e56036a9845387d7dc6498a6f20728c8234a
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 6%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Información general sobre los permisos de uso compartido en Adobe Workfront Planning

{{planning-important-intro}}

Puede compartir o quitar permisos en un espacio de trabajo o vista en Adobe Workfront Planning.

En este artículo se describen los niveles de permisos para los objetos de Workfront Planning.

Para obtener información sobre cómo compartir espacios de trabajo o vistas, consulte los siguientes artículos:

* [Compartir espacios de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

* [Compartir vistas](/help/quicksilver/planning/access/share-views.md)

## Objetos que se pueden compartir en Adobe Workfront Planning

Puede compartir los siguientes objetos:

* Espacios de trabajo

  Al compartir un espacio de trabajo, también se comparten todos los tipos de registros, registros y campos asociados a los espacios de trabajo. Las vistas no se comparten.

* Vistas

## Consideraciones sobre el uso compartido de objetos en Adobe Workfront Planning

* El tipo de licencia de Adobe Workfront funciona junto con los permisos de Workfront Planning para proporcionarle acceso para ver, contribuir o administrar objetos al utilizar Workfront Planning.

  Para obtener información sobre cómo afectan los tipos de licencia a los niveles de permisos de Workfront Planning, consulte [Información general sobre el tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Los administradores del sistema pueden administrar y compartir espacios de trabajo creados por otros usuarios.
* Si no es administrador del sistema, puede contribuir a los espacios de trabajo creados por otros usuarios si los comparten con usted.
* No puede compartir espacios de trabajo o vistas de forma masiva.
* Puede compartir un espacio de trabajo o una vista con las siguientes entidades:
   * Usuarios
   * Grupos
     <!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
* Otros usuarios, incluidos los administradores del sistema, solo pueden acceder a las vistas que han creado o que se han compartido con ellos. A los administradores del sistema solo se les pueden otorgar permisos para Administrar una vista.
* Puede compartir un vínculo a un espacio de trabajo o a una vista desde una página de tipo de registro con otros usuarios. Los usuarios que reciban el vínculo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder al espacio de trabajo o a la página de tipo de registro que se muestra en la vista seleccionada.

## Permisos de uso compartido para objetos de Adobe Workfront Planning

Las tablas de las secciones siguientes ilustran el nivel de permisos que puede seleccionar al compartir un espacio de trabajo o una vista, así como la funcionalidad que permite cada nivel.

>[!IMPORTANT]
>
>No todos los usuarios pueden tener los niveles de permisos que se describen a continuación. La licencia individual de los usuarios determina qué nivel de permisos pueden recibir para los objetos de Workfront Planning.
>
>Para obtener más información, consulte [Información general sobre el tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Permisos de Workspace

Debe conceder a los usuarios permiso para acceder a los espacios de trabajo para que puedan acceder a las entidades siguientes:

* Espacios de trabajo
* Tipos de registro
* Registros
* Campos
* Vistas*

  *Puede permitir que todos los usuarios con permisos de Vista o superiores de un espacio de trabajo también accedan a las vistas del espacio de trabajo. Se trata de un permiso adicional que debe habilitar al compartir una vista. Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).

Los siguientes son los niveles de permisos para espacios de trabajo:

|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Editar | ✓ |            |       |
| Compartir | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de tipo de registro

Los permisos de Tipo de registro se heredan al conceder permisos al espacio de trabajo.

A continuación se indican los niveles de permisos para los tipos de registro:


|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Editar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de registro

Los permisos de registro se heredan al conceder permisos al espacio de trabajo.

A continuación se indican los niveles de permisos para los registros:


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

Debe conceder permiso a los usuarios para que puedan acceder a los siguientes elementos de vista:

* Filtros
* Visibilidad de campo
* Ordenar
* Agrupación
* Altura de la fila
* Configuración


<!--You can share views internally or publicly. -->

Los siguientes son los niveles de permisos para vistas y elementos de vista:

|        | Administrar (solo pueden acceder las personas invitadas) | Ver (solo pueden acceder las personas invitadas) | Todos los usuarios del espacio de trabajo pueden ver* |
|--------|--------|-------|------------------------------|
| Editar | ✓ |       |                            |
| Eliminar | ✓ |       |                            |
| Compartir | ✓ |       |                           |
| Ver | ✓ | ✓ | ✓ |
| Aplicar | ✓ | ✓ | ✓ |

*Los usuarios deben tener permisos de Vista o superiores en un espacio de trabajo para obtener este acceso de vista.

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->


<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |    
-->