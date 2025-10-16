---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Descripción general de la ruta crítica del proyecto
description: La determinación de la ruta crítica de un proyecto es una forma automática para que Adobe Workfront marque una secuencia de tareas en un proyecto que puedan afectar a la cronología del proyecto. Las tareas que pueden afectar a la cronología del proyecto se marcan como tareas de ruta crítica.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 5%

---

# Información general sobre la ruta crítica del proyecto

<!-- Audited: 5/2025 -->

La determinación de la ruta crítica de un proyecto es una forma automática para que Adobe Workfront marque una secuencia de tareas en un proyecto que puedan afectar a la cronología del proyecto. Las tareas que pueden afectar a la cronología del proyecto se marcan como tareas de ruta crítica.

Las siguientes funciones pueden afectar a la ruta crítica de un proyecto:

* La estructura de desglose de trabajo del proyecto.

  Para obtener más información, vea [Determinar la estructura de desglose de trabajo en un proyecto](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md).

* Tiempo (duración) que tarda cada tarea en completarse.
* Dependencias entre las tareas.

  Tenga en cuenta lo siguiente:

   * Cuando una tarea de la ruta crítica tiene una relación de predecesora, sus predecesoras y sucesoras también se encuentran en la ruta crítica si los cambios en las fechas de las predecesoras o sucesoras afectan directamente a sus dependientes.

     >[!TIP]
     >
     >Cuando la fecha sucesora de una tarea no afecta directamente a la fecha de sus tareas dependientes o a las fechas del proyecto, la tarea sucesora no se encuentra en la ruta crítica.
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * Cuando una subtarea se identifica como una tarea de ruta crítica, la tarea principal también se identifica como una tarea de ruta crítica si la fecha de inicio proyectada y la hora de la tarea principal son las mismas que la de la subtarea.

Teniendo en cuenta estas características, el sistema calcula la ruta crítica utilizando la ruta más larga entre la tarea más temprana y la tarea que determina el final del proyecto. El cálculo de ruta crítica tiene en cuenta cuál es la hora más temprana y la más reciente en la que cada tarea puede comenzar y finalizar sin alargar el proyecto. Este proceso determina qué tareas son &quot;críticas&quot; (y pertenecen a la ruta más larga) y cuáles tienen &quot;flotación total&quot; (se puede retrasar sin hacer que el proyecto sea más largo).

Cualquier retraso en la actividad de una tarea en la ruta crítica afecta directamente a la fecha proyectada de finalización del proyecto (no hay flotante en la ruta crítica).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Estándar<p>
   <p>Trabajo o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a Tareas</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores en una tarea </p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on a task </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Ver la ruta crítica

Puede ver las tareas que pertenecen a la ruta crítica en las siguientes áreas de la aplicación de Workfront:

* [Ver la ruta crítica en el gráfico Gantt](#view-the-critical-path-in-the-gantt-chart)
* [Ver la ruta crítica en una lista de tareas o un informe](#view-the-critical-path-in-a-task-list-or-report)

### Ver la ruta crítica en el gráfico Gantt {#view-the-critical-path-in-the-gantt-chart}

Para ver las tareas de la ruta crítica en el diagrama de Gantt:

{{step1-to-projects}}

1. En la lista de proyectos, seleccione un proyecto.

1. En el panel izquierdo, haga clic en **Tareas**. Se abre la pestaña **Tareas**.

1. En la esquina superior derecha de la lista de tareas, haga clic en el icono **Diagrama de Gantt**.

   ![gantt_chart_icon__1_.png](assets/gantt-icon.png)

1. En la esquina superior derecha de la sección del gráfico Gantt, haga clic en el icono **Opciones** ![icono de opciones](assets/options-icon.png) y, a continuación, seleccione la opción **Ruta crítica** en la lista desplegable que aparece. Las tareas que se encuentran en la Ruta crítica ahora tienen una línea roja sobre su cronología.

   ![ruta_crítica_en_Gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Ver la ruta crítica en una lista de tareas o un informe {#view-the-critical-path-in-a-task-list-or-report}

Para ver qué tareas se encuentran en la ruta crítica en una lista de tareas:

{{step1-to-projects}}

1. En la lista de proyectos, seleccione un proyecto.

1. En el panel izquierdo, haga clic en **Tareas**. Se abre la pestaña **Tareas**.

1. Haga clic en el icono **Ver** ![Ver icono](assets/view-icon.png) y, a continuación, seleccione **Estado**. Las tareas que se encuentran en la ruta crítica muestran el indicador **Ruta crítica** en la columna **Indicadores** de la lista.

   O

   Haga clic en el icono **Filtro** ![Icono de filtros](assets/filters-icon.png) y, a continuación, seleccione **+ Nuevo filtro**.
1. En el primer campo, escriba *Es crítico* y, a continuación, selecciónelo cuando aparezca en la sección **Tareas** de la lista.

   ![La tarea es un filtro esencial](assets/task-is-critical.png)

1. Asegúrese de que **Es verdadero** esté seleccionado en el segundo menú desplegable.

   ![Es una lista desplegable de verdadero](assets/critical-path-filter.png)

1. Cierre el panel Filtros. La lista de tareas ahora solo muestra las tareas que se encuentran en la ruta crítica.
