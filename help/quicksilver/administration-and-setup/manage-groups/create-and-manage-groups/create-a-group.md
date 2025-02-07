---
user-type: administrator
product-area: system-administration;user-management
keywords: crear,grupo,subgrupo,nuevo
navigation-topic: create-and-manage-groups
title: Crear un grupo
description: Como administrador de Adobe Workfront, puede crear grupos para organizar usuarios y proyectos y asignar derechos de acceso dentro de Workfront.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1656'
ht-degree: 91%

---

# Crear un grupo

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Como administrador de Adobe Workfront, puede crear grupos para organizar usuarios y proyectos y asignar derechos de acceso dentro de Workfront. Para obtener más información, consulte [Información general sobre los grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Cada subgrupo necesita al menos un administrador de grupo. Los administradores de grupos pueden utilizar la página Grupos para administrar sus grupos en un solo lugar.

Si es administrador de un grupo o de Workfront, también puede crear subgrupos en un grupo. Para obtener instrucciones, consulte [Crear un subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear un grupo de nivel superior desde cero

Estos pasos explican cómo crear un nuevo grupo desde cero. Para obtener información acerca de cómo crear un grupo o subgrupo copiando uno existente, consulte [Crear un grupo de nivel superior copiando un grupo o subgrupo existente](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) en este artículo.

Debe ser administrador de Workfront para crear un grupo de nivel superior.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

1. Sobre la lista de grupos, haga clic en **Nuevo grupo**.

   >[!TIP]
   >
   >En la parte inferior de la lista de grupos, también puede hacer clic en **Añadir más grupos** para añadir un grupo en línea y, a continuación, hacer clic en **Intro** cuando termine de añadir la información del grupo.

1. En el cuadro **Nuevo grupo** que aparece, escriba un nombre para el grupo.
1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de grupo</td> 
      <td>Cambie el nombre del grupo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción para el grupo. Puede escribir hasta 512 caracteres.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activo</td> 
      <td> <p>(Habilitado de forma predeterminada) Activa el grupo en la instancia de Workfront.</p> <p>En campos de escritura anticipada como el que se muestra a continuación, cuando los usuarios normales buscan un grupo para adjuntarlo a un objeto o compartirlo, solo aparecen en la lista los grupos activos.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para facilitar esta tarea a los usuarios, puede deshabilitar la opción Está activo para los grupos que no se estén utilizando en ese momento.</p> <p>Puede ver, filtrar y agrupar fácilmente la lista Grupos en función del estado activo o inactivo mediante este campo. Para obtener información acerca del uso de vistas, filtros y agrupaciones en listas, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos para la creación de informes: filtros, vistas y agrupaciones</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Convertir este grupo y sus subgrupos en públicos</td> 
      <td> <p>(Disponible únicamente si visualiza los detalles de un grupo de nivel superior, no de un subgrupo). Active esta opción para permitir que los usuarios del grupo con acceso de edición de usuario (que no sean administradores del grupo) agreguen este grupo y sus subgrupos al perfil de usuario de otros usuarios.</p> <p>En el caso de los grupos públicos, cualquier usuario (dentro o fuera del grupo) que tenga acceso de usuario de edición puede añadir el grupo al perfil de otros usuarios. No pueden hacerlo para un grupo privado.</p> <p>Solo puede editar esta opción en el grupo principal superior de una jerarquía de grupos que tenga más de un nivel. Todos los subgrupos del grupo principal heredan su configuración.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>No puede hacer público un subgrupo por sí solo, pero puede hacer público su grupo principal de nivel superior, que también hace públicos todos los subgrupos del grupo principal.</li> 
         <li>Un subgrupo que pertenece a un grupo público es público de forma predeterminada, por lo que cualquier usuario con acceso de edición de usuarios también puede añadir el subgrupo a otros usuarios.</li> 
        </ul> </p> <p>Si necesita información sobre el acceso necesario para editar usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>. Para obtener información la edición de usuarios, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar el perfil de un usuario</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coordinador empresarial </td> 
      <td> <p>Puede asignar un usuario como coordinador empresarial a un grupo que administre. Un líder empresarial es alguien que toma decisiones comerciales para el grupo. Para más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Información general sobre el Coordinador empresarial</a><span>.</span></p> <p>Si la persona aún no es miembro del grupo, al añadir su nombre a este campo también se añade al grupo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Para poder quitar el coordinador empresarial de un grupo, debe quitar su nombre del campo Coordinador empresarial.</li> 
         <li>Si quita el nombre del campo Coordinador empresarial, ese usuario seguirá siendo miembro del grupo a menos que lo quite de él. Para obtener instrucciones sobre cómo quitar a alguien de un grupo, consulte la sección <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Administrar las pertenencias a un grupo</a> en el artículo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Administrar un grupo</a>.</li> 
        </ul> </p> <p>Para más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Información general sobre el Coordinador empresarial</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Miembros y administradores de grupo</td> 
      <td>
        <p>Para añadir miembros al grupo, empiece a escribir el nombre de un usuario o grupo existente que desee añadir y, a continuación, seleccione el nombre cuando aparezca.</p> 
        <p>Los usuarios y grupos que añada tendrán acceso a todos los objetos compartidos con el grupo.</p>
        <p>Un grupo de nivel superior debe tener al menos un administrador de grupos. </p>
     </tr> 
     <tr> 
      <td role="rowheader">Buscar personas y grupos en la lista</td> 
      <td> Si necesita encontrar un usuario o grupo ya asignado a este grupo, puede escribir su nombre aquí y seleccionarlo cuando aparezca.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Crear grupo**.

## Crear un grupo de nivel superior copiando un grupo o subgrupo existente {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Como administrador de Workfront, puede crear un nuevo grupo de nivel superior copiando un grupo o subgrupo existente.

Tenga en cuenta lo siguiente cuando desee hacer esto:

* Todos los miembros y los subgrupos que pertenezcan al grupo existente se copiarán en el nuevo grupo de nivel superior.
* Los miembros del grupo copiado conservan las asignaciones que tenían en el grupo original. Por lo tanto, los administradores de grupo del grupo original también se designan como administradores de grupo en el grupo copiado.

Para crear un nuevo grupo de nivel superior copiando un grupo o subgrupo:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![grupos](assets/groups-icon.png).

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Seleccione el grupo que desee copiar y luego haga clic en el icono Copiar ![Icono Copiar](assets/copy-icon.png).
1. En el cuadro **Copiar grupo** que aparece, escriba un **Nombre de grupo** para el grupo copiado.

1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre de grupo</td> 
      <td>Cambie el nombre del grupo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba una descripción para el grupo. Puede escribir hasta 512 caracteres.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activo</td> 
      <td> <p>(Habilitado de forma predeterminada) Activa el grupo en la instancia de Workfront.</p> <p>En campos de escritura anticipada como el que se muestra a continuación, cuando los usuarios normales buscan un grupo para adjuntarlo a un objeto o compartirlo, solo aparecen en la lista los grupos activos.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para facilitar esta tarea a los usuarios, puede deshabilitar la opción Está activo para los grupos que no se estén utilizando en ese momento.</p> <p>Puede ver, filtrar y agrupar fácilmente la lista Grupos en función del estado activo o inactivo mediante este campo. Para obtener información acerca del uso de vistas, filtros y agrupaciones en listas, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementos para la creación de informes: filtros, vistas y agrupaciones</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Convertir este grupo y sus subgrupos en públicos</td> 
      <td> <p>(Disponible únicamente si visualiza los detalles de un grupo de nivel superior, no de un subgrupo). Active esta opción para permitir que los usuarios del grupo con acceso de edición de usuario (que no sean administradores del grupo) agreguen este grupo y sus subgrupos al perfil de usuario de otros usuarios.</p> <p>En el caso de los grupos públicos, cualquier usuario (dentro o fuera del grupo) que tenga acceso de usuario de edición puede añadir el grupo al perfil de otros usuarios. No pueden hacerlo para un grupo privado.</p> <p>Solo puede editar esta opción en el grupo principal superior de una jerarquía de grupos que tenga más de un nivel. Todos los subgrupos del grupo principal heredan su configuración.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>No puede hacer público un subgrupo por sí solo, pero puede hacer público su grupo principal de nivel superior, que también hace públicos todos los subgrupos del grupo principal.</li> 
         <li>Un subgrupo que pertenece a un grupo público es público de forma predeterminada, por lo que cualquier usuario con acceso de edición de usuarios también puede añadir el subgrupo a otros usuarios.</li> 
        </ul> </p> <p>Si necesita información sobre el acceso necesario para editar usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Conceder acceso a usuarios</a>. Para obtener información la edición de usuarios, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Editar el perfil de un usuario</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coordinador empresarial </td> 
      <td> <p>Puede asignar un usuario como coordinador empresarial a un grupo que administre. Un líder empresarial es alguien que toma decisiones comerciales para el grupo. Para más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Información general sobre el Coordinador empresarial</a><span>.</span></p> <p>Si la persona aún no es miembro del grupo, al añadir su nombre a este campo también se añade al grupo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Para poder quitar el coordinador empresarial de un grupo, debe quitar su nombre del campo Coordinador empresarial.</li> 
         <li>Si quita el nombre del campo Coordinador empresarial, ese usuario seguirá siendo miembro del grupo a menos que lo quite de él. Para obtener instrucciones sobre cómo quitar a alguien de un grupo, consulte la sección <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Administrar las pertenencias a un grupo</a> en el artículo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Administrar un grupo</a>.</li> 
        </ul> </p> <p>Para más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Información general sobre el Coordinador empresarial</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Miembros y administradores de grupo</td> 
      <td> 
       <ul> 
        <li> <p>Miembros del grupo: para añadir usuarios y grupos al grupo, empiece a escribir el nombre de un usuario o grupo existente que desee añadir y, a continuación, seleccione el nombre cuando aparezca.</p> <p>Los usuarios y grupos que añada tendrán acceso a todos los objetos compartidos con el grupo.</p> </li> 
        <li> <p>Administradores de grupos: todos los administradores de grupos del grupo original también se designan como administradores de grupos en el grupo copiado. Puede asignar un miembro del grupo como administrador del grupo mediante el menú desplegable situado a la derecha del nombre del usuario.</p> <p>Un grupo de nivel superior debe tener al menos un administrador de grupos.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Buscar personas y grupos en la lista</td> 
      <td> Si necesita encontrar un usuario o grupo ya asignado a este grupo, puede escribir su nombre aquí y seleccionarlo cuando aparezca.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Si el grupo original tiene subgrupos, estos se añaden al nuevo grupo y sus nombres son, de forma predeterminada, “El nombre del subgrupo original (Copiar)”.
   >* Puede eliminar cualquier usuario o subgrupo del grupo original haciendo clic en la X situada a la derecha del nombre del usuario o subgrupo.

1. Haga clic en **Crear grupo**.
