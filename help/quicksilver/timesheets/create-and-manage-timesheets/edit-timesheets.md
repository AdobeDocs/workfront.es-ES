---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Editar información de hoja de horas
description: Como usuario con acceso administrativo a las plantillas de horas, puede editar información sobre las existentes en Adobe Workfront Por ejemplo, puede editar el Propietario, los Aprobadores o el lapso de tiempo de la plantilla de horas.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 2%

---

# Editar información de hoja de horas

Como usuario con acceso administrativo a las plantillas de horas, puede editar información sobre las existentes en Adobe Workfront Por ejemplo, puede editar el Propietario, los Aprobadores o el lapso de tiempo de la plantilla de horas.

Puede editar la información en una sola plantilla de horas o puede editar varias plantillas de horas de forma masiva.

>[!IMPORTANT]
>
>Si los usuarios están asociados con perfiles de hojas de horas y estas se generan automáticamente, los cambios que realice en las hojas de horas existentes no se reflejarán en las hojas de horas que se generarán en fechas futuras. Todas las hojas de horas generadas automáticamente tienen la configuración establecida en Perfiles de hojas de horas. Para obtener más información, consulte [Crear perfiles de hoja de horas](../create-and-manage-timesheets/create-timesheet-profiles.md)


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
   <td> <p>Debe tener acceso administrativo a las hojas de horas. </p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Editar hojas de horas

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Plantillas de horas**.

   El **Todo** El filtro está seleccionado de forma predeterminada y muestra todas las plantillas de horas que puede ver.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Haga clic en **búsqueda** icono ![](assets/search-icon.png) y escriba una palabra clave y busque una hoja de horas específica. Por ejemplo, puede buscar un lapso de tiempo o un nombre de propietario para una hoja de horas.

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de plantillas de horas:

   * Seleccionar **Mis aprobaciones de hojas de horas** en la esquina superior derecha de la página para ver solo las plantillas de horas que apruebe

     O

     Seleccionar **Mis hojas de horas** para ver únicamente las hojas de horas.

     Esto aplica los filtros Mis aprobaciones de hojas de horas o Mis hojas de horas a la lista de hojas de horas.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono Filtro ![](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Creación o edición de filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de hojas de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o de un grupo ha eliminado los filtros Mis aprobaciones de hojas de horas y Mis hojas de horas de los controles de Lista en el área Configuración o de la plantilla Diseño. Para obtener más información, consulte los siguientes artículos:
   >
   >   
   >   
   * [Personalización de filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Opcional) Haga clic en **Ver** ![](assets/view-icon.png) o **Agrupación** ![](assets/grouping.png) iconos para aplicar una vista o agrupación diferente o para crear una nueva.

   Para obtener información sobre la creación de filtros, vistas o agrupaciones, consulte los siguientes artículos:

   * [Creación o edición de filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creación o edición de vistas en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creación de agrupaciones en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleccione una o varias plantillas de horas y haga clic en **Editar** icono ![](assets/edit-icon.png) en la parte superior de la lista de hojas de horas.
1. Consulte o especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Propietario</strong> </td> 
      <td> <p>Nombre del usuario para el que se creó la plantilla de horas. No puede editar este campo. </p> <p>El campo no se muestra al seleccionar varias plantillas de horas. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha de inicio</strong> </td> 
      <td>Es la fecha de inicio de la hoja de horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha de finalización</strong> </td> 
      <td> Fecha de finalización de la plantilla de horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aprobadores</strong> </td> 
      <td> <p>Los aprobadores son usuarios que aprueban la hoja de horas de los usuarios asociados con ella. Solo los usuarios con acceso administrativo a las hojas de horas pueden establecerse como aprobadores. </p> <p>Para obtener más información sobre los derechos administrativos de plantillas de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p>Comience a introducir los nombres de los aprobadores de plantillas de horas y selecciónelos cuando aparezcan en la lista.</p> <p>Puede tener varios aprobadores en una hoja de horas. En este caso, una vez que uno de los aprobadores aprueba la plantilla de horas, esta se marca como <strong>Cerrado</strong> y desaparece de la lista de aprobaciones de hojas de horas de todos los aprobadores restantes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Puede editar el tiempo</strong> </td> 
      <td> <p>Seleccione esta opción si desea permitir que los aprobadores editen las horas en la hoja de horas.</p> <p>Esta opción no está disponible si selecciona varias plantillas de horas. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Horas extra</span> </td> 
      <td> <p>Puede elegir ocultar el cuadro Horas extra en la hoja de horas.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en Guardar.
