---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Desactivar o reactivar un grupo
description: Puede desactivar un grupo que administra y que ya no utilice.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Desactivar o reactivar un grupo

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

Puede desactivar un grupo que administra y que ya no utilice.

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

## Desactivar o reactivar un grupo

>[!IMPORTANT]
>
>Al desactivar un grupo, también se desactivan los subgrupos que se encuentran debajo.
>
>Si necesita reactivar uno de ellos, puede hacerlo después de realizar una de las siguientes acciones:
>
>* Eliminarla de su grupo principal. Para obtener más información, consulte la sección [Quitar un subgrupo de su grupo principal y convertirlo en un grupo de nivel superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) en el artículo [Administrar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Muévalo bajo un grupo activo. Para obtener más información, consulte la sección [Crear, mover, ver, editar, copiar, cambiar el nombre, exportar o eliminar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) en el artículo [Administrar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, seleccione **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra junto con los subgrupos que tienen. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo para abrir su página.

1. Haga clic en el menú Más ![](assets/more-icon.png) junto al nombre del grupo y, a continuación, haga clic en **Desactivar** o **Reactivar**.

   >[!NOTE]
   >
   >La opción Está activo (opción Reactivar en Vista previa) no está disponible si el grupo es un subgrupo de un grupo desactivado. Para poder reactivarlo, debe eliminarlo de su grupo principal o moverlo a un grupo que esté activo, tal como se describe en la nota importante anterior.

1. (Condicional) Si está desactivando el grupo, haga clic en **Desactivar** en el **Desactivar grupo** que se muestra.

## Consideraciones para grupos inactivos

Tenga en cuenta lo siguiente sobre un grupo que desactive desactivando la opción Está activo en la sección [Desactivar o reactivar un grupo](#View) en este artículo.

* Al desactivar un grupo, también se desactivan todos los subgrupos que se encuentran debajo de él. Esto incluye subgrupos que se agregan después de desactivarlos.

   Para obtener información sobre cómo reactivar un subgrupo en esta situación, consulte [Acerca de la reactivación de un subgrupo debajo de un grupo principal inactivo](#about-reactivating-a-subgroup-below-an-inactive-parent-group) en este artículo.

* Cuando vaya al área Grupos en Configuración, solo verá los grupos activos en la lista porque Activo es el filtro predeterminado ![](assets/filter-nwepng.png) para ello. Si desea ver todos los grupos que administra, incluidos los inactivos, puede utilizar el filtro Todos . O utilice el filtro Inactivo para enumerar solo los inactivos.

   Para obtener más información sobre los filtros de las listas, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Desactivar un grupo no cambia lo siguiente:

   * Las asociaciones del grupo con objetos. Los objetos asociados siguen funcionando como antes, sin ningún cambio.

      Por ejemplo, si un proyecto está asociado con un grupo que desactive, el proyecto seguirá utilizando las preferencias y estados del grupo sin ningún cambio.

   * La capacidad de crear un nuevo objeto, como una aprobación, un equipo o una empresa, desde la página del grupo en la configuración. De forma predeterminada, el nuevo objeto está asociado al grupo inactivo.
   * Su capacidad, como administrador, para encontrar el grupo en filtros e informes.

      También puede encontrarlo en los campos de avance de tipo de grupo donde puede que desee administrar la configuración del grupo en el área Configuración . Esto incluye las áreas Preferencias, Notificaciones de eventos y Licencias del sistema.

      Por ejemplo, si va a Configuración > Preferencia de proyecto > Proyectos y borra el campo de avance de tipo encima de las opciones, todavía puede encontrar un grupo inactivo y configurar sus preferencias de proyecto.

## Acerca de la reactivación de un subgrupo debajo de un grupo principal inactivo {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Al desactivar un grupo, también se desactivan todos los subgrupos que se encuentran debajo de él. Si necesita reactivar uno de los subgrupos en un grupo inactivo, puede hacer una de las dos cosas:

* Mueva el subgrupo debajo de un grupo activo. A continuación, active la opción Es activo para el grupo movido, tal como se explica en la sección [Desactivar o reactivar un grupo](#View) en este artículo.

   Para obtener instrucciones sobre cómo mover un grupo, consulte [Mover un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Elimine el subgrupo de su grupo principal (lo que convierte al subgrupo en un grupo de nivel superior). A continuación, active la opción Es activo para el grupo movido, tal como se explica en la sección [Desactivar o reactivar un grupo](#View) en este artículo.

   Para obtener instrucciones sobre cómo quitar un subgrupo de su grupo principal, consulte la sección [Quitar un subgrupo de su grupo principal y convertirlo en un grupo de nivel superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) en el artículo [Administrar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
