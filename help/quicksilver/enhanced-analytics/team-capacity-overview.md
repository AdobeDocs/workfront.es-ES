---
title: Vea la visualización de la capacidad Equipo en el análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización de la capacidad del equipo muestra la cantidad total de capacidad que tiene un equipo de inicio, si está sobreasignada o infraasignada, y la dinámica de la capacidad a lo largo del tiempo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 81118e794dca746b482b8355c24fa997a9f0edc9
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 4%

---

# Vea la visualización de la capacidad Equipo en el análisis mejorado

<!-- Audited: 01/2024 -->

La visualización de la capacidad del equipo muestra la cantidad total de capacidad que tiene un equipo de inicio, si está sobreasignada o infraasignada, y la dinámica de la capacidad a lo largo del tiempo.

![Capacidad del equipo](assets/team-capacity.png)

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
   <td>Ver acceso a proyectos</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Ver </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Para conocer los requisitos previos para utilizar el análisis mejorado, consulte la sección &quot;Requisitos previos&quot; en [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprender la visualización de la capacidad Equipo

La visualización de la capacidad del equipo muestra el volumen de trabajo asignado al equipo de inicio en un día determinado.

* **Burnout**: cuando el color de relleno azul más oscuro está por encima de la línea de puntos, el equipo de inicio tiene más horas de trabajo asignadas de las que puede completar en el número de horas que el equipo está disponible para trabajar. Esto indica que el equipo está sobreasignado y que podría estar acercándose al agotamiento.

  ![Sobrecapacidad](assets/team-capacity-over-capacity.png)

* **Indiscutible**: cuando el color de relleno azul más oscuro está por debajo de la línea de puntos, el equipo de inicio tiene más horas disponibles para trabajar que la cantidad de trabajo asignada a ellos. Esto indica que el equipo está infraasignado y no se puede impugnar.

  ![En capacidad](assets/team-capacity-under-capacity.png)

* **Equilibrio**: cuando el color de relleno azul más claro o más transparente está justo por encima, justo por debajo o en la línea de puntos, el equipo de inicio tiene asignadas una cantidad de horas de trabajo que debe poder completar dentro de sus horas de trabajo disponibles. Esto indica que la carga de trabajo del equipo está más equilibrada.

  ![A capacidad](assets/team-capacity-at-capacity.png)

Al pasar el ratón por encima de cualquier punto de la visualización, se muestran los siguientes detalles de un día determinado:

* **Horas programadas**: este es el número de horas de trabajo planificadas que el equipo necesita completar.
* **Horas disponibles**: Es el número de horas de trabajo que el equipo está disponible para trabajar.
* **Capacidad**: Además de un porcentaje de capacidad, también se muestran las designaciones En capacidad, En capacidad o Sobre capacidad.

Ver esta información le ayuda a determinar lo siguiente:

* Cuando el equipo de inicio estaba sobreasignado o infraasignado.
* Si el equipo de inicio está sobreasignado o subasignado diariamente.
* La consistencia de la carga de trabajo de un equipo local es diaria.
* Si está creando problemas de capacidad con un nuevo trabajo.

Para obtener los mejores datos para esta visualización, consulte [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualización de la visualización de capacidad del equipo

{{step1-to-analytics}}

1. En el panel izquierdo, seleccione **People**.

   ![Seleccionar personas](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![Filtro de intervalo de fechas](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si no ha establecido el filtro Equipo, agregue el filtro Equipo y seleccione cada equipo cuyos datos desee ver.

   Para obtener más información sobre la adición de filtros en el análisis mejorado, consulte [Aplicar filtros en análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. En la visualización Capacidad de los recursos, haga clic en un equipo para ver más información.

   Se muestra la visualización Capacidad del equipo.

   Para obtener más información sobre la visualización de la capacidad de los recursos, consulte [Vea la visualización de la capacidad de los recursos en el análisis mejorado](../enhanced-analytics/resource-capacity-overview.md).

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de periodo de tiempo.

   ![Filtro de intervalo de tiempo](assets/timeframe-filter-350x220.png)

1. Pase el ratón sobre un punto de la línea graficada para ver las horas programadas y planificadas para la fecha determinada, así como el porcentaje de capacidad y si el equipo de inicio estaba por encima, por debajo o en la capacidad en ese momento.

   ![Ventana emergente Capacidad del equipo](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en **Exportar** icono ![Icono Exportar](assets/export.png) en la esquina superior derecha de la visualización, seleccione el formato de exportación:

   * Gráfico (PNG)
   * Tabla de datos (XSLX)

