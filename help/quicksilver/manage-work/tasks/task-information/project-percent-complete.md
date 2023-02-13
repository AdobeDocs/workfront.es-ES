---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Resumen de finalización del porcentaje del proyecto
description: El valor Porcentaje completado de un proyecto se calcula en función de la duración prevista o las horas previstas de las tareas del proyecto. El administrador de Adobe Workfront o un administrador de grupo define qué valor se tiene en cuenta al calcular el porcentaje completado en el sistema cuando configuran la información en el área Preferencias del proyecto. Para obtener información sobre la configuración de las preferencias del proyecto, consulte Configuración de las preferencias de proyecto de todo el sistema.
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 31533bd7ee1890a8343d32770d623d5d9a6007d2
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Resumen de finalización del porcentaje del proyecto

El valor Porcentaje completado de un proyecto se calcula en función de la duración o las horas previstas de las tareas del proyecto. El administrador de Adobe Workfront o un administrador de grupo define qué valor se tiene en cuenta al calcular el porcentaje completado en el sistema cuando configuran la información en el área Preferencias del proyecto.

Para obtener información sobre cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

El porcentaje de finalización de una tarea principal se basa en la duración o horas planificadas de cada una de sus subtareas.

Del mismo modo, el porcentaje de finalización de un proyecto se basa en las duraciones u horas planificadas de cada tarea principal del proyecto.

Las tareas principales son las tareas principales y las tareas independientes que no tienen elementos secundarios.

>[!TIP]
>
>Las tareas principales no se sangran en un plan de proyecto.

## Cómo calcula Workfront el porcentaje completado

* [Actualizar el porcentaje completado en una tarea](#update-the-percent-complete-on-a-task)
* [Cómo calcula Workfront el porcentaje completado en una tarea principal](#how-workfront-calculates-percent-complete-on-a-parent-task)
* [Cómo calcula Workfront el porcentaje completado en un proyecto](#how-workfront-calculates-percent-complete-on-a-project)

### Actualizar el porcentaje completado en una tarea {#update-the-percent-complete-on-a-task}

Puede modificar el porcentaje completado de una tarea manualmente. Esto no es un cálculo.

Workfront utiliza el porcentaje completado de una tarea individual para calcular el porcentaje completado de su tarea principal o el porcentaje completado del proyecto.

Para obtener información sobre la actualización del porcentaje completado de una tarea, consulte [Ver y actualizar el porcentaje completado para las tareas](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Cómo calcula Workfront el porcentaje completado en una tarea principal {#how-workfront-calculates-percent-complete-on-a-parent-task}

Dependiendo de lo que haya seleccionado el administrador de Workfront o de grupo en Preferencias de proyecto a nivel de sistema o grupo, el porcentaje completado de una tarea principal se calcula en función de la duración o las horas planificadas de las tareas.

Consideremos los siguientes escenarios:

* Si el sistema calcula el porcentaje completado en función de las horas planificadas, el porcentaje de la tarea principal finalizada se calcula mediante la fórmula siguiente:

   `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

   El total de horas planificadas del padre representa la suma de todas las horas planificadas de cada uno de los hijos.

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* Si el sistema calcula el porcentaje completado en función de la duración, el porcentaje completado de la tarea principal se calcula mediante la fórmula siguiente:

   `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!IMPORTANT]
   >
   >La duración total de la tarea principal es el total de todas las duraciones de las tareas secundarias. Por ejemplo, una tarea principal con dos hijos que tienen una duración respectiva de 1 día y 2 días tiene una duración total de 3 días, incluso cuando los dos hijos pueden empezar en el mismo día.


### Cómo calcula Workfront el porcentaje completado en un proyecto {#how-workfront-calculates-percent-complete-on-a-project}

Dependiendo de lo que haya seleccionado el administrador de Workfront o de grupo en Preferencias de proyecto a nivel de sistema o grupo, el porcentaje completado de un proyecto se calcula en función de la duración o las horas planificadas de las principales tareas del proyecto.

* Si el sistema calcula el porcentaje completado en función de las horas planificadas, el porcentaje completado del proyecto se calcula mediante la fórmula siguiente:

   `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

   El total de horas previstas del proyecto es la suma de las horas previstas de todas las tareas principales del proyecto.

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

   >[!NOTE]
   >
   >La tarea 1 o la tarea 2 solo pueden ser tareas principales o tareas independientes. En este cálculo no se utilizan las tareas Horas planificadas y Porcentaje completado de elementos secundarios.

* Si el sistema calcula el porcentaje completado en función de la duración, el porcentaje completado del proyecto se calcula mediante la fórmula siguiente:

   `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

   >[!IMPORTANT]
   >
   >La duración del proyecto es el total de todas las duraciones de las tareas principales que muestran un porcentaje completado. Por ejemplo, un proyecto con una tarea independiente con una duración de 2 días y una tarea principal con una duración de 5 días que hayan completado el trabajo en ellos tendrá una duración total de 7 días, incluso si las dos tareas pueden iniciarse el mismo día.

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!NOTE]
   >
   >La tarea 1 o la tarea 2 solo pueden ser tareas principales o tareas independientes. Las tareas secundarias Duración y Porcentaje completado no se utilizan en este cálculo.

## Ejemplo de porcentaje completado en un proyecto mediante Duración

Cuando utilice la Duración de las tareas para calcular el porcentaje completado de un proyecto, tenga en cuenta el siguiente ejemplo:

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

La siguiente información se utiliza para calcular el porcentaje completado del proyecto

* Porcentaje completado de la tarea independiente (Tarea 1 - 20%)
* Porcentaje completado de la tarea principal (Tarea 2 - 25%)
* Duración de la tarea 1 (5 días)
* Duración de la tarea 2 (2 días)
* Duración del proyecto (7 días)


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