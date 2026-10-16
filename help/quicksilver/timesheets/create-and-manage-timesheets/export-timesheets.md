---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Exportar una lista de plantillas de horas
description: Como administrador de personas o aprobador de plantillas de horas, es posible que tenga que descargar una lista de plantillas de horas para ver rápidamente información sobre las plantillas de las personas de las que es responsable. Para ello, exporte una lista de plantillas de horas.
author: Lisa
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-bihpKoVoPCwTpAj-SK-RPPFpaCubsyLAfnfSmpTnyI
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
source-wordcount: '449'
ht-degree: 64%
---
# Exportar una lista de plantillas de horas

<!--Audited: 8/2024-->

Como administrador de personas o aprobador de plantillas de horas, es posible que tenga que descargar una lista de plantillas de horas para ver rápidamente información sobre las plantillas de las personas de las que es responsable. Para ello, exporte una lista de plantillas de horas.

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

## Exportar una lista de plantillas de horas

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

1. Seleccione las hojas de horas que desee exportar y, a continuación, haga clic en el icono **Exportar** ![Icono de exportar](assets/export-38x15.png).

   ![Haga clic en el icono Exportar](assets/export-timesheets.png)

1. Seleccione el tipo de archivo al que desea exportar la lista de plantillas de horas desde las siguientes opciones:

   * PDF horizontal
   * PDF vertical
   * PDF de otros tamaños
   * Excel
   * Excel (xlsx)
   * Delimitado por tabulaciones

   Se descargará en el equipo una lista de plantillas de horas en el formato seleccionado, que incluye la siguiente información:

   * Intervalo de fecha
   * Nombre del propietario
   * Total de horas
   * Cantidad de horas extra
   * Nombres de aprobadores
   * Estado
