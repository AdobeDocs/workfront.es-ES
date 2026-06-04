---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: Tareas personales'
description: Este filtro de tareas devuelve solicitudes de trabajo ad hoc enviadas a un usuario o elementos pendientes agregados por usuarios en su área de Inicio. Las tareas personales no están conectadas a un proyecto, pero se pueden mover a un proyecto si es necesario.
author: Courtney
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/qh9Tp3JY32C-GL2U5ucjapeVoR4dKq0F8K6lysGiOag
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 296
ht-degree: 22%

---

# Filtro: tareas personales

<!--Audited: 10/2024-->

Este filtro de tareas devuelve solicitudes de trabajo ad hoc enviadas a un usuario o elementos pendientes agregados por usuarios en el widget Tareas pendientes en el área de Inicio.

Las solicitudes de trabajo ad hoc y los elementos pendientes se guardan en Adobe Workfront como tareas personales.

Las tareas personales no están conectadas a un proyecto, pero se pueden mover a un proyecto si es necesario. Para obtener más información, consulte [Crear tareas personales](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

![Informe de tareas personales](assets/personal-tasks-report.png)

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
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
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
