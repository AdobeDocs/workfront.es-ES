---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Información general del panel Scrum
description: El guion gráfico de Scrum Agile se muestra junto con el estado de finalización y el gráfico de evolución.
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Resumen del tablero [!UICONTROL Scrum]

El panel de historia ágil [!UICONTROL Scrum] se muestra junto con el estado de finalización y el gráfico de evolución. Estos componentes Agile están disponibles en las siguientes situaciones en [!UICONTROL Adobe Workfront]:

* En iteraciones Agile. Para obtener más información sobre el uso del panel de historias Agile, el gráfico de evolución y el estado de finalización en un entorno Agile puro (con trabajos pendientes y una iteración), consulte [Trabajar en un entorno Agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Al ver un proyecto en una vista Agile. Para obtener información sobre cómo aprovechar el panel de historias Agile, el gráfico de evolución y el estado de finalización dentro de un proyecto existente, consulte [Administrar un proyecto en la vista Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Iteración ágil](assets/agile-iteration-with-callouts.png)

## Diseño y funciones del guion gráfico

![Tablero de historia Agile](assets/agile-storyboard-callouts.png)

El guion gráfico consta de los siguientes elementos:

* **[!UICONTROL Artículo principal] Columna:** A diferencia de otras columnas del guion gráfico, la columna [!UICONTROL Artículo principal] no es un estado de tarea, sino que existe para albergar cualquier artículo que contenga subtareas en la iteración o proyecto. En esta columna solo pueden residir las historias principales que tengan al menos una subtarea en el panel de historias. Las historias principales en sí no cambian de estado a estado en el tablero de historias.

  En una iteración, esta columna aparece en el guion gráfico sólo cuando uno o varios artículos del guion gráfico contienen al menos una subtarea que cumple los siguientes requisitos:

   * Asignado al mismo equipo Agile que la tarea principal
   * Pertenece a la iteración

     En un proyecto, esta columna aparece siempre que una tarea tiene al menos una subtarea.

     ![Columna de artículo principal](assets/agile-parentstory-swimlane.png)

* **Estados de la tarea:** Indique cómo avanza una historia a través de la iteración o proyecto en función de la columna de estado en la que se encuentra la historia.

  Los estados de las tareas se pueden personalizar para el proyecto mediante la modificación de la vista Agile, tal como se describe en [Crear o personalizar una vista Agile](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) en la descripción general de [Vistas en [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* **Ruta de natación:** Cuando una historia principal y sus subtareas aparecen en el guion gráfico, se crea una ruta de natación específica para la historia y sus subtareas. Esto proporciona una distinción visual para ver mejor el progreso de las subtareas de un artículo en el guion gráfico.

  En una iteración, las rutas de natación aparecen en el guion gráfico sólo cuando una historia del guion gráfico contiene al menos una subtarea que cumple los siguientes requisitos:

   * Asignado al mismo equipo Agile que la tarea principal
   * Pertenece a la iteración

  En un proyecto, las rutas de navegación aparecen siempre que una tarea tiene al menos una subtarea o una tarea principal.

* **Historias individuales:** Las historias individuales y los problemas se muestran debajo de cualquier pista de natación en el panel de historias. Esto proporciona una distinción visual de las historias que forman parte de una pista de natación.

## Relación entre subtareas e historias

Si un artículo contiene subtareas, no se puede actualizar la información del propio artículo principal (por ejemplo, puntos/horas o porcentaje completado). Además, no puede mover la historia al tablero de historias para actualizar su estado. En su lugar, cualquier cambio que realice en las subtareas de la historia se reflejará en la historia. Los puntos u horas del artículo combinado de todas las subtareas determinan los puntos u horas del artículo principal.

Por ejemplo, si una historia tiene solo una subtarea valorada en 4 puntos, la historia en sí también tiene 4 puntos. Si cambia el valor de punto de la subtarea a 3, el valor de punto del artículo principal cambiará a 3. Si crea otra subtarea en el mismo artículo y establece el valor de punto de esa subtarea en 4, el valor de punto del artículo se cambia a 7 para reflejar el valor de punto combinado de ambas subtareas.

Esta misma lógica se aplica a las subtareas de segundo nivel (subtareas de subtareas). Si una subtarea tiene una o más subtareas de segundo nivel, la subtarea se calcula en función de las subtareas de segundo nivel.

## Relación entre el guion gráfico y el registro de pendientes

>[!NOTE]
>
>La información de esta sección se aplica solamente a las vistas Agile de una iteración; las vistas Agile de un proyecto no utilizan un registro de pendientes. (Para obtener más información sobre las diferencias entre las vistas Agile de una iteración y un proyecto, vea &quot;Diferencias al usar la vista [!UICONTROL Agile] en un proyecto en versos sobre una iteración&quot; en [Administrar un proyecto en la vista Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)).

El registro de pendientes de iteración muestra solo las historias o subtareas en las que puede establecer una estimación. Si un artículo principal tiene subtareas que se muestran en el guion gráfico (porque están asignadas al mismo equipo Agile y pertenecen a la iteración), la tarea principal no se muestra en el registro de pendientes. En este caso, sólo se muestran las subtareas en el registro de pendientes, mientras que las subtareas y el artículo principal se muestran en el tablero de artículos.

Por ejemplo, supongamos que el artículo A contiene la subtarea 1 y la subtarea 2 (y que ambas subtareas están asignadas al mismo equipo Agile). En esta situación, la historia A se muestra en el guion gráfico en una pista de natación con Subtarea 1 y Subtarea 2. Sin embargo, en el registro de pendientes solo se muestran las subtareas 1 y 2.

Esta misma lógica se aplica a las subtareas de segundo nivel (subtareas de subtareas). Si una subtarea tiene una o más subtareas de segundo nivel asignadas al mismo equipo Agile y pertenecen a la iteración, sólo se mostrará la subtarea de segundo nivel en el registro de pendientes.

Para obtener más información sobre el registro de pendientes, consulte [Administrar el registro de pendientes Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
