---
title: Visualización de las tareas en vuelo en Análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización Tareas en vuelo muestra cuántas tareas (dentro de los criterios de filtro aplicados) están en curso para un proyecto, el porcentaje de trabajo completado para cada tarea y cómo de programadas están las tareas.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 4%

---

# Visualización de las tareas en vuelo en Análisis mejorado

La visualización Tareas en vuelo muestra cuántas tareas (dentro de los criterios de filtro aplicados) están en curso para un proyecto, el porcentaje de trabajo completado para cada tarea y cómo de programadas están las tareas.

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan Adobe Workfront</a>*</td> 
   <td> <p>Empresa o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias de Adobe Workfront</a>*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a proyectos</p> <p>Ver el acceso a las tareas (para actualizar tareas, necesita tener acceso de edición a las tareas).</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permiso para objetos de proyecto y de tarea</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte la sección &quot;Requisitos previos&quot; en [Descripción general del análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprensión de las tareas en la visualización de vuelo

La visualización Tareas en plan de vuelo muestra los siguientes detalles de la tarea:

* **Duración planificada de la tarea**: La longitud de una barra de tareas indica la duración planificada, que se basa en la fecha de inicio y de finalización de la tarea.

  ![](assets/tasks-in-flight-duration-350x80.png)

* **Trabajo completado**: El color azul oscuro de una barra de tareas indica la cantidad de trabajo completado de una tarea. Este porcentaje de finalización se muestra a la derecha de la barra de tareas.

  ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **Esfuerzo de trabajo restante**: el color azul claro de una barra de tareas indica la cantidad de trabajo que debe completarse para una tarea.

  ![](assets/tasks-in-flight-light-blue-350x35.png)

Esta información puede ayudarle a determinar lo siguiente:

* Donde se ha centrado el esfuerzo de trabajo.
* Qué tareas podrían estar poniendo en riesgo un proyecto.
* Cuánto falta para completar una tarea.
* Con quién debe hablar acerca de una tarea específica.

Para obtener los mejores datos para esta visualización, consulte [Descripción general del análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualización de las tareas en la visualización de vuelo

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png) y, a continuación, seleccione **Analytics**.
1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en el análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desee utilizar.

   Para obtener más información sobre cómo agregar filtros en el análisis mejorado, consulte [Aplicar filtros en el análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. En la visualización Plan de vuelo o Diagrama de árbol del proyecto, haga clic en un proyecto para ver más información.

   Se muestran las visualizaciones Evolución y Tareas en vuelo.

   >[!NOTE]
   >
   >Para obtener más información sobre estas otras visualizaciones, consulte:
   >
   >   
   >   
   >   * [Ver la visualización del plan de vuelo en el análisis mejorado](../enhanced-analytics/flight-plan-overview.md)
   >   * [Ver la visualización del diagrama de proyecto en el análisis mejorado](../enhanced-analytics/project-treemap-overview.md)
   >   * [Ver la visualización de evolución en el análisis mejorado](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de periodo de tiempo.

   ![](assets/timeframe-filter-350x220.png)

1. (Opcional) Para cambiar la forma en que se ordenan las tareas, haga clic en el menú **Ordenar por** y, a continuación, seleccione una nueva opción de ordenación:

   * **Fecha de finalización**
   * **Alfabéticamente A-Z**
   * **Estructura de desglose de trabajo** (Esta opción coincide con el orden en que aparecen las tareas en el proyecto).

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de ordenación.

1. Revise el progreso de las tareas en el proyecto seleccionado y, a continuación, pase el ratón sobre una tarea específica para ver la cantidad de horas planificadas, la fecha de vencimiento planificada y el porcentaje de finalización.

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. Haga clic en una tarea para abrir los detalles de la tarea en la parte derecha de la pantalla, donde puede ver más información sobre la tarea, ver o introducir actualizaciones, o realizar cambios en la tarea.

   ![](assets/task-details-qs-350x675.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el **icono Exportar** ![](assets/export.png) en la esquina superior derecha de la visualización y, a continuación, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

