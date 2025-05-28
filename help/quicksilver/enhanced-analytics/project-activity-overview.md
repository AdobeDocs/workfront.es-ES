---
title: Ver la visualización de actividades del proyecto en Análisis mejorado
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualización de actividades del proyecto muestra una vista acumulada de las actividades a nivel de proyecto (las actividades de cada persona asignada al proyecto) que han tenido lugar durante un lapso de tiempo específico. Puede centrarse únicamente en comprender las actividades de un proyecto o comparar las actividades de un proyecto con las de otros proyectos de Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 89%

---

# Ver la visualización de actividades del proyecto en Análisis mejorado

>[!IMPORTANT]
>
>El análisis mejorado se eliminó de Workfront el 27 de mayo. Workfront Data Connect es una nueva solución alternativa que se puede utilizar para replicar las visualizaciones de Analytics mejoradas que utilice actualmente. <br>Consulte la guía de [Desaprobación mejorada de Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) para obtener más información.


<!-- Audited: 12/2023 -->

La visualización de actividades del proyecto muestra una vista acumulada de las actividades a nivel de proyecto (las actividades de cada persona asignada al proyecto) que han tenido lugar durante un lapso de tiempo específico. Puede centrarse únicamente en comprender las actividades de un proyecto o comparar las actividades de un proyecto con las de otros proyectos de Adobe Workfront.

>[!NOTE]
>
>La visualización Actividad por equipo se comporta de manera similar a esta visualización, pero la visualización Actividad por equipo muestra la actividad del equipo local de todos los proyectos.\
>Para obtener información sobre la visualización Actividad por equipo, consulte [Ver la visualización Actividad por equipo en Análisis mejorado](../enhanced-analytics/activity-by-team-overview.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Plan de Workfront</a></td> 
   <td> <p>Business o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre licencias de Adobe Workfront</a></td> 
   <td>   <p>Nuevo:</p> 
   <ul><li>Light o superior</li></ul>
   <p>Actual:</p>
   <ul><li>Revisión o superior</li></ul>
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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Para conocer los requisitos previos para usar el análisis mejorado, consulte la sección “Requisitos previos” en [Información general de Análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprender la visualización de actividades del proyecto

Las actividades del proyecto se muestran en diferentes colores para resumir los eventos específicos de un proyecto a lo largo de un período de tiempo.

* **Usuarios con sesión iniciada**: las casillas moradas muestran que las personas del equipo local iniciaron sesión ese día. Un tono más oscuro indica un número mayor de personas que iniciaron sesión.

  ![Usuarios que iniciaron sesión](assets/project-activity-users-logged-in.png)

* **Cambio de estado de la tarea**: las casillas rosas muestran que las personas cambiaron el estado de una tarea para el proyecto ese día. Un sombreado más oscuro indica que se ha cambiado un número mayor de estados de tarea.

  ![Cambio de estado de tarea](assets/project-activity-task-status-changes.png)

* **Tareas completadas**: las casillas azules muestran que las personas completaron una tarea para el proyecto. Un tono más oscuro indica que se está completando un número mayor de tareas.

  ![Tareas completadas](assets/project-activity-tasks-completed.png)

Al pasar el puntero por encima de una casilla, se muestra el número exacto de veces que se completó la acción en un día determinado. Puede seleccionar un proyecto para ver el desglose de estas actividades por cada colaborador individual del proyecto.

Ver esta información le ayuda a determinar lo siguiente:

* La actividad de un proyecto específico.
* La actividad de un proyecto en comparación con otros proyectos.
* Qué usuarios están trabajando en un proyecto y con qué frecuencia.

Para más información sobre cómo obtener los mejores datos para esta visualización, consulte [Información general de Análisis mejorado](../enhanced-analytics/enhanced-analytics-overview.md).

## Ver visualización de actividades del proyecto

1. Haga clic en el icono del menú principal ![icono del menú principal](assets/main-menu-icon-16x12.png) y, a continuación, seleccione **Analytics**.
1. (Opcional) Para utilizar un intervalo de fecha diferente, seleccione nuevas fechas de inicio y finalización en el filtro de intervalo de fecha.

   ![Seleccionar intervalo de fecha](assets/filters-select-date-range-350x344.png)

   Para obtener información sobre el uso del filtro de intervalo de fecha, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Si selecciona un intervalo de fecha para un período superior a tres meses, la visualización de actividades del proyecto no muestra ningún dato.

1. (Condicional) Si necesita limitar el conjunto de datos del proyecto, seleccione y aplique los filtros que desea utilizar.

   Para obtener más información sobre cómo añadir filtros en Análisis mejorado, consulte [Aplicar filtros en Análisis mejorado](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Después de añadir filtros, se muestran los datos de hasta 50 proyectos y los filtros permanecen activos incluso después de salir de la página o cerrar la sesión de Workfront.

1. (Opcional) Para acercar un intervalo de fecha, seleccione un punto en la visualización para el inicio del intervalo de fecha y arrastre hasta el final del intervalo de fecha.

   Todas las demás visualizaciones se actualizan al mismo intervalo de fecha y se crea un filtro de periodo de tiempo.

   ![Filtro de período de tiempo](assets/timeframe-filter-350x220.png)

1. (Opcional) Para cambiar la forma en que se ordenan los proyectos, haga clic en el menú **Ordenar por** y, a continuación, seleccione una nueva opción de ordenación:

   * **A - Z**
   * **Z - A**
   * **Fecha planificada de finalización**
   * **Fecha planificada de inicio**

   Todas las demás visualizaciones de la página se actualizarán para coincidir con su selección de ordenación.

1. (Condicional) Si hay más de 50 proyectos en el conjunto de datos, utilice las flechas de la esquina inferior izquierda de la visualización para navegar de un grupo de 50 proyectos al siguiente.

   Todas las demás visualizaciones de la página se actualizarán para coincidir con su selección de página.

   ![Paginación](assets/pagination-350x118.png)

1. Haga clic en un proyecto de la visualización para ver más detalles del proyecto.

   La lista se amplía para mostrar las actividades de cada colaborador individual del proyecto.

1. Pase el puntero sobre un cuadro para ver la fecha en la que los usuarios completaron una acción, así como la cantidad de veces que la acción se completó en ese día.

   ![Ventana emergente de actividad](assets/project-activity-activity-pop-up-350x137.png)

1. (Opcional) Para exportar los datos de visualización, haga clic en el **icono Exportar** ![icono Exportar](assets/export.png) en la esquina superior derecha de la visualización y, a continuación, seleccione el formato de exportación:

   * **Gráfico (PNG)**
   * **Tabla de datos (XLSX)**

