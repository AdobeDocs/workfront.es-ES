---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Información general de Kanban
description: Revise este artículo para comprender mejor cómo funciona el Panel Kanban.
author: Jenny
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 47%

---

# Resumen de Kanban

<!-- Audited: 01/2024 -->

Las siguientes secciones le permiten comprender mejor cómo funciona el tablero [!UICONTROL Kanban].

Para obtener una descripción de la metodología K[!UICONTROL anban], consulte [Crear un equipo Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Si está interesado en migrar de un panel [!UICONTROL Kanban] de equipo Agile a [!DNL Workfront] [!UICONTROL Tableros], vea las tarjetas de [Migrar tarjetas de equipo Agile [!UICONTROL Kanban] a [!DNL Workfront] tableros](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## Diseño y funciones del tablero [!UICONTROL Kanban]

El tablero [!UICONTROL Kanban] consta de los siguientes elementos:

**Columna de registro de pendientes**: Muestra todas las tareas que están actualmente en el registro de pendientes. Esta columna no se muestra de forma predeterminada. Para obtener más información sobre el registro de pendientes, incluido cómo mostrarlo en el tablero [!UICONTROL Kanban], consulte [Administrar el registro de pendientes de Agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Estados de la historia**: indica el progreso de una historia en función de la columna de estado en la que se encuentra.

Para obtener más información, consulte [Actualizar el estado de las historias en el tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Los estados de las historias se pueden personalizar para el proyecto mediante la modificación de la vista de Agile, tal como se describe en la sección [[!UICONTROL Crear o personalizar una vista de Agile]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) en [Crear o editar vistas en [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>Se muestra un máximo de cincuenta tarjetas en el panel Kanban de forma predeterminada, pero puede hacer clic en **[!UICONTROL Mostrar más]** para mostrar tarjetas adicionales.

## Relación entre subtareas e historias

Si una historia contiene subtareas, no se puede actualizar la información de la propia historia principal (por ejemplo, puntos/horas o porcentaje completado). Además, no puede mover la historia al tablero [!UICONTROL Kanban] para actualizar su estado. En su lugar, cualquier cambio que realice en las subtareas de la historia se reflejará en la historia. Los puntos de caso combinados de todas las subtareas determinan los puntos u horas de la historia principal.

Por ejemplo, si una historia tiene solo una subtarea valorada en cuatro puntos, la historia en sí también tiene cuatro puntos. Si cambia el valor del punto de la subtarea a tres, el valor de punto de la historia principal cambiará a tres. Si crea otra subtarea en la misma historia y establece el valor de punto de esa subtarea en cuatro, el valor de punto de la historia cambiará a siete para reflejar el valor de punto combinado de ambas subtareas.

Esta misma lógica se aplica a las subtareas de segundo nivel (subtareas de subtareas). Si una subtarea tiene una o más subtareas de segundo nivel, la subtarea se calcula en función de las subtareas de segundo nivel.

## Funciones compatibles

Puede realizar las siguientes acciones al utilizar el Panel Kanban:

* [Añadir una subtarea a una historia existente en el tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Agregar tareas o problemas existentes al tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Asignar usuarios a una historia en el tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Agregar historias y problemas del tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Eliminar historias o problemas del tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Editar información de una historia](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrar por usuario en el tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Administrar el límite de trabajo en curso (WIP) en el tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Reordenar historias en el tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Actualizar el estado de las historias en el tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Usar indicadores en las historias del tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Añadir el registro de asuntos pendientes al tablero [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
