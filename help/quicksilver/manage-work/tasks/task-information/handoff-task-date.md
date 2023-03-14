---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre la fecha de entrega de tareas
description: La fecha de entrega es la fecha en la que una tarea está disponible para el trabajo. Esto suele significar que sus predecesores se han resuelto y que el usuario asignado de la tarea puede empezar a trabajar en ella.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 3%

---

# Información general sobre la fecha de entrega de tareas

La fecha de entrega es la fecha en la que una tarea está disponible para el trabajo. Esto suele significar que sus predecesores se han resuelto y que el usuario asignado de la tarea puede empezar a trabajar en ella.

>[!TIP]
>
>Las fechas de entrega no existen para problemas y proyectos.

## Cómo calcula Adobe Workfront la fecha de entrega

>[!NOTE]
>
>La fecha de entrega solo se calcula si el estado del proyecto es igual a los siguientes estados:
>
>* En espera
>* Al día
>* Finalizadas
>* Inactivo
>


Workfront utiliza las siguientes reglas para calcular la fecha de entrega de una tarea:

* **Cuando la tarea tiene un predecesor incompleto**: La fecha de entrega de la tarea es nula.
* **Cuando la tarea tiene un predecesor completo**: La fecha de entrega es la misma que la fecha de finalización real de la tarea predecesora. Si el predecesor tiene un retraso, Workfront calcula la fecha de entrega de la tarea sucesora mediante la fórmula siguiente:

   `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

   Para obtener información sobre el tiempo de retraso, consulte [Descripción general de los tipos de retraso](../use-prdcssrs/lag-types.md).

   Si la tarea sucesora tiene más de un predecesor, la fecha de entrega se calcula en función de la última fecha de finalización real de los predecesores. Por ejemplo, si las fechas de finalización reales de los dos predecesores son el 8 de noviembre de 2022 y el 20 de noviembre de 2022, la fecha de entrega del sucesor es el 20 de noviembre de 2022.

   >[!NOTE]
   >
   >   El cálculo de la fecha de entrega de una tarea sucesora en función de la fecha de finalización real o de una tarea predecesora es el mismo tanto si la predecesora se aplica como si no. Para obtener más información sobre las predecesoras reforzadas, consulte [Aplicar predecesores](../use-prdcssrs/enforced-predecessors.md).


* **Cuando la tarea no tiene predecesor y**:

   * **La fecha de inicio planeada es anterior**: La fecha de entrega es la misma que la fecha de inicio planeada del proyecto.
   * **La fecha de inicio planeada es futura (cualquier fecha posterior a la fecha actual)**: La fecha de entrega es la misma que la fecha de inicio planeada del proyecto.

>[!NOTE]
>
>Cuando la tarea tiene un predecesor entre proyectos, la fecha de entrega del sucesor se vuelve a calcular solo cuando se produce cualquiera de las siguientes situaciones:
>
>* Se vuelve a calcular manualmente la cronología del proyecto del sucesor. Debe tener permisos de administración para volver a calcular la cronología del proyecto.
>* La cronología del proyecto del sucesor se vuelve a calcular automáticamente por la noche.
>
>Para obtener información sobre cómo volver a calcular la cronología del proyecto, consulte [Volver a calcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Cuando la tarea tiene una restricción forzada para las fechas planificadas**: La fecha de entrega varía según el tipo de restricción y si la tarea tiene o no una fecha de inicio real.\
   Las siguientes son restricciones forzadas en tareas:

   * Debe iniciarse el
   * Debe finalizarse el
   * No iniciar antes del
   * No iniciar después del
   * Fecha fija

   Existen los siguientes escenarios:

   * Cuando la tarea tiene una restricción de Debe comenzar el o No empezar antes de, la Fecha de entrega es la fecha de restricción, a menos que haya una Fecha de inicio real en la tarea. Si hay una Fecha de Inicio Real en la tarea, la Fecha de Entrega es la Fecha de Finalización Real del predecesor.
   * Cuando la tarea tiene una restricción de Must Finish On o Start No Later Than, la Fecha de entrega es siempre la Fecha de finalización real del predecesor, independientemente de si existe o no una Fecha de inicio real en la tarea.
   * Cuando la tarea tiene una restricción de Fechas fijas, la Fecha de entrega es la Fecha de inicio planificada de la tarea, independientemente de si tiene un predecesor o no y de si el predecesor se ha completado o no.


## Localización de la fecha de entrega

Puede mostrar la fecha de entrega de una tarea en un informe de tareas o la vista de una lista de tareas.\
Para obtener más información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
