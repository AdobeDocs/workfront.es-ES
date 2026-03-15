---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Personal Tasks'
description: This task filter returns ad hoc work requests sent to a user, or to-do items added by users in their Home area. Personal tasks are not connected to a project but they can be moved to a project, if needed.
author: Courtney
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 23%

---

# Filtro: tareas personales

<!--Audited: 10/2024-->

This task filter returns ad hoc work requests sent to a user, or to-do items added by users in their To-dos widget in the Home area.

Ad hoc work requests and to-do items are saved in Adobe Workfront as personal tasks.

Personal tasks are not connected to a project but they can be moved to a project, if needed. For information, see [Create personal tasks](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

![Personal tasks report](assets/personal-tasks-report.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Contributor or Request to modify a filter </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filter personal tasks

To create this filter:

1. Go to a list of tasks or a task report.
1. From the **Filter** drop-down menu, click **New filter**.
1. (Conditional) Click **Add a filter rule** of you are accessing the filter from a report, or start selecting your filter criteria in the first field, if you are accessing the filter from a list.
1. (Conditional) Select the following filtering criteria:

   * From a list filter: **Task** > **Personal** **Is true**
   * From a report filter: **Task** > **Personal** > **Equal (Case sensitive)** > **True**.
1. Save the filter.

   The list displays only personal tasks that are not on any projects.
