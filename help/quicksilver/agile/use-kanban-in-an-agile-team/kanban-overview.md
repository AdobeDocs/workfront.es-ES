---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Información general de Kanban
description: Lea este artículo para comprender mejor cómo funciona la junta de Kanban.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: 2c6a828d95df1229780803a173d5013f5b1eb215
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Información general de Kanban

Las secciones siguientes le permiten comprender mejor cómo se usa la variable [!UICONTROL Kanban] funciones de tablero.

Si está interesado en migrar desde un equipo ágil [!UICONTROL Kanban] tablero a [!DNL Workfront] [!UICONTROL Tableros], consulte [Migración de equipos ágiles [!UICONTROL Kanban] tarjetas a [!DNL Workfront] tableros](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL Kanban] diseño y funciones del tablero

La variable [!UICONTROL Kanban] El tablero consta de los siguientes elementos:

**Columna de atrasos**: Muestra todas las tareas que están actualmente en el trabajo pendiente. Esta columna no se muestra de forma predeterminada. Para obtener más información sobre el trabajo pendiente, incluido cómo mostrarlo en la [!UICONTROL Kanban] tablero, consulte [Administrar el trabajo atrasado ágil](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Estados de artículo**: Indica el progreso de un artículo en función de la columna de estado en la que se encuentra el artículo.

Para obtener más información, consulte [Actualizar el estado de los artículos en la variable [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Los estados de artículo se pueden personalizar para el proyecto mediante la modificación de la vista ágil, tal como se describe en la sección [[!UICONTROL Creación o personalización de una vista Águila]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) en [Información general sobre vistas en [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Se muestra un máximo de cincuenta tarjetas en el panel Kanban de forma predeterminada, pero puede hacer clic en **[!UICONTROL Mostrar más]** para mostrar tarjetas adicionales.

## Relación entre subtareas e artículos

Si un artículo contiene subtareas, no se puede actualizar ninguna información sobre el artículo principal en sí (como puntos/horas o porcentaje completado). Además, no se puede mover la historia por el [!UICONTROL Kanban] tablero para actualizar su estado. Cualquier cambio que realice en las subtareas del artículo se verá reflejado en el artículo. Los puntos u horas de artículo combinados para todas las subtareas determinan los puntos u horas del artículo principal.

Por ejemplo, si una historia tiene una sola subtarea valorada en 4 puntos, la historia misma también tiene 4 puntos. Si cambia el valor del punto de subtarea a 3, el valor del punto del artículo principal se cambia a 3. Si crea otra subtarea en el mismo artículo y establece el valor de punto para esa subtarea en 4, el valor de punto del artículo cambia a 7 para reflejar el valor de punto combinado para ambas subtareas.

Esta misma lógica se aplica a las subtareas de segundo nivel (subtareas de subtareas). Si una subtarea tiene una o más subtareas de segundo nivel, la subtarea se calcula en función de las subtareas de segundo nivel.

## Funciones compatibles

Puede realizar las siguientes acciones al usar el panel Kanban:

* [Agregue una subtarea a un artículo existente en el [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Agregue tareas o problemas existentes a [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Asignar usuarios a un artículo sobre [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Agregue artículos y problemas desde el [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Eliminar artículos o problemas del [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Editar información del artículo](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrar por usuario en la variable [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Administre el límite de trabajo en curso (WIP) en el [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Reordenar artículos en [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Actualizar el estado de los artículos en la variable [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Use indicadores en los artículos del [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Añada el trabajo atrasado al [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
