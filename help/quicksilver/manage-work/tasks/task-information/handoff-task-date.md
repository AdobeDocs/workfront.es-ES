---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Resumen de fecha de transferencia de tareas
description: La fecha de transferencia es la fecha en la que una tarea está disponible para trabajar. Esto suele significar que sus predecesoras se han resuelto y que el usuario asignado de la tarea puede empezar a trabajar en ella.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 709b36f4471e5576e45ed918783216a1f7f4abac
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 3%

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

* **Cuando la tarea tiene un predecesor incompleto**: la fecha de entrega de la tarea es nula.
* **Cuando la tarea tiene una predecesora completa**: la fecha de transferencia es la misma que la fecha de finalización real de la tarea predecesora. Si la tarea predecesora tiene un retardo, Workfront calcula la fecha de transferencia de la tarea sucesora mediante la siguiente fórmula:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Para obtener información sobre el tiempo de retardo, consulte [Información general sobre los tipos de retardo](../use-prdcssrs/lag-types.md).

  Si la tarea sucesora tiene más de una predecesora, la fecha de transferencia se calcula según la última fecha real de finalización de las predecesoras. Por ejemplo, si las fechas de finalización reales de las dos predecesoras son el 8 de noviembre de 2022 y el 20 de noviembre de 2022, la fecha de transferencia de la sucesora es el 20 de noviembre de 2022.

  >[!NOTE]
  >
  >   El cálculo de la fecha de transferencia de una tarea sucesora en función de la fecha real de finalización o de una tarea predecesora es el mismo independientemente de si la predecesora es obligatoria o no. Para obtener más información sobre predecesoras forzadas, consulte [Forzar predecesoras](../use-prdcssrs/enforced-predecessors.md).


* **Cuando la tarea no tiene predecesora y**:

   * **La fecha planificada de inicio se encuentra en el pasado**: la fecha de entrega es la misma que la fecha planificada de inicio del proyecto.
   * **La fecha planificada de inicio es futura (cualquier fecha posterior a la fecha actual)**: la fecha de entrega es la misma que la fecha de inicio planificada de la tarea.

>[!NOTE]
>
>Cuando la tarea tiene una predecesora entre proyectos, la fecha de transferencia de la sucesora se vuelve a calcular únicamente cuando se produce una de las siguientes situaciones:
>
>* Se puede recalcular manualmente la escala de tiempo del proyecto del sucesor. Debe tener permisos de administración en el proyecto para volver a calcular la escala de tiempo.
>* La cronología del proyecto del sucesor se recalcula automáticamente por la noche.
>
>Para obtener información sobre cómo recalcular la escala de tiempo del proyecto, consulte [Recalcular escalas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Cuando la tarea tiene una restricción forzada para las fechas planificadas**: la fecha de transferencia varía según el tipo de restricción y si la tarea tiene una fecha de inicio real o no.\
  A continuación se indican restricciones forzadas en tareas:

   * Debe iniciarse el
   * Debe finalizarse el
   * No iniciar antes del
   * No iniciar después del
   * Fecha fija

  Existen los siguientes escenarios:

   * Cuando la tarea tiene una delimitación Debe comenzar el o No comenzar antes del, la fecha de transferencia es la fecha de delimitación, a menos que haya una fecha de inicio real en la tarea. Si hay una fecha de inicio real en la tarea, la fecha de transferencia es la fecha de finalización real de la predecesora.
   * Cuando la tarea tiene una delimitación de Debe finalizar el o No comenzar después del, la fecha de transferencia es siempre la fecha de finalización real de la predecesora, independientemente de si hay o no una fecha de inicio real en la tarea.
   * Cuando la tarea tiene una delimitación de Fechas fijas, la fecha de transferencia es la fecha planificada de inicio de la tarea, independientemente de si tiene una predecesora o no e independientemente de si la predecesora se ha completado o no.

## Localizar la fecha de entrega

Puede mostrar la fecha de transferencia de una tarea en un informe de tareas o en la vista de una lista de tareas.\
Para obtener más información sobre la creación de informes, consulte [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
