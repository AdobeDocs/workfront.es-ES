---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Ver la visualización del diagrama de árbol del proyecto en Análisis mejorado
description: La visualización del diagrama de árbol del proyecto es una vista de horas (o días) que se han trabajado en una ventana de tiempo específica en comparación con otros esfuerzos de trabajo en tamaño. Esto le ayuda a comprender cuánto tiempo han dedicado las personas a un proyecto.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# Ver la visualización del diagrama de árbol del proyecto en Análisis mejorado

La visualización del diagrama de árbol del proyecto es una vista de horas (o días) que se han trabajado en una ventana de tiempo específica en comparación con otros esfuerzos de trabajo en tamaño. Esto le ayuda a comprender cuánto tiempo han dedicado las personas a un proyecto.

![](assets/project-treemap-350x126.png)

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan de Adobe Workfront</a>*</td> 
   <td> <p>Negocios o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Vista</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte la sección &quot;Requisitos previos&quot; en [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprender la visualización del diagrama de árbol del proyecto

Los cuadros de la visualización de diagrama de árbol del proyecto representan los proyectos y el tamaño de los cuadros muestra una comparación de cuánto tiempo se ha invertido en diferentes proyectos. Cuanto más grande sea la caja, más tiempo se invierte en el proyecto.

La visualización del diagrama de árbol del proyecto consta de:

* **Cuadros azules más pequeños**: Los proyectos con menos horas (o días) se muestran como cuadros más pequeños con un color azul claro.

   ![](assets/project-treemap-smaller-box.png)

* **Cuadros azules más grandes y oscuros**: Los proyectos que tienen más horas (o días) se muestran como cuadros más grandes con un color azul oscuro.

   ![](assets/project-treemap-larger-box-350x205.png)

* **Cuadros azules de tamaño medio**: Los proyectos comprendidos entre las dos categorías se muestran como cajas de tamaño mediano con un tono azul entre el azul oscuro y el azul claro. Las cajas de tamaño mediano pueden tener tres tonos azules.

La leyenda de la derecha muestra un desglose de horas completadas para cada sombra azul. Esta leyenda es dinámica y se actualiza según los datos.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Si está viendo la visualización del diagrama de árbol del proyecto por duración en lugar de por horas planificadas, esta leyenda muestra un desglose de los días trabajados para cada sombra de azul.\
>![](assets/project-treemap-days-worked.png)>

Ver esta información le ayuda a determinar:

* Prioridad de los elementos en los que se trabaja durante el intervalo de fechas seleccionado.
* En qué equipos se está gastando tiempo.
* Si los equipos se centran en las cosas correctas.
* Cuando se hace clic en un proyecto específico, ¿cuánto ha cambiado el alcance de un proyecto durante ese período de tiempo?

Para obtener información sobre cómo obtener los mejores datos para esta visualización, consulte [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Ver la visualización del diagrama de árbol del proyecto

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desee utilizar.

   Para obtener más información sobre la adición de filtros en Análisis mejorado, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para cambiar la forma en que se ordenan los proyectos, haga clic en el **Ordenar por** en la esquina superior derecha de la visualización del diagrama de árbol del proyecto y, a continuación, seleccione una nueva opción de clasificación:

   * **A-Z**
   * **Z-A**
   * **Fecha de finalización planificada**
   * **Fecha de inicio planificada**

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con su selección de clasificación.

1. (Condicional) Si hay más de 50 proyectos en el conjunto de datos, utilice las flechas de la esquina inferior izquierda de la visualización para ir de un grupo de 50 proyectos al siguiente.

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de la página.

   ![](assets/pagination-350x118.png)

1. (Opcional) Cambiar la vista de **horas planificadas** a **duration**.

   Las horas planificadas están seleccionadas de forma predeterminada.

1. Pase el ratón sobre un proyecto para ver la condición del proyecto, así como el número total de horas planificadas, el número total de horas completadas y el número promedio de horas dedicadas al proyecto por día.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Si seleccionó la variable **duration** , verá los siguientes detalles de duración:
   >
   >* **Intervalo de tiempo planeado**: Número de días previstos para completar el proyecto.
   >* **Días trabajados**: La duración planeada para cada tarea que se completó dentro del intervalo de fechas seleccionado en la parte superior, dividido por el número de horas en un día.

   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >Para obtener más información sobre la duración, consulte la sección &quot;Vista de duración&quot; en [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Opcional) Para exportar los datos de visualización, haga clic en el **Icono de exportación** ![](assets/export.png) en la esquina superior derecha de la visualización, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

1. Haga clic en un proyecto para abrir las visualizaciones Desglose y Tareas en vuelo para obtener una perspectiva más profunda de cómo las tareas y las horas (o días) contribuyeron al tamaño de un proyecto.

Para obtener más información sobre la visualización Desglose, consulte [Visualización de la visualización de Desglose en Análisis mejorado](../enhanced-analytics/burndown-overview.md). Para obtener más información sobre las tareas en la visualización de vuelo, consulte [Ver las tareas en la visualización de vuelo en Análisis mejorado](../enhanced-analytics/tasks-in-flight-overview.md).

