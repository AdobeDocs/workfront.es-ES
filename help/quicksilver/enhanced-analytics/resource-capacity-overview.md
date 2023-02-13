---
title: Visualización de la capacidad de los recursos en Análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización de la capacidad de los recursos muestra si un equipo ha terminado, se encuentra por debajo o tiene capacidad. Este cálculo se basa en - EDIT ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Visualización de la capacidad de los recursos en Análisis mejorado

La visualización de la capacidad de los recursos muestra si un equipo ha terminado, se encuentra por debajo o tiene capacidad.

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

## Comprender la visualización de la capacidad de los recursos

La visualización de la capacidad de los recursos muestra si un equipo ha terminado, se encuentra por debajo o tiene capacidad. Este cálculo se basa en:

* **Capacidad disponible**: Cantidad total de horas que un equipo doméstico tiene disponibles para trabajar en el período de tiempo filtrado

   >[!NOTE]
   >
   >Si está buscando un período de tiempo futuro, la capacidad disponible se calcula en función de la capacidad del equipo durante los últimos 7 días. Por este motivo, no se tiene en cuenta ningún OPC programado.

* **Capacidad planificada**: Cantidad total de horas de trabajo previstas del equipo de origen en el período de tiempo filtrado

Esta comparación de las horas planificadas y las horas programadas reales de un equipo en casa puede ayudarle a determinar si no está asignando suficiente trabajo al equipo en casa o si puede que se esté produciendo una interrupción del servicio debido a una carga de trabajo pesada.

![](assets/resource-capacity-350x110.png)

En la visualización de la capacidad del recurso , puede ver los siguientes detalles:

* **Capacidad planificada**: En línea con el nombre de un equipo de inicio, el círculo azul representa el número de horas programadas asignadas al equipo de inicio.

   ![](assets/resource-capacity-blue-circle.png)

* **Capacidad real**: En línea con el nombre del equipo de casa, la línea vertical representa el número de horas disponibles para el equipo de casa.

   ![](assets/resource-capacity-vertical-line.png)

* **Sobre la capacidad**: Cuando la línea horizontal y el círculo azul se muestran a la derecha de la línea vertical, se asignó más trabajo al equipo de inicio del que pueden completar en el número de horas disponibles. Esto significa que el equipo puede estar por encima de la capacidad durante el período de tiempo filtrado. El número restante de horas que el equipo necesita completar se muestra a la derecha del círculo azul.

   ![](assets/resource-capacity-over-capacity.png)

* **Bajo capacidad**: Cuando la línea horizontal y el círculo azul se muestran a la izquierda de la línea vertical, el equipo de inicio tiene más horas disponibles que el número de horas de trabajo planificadas que se les asignaron. Esto significa que el equipo puede estar bajo capacidad durante el período de tiempo filtrado. El número adicional de horas disponibles para que el equipo de casa complete el trabajo se muestra a la izquierda del círculo azul.

   ![](assets/resource-capacity-under-capacity.png)

Al pasar el ratón por encima de una fila se muestra el número exacto de horas para la capacidad planificada y la capacidad disponible, así como el número de horas que el equipo en el hogar ha superado o no tiene capacidad.

Ver esta información le ayuda a determinar:

* Si el equipo de origen estaba sobreasignado o subasignado.
* Los proyectos más grandes fueron en los que se concentró el equipo local.
* Qué equipos domésticos están disponibles para el trabajo.

Para obtener información sobre cómo obtener los mejores datos para esta visualización, consulte [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Ver la visualización de la capacidad del recurso

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. En el panel izquierdo, seleccione **People**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si no ha establecido el filtro Equipo , agregue el filtro Equipo y seleccione cada equipo para el que desee ver los datos.

   Para obtener más información sobre la adición de filtros en Análisis mejorado, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de intervalo de tiempo.

   ![](assets/timeframe-filter-350x220.png)

1. Pase el ratón por encima de la línea del equipo principal para ver cuántas horas están aún disponibles para programar, la cantidad de horas programadas para que finalice el equipo de casa y el número total de horas trabajadas, que se etiquetan como de más, menos o con capacidad.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el **Icono de exportación** ![](assets/export.png) en la esquina superior derecha de la visualización, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

1. Haga clic en el nombre del equipo de inicio para obtener más información sobre la visualización de capacidad del equipo.

   Para obtener más información sobre la visualización de la capacidad del equipo, consulte [Ver la visualización de capacidad del equipo en Análisis mejorado](../enhanced-analytics/team-capacity-overview.md).


