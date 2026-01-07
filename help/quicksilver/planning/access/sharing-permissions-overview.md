---
title: Información general sobre los permisos de uso compartido en Adobe Workfront Planning
description: No todos los usuarios de la organización tienen el mismo acceso y permisos para utilizar Adobe Workfront Planning. Este artículo contiene información general sobre cómo compartir o quitar permisos en un espacio de trabajo o vista de Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 6%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Información general sobre los permisos de uso compartido en Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

Puede compartir o quitar permisos en un espacio de trabajo de Adobe Workfront Planning, un tipo de registro o una vista.

También puede compartir formularios de solicitud de Planning. Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

En este artículo se describen los niveles de permisos para espacios de trabajo de Workfront Planning, los tipos de registros, los registros, los campos y las vistas.

## Objetos que se pueden compartir en Adobe Workfront Planning

Puede compartir manualmente algunos objetos de Workfront Planning, mientras que otros objetos heredan estos permisos de otros objetos.

Puede compartir manualmente los siguientes objetos en Workfront Planning:

* Espacios de trabajo

   * Puede compartir espacios de trabajo con personas de su organización.
   * Al compartir un espacio de trabajo, también se comparten todos los tipos de registros, registros y campos asociados a los espacios de trabajo.
   * Al compartir un espacio de trabajo, las vistas no se comparten. Las vistas se comparten por separado.

  Para obtener más información, vea [Compartir espacios de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

* Tipos de registro

   * Puede compartir tipos de registros con personas de su organización.
   * El nivel de permisos otorgados para el espacio de trabajo se muestra como Permisos heredados para el tipo de registro.
   * No se puede compartir un tipo de registro con un nivel de permisos superior al que el usuario tiene en el área de trabajo.

  Para obtener más información, vea [Compartir tipos de registros](/help/quicksilver/planning/access/share-record-types.md).


* Vistas

   * Debe conceder a los usuarios, incluidos los administradores del sistema, permisos para acceder a las vistas por separado de sus permisos para acceder a espacios de trabajo.
   * Al compartir una vista, se comparten todos los elementos de la vista, incluidos los filtros, la agrupación, el orden o la configuración.
   * Al compartir una vista, los registros visibles en la vista no se comparten. Los registros deben compartirse compartiendo espacios de trabajo.
   * Puede compartir una vista públicamente, con personas fuera de su organización cuando genere un vínculo público para una vista.Las personas que accedan a la página de registro desde un vínculo público pueden ver todos los registros y sus campos, incluidos los registros y campos conectados.

  Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).

## Consideraciones sobre el uso compartido de objetos en Adobe Workfront Planning

* El tipo de licencia de Adobe Workfront funciona junto con los permisos de Workfront Planning para permitirle acceder para ver, contribuir o administrar espacios de trabajo y sus objetos.

  Para obtener información acerca de cómo afectan los tipos de licencia a los niveles de permisos de Workfront Planning, vea [Descripción general del tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Los administradores del sistema pueden administrar todos los espacios de trabajo del sistema, incluidos los que no crearon.
* Otros usuarios, incluidos los administradores del sistema, solo pueden acceder a las vistas que han creado o que se han compartido con ellos. A los administradores del sistema solo se les pueden otorgar permisos para administrar una vista.

* Cuando comparte espacios de trabajo y tipos de registros con otros usuarios, el nivel de permiso del tipo de registro se hereda automáticamente a los registros y campos asociados a ellos.

  >[!IMPORTANT]
  >
  >Si la instancia de Workfront de su organización se ha incorporado a la experiencia unificada de Adobe, los usuarios con los que desea compartir objetos de Planning deben agregarse a Adobe Admin Console. No puede compartir objetos de Planning con usuarios de Workfront que no se hayan agregado a Adobe Admin Console.

* Puede compartir objetos de Planning de las siguientes maneras:

   * Internamente, se puede compartir un espacio de trabajo, una vista o un tipo de registro con las siguientes entidades de Workfront:

      * Usuarios
      * Grupos
      * Equipos
      * Compañías
      * Roles

     Puede compartir un objeto de Planning con hasta 100 entidades por objeto.

   * Internamente, compartiendo un vínculo a un espacio de trabajo o a una vista con otros usuarios de Planning. Se dan los siguientes escenarios:

      * Los usuarios que reciban el vínculo a un espacio de trabajo deben ser usuarios activos e iniciar sesión en Workfront para acceder al espacio de trabajo.
      * Los usuarios que reciban un vínculo de uso compartido interno para una vista deben ser usuarios activos e iniciar sesión en Workfront para acceder a la vista.
   * Externamente, compartiendo un vínculo de uso compartido público a una vista con usuarios externos que no tienen cuenta de Workfront.

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


### Permisos para espacios de trabajo

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

### Permisos para tipos de registros

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

Los permisos de Tipo de registro siempre se heredan al conceder permisos al espacio de trabajo.

Puede quitar los permisos heredados del tipo de registro recibidos del espacio de trabajo.

Puede conceder a los usuarios permisos inferiores en el tipo de registro que los que tienen en el espacio de trabajo.

Sin embargo, no puede hacer lo siguiente:

* Conceda permisos superiores al tipo de registro que los usuarios tienen en el espacio de trabajo.
* Asigne a los administradores de espacio de trabajo permisos inferiores en un tipo de registro.
* Quite los permisos de Vista en el tipo de registro o en el espacio de trabajo quitando usuarios de los permisos de tipo de registro.

Se dan los siguientes escenarios:

| Permisos de Workspace | Permisos heredados automáticos para un tipo de registro | Posibles permisos de Tipo de registro cuando los permisos heredados están desactivados (se conceden manualmente) |
|--------|--------|-------------|
| Administrar | Administrar | Administración, eliminación de permisos* |
| Aportar | Aportar | Aportar, Ver, Eliminar permisos* |
| Ver | Ver | Ver, quitar permisos* |

>[!NOTE]
>
>Cuando se quitan permisos de un tipo de registro, los usuarios conservan los permisos de Vista en el espacio de trabajo y en todos los tipos de registros, a menos que se quiten sus permisos del espacio de trabajo.

### Permisos para registros

Los permisos de registro se heredan del tipo de registro, cuando se conceden permisos al espacio de trabajo y al tipo de registro.

A continuación se indican los niveles de permisos para los registros:


|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Crear | ✓ | ✓ |       |
| Eliminar | ✓ | ✓ |       |
| Editar | ✓ | ✓ |       |
| Ver | ✓ | ✓ | ✓ |

### Permisos para registrar campos

Los permisos de campo se heredan del tipo de registro, cuando se conceden permisos al espacio de trabajo y al tipo de registro.

Los siguientes permisos hacen referencia a los propios campos y no a los valores asociados a cada campo. Para editar valores de campo, debe tener permisos para editar registros.

|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Editar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |


### Permisos para vistas

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
