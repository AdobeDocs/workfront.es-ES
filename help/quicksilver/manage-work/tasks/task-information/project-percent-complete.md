---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Resumen de porcentaje completado del proyecto
description: El valor de porcentaje completado de un proyecto se calcula en función de la duración planificada o de las horas planificadas de las tareas del proyecto. El administrador de Adobe Workfront o de un grupo define qué valor se tiene en cuenta al calcular el porcentaje completado en el sistema cuando configuran información en el área Preferencias del proyecto. Para obtener información sobre la configuración de preferencias de proyecto, consulte Configuración de preferencias de proyecto para todo el sistema.
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 94%

---

# Información general de porcentaje completado del proyecto

<!-- Audited 01/2024 -->

El valor de Porcentaje completado de un proyecto se calcula en función de la Duración o de las Horas planificadas de las tareas del proyecto. El administrador de Adobe Workfront o de un grupo define qué valor se tiene en cuenta al calcular el porcentaje completado en el sistema cuando configuran información en el área Preferencias del proyecto.

Para obtener información sobre cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

El porcentaje completado de una tarea principal se basa en la duración o en las horas planificadas de cada una de sus subtareas.

Del mismo modo, el porcentaje completado de un proyecto se basa en las duraciones o las horas planificadas de cada tarea principal del proyecto.

Las tareas principales son las tareas principales y las tareas independientes que no tienen tareas secundarias.

>[!TIP]
>
>Las tareas principales no tienen sangría en un plan de proyecto.

## Cómo calcula Workfront el porcentaje completado

### Actualizar el porcentaje completado de una tarea {#update-the-percent-complete-on-a-task}

Puede modificar el porcentaje completado de una tarea manualmente. Esto no es un cálculo.

Workfront utiliza el porcentaje completado de una tarea individual para calcular el porcentaje completado de su tarea principal o el porcentaje completado del proyecto.

Para obtener información acerca de cómo actualizar el porcentaje completado de una tarea, consulte [Ver y actualizar el porcentaje completado de las tareas](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Cómo calcula Workfront el porcentaje completado en una tarea principal {#how-workfront-calculates-percent-complete-on-a-parent-task}

Según lo que haya seleccionado el administrador de Workfront o del grupo en las Preferencias del proyecto en el nivel de sistema o de grupo, el porcentaje completado de una tarea principal se calcula en función de la duración o de las horas planificadas de las tareas.

Considere los siguientes escenarios:

* Si el sistema calcula el porcentaje completado en función de las horas planificadas, el porcentaje completado de la tarea principal se calcula mediante la siguiente fórmula:

  `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

  El total de horas planificadas de la tarea principal representa la suma de todas las horas planificadas de cada una de las tareas secundarias.

  ![Proyecto con tareas por ciento completadas y horas planificadas](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* Si el sistema calcula el porcentaje completado en función de la duración, el porcentaje completado de la tarea principal se calcula mediante la siguiente fórmula:

  `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

  ![Proyecto con cálculo de porcentaje completado y duración de tareas](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!IMPORTANT]
  >
  >La duración total de la tarea principal es el total de todas las duraciones de las tareas secundarias. Por ejemplo, una tarea principal con dos tareas secundarias que tienen una duración respectiva de 1 día y 2 días tiene una duración total de 3 días, incluso cuando las dos tareas secundarias pueden comenzar el mismo día.


### Cómo calcula Workfront el porcentaje completado de un proyecto {#how-workfront-calculates-percent-complete-on-a-project}

Según lo que haya seleccionado el administrador de Workfront o del grupo en las Preferencias del proyecto en el nivel de sistema o de grupo, el porcentaje completado de un proyecto se calculará en función de la duración o de las horas planificadas de las tareas principales del proyecto.

* Si el sistema calcula el porcentaje completado en función de las horas planificadas, el porcentaje completado del proyecto se calcula mediante la siguiente fórmula:

  `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

  El total de horas planificadas del proyecto es la suma de las horas planificadas de todas las tareas principales del proyecto.

  ![Proyecto con cálculo de horas planificadas y porcentaje completado de tareas](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

  >[!NOTE]
  >
  >La Tarea 1 o la Tarea 2 solo pueden ser tareas principales o independientes. Las tareas Horas planificadas y Porcentaje completado de tareas secundarias no se utilizan en este cálculo.

* Si el sistema calcula el porcentaje completado en función de la Duración, el porcentaje completado del proyecto se calcula mediante la siguiente fórmula:

  `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

  >[!IMPORTANT]
  >
  >La duración del proyecto es el total de todas las duraciones de las tareas principales que muestran un porcentaje completado. Por ejemplo, un proyecto con una tarea independiente con una Duración de 2 días y una tarea principal con una Duración de 5 días en los que se haya completado el trabajo tendrá una Duración total de 7 días, incluso si las dos tareas pueden comenzar el mismo día.

  ![Proyecto con cálculo de porcentaje completado y duración de tareas](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!NOTE]
  >
  >La Tarea 1 o la Tarea 2 solo pueden ser tareas principales o independientes. Las tareas de Duración y Porcentaje completado de tareas secundarias no se utilizan en este cálculo.

## Ejemplo de porcentaje completado en un proyecto mediante Duración

Cuando utilice la Duración de las tareas para calcular el porcentaje completado de un proyecto, tenga en cuenta el siguiente ejemplo:

![Proyecto con cálculo de porcentaje completado y duración de tareas](assets/project-with-tasks-percent-complete-duration-calculation.png)

La siguiente información se utiliza para calcular el porcentaje completado del proyecto

* Porcentaje completado de la tarea independiente (Tarea 1 - 20 %)
* El porcentaje completado de la tarea principal (Tarea 2 - 25 %)
* La duración de la Tarea 1 (5 días)
* La duración de la Tarea 2 (2 días)
* La duración del proyecto (7 días)


Para calcular el porcentaje completado del proyecto mediante Duración:

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

O

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->
