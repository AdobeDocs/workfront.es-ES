---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Informes o listas: mostrar los usuarios asociados a un objeto'
description: Puede mostrar usuarios, funciones y equipos asociados con objetos en informes o listas, así como hacer referencia a ellos en filtros. No se puede agrupar por usuarios, funciones ni equipos asociados a objetos.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 9abdaafb-da2c-4b5d-9117-59afa4a1e71f
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 97%

---

# Informes o listas: mostrar los usuarios asociados a un objeto

Puede mostrar usuarios, funciones y equipos asociados con objetos en informes o listas, así como hacer referencia a ellos en filtros. No se puede agrupar por usuarios, funciones ni equipos asociados a objetos.

Puede mostrar o filtrar por usuarios, funciones o equipos asociados con los siguientes objetos:

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
   <td>Puede mostrar y filtrar por todos los usuarios, funciones y equipos asignados a una tarea en un informe de tareas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Problemas</td> 
   <td>Puede mostrar y filtrar por todos los usuarios, funciones y equipos asignados a un problema en un informe de problemas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Portafolios</td> 
   <td>Puede mostrar todos los usuarios y las funciones que cumplen en el proyecto en un informe de proyecto y agrupar el informe por portafolios. No puede filtrar por los usuarios o sus funciones asociadas en un informe de proyecto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Programas</td> 
   <td>Puede mostrar todos los usuarios y las funciones que cumplen en el proyecto en un informe de proyecto y agrupar el informe por programa. No puede filtrar por los usuarios o sus funciones asociadas en un informe de proyecto.</td> 
  </tr> 
 </tbody> 
</table>

## Mostrar todos los usuarios y las funciones asociados a un proyecto

Puede mostrar todos los usuarios asociados al proyecto en la vista de una lista de proyectos o un informe. Esto incluye a todos los usuarios enumerados en la sección Personas del proyecto. También puede ver las funciones con las que están asociados cuando se les asignan tareas o problemas en el proyecto en un informe de proyecto.

![Proyecto con información de usuario y rol](assets/project-with-user-and-role-information-report-350x100.png)

Para obtener información sobre cómo generar un informe de proyecto para mostrar todos los usuarios y sus funciones en el proyecto, consulte [Ver: lista de usuarios de proyecto con funciones](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

No puede filtrar por usuarios o funciones de trabajo asociadas a proyectos en un filtro de proyecto.

## Mostrar todos los usuarios, funciones o equipos asignados a una tarea

Puede mostrar todos los usuarios, funciones o equipos asignados a una tarea en la vista de una lista de tareas o un informe añadiendo el campo Asignaciones a la vista.

![Campo de asignación](assets/assignments-field-task-view-350x124.png)

Puede filtrar por los usuarios, funciones o equipos asignados a las tareas haciendo referencia a los siguientes campos en un filtro de tareas:

* Usuarios de asignación
* Roles de asignación
* Equipo

![Usuarios y funciones de asignación en el filtro de tareas](assets/assignment-users-roles-task-filter-350x334.png)

## Mostrar todos los usuarios, funciones o equipos asignados a un problema

Puede mostrar todos los usuarios, funciones o equipos asignados a un problema en la vista de una lista de problemas o un informe al añadir el campo Asignaciones a la vista.

Puede filtrar por los usuarios, las funciones o los equipos asignados a los problemas haciendo referencia a los siguientes campos en un filtro de problemas:

* Usuarios de asignación
* Roles de asignación
* Equipo

## Mostrar todos los usuarios y las funciones asociados a un portafolio

Puede mostrar todos los usuarios y funciones asociados a un portafolio mostrándolos en un informe de proyecto y luego agrupando el informe por Portafolio.

Para obtener información sobre cómo generar un informe de proyecto para mostrar todos los usuarios y sus funciones en el proyecto, consulte [Ver: lista de usuarios de proyecto con funciones](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

No puede filtrar por usuarios o funciones asociados a proyectos en un portafolio o filtro de proyecto.

## Mostrar todos los usuarios y las funciones asociados a un programa

Puede mostrar todos los usuarios y funciones asociados a un programa mostrándolos en un informe de proyecto y, a continuación, agrupando el informe por programa.

Para obtener información sobre cómo generar un informe de proyecto para mostrar todos los usuarios y sus funciones en el proyecto, consulte [Ver: lista de usuarios de proyecto con funciones](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

No puede filtrar por usuarios o funciones asociados a proyectos en un filtro de programa o proyecto.
