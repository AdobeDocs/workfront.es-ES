---
title: Información general sobre los permisos de uso compartido en Adobe Workfront Planning
description: No todos los usuarios de la organización tienen el mismo acceso y permisos para utilizar Adobe Workfront Planning. Este artículo contiene información general sobre cómo compartir o quitar permisos en un espacio de trabajo o vista de Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/eF7kBTsursbrsXr8Lo6ql6U5JBLQDvi6nw4JDpRxClw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: d45d85aecbcdabf2c02c347b80c7ee56b97efff0
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 7%
---
<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Información general sobre los permisos de uso compartido en Planificación de Workfront de Adobe


<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después del lanzamiento en Vista previa, las mismas funciones también están disponibles mensualmente en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Puede compartir o quitar permisos en un espacio de trabajo de Adobe Workfront Planning, un tipo de registro o una vista.

También puede compartir formularios de solicitud de Planning. Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

En este artículo se describen los niveles de permisos para espacios de trabajo de Workfront Planning, los tipos de registros, los registros, los campos y las vistas.

## Objetos que se pueden compartir en Adobe Workfront Planning

Puede compartir manualmente algunos objetos de Workfront Planning, mientras que otros objetos heredan estos permisos de otros objetos.

Puede compartir manualmente los siguientes objetos en Workfront Planning:

* Espacios de trabajo

  * Puede compartir espacios de trabajo dentro de su organización con usuarios, grupos, equipos, empresas y roles.
  * Al compartir un espacio de trabajo, también se comparten todos los tipos de registros, registros y campos asociados a los espacios de trabajo.
  * Al compartir un espacio de trabajo, las vistas no se comparten. Las vistas se comparten por separado.

  Para obtener más información, vea [Compartir espacios de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

* Tipos de registro

  * Puede compartir tipos de registros dentro de su organización, con usuarios, grupos, equipos, empresas y roles.
  * El nivel de permisos otorgados para el espacio de trabajo se muestra como Permisos heredados para el tipo de registro.
  * No se puede compartir un tipo de registro con un nivel de permisos superior al que el usuario tiene en el área de trabajo.

  Para obtener más información, vea [Compartir tipos de registros](/help/quicksilver/planning/access/share-record-types.md).

* Registros

  * Puede compartir registros con personas de su organización, con usuarios, grupos, equipos, empresas y funciones del puesto.
  * Los usuarios heredan los permisos del espacio de trabajo y del tipo de registro de forma predeterminada.
  * No se puede compartir un registro con un nivel de permisos superior o inferior al que el usuario tiene en el tipo de registro.

  Para obtener más información, consulte [Compartir registros](/help/quicksilver/planning/access/share-records.md).

<!--
* Fields

    * In the Production environment, field permissions are inherited from record types. 

    * Field permissions grant access to field values, and not to field settings. 
    * You must have both permissions to a record and to a field to see the values of that field for a record. 

    <div class="preview">

    * In the Preview environment, consider the following: 

        * You can share fields inside your organization, with users, groups, teams, companies, and job roles. 
        * Access to a field comes from combining the following settings:

            * **Inherited permissions**: By default, a field inherits the same access someone has on the record type. You can turn off Inherited permissions and give users a lower access to the field than they have for the record type. 
            * The **Everyone with access to the record type can view** or **Only invited people can access** selection. You can either allow everyone with permissions to the workspace to view the field or give permissions only to individual entities. 
    
    For more information, see [Share fields](/help/quicksilver/planning/access/share-fields.md). 

    </div>
-->

* Vistas

  * Debe conceder a los usuarios, incluidos los administradores del sistema, permisos para acceder a las vistas por separado de sus permisos para acceder a espacios de trabajo.
  * Al compartir una vista, se comparten todos los elementos de la vista, incluidos los filtros, la agrupación, el orden o la configuración.
  * Al compartir una vista, los registros visibles en la vista no se comparten. Los registros deben compartirse compartiendo espacios de trabajo.
  * Puede compartir una vista públicamente, con personas fuera de su organización, cuando genere un vínculo público para una vista. Las personas que acceden a la página de registros desde un vínculo público pueden ver todos los registros y sus campos, incluidos los registros y campos conectados.

  Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).


## Consideraciones sobre el uso compartido de objetos en Adobe Workfront Planning

