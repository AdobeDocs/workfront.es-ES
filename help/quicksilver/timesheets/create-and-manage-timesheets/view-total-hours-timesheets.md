---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Ver las horas totales en la plantilla de horas
description: Puede ver la cantidad total de horas en su plantilla de horas. El número total de horas de la plantilla de horas incluye las horas registradas en proyectos, tareas, problemas y todas las horas generales.
author: Lisa
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
TQID: https://experienceleague.adobe.com/oh6bBQz6sfxCpodHahZXtlMMuYYT-4U7-5MP6TQeuIs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 69%
---
# Ver las horas totales en la plantilla de horas

<!--Audited: 8/2024-->

Puede ver la cantidad total de horas en su plantilla de horas. El número total de horas de la plantilla de horas incluye las horas registradas en proyectos, tareas, problemas y todas las horas generales.

El total de horas refleja las horas enviadas mediante la plantilla de horas, el área Actualizaciones o el área Horas para los proyectos, tareas o problemas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td> <p>Ligero o superior </p>
   <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Configuración de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a tareas y problemas</p> </td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Vista o permisos superiores a tareas y problemas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver las horas totales de una plantilla de horas en el encabezado de la plantilla de horas

Puede ver las horas totales de una plantilla de horas en el encabezado de la plantilla de horas.

![Campo de horas totales](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## Ver las horas totales en su plantilla de horas en una lista de plantillas de horas

{{step1-to-timesheets}}

De forma predeterminada, se muestran todas las hojas de horas a las que tiene acceso para ver.

![Lista de hojas de horas](assets/list-of-all-timesheets.png)

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de plantillas de horas:

   * Seleccione **Mis aprobaciones de hojas de horas** en la esquina superior derecha de la página para ver solamente las hojas de horas que usted apruebe,

     O

     Seleccione **Mis plantillas de horas** para ver solamente sus plantillas de horas.

     Esto aplica los filtros **Mis aprobaciones de hojas de horas** o **Mi hoja de horas** a la lista de hojas de horas.

   * Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-nwepng.png) para aplicar un filtro o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de hojas de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o de un grupo ha eliminado esos filtros de los controles de lista en el área de Configuración o de la plantilla de diseño. Para obtener más información, consulte [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Opcional) Haga clic en los iconos **Ver** ![Ver icono](assets/view-icon.png) o **Agrupar** ![Icono de agrupación](assets/grouping.png) para aplicar una vista o agrupación o para crear una nueva.

   Para obtener información sobre la creación de filtros, vistas o agrupaciones, consulte los siguientes artículos:

   * [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Crear o editar vistas en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creación de agrupaciones en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. El número total de horas de cada plantilla de horas se muestra en la columna **Total de horas**.

   ![Columna Horas totales](assets/total-hours-column.png)

   >[!TIP]
   >
   >Al utilizar la vista Estándar para una lista de plantillas de horas, la columna Total de horas se muestra en rojo si la hora registrada para los elementos de la plantilla de horas supera el número de horas en el lapso de tiempo de la plantilla de horas. Para obtener más información, consulte el campo “Total de horas” en [Glosario de terminología de Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
