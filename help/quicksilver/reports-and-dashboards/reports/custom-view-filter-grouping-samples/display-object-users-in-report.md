---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Informes o listas: muestran los usuarios asociados a un objeto"
description: Puede mostrar usuarios, funciones y equipos asociados con objetos en informes o listas, así como hacer referencia a ellos en filtros. No se puede agrupar por usuarios, puestos ni equipos asociados a objetos.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 9abdaafb-da2c-4b5d-9117-59afa4a1e71f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 2%

---

# Informes o listas: muestran los usuarios asociados a un objeto

Puede mostrar usuarios, funciones y equipos asociados con objetos en informes o listas, así como hacer referencia a ellos en filtros. No se puede agrupar por usuarios, puestos ni equipos asociados a objetos.

Puede mostrar o filtrar por usuarios, roles o equipos asociados con los siguientes objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Objeto</td> 
   <td>Usuarios o funciones de trabajo asociados</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proyecto</td> 
   <td> <p>En un informe de proyecto puede mostrar todos los usuarios y las funciones que cumplen en el proyecto. No puede filtrar por los usuarios o sus funciones asociadas en un informe de proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tareas</td> 
   <td>Puede mostrar y filtrar por todos los usuarios, roles y equipos asignados a una tarea en un informe de tareas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Problemas</td> 
   <td>Puede mostrar y filtrar por todos los usuarios, roles y equipos asignados a un problema en un informe de problemas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Portafolios</td> 
   <td>Puede mostrar todos los usuarios y las funciones que cumplen en el proyecto en un informe de proyecto y agrupar el informe por Portfolio. No puede filtrar por los usuarios o sus funciones asociadas en un informe de proyecto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Programas</td> 
   <td>Puede mostrar todos los usuarios y las funciones que cumplen en el proyecto en un informe de proyecto y agrupar el informe por programa. No puede filtrar por los usuarios o sus funciones asociadas en un informe de proyecto.</td> 
  </tr> 
 </tbody> 
</table>

## Mostrar todos los usuarios y los roles asociados a un proyecto

Puede mostrar todos los usuarios asociados a en el proyecto en la vista de una lista de proyectos o un informe. Esto incluye a todos los usuarios enumerados en la sección Personas del proyecto. También puede ver las funciones con las que están asociados cuando se les asignan tareas o problemas en el proyecto en un informe de proyecto.

![](assets/project-with-user-and-role-information-report-350x100.png)

Para obtener información sobre cómo generar un informe de proyecto para mostrar todos los usuarios y sus roles en el proyecto, consulte [Ver: lista de usuarios de proyecto con roles](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

No puede filtrar por usuarios o funciones de trabajo asociadas a proyectos en un filtro de proyecto.

## Mostrar todos los usuarios, roles o equipos asignados a una tarea

Puede mostrar todos los usuarios, roles o equipos asignados a una tarea en la vista de una lista de tareas o un informe agregando el campo Asignaciones a la vista.

![](assets/assignments-field-task-view-350x124.png)

Puede filtrar por los usuarios, roles o equipos asignados a las tareas haciendo referencia a los siguientes campos en un filtro de tareas:

* Usuarios de asignación
* Roles de asignación
* Equipo

![](assets/assignment-users-roles-task-filter-350x334.png)

## Mostrar todos los usuarios, roles o equipos asignados a un problema

Puede mostrar todos los usuarios, roles o equipos asignados a un problema en la vista de una lista de problemas o un informe al agregar el campo Asignaciones a la vista.

Puede filtrar por los usuarios, los roles o los equipos asignados a los problemas haciendo referencia a los siguientes campos en un filtro de problemas:

* Usuarios de asignación
* Roles de asignación
* Equipo

## Mostrar todos los usuarios y las funciones del puesto asociados a un portafolio

Puede mostrar todos los usuarios y funciones asociados a un portafolio mostrándolos en un informe de proyecto y luego agrupando el informe por Portfolio.

Para obtener información sobre cómo generar un informe de proyecto para mostrar todos los usuarios y sus roles en el proyecto, consulte [Ver: lista de usuarios de proyecto con roles](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

No puede filtrar por usuarios o roles asociados a proyectos en un portafolio o filtro de proyecto.

## Mostrar todos los usuarios y los puestos asociados a un programa

Puede mostrar todos los usuarios y roles asociados a un programa mostrándolos en un informe de proyecto y, a continuación, agrupando el informe por programa.

Para obtener información sobre cómo generar un informe de proyecto para mostrar todos los usuarios y sus roles en el proyecto, consulte [Ver: lista de usuarios de proyecto con roles](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

No puede filtrar por usuarios o funciones de trabajo asociadas a proyectos en un filtro de programa o proyecto.
