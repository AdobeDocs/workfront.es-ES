---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Vea la visualización del diagrama de proyecto en el análisis mejorado
description: La visualización del diagrama de proyecto es una vista de horas (o días) que se han trabajado en una ventana de tiempo específica en comparación con otros esfuerzos de trabajo en tamaño. Esto le ayuda a comprender cuánto tiempo han dedicado las personas a un proyecto.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 2%

---

# Vea la visualización del diagrama de proyecto en el análisis mejorado

<!-- Audited: 12/2023 -->

La visualización del diagrama de proyecto es una vista de horas (o días) que se han trabajado en una ventana de tiempo específica en comparación con otros esfuerzos de trabajo en tamaño. Esto le ayuda a comprender cuánto tiempo han dedicado las personas a un proyecto.

![](assets/project-treemap-350x126.png){width="700"}

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan de Adobe Workfront</a></td> 
   <td> <p>Empresa o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias de Adobe Workfront</a></td> 
   <td>   <p>Nuevo:</p> 
   <ul><li>Ligero o superior</li></ul>
   <p>Actual:</p>
   <ul><li>Revisar o superior</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Ver acceso a proyectos</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte la sección &quot;Requisitos previos&quot; en [Descripción general del análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprender la visualización del diagrama de proyecto

Los cuadros de la visualización Diagrama de árbol del proyecto representan proyectos y el tamaño de los cuadros muestra una comparación de cuánto tiempo se ha invertido en diferentes proyectos. Cuanto más grande sea la casilla, más tiempo se dedicará al proyecto.

La visualización del diagrama de proyecto consta de:

* **Cuadros más pequeños de color azul claro**: Los proyectos que tienen menos horas o días se muestran como cuadros más pequeños de color azul claro.

  ![](assets/project-treemap-smaller-box.png)

* **Cuadros azules oscuros más grandes**: Los proyectos que tienen más horas o días se muestran como cuadros más grandes con un color azul oscuro.

  ![](assets/project-treemap-larger-box-350x205.png)

* **Cuadros azules de tamaño Medium**: Los proyectos que se encuentran entre las dos categorías se muestran como cuadros de tamaño mediano con un tono azul entre los colores azul oscuro y azul claro. Hay 3 posibles tonos de azul para las cajas de tamaño mediano.

La leyenda de la derecha muestra un desglose de las horas completadas para cada tono de azul. Esta leyenda es dinámica y se actualiza según los datos.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Si está viendo la visualización del diagrama de proyecto por duración en lugar de por horas planificadas, esta leyenda muestra un desglose de los días trabajados para cada tono de azul.\
>![](assets/project-treemap-days-worked.png)>

Ver esta información le ayuda a determinar lo siguiente:

* Prioridad de los elementos en los que se trabaja durante el intervalo de fechas seleccionado.
* En qué equipos invierten el tiempo.
* Si los equipos se centran en las cosas correctas.
* Cuando se hace clic en un proyecto específico, cuánto cambió el ámbito de un proyecto durante ese período de tiempo.

Para obtener los mejores datos para esta visualización, consulte [Descripción general del análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Ver la visualización del diagrama de proyecto

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png) y, a continuación, seleccione **Analytics**.
1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en el análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desee utilizar.

   Para obtener más información sobre cómo agregar filtros en el análisis mejorado, consulte [Aplicar filtros en el análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para cambiar la forma en que se ordenan los proyectos, haga clic en el menú **Ordenar por** en la esquina superior derecha de la visualización del diagrama de proyecto y, a continuación, seleccione una nueva opción de ordenación:

   * **A - Z**
   * **Z - A**
   * **Fecha planificada de finalización**
   * **Fecha planificada de inicio**

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de ordenación.

1. (Condicional) Si hay más de 50 proyectos en el conjunto de datos, utilice las flechas de la esquina inferior izquierda de la visualización para desplazarse de un grupo de 50 proyectos al siguiente.

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de página.

   ![](assets/pagination-350x118.png)

1. (Opcional) Cambie la vista de **horas planificadas** a **duration**.

   Las horas planificadas están seleccionadas de forma predeterminada.

1. Pase el ratón sobre un proyecto para ver su condición, así como la cantidad de horas planificadas totales, la cantidad de horas completadas totales y la cantidad promedio de horas invertidas en el proyecto por día.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Si seleccionó la vista **duration**, verá los siguientes detalles de duración:
   >
   >* **Plazo planificado**: La cantidad de días planificados para completar el proyecto.
   >* **Días trabajados**: duración planeada de cada tarea que se completó dentro del intervalo de fechas seleccionado en la parte superior, dividida por el número de horas en un día.
   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >Para obtener más información sobre la duración, consulte la sección &quot;Vista de duración&quot; en [Descripción general del análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Opcional) Para exportar los datos de visualización, haga clic en el **icono Exportar** ![](assets/export.png) en la esquina superior derecha de la visualización y, a continuación, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

1. Haga clic en un proyecto para abrir las visualizaciones Evolución y tareas en vuelo para obtener una perspectiva más detallada de cómo las tareas y las horas, o los días, contribuyeron al tamaño de un proyecto.

Para obtener más información sobre la visualización de evolución, consulte [Ver la visualización de evolución en Análisis mejorado](../enhanced-analytics/burndown-overview.md). Para obtener más información sobre la visualización de Tareas en vuelo, consulte [Ver la visualización de Tareas en vuelo en Análisis mejorado](../enhanced-analytics/tasks-in-flight-overview.md).

