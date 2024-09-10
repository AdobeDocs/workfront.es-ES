---
user-type: administrator
product-area: system-administration;user-management
keywords: administrar, agrupar, editar,
navigation-topic: create-and-manage-groups
title: Administrar un grupo
description: Como administrador de grupo, puede administrar un grupo que administre desde el área Grupos de la Configuración. Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 0%

---

# Administrar un grupo

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

Como administrador de grupo, puede administrar un grupo que administre desde el área Grupos de la Configuración. Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>Cuando se le asigne como administrador de un grupo, heredará la función de administrador de grupos de los subgrupos que estén debajo de él. Los únicos usuarios que pueden administrar un subgrupo son los administradores de grupo del grupo superior y los administradores de grupo asignados al subgrupo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Administrar las pertenencias de un grupo

Puede agregar y quitar usuarios y otros grupos de un grupo que administre. También puede asignar miembros del grupo como administradores del grupo y administrar la información de perfil de usuario de los miembros del grupo.

Para obtener instrucciones, vea [Ver y administrar las pertenencias de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Administrar los detalles de un grupo

Puede ver y editar la página Detalles del grupo para un grupo o subgrupo que administre. Esta página incluye una descripción del grupo, los nombres del coordinador empresarial y de los administradores del grupo, así como una opción que permite hacer que el grupo y todos sus subgrupos sean públicos o privados. Además, si su nivel de acceso le permite administrar formularios personalizados, puede adjuntar un formulario personalizado a un grupo.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Para obtener instrucciones, vea [Ver y administrar los detalles de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Editar, copiar o eliminar un grupo

Sin salir de la página principal de un grupo que esté viendo, puede editar, copiar o eliminar rápidamente el grupo.

{{step-1-to-setup}}

1. Haga clic en **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Seleccione el grupo y haga clic en el icono Editar ![](assets/edit-icon.png), Copiar ![](assets/copy-icon.png) o Eliminar ![](assets/delete.png).

   Si necesita información sobre el uso del cuadro que aparece, vea una de las siguientes opciones:

   * **Editar**: [Ver y administrar los detalles de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Copiar**: [Cree un grupo de nivel superior copiando un grupo o subgrupo existente](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) en el artículo [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Eliminar**: [Eliminar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Configurar las preferencias de proyecto, tarea y problema de un grupo

Si usted es administrador de un grupo y el grupo necesita una configuración de preferencias de proyecto, tarea y problema diferente de las establecidas en el sistema, puede pedirle al administrador de Workfront que desbloquee una preferencia para todos los grupos de la organización. Una vez desbloqueado, usted (y los administradores de grupos de todos los demás grupos) pueden configurarlo para los grupos que administre.

Para obtener instrucciones, vea [Configurar las preferencias del proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Configurar las preferencias de tareas y problemas para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Enumeración, adición y configuración de subgrupos

Puede crear, ver, editar, copiar, cambiar el nombre, exportar y eliminar subgrupos debajo de un grupo que administre.

## Configuración de notificaciones de eventos para un grupo

Si un administrador de Workfront desbloquea la capacidad de configurar notificaciones de eventos para los grupos de su organización, puede configurarlas para un grupo que administre. Para obtener instrucciones, vea [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Creación y personalización de estados de un grupo

Como administrador de grupo, puede crear estados personalizados para un grupo de nivel superior que administre. Esto proporciona a su grupo autonomía y ayuda a eliminar la necesidad de decenas de estados personalizados en toda la compañía. (Un administrador de Workfront también puede hacer esto, para cualquier grupo).

También puede personalizar los estados del sistema para un grupo de nivel superior si un administrador de Workfront los ha configurado para permitir la personalización.

Para obtener instrucciones, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Trabajar con proyectos de un grupo

En el área Grupos de la configuración, cuando visualice la página principal de un grupo que administre, puede realizar las siguientes acciones con los proyectos:

* Enumere y trabaje con (edite, copie, elimine y exporte) los proyectos asociados con el grupo y sus subgrupos y que se han compartido con usted
* Cree un nuevo proyecto para el grupo

Para obtener instrucciones, vea [Crear y modificar proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Ver y administrar los procesos de aprobación de un grupo

Cuando visualiza un grupo que administra en el área de Grupos, puede ver y trabajar con los procesos de aprobación para los que los administradores del grupo o uno de sus subgrupos tienen acceso administrativo.

Para obtener instrucciones, consulte [Procesos de aprobación de nivel de grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Ver y administrar las plantillas de diseño de un grupo

Cuando visualiza un grupo que administra en el área de Grupos, puede ver y trabajar con la plantilla de diseño para la que los administradores del grupo o uno de sus subgrupos tienen acceso administrativo.

Para obtener instrucciones, consulte [Crear y modificar plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Ver y administrar las programaciones de los miembros del grupo

Un administrador de grupo que crea una programación para un grupo debe especificar el grupo cuyos administradores administrarán la programación. Normalmente, este es el grupo para el que se crea la programación, pero podría ser un grupo diferente si el administrador del grupo administra varios grupos y especifica uno de los demás en su lugar.

Cuando visualice la página principal de un grupo que administre, si el grupo está designado como aquel cuyos administradores pueden editar una programación, puede ver y administrar la programación desde la página del grupo.

Para obtener instrucciones, consulte [Crear y modificar las programaciones de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Ver y administrar los perfiles de hoja de horas de los miembros del grupo

Cuando visualice la página principal de un grupo que administre, puede administrar los perfiles de plantilla de horas para los que usted y los demás administradores del grupo (o uno de sus subgrupos) tengan permiso de edición. Para obtener instrucciones, consulte [Crear y administrar perfiles de hojas de horas de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Ver y administrar los miembros del subgrupo de un grupo

Cuando está viendo la página principal de un grupo que administra, puede ver y administrar todos los usuarios de los subgrupos del grupo. Para obtener instrucciones, vea [Ver y administrar miembros de subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Ver y administrar los equipos de un grupo

Cuando visualice un grupo que administre en el área de Grupos, podrá visualizar y trabajar con equipos asociados al grupo o a cualquiera de sus subgrupos.

Para obtener instrucciones, vea [Crear y modificar los equipos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Ver y administrar las compañías de un grupo

Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con empresas asociadas al grupo o a cualquiera de sus subgrupos. Para obtener instrucciones, vea [Crear y modificar las compañías de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Ver y administrar los portafolios y programas de un grupo

Cuando está viendo un grupo que administra en el área de Grupos, puede ver y trabajar con portafolios y programas cuando se cumplan las dos condiciones siguientes:

* Están asociados al grupo que está viendo o a cualquiera de sus subgrupos
* Tiene permisos para verlos porque los creó o porque se compartieron con usted

Para obtener instrucciones, vea [Crear y modificar los proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) y [Crear, modificar y ver los programas de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Desactivar o reactivar un grupo

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

Puede mantener un grupo en su estado activo predeterminado o desactivarlo.

La desactivación de un grupo puede ser útil cuando no está en uso actualmente porque los usuarios ya no lo ven en los campos de escritura anticipada cuando buscan un grupo que desean asociar con otro objeto.

Para obtener instrucciones sobre cómo hacer que un grupo sea inactivo o activo, consulte [Desactivar o reactivar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
