---
title: Ver la visualización de capacidad del equipo en Análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización de la capacidad del Equipo muestra la cantidad total de capacidad que tiene un equipo de origen, si está sobreasignado o subasignado, y la dinámica de la capacidad a lo largo del tiempo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Ver la visualización de capacidad del equipo en Análisis mejorado

La visualización de la capacidad del Equipo muestra la cantidad total de capacidad que tiene un equipo de origen, si está sobreasignado o subasignado, y la dinámica de la capacidad a lo largo del tiempo.

![](assets/team-capacity-350x110.png)

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

## Comprender la visualización de capacidad del equipo

La visualización Capacidad del equipo muestra el volumen de trabajo asignado al equipo de casa en un día determinado.

* **Abandono**: Cuando el color de relleno azul más oscuro está por encima de la línea de puntos, el equipo de la casa tiene asignadas más horas de trabajo de las que pueden completar en el número de horas que el equipo está disponible para trabajar. Esto indica que el equipo está sobreasignado y que es posible que se aproxime a la extinción.

   ![](assets/team-capacity-over-capacity.png)

* **Sin respuesta**: Cuando el color de relleno azul más oscuro está por debajo de la línea de puntos, el equipo de casa tiene más horas disponibles para trabajar que la cantidad de trabajo que se les asigna. Esto indica que el equipo está subasignado y puede no ser cuestionado.

   ![](assets/team-capacity-under-capacity.png)

* **Saldo**: Cuando el color de relleno azul más claro o más transparente está justo encima, justo debajo o en la línea de puntos, el equipo doméstico tiene asignadas una cantidad de horas de trabajo que deben poder completar dentro de las horas de trabajo disponibles. Esto indica que la carga de trabajo del equipo es más equilibrada.

   ![](assets/team-capacity-at-capacity.png)

Al pasar el ratón por encima de cualquier punto de la visualización, se muestran los siguientes detalles de un día determinado:

* **Horas programadas**: Este es el número de horas de trabajo planificadas que el equipo necesita completar.
* **Horas disponibles**: Este es el número de horas de trabajo que el equipo está disponible para trabajar.
* **Capacidad**: Además de un porcentaje de capacidad, también se muestran las designaciones En capacidad, En capacidad o En capacidad.

Ver esta información le ayuda a determinar:

* Cuando el equipo de origen estaba sobreasignado o subasignado.
* Si el equipo de origen está sobreasignado o subasignado diariamente.
* La consistencia de la carga de trabajo de un equipo doméstico es diaria.
* Si está creando problemas de capacidad con un nuevo trabajo.

Para obtener información sobre cómo obtener los mejores datos para esta visualización, consulte [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualización de la visualización de capacidad del equipo

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. En el panel izquierdo, seleccione **People**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si no ha establecido el filtro Equipo , agregue el filtro Equipo y seleccione cada equipo para el que desee ver los datos.

   Para obtener más información sobre la adición de filtros en Análisis mejorado, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. En la visualización de la capacidad del recurso, haga clic en un equipo para ver más información.

   Se muestra la visualización Capacidad del equipo .

   Para obtener más información sobre la visualización de la capacidad del recurso, consulte [Visualización de la capacidad de los recursos en Análisis mejorado](../enhanced-analytics/resource-capacity-overview.md).

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de intervalo de tiempo.

   ![](assets/timeframe-filter-350x220.png)

1. Pase el ratón por encima de un punto de la línea gráfica para ver las horas programadas y las horas programadas para la fecha determinada, así como el porcentaje de capacidad y si el equipo de origen ha terminado, se encuentra por debajo o en capacidad en ese momento.

   ![](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el **Icono de exportación** ![](assets/export.png) en la esquina superior derecha de la visualización, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

