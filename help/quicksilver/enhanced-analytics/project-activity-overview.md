---
title: Vea la visualización de la actividad del proyecto en el análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización de la actividad del proyecto muestra una vista agregada de las actividades a nivel de proyecto (las actividades de cada persona asignada al proyecto) que se produjeron durante un lapso de tiempo específico. Puede centrarse únicamente en comprender las actividades de un proyecto o comparar las actividades de un proyecto con otros proyectos de Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 8%

---

# Vea la visualización de la actividad del proyecto en el análisis mejorado

<!-- Audited: 12/2023 -->

La visualización de la actividad del proyecto muestra una vista agregada de las actividades a nivel de proyecto (las actividades de cada persona asignada al proyecto) que se produjeron durante un lapso de tiempo específico. Puede centrarse únicamente en comprender las actividades de un proyecto o comparar las actividades de un proyecto con otros proyectos de Adobe Workfront.

>[!NOTE]
>
>La visualización Actividad por equipo se comporta de manera similar a esta visualización, pero la visualización Actividad por equipo muestra la actividad del equipo de inicio de todos los proyectos.\
>Para obtener información sobre la visualización Actividad por equipo, consulte [Ver la visualización Actividad por equipo en Análisis mejorado](../enhanced-analytics/activity-by-team-overview.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">plan de Workfront</a></td> 
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

## Comprender la visualización de actividades del proyecto

Las actividades de proyecto se muestran en diferentes colores para resumir eventos específicos de un proyecto durante un periodo de tiempo:

* **Usuarios que iniciaron sesión**: Los cuadros morados muestran que las personas asignadas al proyecto iniciaron sesión ese día. Un tono más oscuro indica un número mayor de personas que iniciaron sesión.

  ![](assets/project-activity-users-logged-in.png)

* **Cambio de estado de la tarea**: Los cuadros rosas muestran que las personas cambiaron el estado de una tarea para el proyecto ese día. Un sombreado más oscuro indica que se ha cambiado un número mayor de estados de tarea.

  ![](assets/project-activity-task-status-changes.png)

* **Tareas completadas**: Los cuadros azules muestran que las personas completaron una tarea para el proyecto. Un tono más oscuro indica que se está completando un número mayor de tareas.

  ![](assets/project-activity-tasks-completed.png)

Al pasar el ratón por encima de un cuadro, se muestra el número exacto de veces que se completó la acción en un día determinado. Puede seleccionar un proyecto para ver un desglose de estas actividades por cada colaborador individual del proyecto.

Ver esta información le ayuda a determinar lo siguiente:

* La actividad de un proyecto específico.
* La actividad de un proyecto en comparación con otros proyectos.
* Qué usuarios están trabajando en un proyecto y con qué frecuencia.

Para obtener los mejores datos para esta visualización, consulte [Descripción general del análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualización de la visualización de actividad del proyecto

1. Haga clic en el icono del menú principal ![](assets/main-menu-icon-16x12.png) y, a continuación, seleccione **Analytics**.
1. (Opcional) Para utilizar un intervalo de fechas diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fechas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fechas, consulte [Aplicar filtros en el análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Si selecciona un intervalo de fechas para un periodo superior a tres meses, la visualización de la actividad del proyecto no mostrará ningún dato.

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desee utilizar.

   Para obtener más información sobre cómo agregar filtros en el análisis mejorado, consulte [Aplicar filtros en el análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de agregar filtros, se muestran datos de hasta 50 proyectos y los filtros permanecen activos incluso después de abandonar la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fechas, seleccione un punto en la visualización para el inicio del intervalo de fechas y arrastre hasta el final del intervalo de fechas.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fechas y se crea un filtro de periodo de tiempo.

   ![](assets/timeframe-filter-350x220.png)

1. (Opcional) Para cambiar la forma en que se ordenan los proyectos, haga clic en el menú **Ordenar por** y, a continuación, seleccione una nueva opción de ordenación:

   * **A - Z**
   * **Z - A**
   * **Fecha planificada de finalización**
   * **Fecha planificada de inicio**

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de ordenación.

1. (Condicional) Si hay más de 50 proyectos en el conjunto de datos, utilice las flechas de la esquina inferior izquierda de la visualización para desplazarse de un grupo de 50 proyectos al siguiente.

   Todas las demás visualizaciones de la página se actualizarán para que coincidan con la selección de página.

   ![](assets/pagination-350x118.png)

1. Haga clic en un proyecto en la visualización para ver más detalles del proyecto.

   La lista se amplía para mostrar las actividades de cada colaborador individual del proyecto.

1. Pase el ratón sobre un cuadro para ver la fecha en la que los usuarios completaron una acción, así como la cantidad de veces que la acción se completó para ese día.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el **icono Exportar** ![](assets/export.png) en la esquina superior derecha de la visualización y, a continuación, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XSLX)**