* El tipo de licencia de Adobe Workfront funciona junto con los permisos de Workfront Planning para permitirle acceder para ver, contribuir o administrar espacios de trabajo y sus objetos.

  Para obtener información acerca de cómo afectan los tipos de licencia a los niveles de permisos de Workfront Planning, vea [Descripción general del tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Los administradores del sistema pueden administrar todos los espacios de trabajo del sistema, incluidos los que no crearon.
* Otros usuarios, incluidos los administradores del sistema, solo pueden acceder a las vistas que han creado o que se han compartido con ellos. A los administradores del sistema solo se les pueden otorgar permisos para administrar una vista.

* Cuando comparte espacios de trabajo y tipos de registros con otros usuarios, el nivel de permiso del tipo de registro se hereda automáticamente a los registros y campos asociados a ellos de forma predeterminada.

* Puede compartir objetos de Planning de las siguientes maneras:

  * Internamente, puede compartir objetos de Workfront Planning con las siguientes entidades de Workfront:

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

<!--
<span class="permissions">In addition to the permissions described in the above table, you can also change the owner of a workspace when sharing it. For information, see [Share workspaces](/help/quicksilver/planning/access/share-workspaces.md).</span>
-->

### Permisos para tipos de registros

<!--
 old access:
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

Los permisos de registro se heredan del tipo de registro, cuando se conceden permisos al espacio de trabajo y al tipo de registro, de forma predeterminada.

<!--
In the Production environment, the following are the levels of permissions for records: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |     ✓       |       |
| Delete | ✓      |     ✓       |       |
| Edit   | ✓      |    ✓        |       |
| View   | ✓      | ✓          | ✓     |
-->

Los siguientes son niveles de permisos para registros:

|        | Administrar | Ver |
|--------|--------|-------|
| Crear | ✓ |       |
| Eliminar | ✓ |       |
| Editar | ✓ |       |
| Ver | ✓ | ✓ |

Los permisos de registro siempre se heredan cuando se conceden permisos al espacio de trabajo y al tipo de registro.

Puede quitar los permisos heredados del registro recibidos del tipo de registro. Los administradores de Workspace y los creadores de registros conservan los permisos de administración del registro.

No puede conceder a los usuarios permisos inferiores o superiores en el registro a los que tienen en el tipo de registro.

Se dan los siguientes escenarios:

| Permisos de tipo de registro y Workspace | Permisos heredados automáticos para un registro | Posibles permisos de Registro cuando los permisos heredados están desactivados (se conceden manualmente) |
|--------|--------|-------------|
| Administrar | Administrar | Administración, eliminación de permisos* |
| Aportar | Administrar | Administración, eliminación de permisos* |
| Ver | Ver | Ver, quitar permisos* |

>[!NOTE]
>
>*Cuando se quitan permisos de un registro, los usuarios conservan los permisos de Vista en el espacio de trabajo y el tipo de registro, a menos que se quiten sus permisos del espacio de trabajo.

### Permisos para registrar campos


#### Permisos para registrar campos en el entorno de producción


Los permisos para editar la configuración de campo se heredan del tipo de registro, cuando se conceden permisos al espacio de trabajo y al tipo de registro.

Los siguientes permisos hacen referencia a la configuración de los campos y no a los valores asociados a cada campo. Para editar valores de campo, debe tener permisos para editar registros.

|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Editar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |


<div class="preview">

#### Permisos para registrar campos en el entorno de vista previa

Los permisos para la configuración de campos se heredan del tipo de registro, cuando se conceden permisos al espacio de trabajo y al tipo de registro.

Los siguientes permisos hacen referencia a la configuración de los campos y no a los valores asociados a cada campo.

|        | Administrar | Aportar | Ver |
|--------|--------|------------|-------|
| Crear | ✓ |            |       |
| Eliminar | ✓ |            |       |
| Editar | ✓ |            |       |
| Ver | ✓ | ✓ | ✓ |


Los permisos para los valores de campo se heredan del tipo de registro y funcionan junto con los permisos para los registros.

Puede administrar permisos para los valores de campos individuales y restringir los campos que puedan contener información confidencial.

Puede conceder los siguientes permisos a los valores de campo compartiendo un campo:

|        | Administrar | Ver |
|--------|--------|------|
| Eliminar | ✓ |      |
| Editar | ✓ |      |
| Ver | ✓ | ✓ |

Los usuarios deben tener al menos permisos de visualización en el tipo de registro para acceder a los campos.

</div>

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

>[!NOTE]
>
>*Los usuarios deben tener permisos de Vista o superiores en un espacio de trabajo para obtener este acceso de vista.


<!--
old view permissions, before sharing View permissions to a view through a workspace:
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
