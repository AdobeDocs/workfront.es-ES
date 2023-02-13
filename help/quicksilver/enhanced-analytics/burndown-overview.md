---
title: Visualización de la visualización de Desglose en Análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización Desglose muestra la reorganización de un proyecto específico a lo largo del tiempo y le ayuda a comprender la relación entre la condición del proyecto, la velocidad y las horas o días restantes.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Visualización de la visualización de Desglose en Análisis mejorado

La visualización Desglose muestra la reorganización de un proyecto específico a lo largo del tiempo y le ayuda a comprender la relación entre la condición del proyecto, la velocidad y las horas o días restantes.

![](assets/burndown-350x112.png)

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
   <td> <p>Ver acceso a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso.<br>Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
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

## Comprender la visualización de Desglose

La línea azul sólida muestra la velocidad planeada desde la fecha de inicio hasta la fecha de finalización planificada. Esta línea se ajusta a medida que se agrega, elimina o actualiza el trabajo y cambia a una línea vertical discontinua cuando el proyecto alcanza la fecha de finalización prevista.

![](assets/burndown-planned-line.png)

La línea real muestra la cantidad de horas (o días) que se emplearon en el proyecto a lo largo del tiempo. El color de esta línea indica la condición del proyecto cada día:

* **Verde**: El proyecto está en el destino.

   ![](assets/burndown-green.png)

* **Naranja**: El proyecto está en riesgo.

   ![](assets/burndown-orange.png)

* **Rojo**: El proyecto está en problemas.

   ![](assets/burndown-red.png)

Para obtener más información sobre estas condiciones de proyecto, consulte [Descripción general de la condición y el tipo de condición del proyecto](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Cuando la línea real aumenta verticalmente, se ha añadido trabajo al proyecto. Cuando la línea se desplaza hacia abajo verticalmente, se ha eliminado o completado el trabajo del proyecto.

Debajo del eje x de la visualización, puede ver más información sobre cómo cambiaron las tareas y las horas (o días) en un día determinado (la cantidad añadida, la cantidad completada y la diferencia entre ambos).

Ver toda esta información en la visualización Desglose le ayuda a determinar:

* La salud del proyecto individual a lo largo del tiempo
* Cómo los problemas que llegaban (o el trabajo no planificado) impactaron en el trabajo planificado.
* Los eventos que ampliaron el proyecto más allá de la fecha de finalización original.

Para obtener información sobre cómo obtener los mejores datos para esta visualización, consulte [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualización de la visualización de Descarga

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desee utilizar.

   Para obtener más información sobre la adición de filtros en Análisis mejorado, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de intervalo de tiempo.

   ![](assets/timeframe-filter-350x220.png)

1. En la visualización de plan de vuelo o diagrama de proyecto, haga clic en un proyecto para ver más información.

   Se muestran las visualizaciones Desglosar y Tareas en vuelo .

   >[!NOTE]
   >
   >Para obtener más información sobre estas otras visualizaciones, consulte:
   >
   >   
   >   
   >   * [Visualización del plan de vuelo en Análisis mejorado](../enhanced-analytics/flight-plan-overview.md)
   >   * [Ver la visualización del diagrama de árbol del proyecto en Análisis mejorado](../enhanced-analytics/project-treemap-overview.md)
   >   * [Ver las tareas en la visualización de vuelo en Análisis mejorado](../enhanced-analytics/tasks-in-flight-overview.md)


1. (Opcional) Cambie la vista de horas planificadas a **duration**.

   Las horas planificadas están seleccionadas de forma predeterminada.

   >[!NOTE]
   >
   >Selección **duration** cambia toda la información de horas a días.\
   >![](assets/duration-burndown-350x112.png)\
   >Para obtener más información sobre la duración en el área de Análisis mejorado, consulte la sección &quot;Vista de duración&quot; en [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

1. Haga clic en cualquier punto del gráfico de líneas.

   A continuación se muestra la fecha exacta y más información sobre las tareas y las horas (o días) del día seleccionado.

   ![](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Si la velocidad real es una línea plana que se ejecuta a lo largo del eje x (en línea con 0 horas o 0 días) de la visualización, esto significa que no se agregaron horas (o días) programadas al proyecto.\
   >Si la velocidad real es una línea plana por encima del eje x (en línea con un número de horas o de días) que nunca se reduce, significa que no se completaron tareas dentro del período de tiempo filtrado.

1. (Opcional) Para exportar los datos de visualización, haga clic en el **Exportar** icono ![](assets/export.png)en la esquina superior derecha de la visualización, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

1. (Opcional) Para ver detalles sobre el progreso de las tareas en el proyecto seleccionado, consulte la visualización Tareas en vuelo que aparece debajo de la visualización Desglosar .
