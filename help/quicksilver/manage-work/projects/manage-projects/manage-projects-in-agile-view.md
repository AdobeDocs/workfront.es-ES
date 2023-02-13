---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Administrar un proyecto en la vista Águila
description: Planes requeridos, tipos de licencia y acceso a los permisos de tipo de licencia de Adobe Workfront Plan Team, Pro, Business o Enterprise Workfront Review, Work or Plan en el modelo de acceso Editar acceso y capacidad de crear informes, tableros y calendarios
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1311'
ht-degree: 0%

---

# Administrar un proyecto en la vista Águila

Planes, tipos de licencia y acceso requeridos

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Plan de Adobe Workfront</a> </p> </td> 
   <td> <p>Equipo, Pro, Negocios o Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="https://one.workfront.com/s/article/Understanding-License-Types-906212506?language=en_US&amp;r=16&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank">Tipo de licencia de Workfront</a> </p> </td> 
   <td> <p>Revisión, trabajo o plan </p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
  --> 
 </tbody> 
</table>

Puede aprovechar la funcionalidad ágil para su proyecto

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(such as story boards and burndown charts)
</MadCap:conditionalText>
-->

 sin los desafíos administrativos que normalmente acompañan a las prácticas ágiles (como administrar un trabajo acumulado del equipo o crear iteraciones).

