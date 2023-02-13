---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Eliminar partes de horas en Adobe Workfront
description: Los cambios que realice en un perfil de parte de horas no serán efectivos de inmediato para las hojas de horas existentes, tal como se explica en Crear, editar y asignar perfiles de parte de horas. Para que los cambios estén visibles en las hojas de horas existentes, debe eliminar las hojas de horas que se hayan generado y generar otras nuevas. Esto se aplica solo a las hojas de horas que se han generado asociando perfiles de hojas de horas con usuarios.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Eliminar partes de horas en Adobe Workfront

Los cambios que realice en un perfil de parte de horas no serán efectivos de inmediato para las hojas de horas existentes, como se explica en [Crear, editar y asignar perfiles de parte de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Para que los cambios estén visibles en las hojas de horas existentes, debe eliminar las hojas de horas que se hayan generado y generar otras nuevas. Esto se aplica solo a las hojas de horas que se han generado asociando perfiles de hojas de horas con usuarios.

>[!NOTE]
>
>Las hojas de horas que se han creado manualmente no se pueden volver a crear regenerando las hojas de horas, a menos que los usuarios se hayan asociado con un perfil de parte de horas desde que el parte de horas se creó manualmente. La eliminación de un parte de horas creado manualmente puede causar la pérdida de datos. Para obtener información sobre cómo crear una sola hoja de horas, consulte [Crear un parte de horas de un solo uso](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Los administradores de Adobe Workfront o los administradores de grupos pueden generar hojas de horas para todos los miembros del sistema. Para obtener más información sobre la generación manual de hojas de hora, consulte:

* [Generar hojas de hora manualmente](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [Creación y administración de perfiles de hojas de horas de un grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* No se puede recuperar un parte de horas eliminado.
>* Se recomienda no eliminar las partes de horas anteriores, ya que no se generan automáticamente en función de perfiles de hojas de horas. Puede eliminar las hojas de horas actuales y futuras y generarlas manualmente si desea que los cambios en los perfiles de hojas de horas se puedan ver inmediatamente en las nuevas hojas de horas.
>* Al eliminar partes de horas, no se eliminan las horas registradas en relación con tareas, problemas y proyectos. Solo las horas generales se eliminan con el parte de horas. En un editor de texto independiente, anote qué horas generales están asociadas con el parte de horas. Una vez eliminado el parte de horas, puede registrarlos en el nuevo parte de horas.
>


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
   <td> <p>Debe tener acceso administrativo a las hojas de horas. </p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Eliminar partes de horas de una lista

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Hojas de tiempo**. La variable **Todo** está seleccionado de forma predeterminada y muestra todas las partes de horas a las que tiene acceso para ver.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de partes de horas:

   * Select **Aprobaciones de Mi parte de horas** en la esquina superior derecha de la página para ver solo las partes de horas que aprueba

      O

      Select **Mis hojas de hora** para ver solo sus partes de horas.

      Esto aplica los filtros Mis aprobaciones de parte de horas o Mi parte de horas a la lista de partes de horas.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono Filtro ![](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   Las opciones Mis aprobaciones de parte de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o un administrador de grupo han eliminado los filtros Mis aprobaciones de parte de horas y Mis hojas de horas de los controles de lista del área Configuración o de la plantilla Diseño. Para obtener más información, consulte los siguientes artículos:
   * [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Opcional) Haga clic en el **Ver** ![](assets/view-icon.png) o **Agrupación** ![](assets/grouping.png) para aplicar una vista o agrupación diferente o para crear una nueva.

   Para obtener información sobre la creación de filtros, vistas o agrupaciones, consulte los siguientes artículos:

   * [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Crear o editar vistas en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Crear agrupaciones en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleccione una o varias partes de horas que desee eliminar y haga clic en el botón **Eliminar**  ![](assets/delete.png) en la parte superior de la lista de partes de horas.

1. Haga clic en **Eliminar**.

   Las partes de horas seleccionadas se eliminan y no se pueden recuperar.

   Para generar nuevas hojas de horas, asegúrese de que los usuarios estén asociados a un perfil de parte de horas y pida al administrador de Workfront o a un administrador de grupo que genere nuevas hojas de horas.

   Para obtener más información, consulte lo siguiente:

   * [Crear, editar y asignar perfiles de parte de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Generar hojas de hora manualmente](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [Creación y administración de perfiles de hojas de horas de un grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Eliminar un parte de horas de la página parte de horas

1. Haga clic en el [!UICONTROL **Menú principal**] icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en el parte de horas que desee eliminar para abrirlo.
1. Haga clic en el [!UICONTROL **Más**] icono ![](assets/more-icon.png) a la derecha del nombre del parte de horas y, a continuación, haga clic en **Eliminar**.

   ![Eliminar parte de horas de la página hoja de horas](assets/delete-timesheet-from-timesheet-page.png)
1. Haga clic en [!UICONTROL **Eliminar**] para confirmar.

   El parte de horas se elimina y no se puede recuperar.
