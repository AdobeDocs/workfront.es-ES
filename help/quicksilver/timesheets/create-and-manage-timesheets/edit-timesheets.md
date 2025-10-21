---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Editar información de la plantilla de horas
description: Como usuario con acceso administrativo a las plantillas de horas, puede editar información sobre las existentes en Adobe Workfront. Por ejemplo, puede editar el Propietario, los Aprobadores o el lapso de tiempo de la plantilla de horas.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 94%

---

# Editar información de la plantilla de horas

Como usuario con acceso administrativo a las plantillas de horas, puede editar información sobre las existentes en Adobe Workfront. Por ejemplo, puede editar el Propietario, los Aprobadores o el lapso de tiempo de la plantilla de horas.

Puede editar la información en una sola plantilla de horas o puede editar varias plantillas de horas de forma masiva.

>[!IMPORTANT]
>
>Si los usuarios están asociados con perfiles de plantillas de horas y estas se generan automáticamente, los cambios que realice en las plantillas de horas existentes no se reflejarán en las plantillas de horas que se generarán en fechas futuras. Todas las plantillas de horas generadas automáticamente tienen la configuración establecida en Perfiles de plantillas de horas. Para obtener más información, consulte [Crear perfiles de plantillas de horas](../create-and-manage-timesheets/create-timesheet-profiles.md)

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
   <td>
   <p>Estándar</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td><p>Acceso administrativo a hojas de horas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar plantillas de horas

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y luego haga clic en **Plantillas de horas**.

   El filtro **Todas** está seleccionado de manera predeterminada, el cual muestra todas las plantillas de horas que tiene acceso para ver.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Haga clic en el icono **buscar** ![](assets/search-icon.png), escriba una palabra clave y busque una plantilla de horas específica. Por ejemplo, puede buscar un lapso de tiempo o un nombre de propietario para una plantilla de horas.

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de plantillas de horas:

   * Seleccione **Aprobaciones de Mis plantillas de horas** en la esquina superior derecha de la página para ver solamente las plantillas de horas que usted apruebe

     O

     Seleccione **Mis plantillas de horas** para ver solamente sus plantillas de horas.

     Esto aplica los filtros Mis aprobaciones de plantillas de horas o Mis plantillas de horas a la lista de plantillas de horas.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono de Filtro ![](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de plantillas de horas y Mis plantillas de horas no se muestran en la parte superior de la lista de plantillas de horas ni en la lista de filtros si el administrador de Workfront o de un grupo ha eliminado estos filtros de los Controles de lista en el área Configuración o de la Plantilla de diseño.Para obtener más información, consulte los siguientes artículos:
   >
   >   
   >   
   >   * [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Opcional) Haga clic en los iconos **Ver** ![](assets/view-icon.png) o **Agrupar** ![](assets/grouping.png) para aplicar una vista o agrupación diferente o para crear una nueva.

   Para obtener información sobre la creación de filtros, vistas o agrupaciones, consulte los siguientes artículos:

   * [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Crear o editar vistas en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creación de agrupaciones en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleccione una o varias plantillas de horas y luego haga clic en el icono **Editar** ![](assets/edit-icon.png) en la parte superior de la lista de plantillas de horas.
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
      <td>Esta la fecha de inicio de la plantilla de horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha de finalización</strong> </td> 
      <td> Esta es la fecha de finalización de la plantilla de horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Estado</strong> </td> 
      <td> Este es el estado de la plantilla de horas.
      Las siguientes son posibles opciones de estado de la plantilla de horas: 
      <ul><li><b>Abrir</b>: la plantilla de horas está abierta y las entradas de horas se pueden editar.</li>
      <li><b>Enviada</b>: la plantilla de horas se envía para su aprobación a los aprobadores designados.</li>
      <li><b>Rechazada</b>: la plantilla de horas no fue aprobada por los aprobadores y ahora está disponible nuevamente para que el usuario edite las entradas de tiempo.</li>
      <li><b>Cerrada</b>: la plantilla de horas está cerrada por el usuario o aprobada por el aprobador y, como resultado, ahora está cerrada. No se puede añadir tiempo a una plantilla de horas cerrada.</li>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aprobadores</strong> </td> 
      <td> <p>Los aprobadores son usuarios que aprueban la plantilla de horas de los usuarios asociados con ella. Solo los usuarios con acceso administrativo a las plantillas de horas pueden establecerse como aprobadores. </p> <p>Para obtener más información sobre los derechos administrativos de la plantilla de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder acceso administrativo a los usuarios a ciertas áreas</a>.</p> <p>Comience a introducir los nombres de los aprobadores de plantillas de horas y selecciónelos cuando aparezcan en la lista.</p> <p>Puede tener varios aprobadores en una plantilla de horas. En este caso, una vez que uno de los aprobadores aprueba la plantilla de horas, esta se marca como <strong>Cerrada</strong> y desaparece de la lista de aprobaciones de plantillas de horas de todos los aprobadores restantes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Puede editar el tiempo</strong> </td> 
      <td> <p>Seleccione esta opción si desea permitir que los aprobadores editen las horas en la plantilla de horas.</p> <p>Esta opción no está disponible si selecciona varias plantillas de horas. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Horas extra</span> </td> 
      <td> <p>Puede elegir ocultar el cuadro Horas extra en la plantilla de horas.</p> <p>Esta opción está desactivada de forma predeterminada.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