Si desea trabajar en un entorno ágil que utilice un trabajo acumulado del equipo y le permite crear iteraciones a partir de tareas en el trabajo pendiente, siga las instrucciones de [Trabajar en un entorno ágil](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Edite el acceso a las siguientes áreas:</p> 
    <ul> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Informes, tableros y calendarios</p> </li> 
     <li> <p>Filtros, Vistas, Agrupaciones</p> </li> 
    </ul> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos del proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Comprender los proyectos de Agile

* [Funcionalidad ágil en un proyecto](#agile-functionality-in-a-project)
* [Diferencias entre el uso de la vista Águila en un proyecto y el de una iteración](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Funcionalidad ágil en un proyecto {#agile-functionality-in-a-project}

La siguiente funcionalidad ágil está disponible al administrar un proyecto en una vista ágil:

* Estado de finalización\
   Para obtener información más detallada sobre el estado de finalización, consulte [Resumen del estado de finalización de iteración](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Tablero de historia\
   Para obtener información más detallada sobre el tablero de artículos, consulte la [Tablero de limpieza](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) para obtener más información.

Existen algunas diferencias al utilizar vistas ágiles en un proyecto en comparación con trabajar en un entorno totalmente ágil (con registros atrasados e iteraciones). Para obtener más información, consulte [Diferencias entre el uso de la vista Águila en un proyecto y el de una iteración](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) en este artículo.

### Diferencias entre el uso de la vista Águila en un proyecto y el de una iteración {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Las tareas y subtareas siguen distintas reglas de visualización en el panel de artículos](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [No se utilizan registros de registro e iteraciones](#backlogs-and-iterations-are-not-used)
* [El orden de las tareas se mantiene en la vista Águila y no se puede reordenar](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [Las tareas solo se miden en horas planificadas](#tasks-are-measured-only-in-planned-hours)
* [El Agile Team no se usa](#the-agile-team-is-not-used)
* [Cada usuario del proyecto puede ver el proyecto en una vista Agile diferente](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Las tareas y subtareas siguen distintas reglas de visualización en el panel de artículos {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Las tareas que no tienen una tarea principal ni una subtarea siempre se muestran como una tarjeta de artículo único en el tablero de artículos.\
   Por ejemplo, estas tareas aparecen de la siguiente manera en la vista de lista de proyectos:

   ![Lista de proyectos ágiles: tareas sin tareas principales o subtareas](assets/agile-project-single-list-nwe.png) Estas tareas aparecen de la siguiente manera en la vista ágil del proyecto:

   ![Vista ágil del proyecto: tareas sin tareas principales o subtareas](assets/agile-project-singlecard-nwe.png)

* Las tareas principales que tienen subtareas siempre se muestran en la **Historias** del tablero de artículos. Las subtareas se muestran en la ruta de navegación de la tarea principal.\
   Por ejemplo, estas tareas aparecen de la siguiente manera en la vista de lista de proyectos:

   ![Lista de proyectos de Agile: tareas con elementos principales y subtareas](assets/agile-project-parent-list-nwe.png)\
   Estas tareas aparecen de la siguiente manera en la vista ágil del proyecto:

   ![Vista de proyecto ágil: tareas con elementos principales y subtareas](assets/agile-project-parent-nwe.png)

* Las subtareas de segundo nivel (subtareas de subtareas) se muestran como una tarjeta gris colgante de la tarea principal inmediata.
* Las subtareas de tercer nivel (subtareas de subtareas de subtareas) nunca se muestran en el panel de artículos.

#### No se utilizan registros de registro e iteraciones {#backlogs-and-iterations-are-not-used}

Al ver un proyecto en una vista ágil, no se utilizan los siguientes componentes ágiles:

* **Retraso:** No se utiliza ningún retraso porque las tareas del proyecto se muestran automáticamente como artículos.
* **Iteraciones:** En lugar de crear iteraciones para definir las fechas en las que se completará el trabajo, los días designados actualmente en el cronograma del proyecto se convierten en días laborables.

#### El orden de las tareas se mantiene en la vista Águila y no se puede reordenar {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

El orden en que aparecen las tareas en un proyecto se mantiene cuando se ve el proyecto en un tablero de artículos ágil.

No se pueden reordenar las tareas del proyecto al visualizarlo en una vista ágil. Como la modificación del orden de tareas puede afectar a otras tareas que pueden tener dependencias, debe ver el proyecto en una vista estándar para modificar el orden de las tareas.

#### Las tareas solo se miden en horas planificadas {#tasks-are-measured-only-in-planned-hours}

Las tareas de un proyecto siempre se miden en horas planificadas.

En una iteración, las tareas (artículos) se pueden medir en horas o puntos.

#### El Agile Team no se usa {#the-agile-team-is-not-used}

Dado que los equipos ágiles completan el trabajo en iteraciones asignadas a ellos, no se utilizan equipos ágiles al ver un proyecto en una vista ágil.

En su lugar, cualquier usuario del proyecto se convierte esencialmente en el equipo ágil para ese proyecto.

#### Cada usuario del proyecto puede ver el proyecto en una vista Agile diferente {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

A diferencia de una iteración ágil, los usuarios de un proyecto pueden personalizar la vista ágil por sí mismos, mientras que otros usuarios utilizan una vista ágil diferente.

En una iteración ágil, la información disponible en el tablero de artículos ágil (como las columnas de estado disponibles) se determina en el nivel de equipo.

Para obtener información sobre cómo personalizar una vista ágil, consulte  [Creación o personalización de una vista Águila](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) en  [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## Ver un proyecto en la vista Águila

1. Vaya al proyecto que desea ver en una vista ágil.
1. Haga clic en el **Águila** icono.\
   ![Icono Águila](assets/agile-icon-nwe.png)\
   El proyecto se muestra en la vista ágil predeterminada.\
   Si anteriormente ha visto el proyecto en una vista ágil personalizada, el proyecto se muestra en esa vista en lugar de en la vista ágil predeterminada.

1. (Opcional) Si ha creado una vista ágil personalizada o si otro usuario ha creado una vista ágil personalizada y la ha compartido con usted, puede verla en lugar de la vista ágil predeterminada.\
   Haga clic en el **Ver** menú desplegable y, a continuación, haga clic en la vista ágil personalizada que desee ver.

   La próxima vez que haga clic en el botón **Águila** icono.\
   Para obtener información sobre cómo crear una nueva vista ágil, consulte [Creación y personalización de vistas de Agile](#create-and-customize-agile-views).\
   El proyecto se muestra en la vista ágil personalizada.

1. (Condicional) Si las tareas del proyecto utilizan estados distintos de &quot;Nuevo&quot;, &quot;En curso&quot; o &quot;Completado&quot; (los estados predeterminados de la vista Águila), debe agregar los estados adicionales a la vista Águila para que se muestren todas las tareas de esos estados.\
   Si las tareas están en un estado que no se muestra en el tablero de artículos ágil, la tarea en sí no se muestra en el tablero de artículos ágil (sin embargo, el porcentaje completado de estas tareas sigue contribuyendo al porcentaje completado de cualquier tarea principal y al porcentaje completado del proyecto general).\
   Para agregar estados a la vista ágil, cree una nueva vista ágil o personalice una vista ágil existente, tal como se describe en la sección &quot;Crear o personalizar una vista Águila&quot; del artículo [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Opcional) Para volver a la vista de lista, haga clic en el **Lista** icono.\
   ![](assets/list-icon.png)

## Creación y personalización de vistas de Agile {#create-and-customize-agile-views}

Al igual que con las vistas estándar en Workfront, puede personalizar las vistas ágiles existentes o crear nuevas vistas ágiles desde cero. A diferencia de las vistas estándar, no puede crear nuevas vistas ágiles basadas en las vistas ágiles existentes.

Para obtener más información sobre la creación y personalización de vistas ágiles, consulte la sección &quot;Crear o personalizar una vista Águila&quot; en el artículo [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## Compartir una vista Agile existente

Para obtener información sobre cómo compartir una vista ágil, consulte [Compartir un filtro, una vista o una agrupación](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Eliminar una vista ágil existente

Para obtener información sobre cómo eliminar una vista, consulte la sección &quot;Eliminar una vista&quot; del artículo [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 
