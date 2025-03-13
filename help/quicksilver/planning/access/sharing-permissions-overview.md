---
title: Información general sobre los permisos de uso compartido en Adobe Workfront Planning
description: No todos los usuarios de la organización tienen el mismo acceso y permisos para utilizar Adobe Workfront Planning. Este artículo contiene información general sobre cómo compartir o quitar permisos en un espacio de trabajo o vista de Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: a3c82d8be6945a91a249d64923c6377a5edfa268
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 12%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Información general sobre los permisos de uso compartido en Adobe Workfront Planning

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>



{{planning-important-intro}}

Puede compartir o quitar permisos en un espacio de trabajo o vista de Adobe Workfront Planning.

En este artículo se describen los niveles de permisos para los objetos de Workfront Planning.

## Objetos que se pueden compartir en Adobe Workfront Planning

Puede compartir manualmente los siguientes objetos en Workfront Planning:

* Espacios de trabajo

   * Puede compartir espacios de trabajo con personas de su organización.
   * Al compartir un espacio de trabajo, también se comparten todos los tipos de registros, registros y campos asociados a los espacios de trabajo.
   * Al compartir un espacio de trabajo, las vistas no se comparten. Las vistas se comparten por separado.

  Para obtener más información, vea [Compartir espacios de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

<!--
<div class="preview">

* Record types

    * You can share record types with people inside your organization.
    * The level of permissions granted for the workspace displays as Inherited permissions for the record type. 
    * You cannot share a record type with a higher permission level than the user has on the workspace. 

    For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>
-->

* Vistas

   * Debe conceder a los usuarios, incluidos los administradores del sistema, permisos para acceder a las vistas por separado de sus permisos para acceder a espacios de trabajo.
   * Al compartir una vista, se comparten todos los elementos de la vista, incluidos los filtros, la agrupación, el orden o la configuración.
   * Al compartir una vista, los registros visibles en la vista no se comparten. Los registros deben compartirse compartiendo espacios de trabajo.
   * Puede compartir una vista públicamente, con personas fuera de su organización cuando genere un vínculo público para una vista.Las personas que accedan a la página de registro desde un vínculo público pueden ver todos los registros y sus campos, incluidos los registros y campos conectados.

  Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).

Internamente, se puede compartir un espacio de trabajo o una vista con las siguientes entidades de Workfront:

* Usuarios
* Grupos

<div class="preview">

* Equipos
* Compañías
* Roles

</div>

<span class="preview"> Cuando comparte espacios de trabajo y tipos de registros con otros, el nivel de permiso del tipo de registro se hereda automáticamente a los registros y campos asociados a ellos. </span>

## Consideraciones sobre el uso compartido de objetos en Adobe Workfront Planning

* El tipo de licencia de Adobe Workfront funciona junto con los permisos de Workfront Planning para permitirle acceder para ver, contribuir o administrar espacios de trabajo y sus objetos.

  Para obtener información acerca de cómo afectan los tipos de licencia a los niveles de permisos de Workfront Planning, vea [Descripción general del tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Los administradores del sistema pueden administrar todos los espacios de trabajo del sistema, incluidos los que no crearon.
* Otros usuarios, incluidos los administradores del sistema, solo pueden acceder a las vistas que han creado o que se han compartido con ellos. A los administradores del sistema solo se les pueden otorgar permisos para administrar una vista.
* Puede compartir un vínculo a un espacio de trabajo o a una vista con otros usuarios.

  Se dan los siguientes escenarios:
   * Los usuarios que reciban el vínculo a un espacio de trabajo deben ser usuarios activos e iniciar sesión en Workfront para poder acceder al espacio de trabajo.
   * Los usuarios que reciban el vínculo a una vista pueden acceder a la vista de las siguientes maneras:

      * Deben ser usuarios activos e iniciar sesión en Workfront, si el vínculo a la vista se ha compartido internamente.
      * Pueden ser usuarios externos de Workfront y acceder a la vista desde un vínculo compartido públicamente, sin iniciar sesión en Workfront.

## Permisos de uso compartido para objetos de Adobe Workfront Planning

Las tablas de las secciones siguientes ilustran el nivel de permisos que puede seleccionar al compartir un espacio de trabajo o una vista, así como la funcionalidad que permite cada nivel.

>[!IMPORTANT]
>
>No todos los usuarios pueden tener los niveles de permisos que se describen a continuación. La licencia individual de los usuarios determina qué nivel de permisos pueden recibir para los objetos de Workfront Planning.
>
>Solo los usuarios con licencia estándar (o de planificación) pueden tener permisos de contribución o administración en los espacios de trabajo y permisos de administración en las vistas.
> 
>Los usuarios con todos los demás tipos de licencia pueden tener permisos de visualización en espacios de trabajo y vistas.
>
>Para obtener más información, consulte [Descripción general del tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Permisos de Workspace

Debe conceder a los usuarios permiso para acceder a los espacios de trabajo para que puedan acceder a las entidades siguientes:

* Espacios de trabajo
* Tipos de registro
* Registros
* Campos

Los siguientes son los niveles de permisos para espacios de trabajo:

|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Editar | ✓ |            |       |
| Compartir | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de tipo de registro

<!--In the Production environment,--> Los permisos de Tipo de registro se heredan <!--always--> al conceder permisos al área de trabajo.

A continuación se indican los niveles de permisos para los tipos de registro:


|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Editar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |

<!--

<div class="preview">

In the Preview environment, you can remove the record type's inherited permissions received from the workspace. 

You can give users different permissions on the record type than they have on the workspace. However, you can never grant higher permissions for the record type than users have on the workspace. 

The following scenarios exist: 

|   Workspace permissions     | Automatic inherited permissions for a Record Type |Possible Record Type permissions when Inherited permissions are turned off (granted manually)| 
|--------|--------|-------------|
| Manage |   Manage    |   Manage, Remove permissions           | 
| Contribute |     Contribute |  Contribute, View, Remove permissions        |
| View   |  View     |      View, Remove permissions        |     

</div>

-->

### Permisos de registro

Los permisos de registro se heredan de <!--<span class="preview">the record type</span>, when you grant permissions to -->el espacio de trabajo<!-- and <span class="preview">the record type</span>-->.

A continuación se indican los niveles de permisos para los registros:


|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Crear | ✓ | ✓ |       |
| Eliminar | ✓ | ✓ |       |
| Editar | ✓ | ✓ |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos de campo

Los permisos de campo se heredan de <!--<span class="preview">the record type</span>, when you grant permissions to -->el área de trabajo <!--and <span class="preview">the record type</span>-->.

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

Puede compartir vistas de forma interna o pública.

Los siguientes son los niveles de permisos para vistas y elementos de vista:

| Uso compartido interno | Administrar (solo pueden acceder las personas invitadas) | Ver (solo pueden acceder las personas invitadas) | Todos los usuarios del espacio de trabajo pueden ver* |
|--------|--------|-------|------------------------------|
| Editar | ✓ |       |                            |
| Eliminar | ✓ |       |                            |
| Compartir | ✓ |       |                           |
| Ver | ✓ | ✓ | ✓ |
| Aplicar | ✓ | ✓ | ✓ |

| Uso compartido público | Ver |
|--------|-------|
| Ver | ✓ |
| Aplicar | ✓ |

*Los usuarios deben tener permisos de Vista o superiores en un espacio de trabajo para obtener este acceso de vista.

<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |  


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->