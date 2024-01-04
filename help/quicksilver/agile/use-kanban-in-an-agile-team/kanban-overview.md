---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Resumen de Kanban
description: Revise este artículo para comprender mejor cómo funciona el Panel Kanban.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: fa499d74df891441e729c32188e9b2f74e4ef5c0
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Resumen de Kanban

<!-- Audited: 01/2024 -->

Las siguientes secciones le permiten comprender mejor cómo se utilizan las [!UICONTROL Kanban] funciones de tablero.

Para obtener una descripción de la K[!UICONTROL anban] metodología, consulte [Crear un equipo Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Si le interesa migrar de un equipo Agile [!UICONTROL Kanban] tablero para [!DNL Workfront] [!UICONTROL Tableros], consulte [Migrar el equipo Agile [!UICONTROL Kanban] tarjetas a [!DNL Workfront] tableros](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL Kanban] diseño y funciones del tablero

El [!UICONTROL Kanban] El tablero consta de los siguientes elementos:

**Columna de trabajo pendiente**: Muestra todas las tareas que están actualmente en el registro de pendientes. Esta columna no se muestra de forma predeterminada. Para obtener más información sobre el registro de pendientes, incluido cómo mostrarlo en la [!UICONTROL Kanban] tablero, consulte [Administrar el registro de pendientes Agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Estados de historias**: indica el progreso de una historia en función de la columna de estado en la que se encuentra.

Para obtener más información, consulte [Actualizar el estado de las historias en el [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Los estados de las historias se pueden personalizar para el proyecto modificando la vista Agile, tal como se describe en la sección [[!UICONTROL Creación o personalización de una vista de Agile]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Creación o edición de vistas en [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>De forma predeterminada, se muestra un máximo de cincuenta tarjetas en el panel Kanban, pero puede hacer clic en **[!UICONTROL Mostrar más]** para mostrar tarjetas adicionales.

## Relación entre subtareas e historias

Si un artículo contiene subtareas, no se puede actualizar la información del propio artículo principal (por ejemplo, puntos/horas o porcentaje completado). Además, no puede mover la historia a través de [!UICONTROL Kanban] para actualizar su estado. En su lugar, cualquier cambio que realice en las subtareas de la historia se reflejará en la historia. Los puntos u horas del artículo combinado de todas las subtareas determinan los puntos u horas del artículo principal.

Por ejemplo, si una historia tiene solo una subtarea valorada en 4 puntos, la historia en sí también tiene 4 puntos. Si cambia el valor de punto de la subtarea a 3, el valor de punto del artículo principal cambiará a 3. Si crea otra subtarea en el mismo artículo y establece el valor de punto de esa subtarea en 4, el valor de punto del artículo se cambia a 7 para reflejar el valor de punto combinado de ambas subtareas.

Esta misma lógica se aplica a las subtareas de segundo nivel (subtareas de subtareas). Si una subtarea tiene una o más subtareas de segundo nivel, la subtarea se calcula en función de las subtareas de segundo nivel.

## Funciones compatibles

Puede realizar las siguientes acciones al utilizar el Panel Kanban:

* [Agregar una subtarea a un artículo existente en [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Agregar tareas o problemas existentes al [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Asignar usuarios a una historia en [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Agregar historias y problemas del [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Eliminar artículos o problemas de la [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Editar información de la historia](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrar por usuario en [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Administrar el límite de trabajo en curso (WIP) en [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Reordenar historias en el [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Actualizar el estado de las historias en el [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Use marcas en las historias de la [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Añada el registro de pendientes a [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
