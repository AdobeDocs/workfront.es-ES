---
content-type: overview;how-to-procedural
product-area: projects
keywords: analytics, métricas, proyecto, mejorado, tareas, asignado, completo, estado, vencido, próximo
navigation-topic: manage-projects
title: Resumen de las métricas del proyecto
description: Las métricas de proyecto le proporcionan una visualización de lo que está sucediendo en un proyecto, lo que le permite evaluar rápidamente las necesidades y el estado de un proyecto. Aprenda a interpretar el área de Métricas en el panel izquierdo de un proyecto.
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1266'
ht-degree: 0%

---

# Resumen de las métricas del proyecto

Las métricas de proyecto proporcionan una vista general en formato de gráfico sobre el rendimiento de un proyecto.

## Requisitos de acceso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Workfront*</td> 
   <td> <p>Revisar o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver acceso a proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los proyectos, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Conceder acceso a los proyectos</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos de un proyecto</p> <p> Para obtener información acerca de los permisos del proyecto, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Compartir un proyecto en Adobe Workfront</a>.</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Para acceder al área de Métricas desde el panel izquierdo de un proyecto, debe:

* Tenga activadas las métricas de la opción del panel izquierdo en el área Proyectos de la plantilla de diseño.

  Para saber cómo un administrador de Workfront o de un grupo puede personalizar el panel izquierdo con una plantilla de diseño, consulte [Personalizar el panel izquierdo con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Descripción general del área de métricas del proyecto

Las métricas de proyecto le proporcionan una visualización de lo que está sucediendo en un proyecto, lo que le permite evaluar rápidamente las necesidades y el estado de un proyecto.

![](assets/project-metrics-full-screen-350x238.png)

En el área Métricas, puede ver el estado general de un proyecto, así como lo siguiente:

* Lugar de trabajo activo o paralizado
* Quién tiene elementos de trabajo abiertos asignados a ellos
* Detalles sobre tareas o problemas que han vencido o que están cerca de la fecha planificada de finalización

También puede explorar en profundidad cada gráfico para ver más de cerca las tareas o problemas de una categoría específica.

Para obtener más información sobre cómo ver estas tareas o problemas, consulte [Ver detalles de métricas](#view-metrics-details).

>[!TIP]
>
>Para ver las métricas de un nivel superior de un grupo de proyectos dentro de un programa, portafolio, etc., vaya al área de Análisis mejorado.\
>Para obtener más información acerca de los análisis mejorados, consulte [Descripción general de los análisis mejorados](../../../enhanced-analytics/enhanced-analytics-overview.md).

## KPI de proyecto

Los indicadores clave de rendimiento (KPI) se muestran en la parte superior del área de Métricas.

![](assets/project-metrics-kpis-350x52.png)

Estos KPI se dividen en las siguientes categorías:

| Tareas completadas | **Tareas completadas** muestra el número de tareas en un estado Completo. Este número también incluye tareas que tienen un estado personalizado que equivale a Completado. |
|---|---|
| Tareas incompletas | **Tareas incompletas** muestra el número de tareas que no se encuentran en estado Completado o Cerrado o un estado que equivale a Completado. |
| Tareas vencidas | **Tareas vencidas** muestra el número de tareas que han pasado la Fecha planificada de finalización y no están en estado completo o cerrado, o un estado que equivale a completo o cerrado. |
| Total de tareas | **Tareas totales** muestra la cantidad total de tareas en el proyecto. |

>[!TIP]
>
>Para mostrar una lista de elementos de trabajo para un KPI específico, haga clic en ese KPI. En esa lista, puede hacer clic en un elemento de trabajo específico para ver más detalles en una nueva pestaña.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Para obtener más información, consulte [Ver detalles de métricas](#view-metrics-details).

## Gráfico de barras de tareas o problemas

En el gráfico de barras que aparece debajo de los KPI del proyecto, puede ver el estado o la prioridad de los elementos de trabajo del proyecto. La vista de tareas está seleccionada de forma predeterminada.

Cuando se selecciona el estado en este gráfico, puede ver todos los estados de las tareas o problemas de un proyecto. Cada estado se agrupa en una barra del gráfico. En este gráfico se muestran todos los estados de sistema y personalizados predeterminados.

![](assets/project-metrics-task-issue-by-status-350x120.png)

Cuando se selecciona la prioridad en este gráfico, puede ver todas las prioridades de tareas o problemas de un proyecto.

![](assets/project-metrics-task-issue-by-priority-350x121.png)

>[!TIP]
>
>Para mostrar una lista de elementos de trabajo con un estado o prioridad específicos, haga clic en una barra del gráfico. En esa lista, puede hacer clic en un elemento de trabajo específico para ver más detalles en una nueva pestaña.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Para obtener más información, consulte [Ver detalles de métricas](#view-metrics-details).

## Gráfico de anillo

El gráfico circular situado debajo de los KPI del proyecto le permite ver la proporción de elementos de trabajo completados frente a elementos de trabajo incompletos en un proyecto.

![](assets/tasks-issues-by-complete-status-350x250.png)

En el menú desplegable situado encima del gráfico, puede seleccionar:

| Todas las tareas | Al seleccionar **tareas**, se muestra la cantidad total de tareas en el proyecto, así como la relación entre las tareas completadas y las incompletas. |
|---|---|
| Todos los problemas | Al seleccionar **problemas**, se muestra el número total de problemas en el proyecto, así como la relación entre los problemas completados y los incompletos. |

>[!TIP]
>
>Para mostrar una lista de los elementos de trabajo completados o incompletos, haga clic en esa sección del gráfico de anillo. En esa lista, puede hacer clic en un elemento de trabajo específico para ver más detalles en una nueva pestaña.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Para obtener más información, consulte [Ver detalles de métricas](#view-metrics-details).

## Gráfico de barras de usuario asignado

El gráfico de barras de personas asignadas muestra el número de tareas asignadas a cada persona en el proyecto. Este número varía en función de la categoría que seleccione en el menú desplegable.

![](assets/tasks-issues-by-assignee-350x104.png)

Puede elegir ver las asignaciones de tareas de un proyecto en las siguientes categorías:

| Completar | Al seleccionar **Completar** se muestra el número de tareas asignadas a cada usuario que se han completado. |
|---|---|
| Incompletas | Si se selecciona **Incompleto**, se muestra el número de tareas asignadas a cada usuario que aún no se han completado. |
| Próximamente | Al seleccionar **Próximas**, se muestra el número de tareas asignadas a cada usuario que aún no ha alcanzado la Fecha planificada de inicio. |
| Vencido sin pagar | Si se selecciona **Vencidas**, se muestra el número de tareas asignadas a cada usuario que han pasado la fecha planificada de finalización y que aún no se han completado. |

>[!TIP]
>
>Para mostrar una lista de los elementos de trabajo de la categoría seleccionada que están asignados a un usuario específico, haga clic en la barra situada junto al nombre del usuario en el gráfico. En esa lista, puede hacer clic en un elemento de trabajo específico para ver más detalles en una nueva pestaña.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Para obtener más información, consulte [Ver detalles de métricas](#view-metrics-details).

## Detalles de Ver métricas {#view-metrics-details}

Puede interactuar con los gráficos en el área de Métricas para ver diferentes aspectos de un gráfico o ver más de cerca las tareas y problemas dentro de un gráfico.

1. Vaya al proyecto para el que desee ver las métricas.
1. En el panel izquierdo, haga clic en **Mostrar más** para mostrar más secciones y luego haga clic en **Métricas**.\
   Los gráficos del área Métricas muestran información sobre las tareas de forma predeterminada.\
   ![](assets/metrics-section-350x298.png)

1. (Condicional) Si aparece una flecha desplegable en un gráfico, haga clic en el icono **Flecha desplegable** ![](assets/dropdown-arrow.png) del gráfico y seleccione la opción que desee en el menú.\
   Para obtener información sobre las opciones que aparecen en los menús de cada gráfico, consulte la sección correspondiente más arriba.

1. (Opcional) Para examinar más de cerca las tareas o problemas de cualquier métrica de la página, haga lo siguiente:

   1. Haga clic en el elemento (como las tareas asignadas a un usuario específico, los problemas con prioridad alta o todas las tareas vencidas) cuyos detalles desee ver.

      Se muestra una lista de tareas o problemas.

      ![](assets/completed-tasks-dialog-350x75.png)

   1. Utilice las flechas de la parte inferior de la lista para localizar la tarea o el problema que desea ver.

      O

      Seleccione un número específico para mostrar tareas o problemas en una página específica.

      ![](assets/pagination-300x152.png)

   1. Seleccione una tarea o un problema para ver más detalles.

      La tarea o el problema se abre en una nueva pestaña.

1. (Opcional) Para exportar el panel de métricas del proyecto a un archivo .png, haga clic en el icono **Exportar** ![](assets/export.png) y, a continuación, seleccione **Exportar como PNG** en el menú desplegable.

   >[!TIP]
   >
   >Al exportar el tablero, el archivo exportado incluye solo lo que se muestra actualmente en la ventanilla. Para incluir determinados elementos en el archivo exportado, es posible que tenga que desplazarse hacia arriba o hacia abajo en la página o ajustar la configuración de zoom del explorador.
