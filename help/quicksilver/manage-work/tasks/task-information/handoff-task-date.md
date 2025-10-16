---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Resumen de fecha de transferencia de tareas
description: La fecha de transferencia es la fecha en la que una tarea se pone disponible para trabajar. Esto suele significar que sus predecesoras se resolvieron y que el usuario asignado de la tarea puede comenzar a trabajar en ella.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 99%

---

# Información general sobre la fecha de transferencia de tareas

La fecha de transferencia es la fecha en la que una tarea se pone disponible para trabajar. Esto suele significar que sus predecesoras se resolvieron y que el usuario asignado de la tarea puede comenzar a trabajar en ella.

>[!TIP]
>
>Los problemas y proyectos no tienen fechas de transferencia.

## Cálculo de la fecha de transferencia por parte de Adobe Workfront

>[!NOTE]
>
>La fecha de transferencia solo se calcula si el estado del proyecto equivale a los siguientes estados:
>
>* En espera
>* Al día
>* Completar
>* Inactivo
>

Workfront usa las siguientes reglas para calcular la fecha de transferencia de una tarea:

* **Cuando la tarea tiene un predecesor incompleto**: la fecha de transferencia de la tarea es nula.
* **Cuando la tarea tiene un predecesor completo**: la fecha de transferencia es la misma que la fecha real de finalización de la tarea predecesora. Si la tarea predecesora tuviera un retardo, Workfront calculará la fecha de transferencia de la tarea sucesora con la siguiente fórmula:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Para obtener información acerca del tiempo de retardo, consulte [Información general sobre los tipos de retardo](../use-prdcssrs/lag-types.md).

  Si la tarea sucesora tuviera más de una predecesora, la fecha de transferencia se calculará según la última fecha real de finalización de las predecesoras. Por ejemplo, si las fechas reales de finalización de las dos predecesoras fueran el 8 de noviembre de 2022 y el 20 de noviembre de 2022, la fecha de transferencia de la sucesora será el 20 de noviembre de 2022.

  >[!NOTE]
  >
  >   El cálculo de la fecha de transferencia de una tarea sucesora en función de la fecha real de finalización o de una tarea predecesora es el mismo, independientemente de si la predecesora es obligatoria o no. Para obtener más información sobre forzar predecesoras, consulte [Forzar predecesoras](../use-prdcssrs/enforced-predecessors.md).


* **Cuando la tarea no tiene predecesora y**:

   * **La fecha de inicio planificada es anterior**: la fecha de transferencia será la misma que la fecha de inicio planificada del proyecto si la tarea no tuviera establecida una restricción forzada. Para los casos en los que las tareas tienen restricciones forzadas, consulte la sección “Cuando la tarea tiene una restricción forzada para las fechas planificadas” a continuación.
   * **La fecha de inicio planificada es futura (cualquier fecha posterior a la fecha actual)**: la fecha de transferencia será la misma que la fecha de inicio planificada de la tarea si esta no tuviera establecida una delimitación forzada. Para los casos en los que las tareas tienen restricciones forzadas, consulte la sección “Cuando la tarea tiene una restricción forzada para las fechas planificadas” a continuación.

>[!NOTE]
>
>Si la tarea tuviera una predecesora entre proyectos, la fecha de transferencia de la sucesora se volverá a calcular únicamente cuando se produzca una de las siguientes situaciones:
>
>* Se puede recalcular manualmente la línea de tiempo del proyecto de la sucesora. Es necesario tener Administrar permisos del proyecto para volver a calcular la línea de tiempo.
>* La línea de tiempo del proyecto de la sucesora se recalcula automáticamente por la noche.
>
>Para obtener información sobre cómo recalcular la línea de tiempo del proyecto, consulte [Recalcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Cuando la tarea tiene una restricción forzada para las fechas planificadas**: la fecha de transferencia variará según el tipo de restricción y si la tarea tuviera o no una fecha real de inicio.\
  A continuación, se indican restricciones forzadas en tareas:

   * Debe iniciarse el
   * Debe finalizarse el
   * No iniciar antes del
   * No iniciar después del
   * Fecha fija

  Se dan los siguientes escenarios:

   * **Cuando la tarea tiene una restricción Debe iniciarse el o No iniciar antes del**: si la fecha de restricción de la tarea fuera anterior y no hubiera una fecha real de inicio en la tarea (la tarea aún no comenzó), la fecha de transferencia será la fecha más cercana posible en la que se pueda comenzar a trabajar en la tarea. Si la tarea se inició, la fecha de transferencia será igual a la fecha de inicio del proyecto.
   * **Si la tarea tiene una delimitación de Debe finalizarse el o No iniciar después del**: si la fecha de restricción de la tarea fuera futura y no hubiera una fecha real de inicio en la tarea (la tarea aún no comenzó), la fecha de transferencia será la fecha de inicio planificada para la tarea.  Si la tarea tiene como fecha real de inicio, la fecha de transferencia será la fecha de inicio del proyecto.
   * **Si la tarea tiene una restricción de fechas fijas**: la fecha de transferencia será la fecha de inicio planificada de la tarea, independientemente de si tuviera una predecesora o no e independientemente de si la predecesora se completó o no.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## Localizar la fecha de transferencia

Es posible mostrar la fecha de transferencia de una tarea en un informe de tareas o en la vista de una lista de tareas.\
Para obtener más información sobre cómo generar informes, consulte [Creación de informes personalizados](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
