---
title: Ver la visualización de la actividad del proyecto en Análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización de la actividad del proyecto muestra una vista agregada de las actividades en el nivel del proyecto (las actividades de cada persona asignada al proyecto) que se produjeron durante un intervalo de tiempo específico. Puede limitar el enfoque para comprender las actividades de un proyecto o comparar las actividades de un proyecto con otros proyectos de Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 1%

---

# Ver la visualización de la actividad del proyecto en Análisis mejorado

La visualización de la actividad del proyecto muestra una vista agregada de las actividades en el nivel del proyecto (las actividades de cada persona asignada al proyecto) que se produjeron durante un intervalo de tiempo específico. Puede limitar el enfoque para comprender las actividades de un proyecto o comparar las actividades de un proyecto con otros proyectos de Adobe Workfront.

>[!NOTE]
>
>La visualización Actividad por equipo se comporta de manera similar a esta visualización, pero la visualización Actividad por equipo muestra la actividad del equipo principal de todos los proyectos.\
>Para obtener información sobre la visualización Actividad por equipo, consulte [Visualización de la actividad por equipo en Análisis mejorado](../enhanced-analytics/activity-by-team-overview.md).

<!--WRITER bad link; there is no Activity by Team.png
[![](assets/project-activity-350x114.png)](../Resources/Images/Analytics/Activity by Team.png)
-->

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan de Workfront</a>*</td> 
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

## Comprender la visualización de la actividad del proyecto

Las actividades de proyecto se muestran en diferentes colores para resumir eventos específicos de un proyecto durante un período de tiempo:

* **Usuarios con sesión iniciada**: Los cuadros morados muestran que las personas asignadas al proyecto iniciaron sesión ese día. Un tono más oscuro indica un número mayor de personas que inician sesión.

   ![](assets/project-activity-users-logged-in.png)

* **Cambio de estado de la tarea**: Los cuadros rosas muestran que las personas cambiaron el estado de una tarea para el proyecto ese día. Un sombreado más oscuro indica que se ha cambiado un número mayor de estados de tarea.

   ![](assets/project-activity-task-status-changes.png)

* **Tareas completadas**: Los cuadros azules muestran que las personas completaron una tarea para el proyecto. Un tono más oscuro indica un número mayor de tareas que se están completando.

   ![](assets/project-activity-tasks-completed.png)

Al pasar el ratón por encima de un cuadro, se muestra la cantidad exacta de veces que la acción se completó en un día determinado. Puede seleccionar un proyecto para ver un desglose de estas actividades por cada colaborador individual en el proyecto.

Ver esta información le ayuda a determinar:

* La actividad de un proyecto específico.
* La actividad de un proyecto en comparación con otros proyectos.
* Qué usuarios están trabajando en un proyecto y con qué frecuencia.

Para obtener información sobre cómo obtener los mejores datos para esta visualización, consulte [Resumen de análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Ver la visualización de la actividad del proyecto

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png)y, a continuación, seleccione **Analytics**.
1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Si selecciona un intervalo de fechas para un periodo bueno a más de 3 meses, la visualización de actividad del proyecto no muestra ningún dato.

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desee utilizar.

   Para obtener más información sobre la adición de filtros en Análisis mejorado, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de intervalo de tiempo.

   ![](assets/timeframe-filter-350x220.png)

1. (Opcional) Para cambiar la forma en que se ordenan los proyectos, haga clic en el **Ordenar por** a continuación, seleccione una nueva opción de clasificación:

   * **A-Z**
   * **Z-A**
   * **Fecha de finalización planificada**
   * **Fecha de inicio planificada**

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con su selección de clasificación.

1. (Condicional) Si hay más de 50 proyectos en el conjunto de datos, utilice las flechas de la esquina inferior izquierda de la visualización para ir de un grupo de 50 proyectos al siguiente.

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de la página.

   ![](assets/pagination-350x118.png)

1. Haga clic en un proyecto en la visualización para ver más detalles del proyecto.

   La lista se expande para mostrar las actividades de cada colaborador individual en el proyecto.

1. Pase el ratón sobre un cuadro para ver la fecha en la que los usuarios completaron una acción, así como el número de veces que se completó la acción para ese día.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el **Icono de exportación** ![](assets/export.png) en la esquina superior derecha de la visualización, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

