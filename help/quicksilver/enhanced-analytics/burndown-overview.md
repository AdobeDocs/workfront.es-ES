---
title: Vea la visualización Evolución en el análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización Evolución muestra la evolución de un proyecto específico a lo largo del tiempo y le ayuda a comprender la relación entre las condiciones del proyecto, la velocidad y las horas o días restantes.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Vea la visualización Evolución en el análisis mejorado

<!-- Audited: 12/2023 -->

La visualización Evolución muestra la evolución de un proyecto específico a lo largo del tiempo y le ayuda a comprender la relación entre las condiciones del proyecto, la velocidad y las horas o días restantes.

![Ejemplo de evolución de análisis mejorada](assets/burndown120623.png)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>
      <p>Nuevo: Cualquiera</p>
      <p>o</p>
      <p>Actual: Empresa o superior</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
      <p>Nuevo: claro o superior</p>
      <p>o</p>
      <p>Actual: revisar o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Ver acceso a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Para conocer los requisitos previos para utilizar el análisis mejorado, consulte la sección &quot;Requisitos previos&quot; en [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites).

## Comprender la visualización Evolución

La línea azul continua muestra la velocidad planificada desde la fecha de inicio hasta la fecha planificada de finalización. Esta línea se ajusta a medida que se agrega, elimina o actualiza el trabajo, y cambia a una línea vertical discontinua cuando el proyecto alcanza la fecha planificada de finalización.

![Velocidad planificada](assets/burndown-planned-line.png)

La línea real muestra el número de horas o días empleados en el proyecto a lo largo del tiempo. El color de esta línea indica la condición del proyecto cada día:

* **Verde**: el proyecto está en el destino.

  ![En el destino](assets/burndown-green.png)

* **Naranja**: el proyecto está en riesgo.

  ![En riesgo](assets/burndown-orange.png)

* **Rojo**: el proyecto está en problemas.

  ![En problemas](assets/burndown-red.png)

Para obtener más información sobre estas condiciones de proyecto, consulte [Descripción general de la condición y el tipo de condición del proyecto](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Cuando la línea real se mueve verticalmente, se ha añadido trabajo al proyecto. Cuando la línea se desplaza verticalmente, se ha eliminado o completado el trabajo del proyecto.

Debajo del eje x de la visualización, puede ver más información sobre cómo las tareas y las horas, o los días, cambiaron en un día determinado (la cantidad agregada, la cantidad completada y la diferencia entre los dos).

Ver toda esta información en la visualización de evolución le ayuda a determinar lo siguiente:

* Estado del proyecto individual a lo largo del tiempo
* Impacto en el trabajo planificado de los problemas que se presentaban (o del trabajo no planificado)
* Qué eventos extendieron el proyecto más allá de la fecha de finalización original

Para obtener los mejores datos para esta visualización, consulte [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Ver la visualización de evolución

{{step1-to-analytics}}

1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![Seleccionar fechas](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desee utilizar.

   Para obtener más información sobre la adición de filtros en el análisis mejorado, consulte [Aplicar filtros en análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrástrelo hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea automáticamente un filtro de periodo de tiempo.

   ![Filtro de intervalo de tiempo](assets/timeframe-filter-350x220.png)

1. En la visualización Plan de vuelo o Diagrama de árbol del proyecto, haga clic en un proyecto para ver más información.

   Se muestran las visualizaciones Evolución y Tareas en vuelo.

   >[!NOTE]
   >
   >Para obtener más información sobre estas otras visualizaciones, consulte:
   >
   >   * [Visualización del plan de vuelo en el análisis mejorado](../enhanced-analytics/flight-plan-overview.md)
   >   * [Vea la visualización del diagrama de proyecto en el análisis mejorado](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visualización de las tareas en vuelo en Análisis mejorado](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (Opcional) Cambie la vista de horas planificadas a **duration**.

   Las horas planificadas están seleccionadas de forma predeterminada.

   >[!NOTE]
   >
   >Seleccionar **duration** cambia toda la información de horas a días.\
   >![Evolución de duración](assets/duration-burndown-350x112.png)\
   >Para obtener más información sobre la duración en el área de Análisis mejorado, consulte la sección &quot;Vista de duración&quot; en [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. Haga clic en cualquier punto del gráfico de líneas.

   Se muestra la fecha exacta y más información sobre las tareas y las horas (o días) del día seleccionado debajo del gráfico.

   ![Detalles de evolución](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Si la velocidad real es una línea plana que se ejecuta a lo largo del eje x (en línea con 0 horas o 0 días) de la visualización, significa que no se añadieron horas planificadas (o días) al proyecto.\
   >Si la velocidad real es una línea plana por encima del eje x (en línea con un número de horas o de días) que nunca desciende, significa que no se completó ninguna tarea dentro del período de tiempo filtrado.

1. (Opcional) Para exportar los datos de visualización, haga clic en **Exportar** icono ![Icono Exportar](assets/export.png)en la esquina superior derecha de la visualización y seleccione el formato de exportación:

   * Gráfico (PNG)
   * Tabla de datos (XSLX)

1. (Opcional) Para ver detalles sobre el progreso de las tareas en el proyecto seleccionado, observe la visualización Tareas en vuelo que aparece debajo de la Visualización de evolución. Para obtener más información, consulte [Visualización de las tareas en vuelo en Análisis mejorado](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).
