---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Información general sobre la ruta crítica del proyecto
description: La determinación de la ruta crítica de un proyecto es una forma automática para que Adobe Workfront marque una secuencia de tareas en un proyecto que puedan afectar a la cronología del proyecto. Las tareas que pueden afectar a la cronología del proyecto se marcan como tareas de ruta crítica.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# Información general sobre la ruta crítica del proyecto

La determinación de la ruta crítica de un proyecto es una forma automática para que Adobe Workfront marque una secuencia de tareas en un proyecto que puedan afectar a la cronología del proyecto. Las tareas que pueden afectar a la cronología del proyecto se marcan como tareas de ruta crítica.

Las siguientes funciones pueden afectar a la ruta crítica de un proyecto:

* La estructura de desglose de trabajo del proyecto.

  Para obtener más información acerca de la estructura de desglose de trabajo, vea [Determinar la estructura de desglose de trabajo en un proyecto](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* Tiempo (duración) que tarda cada tarea en completarse.
* Dependencias entre las tareas.

  Tenga en cuenta lo siguiente:

   * Cuando una tarea de la ruta crítica tiene una relación de predecesora, sus predecesoras y sucesoras también se encuentran en la ruta crítica si los cambios en las fechas de las predecesoras o sucesoras afectan directamente a sus dependientes.

     >[!TIP]
     >
     >Cuando la fecha del sucesor de una tarea no afecta directamente a la fecha de sus tareas dependientes y no afecta a las fechas del proyecto, la tarea sucesora no se encuentra en la ruta crítica.
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * Cuando una subtarea se identifica como una tarea de ruta crítica, la tarea principal también se identifica como una tarea de ruta crítica, si la fecha y hora de inicio proyectadas de la tarea principal es la misma que la de la subtarea.

Teniendo en cuenta estas características, el sistema calcula la ruta crítica utilizando la ruta más larga entre la tarea más temprana y la tarea que determina el final del proyecto. El cálculo de ruta crítica tiene en cuenta cuál es la hora más temprana y la más reciente en la que cada tarea puede comenzar y finalizar sin alargar el proyecto. Este proceso determina qué tareas son &quot;críticas&quot; (y pertenecen a la ruta más larga) y cuáles tienen &quot;flotación total&quot; (se puede retrasar sin hacer que el proyecto sea más largo).

Cualquier retraso en la actividad de una tarea en la ruta crítica afecta directamente a la fecha proyectada de finalización del proyecto (no hay flotante en la ruta crítica).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización o superior a Tareas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores en una tarea </p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ver la ruta crítica

Puede ver las tareas que pertenecen a la ruta crítica en las siguientes áreas de la aplicación de Workfront:

* [Ver la ruta crítica en el gráfico Gantt](#view-the-critical-path-in-the-gantt-chart)
* [Ver la ruta crítica en una lista de tareas o un informe](#view-the-critical-path-in-a-task-list-or-report)

### Ver la ruta crítica en el gráfico Gantt {#view-the-critical-path-in-the-gantt-chart}

Para ver las tareas de la ruta crítica en el diagrama de Gantt:

1. Vaya a un proyecto para el que desee ver la ruta crítica.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Haga clic en el icono **Diagrama de Gantt** en la esquina superior derecha de la lista de tareas.

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. Expanda el menú **Opciones** y, a continuación, habilite la opción **Ruta crítica**.

   Las tareas que se encuentran en la ruta crítica tienen una línea roja sobre su escala de tiempo en el gráfico Gantt.

   ![ruta_crítica_en_Gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Ver la ruta crítica en una lista de tareas o un informe {#view-the-critical-path-in-a-task-list-or-report}

Para ver qué tareas se encuentran en la ruta crítica en una lista de tareas:

1. Vaya a un proyecto para el que desee ver la ruta crítica.
1. Haga clic en **Tareas** en el panel izquierdo.
1. En el menú desplegable **Ver**, seleccione **Estado**.

   Las tareas que se encuentran en la ruta crítica tienen el indicador **Ruta crítica** en la columna **Indicadores** de la lista.

   Puede aplicar la misma vista a un informe de tareas.

   Para obtener más información acerca de la creación de informes, vea el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   O

   En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.

1. Haga clic en **Agregar regla de filtro** y empiece a escribir **Es crítico** en **Mostrar solo tareas en las que el campo ...**.

1. Selecciónelo cuando aparezca en la lista.
1. Haga clic en **Guardar filtro**.

   La lista solo debe mostrar las tareas que se encuentran en la ruta crítica.
