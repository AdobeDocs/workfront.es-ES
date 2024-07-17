---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Resumen de fecha de transferencia de tareas
description: La fecha de transferencia es la fecha en la que una tarea está disponible para trabajar. Esto suele significar que sus predecesoras se han resuelto y que el usuario asignado de la tarea puede empezar a trabajar en ella.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 2%

---

# Resumen de fecha de transferencia de tareas

La fecha de transferencia es la fecha en la que una tarea está disponible para trabajar. Esto suele significar que sus predecesoras se han resuelto y que el usuario asignado de la tarea puede empezar a trabajar en ella.

>[!TIP]
>
>Las fechas de transferencia no existen para problemas y proyectos.

## Cálculo de la fecha de transferencia por parte de Adobe Workfront

>[!NOTE]
>
>La fecha de entrega solo se calcula si el estado del proyecto equivale a los siguientes estados:
>
>* En espera
>* Al día
>* Completar
>* Inactivo
>

Workfront utiliza las siguientes reglas para calcular la fecha de transferencia de una tarea:

* **Cuando la tarea tiene un predecesor incompleto**: La fecha de transferencia de la tarea es nula.
* **Cuando la tarea tiene un predecesor completo**: la fecha de transferencia es la misma que la fecha real de finalización de la tarea predecesora. Si la tarea predecesora tiene un retardo, Workfront calcula la fecha de transferencia de la tarea sucesora mediante la siguiente fórmula:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Para obtener información acerca del tiempo de retardo, vea [Información general sobre los tipos de retardo](../use-prdcssrs/lag-types.md).

  Si la tarea sucesora tiene más de una predecesora, la fecha de transferencia se calcula según la última fecha real de finalización de las predecesoras. Por ejemplo, si las fechas de finalización reales de las dos predecesoras son el 8 de noviembre de 2022 y el 20 de noviembre de 2022, la fecha de transferencia de la sucesora es el 20 de noviembre de 2022.

  >[!NOTE]
  >
  >   El cálculo de la fecha de transferencia de una tarea sucesora en función de la fecha real de finalización o de una tarea predecesora es el mismo independientemente de si la predecesora es obligatoria o no. Para obtener más información sobre predecesoras forzadas, vea [Aplicar predecesoras](../use-prdcssrs/enforced-predecessors.md).


* **Cuando la tarea no tiene predecesora y**:

   * **La fecha planificada de inicio es anterior**: la fecha de transferencia es la misma que la fecha planificada de inicio del proyecto si la tarea no tiene establecida una restricción forzada. Para los casos en los que las tareas tienen restricciones forzadas, consulte la sección &quot;Cuando la tarea tiene una restricción forzada para las fechas planificadas&quot; a continuación.
   * **La fecha planificada de inicio es futura (cualquier fecha posterior a la fecha actual)**: la fecha de transferencia es la misma que la fecha planificada de inicio de la tarea si esta no tiene establecida una delimitación forzada. Para los casos en los que las tareas tienen restricciones forzadas, consulte la sección &quot;Cuando la tarea tiene una restricción forzada para las fechas planificadas&quot; a continuación.

>[!NOTE]
>
>Cuando la tarea tiene una predecesora entre proyectos, la fecha de transferencia de la sucesora se vuelve a calcular únicamente cuando se produce una de las siguientes situaciones:
>
>* Se puede recalcular manualmente la escala de tiempo del proyecto del sucesor. Debe tener permisos de administración en el proyecto para volver a calcular la escala de tiempo.
>* La cronología del proyecto del sucesor se recalcula automáticamente por la noche.
>
>Para obtener información sobre cómo recalcular la escala de tiempo del proyecto, vea [Recalcular escala de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Cuando la tarea tiene una restricción forzada para las fechas planificadas**: la fecha de transferencia varía según el tipo de restricción y si la tarea tiene o no una fecha de inicio real.\
  A continuación se indican restricciones forzadas en tareas:

   * Debe iniciarse el
   * Debe finalizarse el
   * No iniciar antes del
   * No iniciar después del
   * Fecha fija

  Existen los siguientes escenarios:

   * **Cuando la tarea tiene una delimitación Debe comenzar el o No comenzar antes del**: Si la fecha de delimitación de la tarea es anterior y no hay una fecha de comienzo real en la tarea (la tarea aún no ha comenzado), la fecha de transferencia es la fecha más cercana posible en la que se puede comenzar a trabajar en la tarea. Si la tarea se ha iniciado, la fecha de entrega es igual a la fecha de inicio del proyecto.
   * **Cuando la tarea tiene una delimitación de Debe finalizar el o No comenzar después del**: Si la fecha de delimitación de la tarea es futura y no hay una fecha de comienzo real en la tarea (la tarea aún no ha comenzado), la fecha de transferencia es la fecha de comienzo planificada para la tarea. Si la tarea tiene como fecha de inicio real, la fecha de entrega es la fecha de inicio del proyecto.
   * **Cuando la tarea tiene una delimitación de Fechas fijas**: La fecha de transferencia es la fecha planificada de inicio de la tarea, independientemente de si tiene una predecesora o no e independientemente de si la predecesora se ha completado o no.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## Localizar la fecha de entrega

Puede mostrar la fecha de transferencia de una tarea en un informe de tareas o en la vista de una lista de tareas.\
Para obtener más información sobre cómo generar un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
