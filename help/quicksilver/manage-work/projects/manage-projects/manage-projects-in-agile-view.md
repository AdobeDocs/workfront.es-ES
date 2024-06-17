---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Administrar un proyecto en la vista de Agile
description: Puede aprovechar la funcionalidad Agile para su proyecto sin los desafíos administrativos que normalmente acompañan a las prácticas Agile (como administrar un registro de asuntos pendientes del equipo o crear iteraciones).
author: Alina and Lisa
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1423'
ht-degree: 0%

---

# Administrar un proyecto en la vista de Agile

<!-- Audited: 2/2024 -->

Puede aprovechar la funcionalidad Agile para su proyecto sin los desafíos administrativos que normalmente acompañan a las prácticas Agile (como administrar un registro de asuntos pendientes del equipo o crear iteraciones).

Si desea trabajar en un entorno Agile que utilice un registro de asuntos pendientes del equipo y le permita crear iteraciones a partir de las tareas del registro de asuntos pendientes, siga las instrucciones de [Trabajar en un entorno ágil](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Actual: revisar o superior</p> 
   <p>Nuevo: Colaborador o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuración del nivel de acceso</td> 
   <td> <p>Edite el acceso a las siguientes áreas:</p> 
    <ul> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Informes, paneles y calendarios</p> </li> 
     <li> <p>Filtros, vistas y agrupaciones</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos del proyecto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comprender los proyectos de Agile

>[!NOTE]
>
>Esta sección solo se aplica a la vista de Agile heredada, no a la vista de tablero de un proyecto.

* [Funcionalidad Agile en un proyecto](#agile-functionality-in-a-project)
* [Diferencias entre utilizar la vista de Agile en un proyecto y en una iteración](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Funcionalidad Agile en un proyecto {#agile-functionality-in-a-project}

La siguiente funcionalidad Agile está disponible al administrar un proyecto en una vista Agile:

* Estado de finalización\
  Para obtener información más detallada sobre el estado de finalización, consulte [Resumen del estado de finalización de iteraciones](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Tablero de historias\
  Para obtener información más detallada sobre el guion gráfico, consulte la [Tablero Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) sección.

Existen algunas diferencias entre utilizar las vistas de Agile en un proyecto y trabajar en un entorno Agile puro (con trabajos pendientes e iteraciones). Para obtener más información, consulte [Diferencias entre utilizar la vista de Agile en un proyecto y en una iteración](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) en este artículo.

### Diferencias entre utilizar la vista de Agile en un proyecto y en una iteración {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Las tareas y subtareas siguen diferentes reglas de visualización en una vista de proyecto de Agile y en el guion gráfico de una iteración](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [Los trabajos pendientes y las iteraciones no se utilizan en la vista de Agile](#backlogs-and-iterations-are-not-used)
* [El orden de las tareas se mantiene en la vista de Agile y no se puede reordenar](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [Las tareas se miden solamente en horas planificadas en una lista de proyectos](#tasks-are-measured-only-in-planned-hours)
* [El equipo Agile no se utiliza en una vista Agile](#the-agile-team-is-not-used)
* [Cada usuario del proyecto puede ver el proyecto en una vista diferente de Agile](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Las tareas y subtareas siguen diferentes reglas de visualización en una vista de proyecto de Agile y en el guion gráfico de una iteración {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Las tareas que no tienen una tarea principal ni una subtarea se muestran siempre como una tarjeta de artículo único en el panel de artículos de la vista de Agile.\
  Por ejemplo, estas tareas aparecen de la siguiente manera en la vista de la lista de proyectos:

  ![Lista de proyectos de Agile: tareas sin tareas principales ni subtareas](assets/agile-project-single-list-nwe.png)

  Estas tareas aparecen de la siguiente manera en la vista Agile del proyecto:

  ![Vista Agile del proyecto: tareas sin tareas principales ni subtareas](assets/agile-project-singlecard-nwe.png)

* Las tareas principales que tienen subtareas siempre se muestran en la variable **Historias** del guion gráfico de la vista de Agile. Las subtareas se muestran en la barra de tareas de la tarea principal.\
  Por ejemplo, estas tareas aparecen de la siguiente manera en la vista de la lista de proyectos:

  ![Lista de proyectos de Agile: tareas con tareas principales y subtareas](assets/agile-project-parent-list-nwe.png)\
  Estas tareas aparecen de la siguiente manera en la vista Agile del proyecto:

  ![Vista de proyecto de Agile: tareas con tareas principales y subtareas](assets/agile-project-parent-nwe.png)

* Las subtareas de segundo nivel (subtareas de subtareas) se muestran como una tarjeta gris que se bloquea en la tarea principal inmediata.
* Las subtareas de tercer nivel (subtareas de subtareas de subtareas) nunca se muestran en la vista Agile.

#### Los trabajos pendientes y las iteraciones no se utilizan en la vista de Agile {#backlogs-and-iterations-are-not-used}

Cuando se visualiza un proyecto en una vista Agile, no se utilizan los siguientes componentes Agile:

* **Registro de pendientes:** No se utiliza ningún registro de pendientes porque todas las tareas del proyecto se muestran automáticamente como historias.
* **Iteraciones:** En lugar de crear iteraciones para definir las fechas en que se realizará el trabajo, los días designados actualmente en la escala de tiempo del proyecto se convierten en días laborables.

#### El orden de las tareas se mantiene en la vista de Agile y no se puede reordenar {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

El orden en que aparecen las tareas en un proyecto se mantiene cuando se ve el proyecto en un panel de historias Agile.

No se pueden reordenar las tareas del proyecto al verlo en una vista Agile. Dado que modificar el orden de las tareas puede afectar a otras tareas que pueden tener dependencias, debe ver el proyecto en una vista estándar para poder modificar el orden de las tareas.

#### Las tareas se miden solamente en horas planificadas en una lista de proyectos {#tasks-are-measured-only-in-planned-hours}

Las tareas de un proyecto siempre se miden en horas planificadas.

En una iteración, las tareas (historias) se pueden medir en horas o puntos.

#### El equipo Agile no se utiliza en una vista Agile {#the-agile-team-is-not-used}

Debido a que los equipos Agile completan el trabajo en las iteraciones que se les asignan, los equipos Agile no se utilizan al ver un proyecto en una vista Agile.

En su lugar, los usuarios del proyecto se convertirán esencialmente en el equipo Agile de ese proyecto.

#### Cada usuario del proyecto puede ver el proyecto en una vista diferente de Agile {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

A diferencia de una iteración Agile, los usuarios de un proyecto pueden personalizar la vista Agile por sí mismos, mientras que otros usuarios utilizan una vista Agile diferente.

En una iteración Agile, la información disponible en el panel de historias Agile (como las columnas de estado disponibles) se determina en el nivel de equipo.

Para obtener información sobre cómo personalizar una vista Agile, consulte [Creación o personalización de una vista de Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Creación o edición de vistas en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Ver un proyecto en la vista de Agile

1. Vaya al proyecto que desee ver en una vista Agile, en la lista de tareas o en la lista de problemas.
1. Haga clic en **Vista de tablero** icono ![Icono de tablero](assets/board-icon-for-agile-view.png).

   La vista de tablero del proyecto se muestra de forma predeterminada.

   ![Vista de tablero del proyecto](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (Opcional) Haga clic en **Configurar** para definir las opciones de las columnas y las tarjetas.

   Para obtener más información, consulte [Administrar columnas del tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) y [Personalizar los campos que se muestran en una tarjeta](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). Tenga en cuenta que no puede definir directivas de columna en la vista de tablero de un proyecto.

1. (Opcional) Haga clic en **Usar Agile heredado** para utilizar la vista heredada de agile en lugar de la vista de tablero.

1. (Opcional: solo vista Agile heredada) Si ha creado una vista Agile personalizada, o si otro usuario ha creado una vista Agile personalizada y la ha compartido con usted, puede verla en lugar de la vista Agile predeterminada.

   Haga clic en **Ver** menú desplegable y, a continuación, haga clic en la vista de agile personalizada que desee ver.

   La vista Agile personalizada se utilizará la próxima vez que haga clic en **Agile** icono.

   Para obtener información sobre cómo crear una nueva vista Agile, consulte [Creación y personalización de vistas de Agile](#create-and-customize-agile-views), más abajo.

   El proyecto se muestra en la vista Agile personalizada.

1. (Condicional: solo vista Agile heredada) Si las tareas del proyecto utilizan estados que no sean &quot;Nuevo&quot;, &quot;En curso&quot; o &quot;Completado&quot; (los estados predeterminados de la vista Agile), debe agregar los estados adicionales a la vista Agile para que se muestren todas las tareas de esos estados.

   Si las tareas están en un estado que no se muestra en el panel de historias Agile, la tarea en sí no se muestra en el panel de historias Agile (sin embargo, el porcentaje completado de estas tareas sigue contribuyendo al porcentaje completado de cualquier tarea principal y al porcentaje completado del proyecto general).

   Para agregar estados a la vista Agile, cree una nueva vista Agile o personalice una vista Agile existente, tal como se describe en [Creación y personalización de vistas de Agile](#create-and-customize-agile-views), más abajo.

1. (Opcional) Para volver a la vista de lista, haga clic en **Lista** icono.

## Creación y personalización de vistas de Agile {#create-and-customize-agile-views}

>[!NOTE]
>
>Esta sección solo se aplica a la vista de Agile heredada, no a la vista de tablero de un proyecto.

Al igual que con las vistas estándar en Workfront, puede personalizar las vistas Agile existentes o crear nuevas vistas Agile desde cero. A diferencia de las vistas estándar, no puede crear nuevas vistas de Agile basadas en vistas de Agile existentes.

Para obtener más información sobre la creación y personalización de vistas de Agile, consulte la [Creación o personalización de una vista de Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) en el artículo [Creación o edición de vistas en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Compartir una vista de Agile existente

>[!NOTE]
>
>Esta sección solo se aplica a la vista de Agile heredada, no a la vista de tablero de un proyecto.

Puede compartir una vista de Agile que haya creado o a la que tenga permisos de la misma manera que comparte cualquier otra vista, filtro o agrupación.

Para obtener más información, consulte [Compartir un filtro, una vista o una agrupación](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Eliminar una vista de Agile existente

>[!NOTE]
>
>Esta sección solo se aplica a la vista de Agile heredada, no a la vista de tablero de un proyecto.

Puede quitar una vista de Agile del mismo modo que quita cualquier otra vista, filtro o agrupación.

Para obtener más información, consulte la [Eliminación de filtros, vistas y agrupaciones](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
