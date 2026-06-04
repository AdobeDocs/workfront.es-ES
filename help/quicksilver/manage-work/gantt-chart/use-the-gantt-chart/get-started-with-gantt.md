---
content-type: overview
navigation-topic: use-the-gantt-chart
title: Introducción al gráfico [!UICONTROL Gantt]
description: Los diagramas de Gantt de Adobe Workfront proporcionan una representación visual de la cronología de una lista de tareas o proyectos.
author: Alina
feature: Work Management
exl-id: 96c4e254-ebbe-41d8-a178-7a79ac0abbbd
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/pqhHIt4ISb8XZ0ApgM-oqkFwc-L2KHOZVsVhwbSJ5jQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 538
ht-degree: 8%

---

# Empezar a usar el [!UICONTROL gráfico Gantt]

<!-- Audited: 08/2025 -->

Los diagramas de Gantt de Adobe Workfront proporcionan una representación visual de la cronología de una lista de tareas o proyectos.

En [!DNL Adobe Workfront], hay dos [!UICONTROL diagramas de Gantt] con una funcionalidad similar:

* **La lista de tareas [!UICONTROL Diagrama de Gantt]**: muestra información sobre las tareas y su cronología a nivel de proyecto. Un [!UICONTROL gráfico Gantt] similar muestra información sobre tareas de plantilla en el nivel de plantilla.
* **La lista de proyectos [!UICONTROL Diagrama de Gantt]**: muestra información sobre los proyectos y su cronología.

Aunque se ven y se sienten similares, la funcionalidad de cada uno es diferente.

## Consideraciones sobre el gráfico Gantt

* Puede editar la información en el siguiente [!UICONTROL gráfico Gantt]:
   * Una lista de tareas
* No se puede editar la información en los siguientes [!UICONTROL diagramas de Gantt]:
   * Una lista de tareas de plantilla
   * Una lista de proyectos
* No hay ninguna opción de [!UICONTROL gráfico Gantt] para una lista de plantillas.
* Puede configurar la información que se muestra en la lista de tareas [!UICONTROL Diagrama de Gantt] y en la lista de proyectos [!UICONTROL Diagrama de Gantt].
* No puede configurar los colores ni las fuentes en las que se muestra la información del [!UICONTROL gráfico Gantt].
* Cuando la información se actualiza desde las tareas, se refleja automáticamente tanto en la lista de tareas [!UICONTROL Diagrama de Gantt] como en la lista de proyectos [!UICONTROL Diagrama de Gantt].
* Cuando la información se actualiza desde las tareas de plantilla, se refleja automáticamente en la lista de tareas de plantilla [!UICONTROL Diagrama de Gantt].

## Obtener acceso al [!UICONTROL gráfico Gantt]

Los gráficos [!UICONTROL Gantt] de [!DNL Workfront] proporcionan una representación visual de una lista de tareas o proyectos.

Puede ver la lista de tareas [!UICONTROL Diagrama de Gantt] directamente desde la lista de tareas de un proyecto o desde un informe de tareas.

Puede ver la lista de proyectos [!UICONTROL Diagrama de Gantt] en una lista de proyectos o un informe de proyectos.

### Lista de tareas [!UICONTROL Diagrama de Gantt] {#task-list-gantt-chart}

<!--
The task list [!UICONTROL Gantt Chart] is accessible in the following areas:

* In a Project

   * [!UICONTROL Tasks] section
   * [!UICONTROL Subtasks] section of a task

* In a [!UICONTROL Template]

* In a [!UICONTROL Task] report
-->

Para obtener acceso a la lista de tareas [!UICONTROL Diagrama de Gantt] de un proyecto o una plantilla:

1. Vaya a cualquiera de las siguientes áreas:

   * Cree un proyecto y luego haga clic en [!UICONTROL **Tareas**] en el panel izquierdo.
   * Seleccione una plantilla y luego haga clic en [!UICONTROL **Tareas de plantilla**] en el panel izquierdo
   * Una tarea o tarea de plantilla y, a continuación, haga clic en [!UICONTROL **Subtareas**] en el panel izquierdo.
   * Un informe de tareas

1. Haga clic en el icono [!UICONTROL **Gantt**] ![icono Gantt](assets/gantt-icon-nwe.png) en la parte superior de la lista de tareas.

   ![Gantt de lista de tareas](assets/task-list-gantt.png)

   La lista de tareas [!UICONTROL Diagrama de Gantt] se abre a la derecha de la lista de tareas.

1. Para configurar la información que desea mostrar en el gráfico [!UICONTROL Gantt] de la tarea, haga clic en el icono [!UICONTROL **Configuración**] y, a continuación, habilite cualquiera de las siguientes opciones:

   * [!UICONTROL Actual Dates]
   * [!UICONTROL Asignaciones]
   * [!UICONTROL Línea de base]
   * [!UICONTROL Fecha de compromiso]
   * [!UICONTROL % completado]
   * [!UICONTROL Ruta crítica]
   * [!UICONTROL Diamantes de hito]
   * [!UICONTROL Líneas de hito]
   * [!UICONTROL Predecesoras]
   * [!UICONTROL Estado de progreso]
   * [!UICONTROL Fechas proyectadas]

1. Comience a editar las tareas como se describe en los siguientes artículos:

   * [Configurar cómo se muestra la información en el gráfico Gantt](../use-the-gantt-chart/configure-info-on-gantt-chart.md)
   * [Actualización de la información en el gráfico Gantt de la lista de tareas](../use-the-gantt-chart/update-info-task-list-gantt.md)

### Lista de proyectos [!UICONTROL Diagrama de Gantt] {#project-list-gantt-chart}

<!--
The project list [!UICONTROL Gantt Chart] is accessible in the following areas:

* In the [!UICONTROL Projects] area
* In the [!UICONTROL Projects] section of a [!UICONTROL Portfolio]
* In the [!UICONTROL Projects] section of a [!UICONTROL Program]
* In a [!UICONTROL Project] report
-->

Para obtener acceso a la lista de proyectos [!UICONTROL Diagrama de Gantt]:

1. Vaya a cualquiera de las siguientes áreas:

   * El área [!UICONTROL **Proyectos**]
   * La sección [!UICONTROL **Proyectos**] de un [!UICONTROL Portfolio]
   * La sección [!UICONTROL **Proyectos**] de un [!UICONTROL Programa]
   * Un informe de [!UICONTROL **proyecto**]

1. Haga clic en el icono [!UICONTROL **Gantt**] que se encuentra en la parte superior de la lista de proyectos.

   ![Gantt de lista de proyectos](assets/project-list-gantt.png)

   Se abre la lista de proyectos [!UICONTROL Diagrama de Gantt].

1. Para configurar la información que desea mostrar en el gráfico del proyecto [!UICONTROL Gantt], haga clic en el icono [!UICONTROL **Configuración**] y, a continuación, habilite cualquiera de las siguientes opciones:

   * [!UICONTROL Actual Dates]
   * [!UICONTROL % completado]
   * [!UICONTROL Diamantes de hito]
   * [!UICONTROL Líneas de hito]
   * [!UICONTROL Predecesoras]
   * [!UICONTROL Estado de progreso]
   * [!UICONTROL Fechas proyectadas]
