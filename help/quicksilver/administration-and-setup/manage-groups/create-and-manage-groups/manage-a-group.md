---
user-type: administrator
product-area: system-administration;user-management
keywords: administrar,agrupar,editar,
navigation-topic: create-and-manage-groups
title: Administrar un grupo
description: Como administrador de grupos, puede administrar un grupo que administre desde el área Grupos de Configuración. Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# Administrar un grupo

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

Como administrador de grupos, puede administrar un grupo que administre desde el área Grupos de Configuración. Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>Cuando se le asigna como administrador de un grupo, hereda la función de administrador de grupo para cualquier subgrupo que se encuentre debajo de ella. Los únicos usuarios que pueden administrar un subgrupo son los administradores de grupo para el grupo superior encima y los administradores de grupo asignados al subgrupo.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o administrador de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Administrar las suscripciones de un grupo

Puede agregar y eliminar usuarios y otros grupos de un grupo que administre. También puede asignar miembros del grupo como administradores para el grupo y administrar la información de perfil de usuario de los miembros del grupo.

Para obtener instrucciones, consulte [Ver y administrar las suscripciones de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Administrar los detalles de un grupo

Puede ver y editar la página Detalles del grupo para un grupo o subgrupo que administra. Esta página incluye una descripción del grupo, los nombres del líder empresarial y los administradores de grupos, y una opción que permite hacer que el grupo y todos sus subgrupos sean públicos o privados. Además, si el nivel de acceso le permite administrar formularios personalizados, puede adjuntar un formulario personalizado a un grupo.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Para obtener instrucciones, consulte [Ver y administrar los detalles de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Editar, copiar o eliminar un grupo

Sin salir de la página principal de un grupo que esté viendo, puede editar, copiar o eliminar rápidamente

<!--
DRAFTED IN FLARE:
or deactivate

-->

el grupo.

<!--
DRAFTED IN FLARE:
Make this change when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra junto con los subgrupos que tienen. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Seleccione el grupo y haga clic en Editar ![](assets/edit-icon.png), Copiar ![](assets/copy-icon.png)o Eliminar ![](assets/delete.png) icono.

   Si necesita información sobre el uso del cuadro que aparece, consulte una de las siguientes opciones:

   * **Editar**: [Ver y administrar los detalles de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Copiar**: [Crear un grupo de nivel superior copiando un grupo o subgrupo existente](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) en el artículo [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Eliminar**: [Eliminar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Configuración de las preferencias de proyecto, tarea y problema para un grupo

Si es un administrador de grupos y su grupo necesita diferentes configuraciones de proyecto, tarea y preferencia de publicación de las que están establecidas a nivel de sistema, puede solicitar al administrador de Workfront que desbloquee una preferencia para todos los grupos de la organización. Una vez desbloqueado, usted (y los administradores de grupo de todos los demás grupos) pueden configurarlo para los grupos que administra.

Para obtener instrucciones, consulte [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y  [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Enumerar, agregar y configurar subgrupos

Puede crear, ver, editar, copiar, cambiar el nombre, exportar y eliminar subgrupos debajo de un grupo que administre.

## Configuración de notificaciones de eventos para un grupo

Si un administrador de Workfront desbloquea la capacidad de configurar notificaciones de eventos para los grupos de su organización, puede configurarlas para un grupo que administre. Para obtener instrucciones, consulte [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Crear y personalizar estados para un grupo

Como administrador de grupos, puede crear estados personalizados para un grupo de nivel superior que administre. Esto le da autonomía a su grupo y le ayuda a eliminar la necesidad de docenas de estados personalizados a nivel de empresa. (Un administrador de Workfront también puede hacerlo, para cualquier grupo).

También puede personalizar los estados del sistema para un grupo de nivel superior si un administrador de Workfront los ha configurado para permitir la personalización.

Para obtener instrucciones, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Trabajar con los proyectos de un grupo

En el área Grupos de Configuración, cuando esté viendo la página principal de un grupo que administre, puede hacer lo siguiente con los proyectos:

* Enumerar y trabajar con (editar, copiar, eliminar y exportar) los proyectos asociados al grupo y sus subgrupos y que se han compartido con usted
* Crear un nuevo proyecto para el grupo

Para obtener instrucciones, consulte [Creación y modificación de los proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Ver y administrar los procesos de aprobación de un grupo

Cuando visualiza un grupo que administra en el área Grupos , puede ver y trabajar con los procesos de aprobación para los que los administradores del grupo, o uno de sus subgrupos, tienen acceso administrativo.

Para obtener instrucciones, consulte [Procesos de aprobación a nivel de grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Ver y administrar las plantillas de diseño de un grupo

Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con la plantilla Diseño para el cual los administradores del grupo, o uno de sus subgrupos, tienen acceso administrativo.

Para obtener instrucciones, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Ver y administrar las programaciones de los miembros del grupo

Un administrador de grupo que crea una programación para un grupo debe especificar el grupo cuyos administradores administrarán la programación. Normalmente, este es el grupo para el que se está creando la programación, pero podría ser un grupo diferente si el administrador del grupo administra varios grupos y especifica uno de los demás en su lugar.

Cuando visualiza la página principal de un grupo que administra, si el grupo está designado como el grupo cuyos administradores pueden editar una programación, puede ver y administrar la programación desde la página del grupo.

Para obtener instrucciones, consulte [Crear y modificar las programaciones de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Ver y administrar los perfiles de parte de horas de los miembros del grupo

Cuando está viendo la página principal de un grupo que administra, puede administrar los perfiles de parte de horas que usted y los demás administradores del grupo (o uno de sus subgrupos) tienen permiso para editar. Para obtener instrucciones, consulte [Creación y administración de perfiles de hojas de horas de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Ver y administrar los miembros del subgrupo de un grupo

Cuando está viendo la página principal de un grupo que administra, puede ver y administrar todos los usuarios de los subgrupos del grupo. Para obtener instrucciones, consulte [Ver y administrar miembros de subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Ver y administrar los equipos de un grupo

Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con equipos asociados al grupo o a cualquiera de sus subgrupos.

Para obtener instrucciones, consulte [Crear y modificar los equipos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Ver y administrar las empresas de un grupo

Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con empresas asociadas con el grupo o con cualquiera de sus subgrupos. Para obtener instrucciones, consulte [Crear y modificar las empresas de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Ver y administrar las carteras y los programas de un grupo

Cuando visualiza un grupo que administra en el área Grupos , puede ver y trabajar con portafolios y programas cuando ambos sean verdaderos:

* Están asociados al grupo que está viendo o a cualquiera de sus subgrupos
* Tiene permisos para verlos porque los creó o se compartieron con usted

Para obtener instrucciones, consulte [Creación y modificación de los proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) y [Crear, modificar y ver los programas de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Desactivar o reactivar un grupo

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

Puede mantener un grupo en su estado activo predeterminado o desactivarlo.

Desactivar un grupo puede resultar útil cuando no se está utilizando actualmente porque los usuarios ya no lo ven en los campos de tipo anterior cuando buscan un grupo que desean asociar con otro objeto.

Para obtener instrucciones sobre cómo hacer que un grupo sea inactivo o activo, consulte [Desactivar o reactivar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
