---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Editar información de hoja de horas
description: Como usuario con acceso administrativo a Hojas de horas, puede editar información sobre hojas de horas existentes en Adobe Workfront . Por ejemplo, puede editar el Propietario, los Aprobadores o el lapso de tiempo del parte de horas.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 2%

---

# Editar información de hoja de horas

Como usuario con acceso administrativo a Hojas de horas, puede editar información sobre hojas de horas existentes en Adobe Workfront . Por ejemplo, puede editar el Propietario, los Aprobadores o el lapso de tiempo del parte de horas.

Puede editar información en un solo parte de horas o puede editar varias partes de horas de forma masiva.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe tener acceso administrativo a las hojas de horas. </p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Editar partes de horas

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Hojas de tiempo**.

   La variable **Todo** está seleccionado de forma predeterminada que muestra todas las hojas de horas a las que tiene acceso para ver.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Haga clic en el **búsqueda** icono ![](assets/search-icon.png) y escriba una palabra clave y busque un parte de horas específico. Por ejemplo, puede buscar un marco de tiempo de parte de horas o un nombre de propietario.

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de partes de horas:

   * Select **Aprobaciones de Mi parte de horas** en la esquina superior derecha de la página para ver solo las partes de horas que aprueba

      O

      Select **Mis hojas de hora** para ver solo sus partes de horas.

      Esto aplica los filtros Mis aprobaciones de parte de horas o Mi parte de horas a la lista de partes de horas.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono Filtro ![](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de parte de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o un administrador de grupo han eliminado los filtros Mis aprobaciones de parte de horas y Mis hojas de horas de los controles de lista del área Configuración o de la plantilla Diseño. Para obtener más información, consulte los siguientes artículos:
   * [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Opcional) Haga clic en el **Ver** ![](assets/view-icon.png) o **Agrupación** ![](assets/grouping.png) para aplicar una vista o agrupación diferente o para crear una nueva.

   Para obtener información sobre la creación de filtros, vistas o agrupaciones, consulte los siguientes artículos:

   * [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Crear o editar vistas en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Crear agrupaciones en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleccione una o varias partes de horas y haga clic en el botón **Editar** icono ![](assets/edit-icon.png) en la parte superior de la lista de hojas de horas.
1. Vea o especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Propietario</strong> </td> 
      <td> <p>Es el nombre del usuario para el que se creó el parte de horas. No se puede editar este campo. </p> <p>El campo no se muestra cuando selecciona varias partes de horas. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha de inicio</strong> </td> 
      <td>Esta es la fecha de inicio del parte de horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha de finalización</strong> </td> 
      <td> Esta es la fecha de finalización del parte de horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aprobadores</strong> </td> 
      <td> <p>Los aprobadores son usuarios que aprueban el parte de horas para los usuarios asociados al parte de horas. Solo los usuarios con acceso administrativo a Hojas de horas pueden configurarse como aprobadores. </p> <p>Para obtener más información sobre los derechos administrativos del parte de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p>Comience a introducir los nombres de los aprobadores de hojas de horas y selecciónelos cuando aparezcan en la lista.</p> <p>Puede tener varios aprobadores en un parte de horas. En este caso, después de que uno de los aprobadores apruebe el parte de horas, el parte de horas se marca como <strong>Cerrado</strong> y desaparece de la lista de aprobaciones de parte de horas de todos los aprobadores restantes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Puede editar el tiempo</strong> </td> 
      <td> <p>Seleccione esta opción si desea permitir que los aprobadores editen las horas en el parte de horas.</p> <p>Esta opción no está disponible cuando selecciona varias partes de horas. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Horas extra</span> </td> 
      <td> <p>Puede elegir ocultar el cuadro Tiempo extra del parte de horas.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en Guardar.
