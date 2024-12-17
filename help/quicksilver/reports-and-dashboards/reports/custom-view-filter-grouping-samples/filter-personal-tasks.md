---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: Tareas personales'
description: Este filtro de tareas devuelve solicitudes de trabajo ad hoc enviadas a un usuario o elementos pendientes agregados por usuarios en su área de Inicio. Las tareas personales no están conectadas a un proyecto, pero se pueden mover a un proyecto si es necesario.
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 29%

---

# Filtro: tareas personales

<!--Audited: 10/2024-->

Este filtro de tareas devuelve solicitudes de trabajo ad hoc enviadas a un usuario o elementos pendientes agregados por usuarios en el widget Tareas pendientes en el área de Inicio.

Las solicitudes de trabajo ad hoc y los elementos pendientes se guardan en Adobe Workfront como tareas personales.

Las tareas personales no están conectadas a un proyecto, pero se pueden mover a un proyecto si es necesario. Para obtener más información, consulte [Crear tareas personales](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

![](assets/personal-tasks-report.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
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

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar tareas personales

Para crear este filtro:

1. Ir a una lista de tareas o a un informe de tareas.
1. En el menú desplegable **Filtro**, haga clic en **Nuevo filtro**.
1. (Condicional) Haga clic en **Agregar una regla de filtro** si está teniendo acceso al filtro desde un informe, o comience a seleccionar los criterios de filtro en el primer campo si está teniendo acceso al filtro desde una lista.
1. (Condicional) Seleccione los siguientes criterios de filtrado:

   * De un filtro de lista: **Tarea** > **Personal** **Es verdadera**
   * De un filtro de informe: **Tarea** > **Personal** > **Igual (distingue mayúsculas de minúsculas)** > **Verdadero**.
1. Guarde el filtro.

   La lista muestra únicamente las tareas personales que no están en ningún proyecto.
