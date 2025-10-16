---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Eliminación de plantillas de horas en Adobe Workfront
description: Los cambios que realice en un perfil de plantilla de horas no entrarán en vigor de inmediato en las plantillas existentes, como se explica en Crear, editar y asignar perfiles de plantilla de horas. Para que los cambios sean visibles en las plantillas de horas existentes, debe eliminar las que se hayan generado y generar nuevas. Esto solo se aplica a las hojas de horas que se han generado al asociar perfiles de hojas de horas con usuarios.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 40%

---

# Eliminación de plantillas de horas en Adobe Workfront

Los cambios que realice en un perfil de hoja de horas no entrarán en vigor de inmediato en las hojas de horas existentes, como se explica en [Crear, editar y asignar perfiles de hoja de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Para que los cambios sean visibles en las plantillas de horas existentes, debe eliminar las que se hayan generado y generar nuevas. Esto solo se aplica a las hojas de horas que se han generado al asociar perfiles de hojas de horas con usuarios.

>[!NOTE]
>
>Las plantillas de horas que se hayan creado manualmente no se pueden volver a crear regenerando las plantillas de horas, a menos que los usuarios se hayan asociado a un perfil de plantilla de horas desde que se creó manualmente la plantilla de horas. La eliminación de una plantilla de horas creada manualmente puede causar la pérdida de datos. Para obtener información sobre cómo crear una sola hoja de horas, consulte [Crear una hoja de horas de un solo uso](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Los administradores de Adobe Workfront o de grupos pueden generar plantillas de horas para todos los miembros del sistema. Para obtener más información sobre la generación manual de plantillas de horas, consulte:

* [Generar manualmente hojas de horas](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [Crear y administrar los perfiles de plantillas de horas de un grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* No puede recuperar una hoja de horas eliminada.
>* Se recomienda no eliminar las plantillas de horas anteriores, ya que no se generan automáticamente según los perfiles de las plantillas de horas. Puede eliminar las plantillas de horas actuales y futuras y generarlas manualmente si desea que los cambios en los perfiles de la plantilla de horas sean visibles inmediatamente en las nuevas plantillas de horas.
>* Al eliminar las hojas de horas, las horas registradas en las tareas, los problemas y los proyectos no se eliminan. Con la plantilla de horas solo se eliminan las horas generales. En un editor de texto independiente, anote las horas generales asociadas con la plantilla de horas. Una vez eliminada la plantilla de horas, puede registrarlas en la nueva plantilla.
>

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

## Eliminación de plantillas de horas de una lista

1. Haga clic en el icono de **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Plantilla de horas**. El filtro **Todos** está seleccionado de manera predeterminada y muestra todas las hojas de horas que puede ver.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

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

1. Seleccione una o varias hojas de horas que desee eliminar y haga clic en el icono **Eliminar** ![](assets/delete.png) en la parte superior de la lista de hojas de horas.

1. Haga clic **eliminar**.

   Las hojas de horas seleccionadas se eliminan y no se pueden recuperar.

   Para generar nuevas plantillas de horas, asegúrese de que los usuarios estén asociados a un perfil de plantilla de horas y pida al administrador de Workfront o a un administrador de grupo que genere nuevas plantillas de horas.

   Para obtener más información, consulte los artículos:

   * [Crear, editar y asignar perfiles de plantillas de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Generar plantillas de horas manualmente](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [Crear y administrar los perfiles de plantillas de horas de un grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Eliminar una plantilla de horas de la página de plantilla

1. Haga clic en el icono [!UICONTROL **Menú principal**] ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en la plantilla de horas que desee eliminar para abrirla.
1. Haga clic en el icono [!UICONTROL **Más**] ![](assets/more-icon.png) a la derecha del nombre de la hoja de horas y luego haga clic en **Eliminar**.

   ![Eliminar hoja de horas de la página de hoja de horas](assets/delete-timesheet-from-timesheet-page.png)
1. Haga clic en [!UICONTROL **Eliminar**] para confirmar.

   La plantilla de horas se elimina y no se puede recuperar.
