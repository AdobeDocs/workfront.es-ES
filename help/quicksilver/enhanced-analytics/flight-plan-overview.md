---
title: Visualización del plan de vuelo en el análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización del plan de vuelo muestra cuántos proyectos (dentro de los criterios de filtro aplicados) estaban en vuelo, qué cambios de condición ocurrieron a lo largo de la vida de estos proyectos y en qué medida se ajustaron estos proyectos a los plazos de finalización planificados.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 4%

---

# Visualización del plan de vuelo en el análisis mejorado

La visualización del plan de vuelo muestra cuántos proyectos (dentro de los criterios de filtro aplicados) estaban en vuelo, qué cambios de condición ocurrieron a lo largo de la vida de estos proyectos y en qué medida se ajustaron estos proyectos a los plazos de finalización planificados.

![](assets/flight-plan-350x132.png)

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
   <td> <p>Ver acceso a proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso al proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte la sección &quot;Requisitos previos&quot; en [Descripción general del análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprender la visualización del plan de vuelo

En la duración real de un proyecto, solo puede ver las siguientes condiciones de proyecto:

* Bien encaminado
* En riesgo
* Con problemas

Para obtener más información sobre las condiciones del proyecto, consulte [Información general sobre la condición del proyecto y el tipo de condición](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

La visualización del plan de vuelo muestra los siguientes detalles del proyecto:

* **Duración planificada**: la línea azul horizontal representa la longitud planificada del proyecto, con los triángulos al final de la línea que indican la fecha de inicio y la fecha de finalización.

  ![](assets/planned-duration-line-350x37.png)

* **Duración real**: la línea gruesa y coloreada debajo de la duración planeada representa la duración real del proyecto. El color de la línea cambia según la condición del proyecto en ese momento en particular de la duración del proyecto.

  ![](assets/actual-duration-line.png)

* **Condición real**: la línea gruesa y coloreada también muestra la condición de un proyecto en diferentes momentos del tiempo. El color de la línea cambia según la condición del proyecto:

   * **Verde**: en el destino
   * **Naranja**: En riesgo
   * **Rojo**: con problemas

  ![](assets/actual-condition-color.png)

Al pasar el ratón por encima de una fila del proyecto en la visualización Plan de vuelo, puede ver información sobre el periodo de tiempo planificado del proyecto, la condición del proyecto actual y, si corresponde, la condición personalizada. Para obtener una vista más detallada de lo que puede haber afectado a la duración o condición, puede ver las otras visualizaciones en el área de Análisis mejorado.

Ver esta información le ayuda a determinar lo siguiente:

* Los eventos que extienden un proyecto más allá de la fecha planificada de finalización original.
* Cuándo un proyecto empieza a tener problemas.
* Cuántos proyectos están abiertos durante el mismo período de tiempo.
* Cuántos proyectos están activos.
* Qué proyectos necesitan atención o apoyo extra.

Para obtener información sobre cómo obtener los mejores datos para esta visualización, consulte [Descripción general del análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualización de la visualización Plan de vuelo

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon-16x12.png) y luego seleccione **Analytics**.
1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en el análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desee utilizar.

   Para obtener más información sobre cómo agregar filtros en el análisis mejorado, consulte [Aplicar filtros en el análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de periodo de tiempo.

   ![](assets/timeframe-filter-350x220.png)

1. (Opcional) Para cambiar la forma en que se ordenan los proyectos, haga clic en el menú **Ordenar por** en la esquina superior derecha de la visualización Plan de vuelo y, a continuación, seleccione una nueva opción de clasificación:

   * **A - Z**
   * **Z - A**
   * **Fecha planificada de finalización**
   * **Fecha planificada de inicio**

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de ordenación.

1. (Condicional) Si hay más de 50 proyectos en el conjunto de datos, utilice las flechas de la esquina inferior izquierda de la visualización para desplazarse de un grupo de 50 proyectos al siguiente.

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de página.

   ![](assets/pagination-350x118.png)

1. Pase el ratón sobre el gráfico de barras del proyecto para ver la línea de fecha azul y los siguientes detalles:

   * Cronología planificada
   * Condición actual
   * Condición personalizada (si corresponde)

   ![](assets/project-bar-graph-350x143.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el icono **Exportar** ![](assets/export.png) en la esquina superior derecha de la visualización y, a continuación, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

1. Para ver más información sobre el proyecto, haga clic en un proyecto de la visualización para abrir las visualizaciones Evolución y Tareas en vuelo.

   Estas visualizaciones pueden ayudarle a obtener un conocimiento más profundo de lo que provocó que el proyecto se saliera de la pista. También facilitan el registro de un proyecto en curso.\
   Para obtener más información sobre la visualización de evolución, consulte [Ver la visualización de evolución en Análisis mejorado](../enhanced-analytics/burndown-overview.md). Para obtener más información sobre la visualización de Tareas en vuelo, consulte [Ver la visualización de Tareas en vuelo en Análisis mejorado](../enhanced-analytics/tasks-in-flight-overview.md).

