---
title: Ver y administrar los detalles de un grupo
description: Puede ver y editar la página Detalles del grupo para un grupo o subgrupo que administre.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 1%

---

# Ver y administrar los detalles de un grupo

Puede ver y editar la página Detalles del grupo para un grupo o subgrupo que administre. Esta página incluye:

* Una descripción del grupo
* Nombres del coordinador empresarial y de los administradores del grupo
* Una opción que le permite convertir el grupo y sus subgrupos en públicos o privados

  <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

Para obtener información acerca de otras formas de administrar un grupo, vea [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Para obtener información acerca de cómo desactivar o reactivar un grupo, vea [Desactivar o reactivar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

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

## Ver y administrar los detalles de un grupo

{{step-1-to-setup}}

1. Haga clic en **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo de nivel superior que desee editar.
1. Si desea desactivar o reactivar el grupo,
1. En el menú de la izquierda, haga clic en **Detalles del grupo** y, a continuación, siga uno de estos procedimientos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td> <p>Puede escribir hasta 512 caracteres.</p> <p>Si el campo está en blanco, haga clic en <strong>Agregar</strong> para escribir una descripción.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Activo</td> 
      <td> <p>(Habilitado de forma predeterminada) Activa el grupo en la instancia de Workfront.</p> <p>En campos de escritura anticipada como el que se muestra a continuación, cuando los usuarios normales buscan un grupo para adjuntarlo a un objeto o compartirlo, solo se muestran en la lista los grupos activos.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para optimizar esto para los usuarios, puede deshabilitar la opción Está activo para los grupos que no están en uso actualmente.</p> <p>Puede ver, filtrar y agrupar fácilmente la lista Grupos en función del estado activo o inactivo mediante este campo. Para obtener información acerca del uso de vistas, filtros y agrupaciones en listas, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de informes: filtros, vistas y agrupaciones</a>.</p> <p>Para obtener información acerca de los grupos inactivos, vea la sección <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Consideraciones para grupos inactivos</a> en el artículo <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Eliminar o desactivar un formulario personalizado</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accesibilidad del grupo</td> 
      <td> <p>(Disponible únicamente si visualiza los detalles de un grupo, no de un subgrupo). Habilite o deshabilite la opción <strong>Convertir este grupo y los subgrupos en privados</strong>.</p> <p>En el caso de los grupos públicos, cualquier usuario (dentro o fuera del grupo) que tenga acceso de usuario de edición puede agregar el grupo al perfil de otros usuarios. No pueden hacerlo para un grupo privado.</p> <p>Solo puede editar esta opción en el grupo principal superior de una jerarquía de grupos que tenga más de un nivel. Todos los subgrupos del grupo principal heredan su configuración.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partes interesadas del grupo</td> 
      <td> 
       <ul> 
        <li><strong>Administradores de grupo</strong>: Agregue o elimine usuarios con una licencia de Planificador como administradores de grupo para el grupo. Empiece a escribir el nombre de un usuario y, a continuación, haga clic en él cuando aparezca en el menú desplegable.</li> 
        <li><strong>Coordinador empresarial</strong>: realice una de las siguientes acciones:
         <ul>
          <li>Si todavía no ha asignado un coordinador empresarial para el grupo, haga clic en <strong>Agregar</strong>, empiece a escribir el nombre del usuario que desea asignar y, a continuación, haga clic en el nombre de la persona cuando aparezca.</li>
          <li>Si el grupo ya tiene un coordinador empresarial y desea cambiarlo, haga doble clic en el nombre del coordinador empresarial existente. Elimine el nombre, empiece a escribir el nombre del usuario que desea asignar y, a continuación, haga clic en el nombre de la persona cuando aparezca.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agregar formulario personalizado</td> 
      <td>Si su nivel de acceso le permite administrar formularios personalizados, agregue un formulario personalizado al grupo. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Formularios personalizados</a>.</td> 
     </tr> 
    </tbody> 
   </table>
