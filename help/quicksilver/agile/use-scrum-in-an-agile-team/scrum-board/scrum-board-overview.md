---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Información general del panel Scrum
description: El tablero de historias de Agile de Scrum se muestra junto con el estado de finalización y el gráfico de evolución.
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: a9dbfe21337be9cd9929f4e982e4979265ca14e1
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 77%

---

# Información general del tablero de [!UICONTROL Scrum]

<!-- Audited: 5/2025 -->

El tablero de historias de Agile de [!UICONTROL Scrum] se muestra junto con el estado de finalización y el gráfico de evolución. Estos componentes de Agile están disponibles en las siguientes situaciones en [!UICONTROL Adobe Workfront]:

* En iteraciones de Agile. Para obtener más información sobre el uso del tablero de historias de Agile, el gráfico de evolución y el estado de finalización en un entorno Agile puro (con registros de asuntos pendientes y una iteración), consulte [Trabajar en un entorno Agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Al ver un proyecto en una vista de Agile. Para obtener información sobre cómo aprovechar el tablero de historias de Agile, el gráfico de evolución y el estado de finalización dentro de un proyecto existente, consulte [Administrar un proyecto en la vista de Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Iteración de Agile](assets/agile-iteration-with-callouts.png)

## Diseño y funciones del tablero de historias

![Tablero de historias de Agile](assets/agile-storyboard-callouts.png)

El tablero de historias consta de los siguientes elementos:

* **Columna de historia principal**: a diferencia de otras columnas del panel de historias, la columna [!UICONTROL Historia principal] no es un estado de tarea, sino que existe para albergar cualquier historia que contenga subtareas en la iteración o proyecto. Esta columna solo puede incluir las historias principales que tengan al menos una subtarea en el tablero de historias. Las historias principales en sí no cambian de estado a estado en el tablero de historias.

  En una iteración, esta columna aparece en el tablero de historias solo cuando una o varias historias del tablero de historias contienen al menos una subtarea que cumple los siguientes requisitos:

   * Asignado al mismo equipo Agile que la tarea principal.
   * Pertenece a la iteración.

     En un proyecto, esta columna aparece siempre que una tarea tiene al menos una subtarea.

     ![Columna de la historia principal](assets/agile-parentstory-swimlane.png)

* **Estados de la tarea**: indique el progreso de una historia en la iteración o proyecto en función de la columna de estado en la que se encuentre la historia.

  Los estados de las tareas se pueden personalizar para el proyecto mediante la modificación de la vista Agile.

* **Ruta de natación**: Cuando una historia principal y sus subtareas aparecen en el guion gráfico, se crea una ruta de natación específica para la historia y sus subtareas. Esto proporciona una distinción visual para ver mejor el progreso de las subtareas de una historia en el tablero de historias.

  En una iteración, los diagramas de flujo aparecen en el tablero de historias solo cuando una historia del tablero contiene al menos una subtarea que cumple los siguientes requisitos:

   * Asignado al mismo equipo Agile que la tarea principal.
   * Pertenece a la iteración.

  En un proyecto, los diagramas de flujo aparecen siempre que una tarea tiene al menos una subtarea o una tarea principal.

* **Historias individuales**: Las historias y los problemas individuales se muestran debajo de cualquier pista de natación en el panel de historias. Esto proporciona una distinción visual de las historias que forman parte de un diagrama de flujo.

## Relación entre subtareas e historias

Si un artículo contiene subtareas, no se puede actualizar la información del propio artículo principal (como puntos/horas o porcentaje completado). Además, no puede mover la historia al tablero de historias para actualizar su estado. En su lugar, cualquier cambio que realice en las subtareas de la historia se reflejará en la historia. Los puntos de caso combinados de todas las subtareas determinan los puntos u horas de la historia principal.

Por ejemplo, si una historia tiene solo una subtarea valorada en cuatro puntos, la historia en sí también tiene cuatro puntos. Si cambia el valor del punto de la subtarea a tres, el valor de punto de la historia principal cambiará a tres. Si crea otra subtarea en la misma historia y establece el valor de punto de esa subtarea en cuatro, el valor de punto de la historia cambiará a siete para reflejar el valor de punto combinado de ambas subtareas.

Esta misma lógica se aplica a las subtareas de segundo nivel (subtareas de subtareas). Si una subtarea tiene una o más subtareas de segundo nivel, la subtarea se calcula en función de las subtareas de segundo nivel.

## Relación entre el tablero de historias y el registro de asuntos pendientes

El registro de asuntos pendientes de iteración muestra solo las historias o subtareas en las que puede establecer una estimación. Si una historia principal tiene subtareas que se muestran en el tablero de historias (porque están asignadas al mismo equipo Agile y pertenecen a la iteración), la tarea principal no se muestra en el registro de asuntos pendientes. En este caso, solo se muestran las subtareas en el registro de asuntos pendientes, mientras que las subtareas y la historia principal se muestran en el tablero de historias.

Por ejemplo, supongamos que la historia A contiene la subtarea 1 y la subtarea 2 (y que ambas subtareas están asignadas al mismo equipo Agile). En esta situación, la historia A se muestra en el tablero de historias en un diagrama de flujo con la subtarea 1 y la subtarea 2. Sin embargo, en el registro de asuntos pendientes solo se muestran las subtareas 1 y 2.

Esta misma lógica se aplica a las subtareas de segundo nivel (subtareas de subtareas). Si una subtarea tiene una o más subtareas de segundo nivel asignadas al mismo equipo Agile y pertenecen a la iteración, solamente se muestra la subtarea de segundo nivel en el registro de asuntos pendientes.

Para obtener más información sobre el registro de asuntos pendientes, consulte [Administrar el registro de asuntos pendientes de Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
