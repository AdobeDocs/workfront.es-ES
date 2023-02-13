---
title: Visualización del plan de vuelo en Análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización del plan de vuelo muestra cuántos proyectos (dentro de los criterios de filtro aplicados) estaban en fuga, qué cambios de condición se produjeron a lo largo de la vida de estos proyectos y cuán cerca se ajustaron a los plazos de finalización planeados.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# Visualización del plan de vuelo en Análisis mejorado

La visualización del plan de vuelo muestra cuántos proyectos (dentro de los criterios de filtro aplicados) estaban en fuga, qué cambios de condición se produjeron a lo largo de la vida de estos proyectos y cuán cerca se ajustaron a los plazos de finalización planeados.

![](assets/flight-plan-350x132.png)

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
   <td> <p>Ver acceso al proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte la sección &quot;Requisitos previos&quot; en [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprender la visualización del plan de vuelo

En la duración real de un proyecto, solo puede ver las siguientes condiciones del proyecto:

* Bien encaminado
* En riesgo
* Con problemas

Para obtener más información sobre las condiciones del proyecto, consulte [Descripción general de la condición y el tipo de condición del proyecto](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

La visualización del plan de vuelo muestra los siguientes detalles del proyecto:

* **Duración prevista**: La línea azul horizontal representa la longitud planificada del proyecto, con triángulos en cualquier extremo de la línea que indican la fecha de inicio y la fecha de finalización.

   ![](assets/planned-duration-line-350x37.png)

* **Duración real**: La línea gruesa y de color debajo de la duración planificada representa la duración real del proyecto. El color de la línea cambia dependiendo de la condición del proyecto en ese momento en particular en la vida del proyecto.

   ![](assets/actual-duration-line.png)

* **Condición real**: La línea gruesa y de color también muestra la condición de un proyecto en diferentes momentos del tiempo. El color de la línea cambia según la condición del proyecto:

   * **Verde**: En Target
   * **Naranja**: En riesgo
   * **Rojo**: En problemas

   ![](assets/actual-condition-color.png)

Al pasar el ratón por encima de una fila de proyecto en la visualización del plan de vuelo, puede ver información sobre el marco de tiempo planificado del proyecto, la condición del proyecto actual y, si corresponde, la condición personalizada. Para obtener una vista más detallada de lo que puede haber afectado a la duración o condición, puede ver las otras visualizaciones del área Análisis mejorado .

Ver esta información le ayuda a determinar:

* Qué eventos extienden un proyecto más allá de la fecha de finalización planeada original.
* Cuando un proyecto empieza a tener problemas.
* Cuántos proyectos están abiertos durante el mismo período de tiempo.
* ¿Cuántos proyectos están activos?
* Qué proyectos necesitan atención o apoyo extra.

Para obtener información sobre cómo obtener los mejores datos para esta visualización, consulte [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualización del plan de vuelo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desee utilizar.

   Para obtener más información sobre la adición de filtros en Análisis mejorado, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de intervalo de tiempo.

   ![](assets/timeframe-filter-350x220.png)

1. (Opcional) Para cambiar la forma en que se ordenan los proyectos, haga clic en el **Ordenar por** en la esquina superior derecha de la visualización del plan de vuelo y, a continuación, seleccione una nueva opción de clasificación:

   * **A-Z**
   * **Z-A**
   * **Fecha de finalización planificada**
   * **Fecha de inicio planificada**

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con su selección de clasificación.

1. (Condicional) Si hay más de 50 proyectos en el conjunto de datos, utilice las flechas de la esquina inferior izquierda de la visualización para ir de un grupo de 50 proyectos al siguiente.

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de la página.

   ![](assets/pagination-350x118.png)

1. Pase el ratón sobre el gráfico de la barra del proyecto para ver la línea de fecha azul, así como los siguientes detalles:

   * Plazo planificado
   * Condición actual
   * Condición personalizada (si corresponde)

   ![](assets/project-bar-graph-350x143.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el **Exportar** icono ![](assets/export.png) en la esquina superior derecha de la visualización, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

1. Para ver más información del proyecto, haga clic en un proyecto de la visualización para abrir las visualizaciones Desglosar y Tareas en vuelo .

   Estas visualizaciones pueden ayudarle a comprender mejor qué ha hecho que el proyecto se desrastree. También facilitan la facturación de un proyecto en curso.\
   Para obtener más información sobre la visualización Desglose, consulte [Visualización de la visualización de Desglose en Análisis mejorado](../enhanced-analytics/burndown-overview.md). Para obtener más información sobre las tareas en la visualización de vuelo, consulte [Ver las tareas en la visualización de vuelo en Análisis mejorado](../enhanced-analytics/tasks-in-flight-overview.md).

