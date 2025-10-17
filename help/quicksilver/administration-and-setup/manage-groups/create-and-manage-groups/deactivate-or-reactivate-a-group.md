---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Desactivar o reactivar un grupo
description: Puede desactivar un grupo que administre y que ya no utilice.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 91%

---

# Desactivar o reactivar un grupo

Puede desactivar un grupo que administre y que ya no utilice.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desactivar o reactivar un grupo

>[!IMPORTANT]
>
>Al desactivar un grupo, también se desactivan los subgrupos que estén por debajo de él.
>
>Si necesita reactivar alguno, puede hacerlo después de realizar una de las siguientes acciones:
>
>* Elimínelo de su grupo principal. Para obtener más información, consulte la sección [Quitar un subgrupo de su grupo principal y convertirlo en un grupo de nivel superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) en el artículo [Administrar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Muévalo a un grupo activo. Para obtener más información, consulte la sección [Crear, mover, ver, editar, copiar, cambiar el nombre, exportar o eliminar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) en el artículo [Administrar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

{{step-1-to-setup}}

1. En el panel izquierdo, seleccione **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo para abrir su página.

1. Haga clic en el menú Más ![Más icono](assets/more-icon.png) junto al nombre del grupo y, a continuación, haga clic en **Desactivar** o **Reactivar**.

   >[!NOTE]
   >
   >La opción Está activo (opción Reactivar en Vista previa) no está disponible si el grupo es un subgrupo de un grupo desactivado. Antes de poder reactivarlo, debe eliminarlo de su grupo principal o moverlo a un grupo que esté activo, tal como se describe en la nota importante anterior.

1. (Condicional) Si está desactivando el grupo, haga clic en **Desactivar** en el cuadro **Desactivar grupo** que aparece.

## Consideraciones para grupos inactivos

Tenga en cuenta lo siguiente en relación con un grupo que desactive deshabilitando la opción Está activo, como se explica en la sección [Desactivar o reactivar un grupo](#View) de este artículo.

* Al desactivar un grupo también se desactivan todos los subgrupos por debajo de él. Esto incluye los subgrupos que se añaden después de desactivarlos.

  Para obtener información sobre cómo reactivar un subgrupo en esta situación, consulte [Acerca de la reactivación de un subgrupo debajo de un grupo principal inactivo](#about-reactivating-a-subgroup-below-an-inactive-parent-group) en este artículo.

* Cuando vaya al área de Grupos en Configuración, solo verá los grupos activos en la lista, ya que Activo es el filtro predeterminado ![Icono de filtro](assets/filter-nwepng.png) para él. Si desea ver todos los grupos que administra, incluidos los inactivos, puede utilizar el filtro Todos. O bien, utilice el filtro Inactivo para enumerar solo los inactivos.

  Para obtener más información sobre los filtros de las listas, consulte [Información general sobre los filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* La desactivación de un grupo no cambia lo siguiente:

   * Asociaciones del grupo a objetos. Los objetos asociados siguen funcionando como antes, sin ningún cambio.

     Por ejemplo, si un proyecto está asociado con un grupo que usted desactiva, el proyecto continúa utilizando las preferencias y los estados del grupo sin ningún cambio.

   * Su capacidad para crear un nuevo objeto, como una aprobación, un equipo o una compañía, desde la página del grupo en la configuración. De forma predeterminada, el nuevo objeto está asociado al grupo inactivo.
   * Su capacidad, como administrador, para encontrar el grupo en filtros y la creación de informes.

     También puede encontrarlo en los campos de escritura anticipada de grupo en los que puede que desee administrar la configuración del grupo en el área de Configuración. Esto incluye las áreas Preferencias, Notificaciones de eventos y Licencias del sistema.

     Por ejemplo, si va a Configuración > Preferencia del proyecto > Proyectos y borra el campo de escritura anticipada situado encima de las opciones, aún puede encontrar un grupo inactivo y configurar sus preferencias de proyecto.

## Acerca de la reactivación de un subgrupo debajo de un grupo principal inactivo {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Al desactivar un grupo también se desactivan todos los subgrupos por debajo de él. Si necesita reactivar uno de los subgrupos en un grupo inactivo, puede hacer una de las dos cosas:

* Desplace el subgrupo bajo un grupo activo. A continuación, habilite la opción Está activo para el grupo desplazado, como se explica en la sección [Desactivar o reactivar un grupo](#View) de este artículo.

  Para obtener instrucciones sobre cómo mover un grupo, consulte [Mover un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Elimine el subgrupo de su grupo principal (lo que lo convierte en un grupo de nivel superior). A continuación, habilite la opción Está activo para el grupo desplazado, como se explica en la sección [Desactivar o reactivar un grupo](#View) de este artículo.

  Para obtener instrucciones sobre cómo quitar un subgrupo de su grupo principal, consulte la sección [Quitar un subgrupo de su grupo principal y convertirlo en un grupo de nivel superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) en el artículo [Administrar un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
