---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Crear un subgrupo
description: Puede crear un subgrupo en un grupo que administra para organizar usuarios y proyectos y para asignar derechos de acceso dentro de Adobe Workfront. Normalmente, los administradores de grupos administran grupos y subgrupos. Pueden usar la página Grupos para administrar sus grupos y subgrupos en un solo lugar.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 3%

---

# Crear un subgrupo

Puede crear un subgrupo en un grupo que administra para organizar usuarios y proyectos y para asignar derechos de acceso dentro de Adobe Workfront.

Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Sin embargo, normalmente los administradores de grupos administran grupos y subgrupos. Pueden usar la página Grupos para administrar sus grupos y subgrupos en un solo lugar. Para obtener información sobre cómo funcionan los grupos y subgrupos en Workfront, consulte [Información general sobre grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md) y [Información general de subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## Agregar un subgrupo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra junto con los subgrupos que tienen. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Seleccione el grupo o subgrupo existente donde desea agregar un nuevo subgrupo.
1. Haga clic en **Nuevo subgrupo**.
1. En el **Nuevo subgrupo** que aparece, escriba una **Nombre del grupo** para el subgrupo.
1. (Opcional) especifique cualquiera de las siguientes informaciones:

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
      <td>Escriba una descripción para el subgrupo. Se pueden escribir hasta 512 caracteres.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activo</td> 
      <td> <p>(Habilitado de forma predeterminada) Activa el grupo en la instancia de Workfront.</p> <p>En los campos de tipo anterior, como el que se muestra a continuación, cuando los usuarios habituales buscan un grupo para adjuntarlo a un objeto o para compartir un objeto con él, solo se muestran en la lista los grupos activos.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para racionalizar esto para los usuarios, puede desactivar la opción Está activo para los grupos que no están actualmente en uso.</p> <p>Puede ver, filtrar y agrupar fácilmente la lista Grupos en función del estado activo o inactivo mediante este campo. Para obtener información sobre el uso de vistas, filtros y agrupaciones en listas, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementos de informes: filtros, vistas y agrupaciones</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Convertir este grupo y sus subgrupos en públicos</td> 
      <td> <p>(Disponible solo si está viendo Detalles para un grupo de nivel superior, no un subgrupo). Active esta opción para permitir que los usuarios del subgrupo con acceso de usuario de edición (que no son administradores del grupo) agreguen este grupo y sus subgrupos al perfil de usuario de otros usuarios.</p> <p>Para un grupo público, cualquier usuario (dentro o fuera del grupo) que tenga acceso de usuario de edición puede agregar el grupo al perfil de otros usuarios. No pueden hacerlo para un grupo privado.</p> <p>Esta opción solo se puede editar en el grupo principal superior de una jerarquía de grupos que tenga más de un nivel. Todos los subgrupos del grupo principal heredan su configuración.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>No se puede hacer público un subgrupo por sí solo, pero se puede hacer público su grupo principal de nivel superior, lo que también hace públicos todos los subgrupos de los padres.</li> 
         <li>Un subgrupo que pertenece a un grupo público es público de forma predeterminada, por lo que cualquier usuario con acceso de usuario de edición también puede agregar el subgrupo a otros usuarios.</li> 
        </ul> </p> <p>Si necesita información sobre el acceso necesario para editar usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Conceder acceso a los usuarios</a>. Para obtener información sobre la edición de usuarios, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Edición del perfil de un usuario</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coordinador empresarial </td> 
      <td> <p>Puede asignar un usuario como líder empresarial para un subgrupo que administra. Un líder empresarial es alguien que toma decisiones comerciales para el subgrupo. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Información general de Business Leader</a><span>.</span></p> <p>Si la persona no es ya miembro del subgrupo, al agregar su nombre a este campo también se añaden al grupo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Para poder quitar el encabezado de negocio de un subgrupo, debe quitar su nombre del campo Líder de negocio .</li> 
         <li>Si elimina el nombre del campo Líder empresarial , ese usuario seguirá siendo miembro del subgrupo a menos que los elimine de él. Para obtener instrucciones sobre cómo quitar a alguien de un grupo, consulte la sección <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Administrar las suscripciones de un grupo</a> en el artículo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Administrar un grupo</a>.</li> 
        </ul> </p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Información general de Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Miembros y administradores de grupo</td> 
      <td> 
       <ul> 
        <li> <p>Miembros del grupo: Para agregar usuarios y grupos al subgrupo, empiece a escribir el nombre de un usuario o grupo existente que desee agregar y, a continuación, seleccione el nombre cuando aparezca.</p> <p>Los usuarios y grupos que agregue tendrán acceso a todos los objetos compartidos con el grupo.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Administradores de grupo: Un subgrupo hereda los administradores de grupo del grupo que están encima de él, por lo que es opcional especificar un usuario como administrador de grupo para un subgrupo. Puede asignar un miembro del grupo como administrador para el grupo mediante el menú desplegable situado a la derecha del nombre del usuario.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Buscar personas y grupos en la lista</td> 
      <td> Si necesita encontrar un usuario o grupo ya asignado a este subgrupo, puede escribir su nombre aquí y seleccionarlo cuando aparezca.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar.**
