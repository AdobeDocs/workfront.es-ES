---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Diferenciación entre fechas proyectadas y estimadas
description: Existen varios tipos de fechas que muestran la cronología de las tareas entre el momento en que pueden empezar y el momento en que pueden completarse.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# Diferenciación entre fechas proyectadas y estimadas

Existen varios tipos de fechas que muestran la cronología de las tareas entre el momento en que pueden empezar y el momento en que pueden completarse. 

A continuación se indican algunas fechas que muestran la cronología de las tareas:

* Fechas de inicio y finalización planificadas
* Fechas de inicio y finalización previstas
* Fechas de inicio y de vencimiento estimadas
* Fechas reales de inicio y finalización

Este artículo describe las diferencias entre las fechas estimadas y las fechas proyectadas para los proyectos. Cuando se crea la tarea por primera vez, las fechas Planificada, Proyectada y Estimada deberían coincidir. Existen algunas excepciones. 

Para obtener más información sobre el proyecto, la tarea y las fechas de publicación en Adobe Workfront, consulte [Información general sobre las fechas del proyecto, la tarea y el problema en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Resumen de fechas planificadas

Las fechas planificadas son las fechas que define el propietario del proyecto como las fechas de inicio y finalización de las tareas. 

Tanto usted como el Propietario del proyecto pueden modificar manualmente las fechas planificadas de una tarea.

## Resumen de fechas reales

Cuando se crea una tarea por primera vez, no tiene fechas reales, ya que aún no se ha iniciado ni completado.

## Resumen de fechas previstas y estimadas

Durante la vida de un proyecto, las fechas previstas y estimadas se ajustan más a la realidad del proyecto, ya que tienen en cuenta lo que puede influir en el comienzo y final reales de una tarea. Esto hace que cambien con respecto a las fechas previstas.

Tenga en cuenta lo siguiente cuando trabaje con fechas proyectadas y estimadas en tareas:

* No puede modificar manualmente las fechas estimadas ni las fechas proyectadas de las tareas. Adobe Workfront los calcula.
* Cuando crea una tarea, las fechas Proyectadas y Estimadas deben ser idénticas y deben ilustrar los tiempos reales en que las tareas pueden comenzar o finalizar.\
   Ciertas actualizaciones que realice en las tareas afectan directamente a los valores de las fechas proyectadas y estimadas. 

   Por ejemplo, si el usuario inicia o completa una tarea, la tarea muestra las fechas de inicio y finalización reales que influyen en las fechas previstas y estimadas de la tarea. Además, si un usuario asignado de la tarea modifica la Fecha de confirmación, esta fecha influye en la Fecha prevista de la tarea.

## Diferencia entre fechas proyectadas y estimadas

La diferencia entre las fechas proyectadas y las estimadas es:

* Las fechas proyectadas se ven afectadas por un usuario que realiza las siguientes actualizaciones sobre la tarea:

   * Agregar una fecha de restricción añadiendo una restricción de tarea fija
   * Agregar una fecha de confirmación

* Las fechas estimadas solo tienen en cuenta el progreso real de una tarea en un momento determinado.

**Ejemplo:** Si tenemos una tarea que tiene una Fecha de Inicio Planificada del 20 de Septiembre y una Fecha de Finalización Planificada del 24 de Septiembre, y tiene la Fecha de Restricción Debe Terminar el 24 de Septiembre, la Fecha de Finalización Prevista. Esta tarea tiene una duración de 4 días.

La fecha de finalización estimada se calcula en función del progreso actual del trabajo en la tarea. Por lo tanto, si hoy es 23 de septiembre y la tarea aún no ha comenzado, la Fecha estimada de finalización es el 27 de septiembre (debería completarse después de 4 días, suponiendo que el trabajo se inicie hoy).

Si la tarea se completa al 50 % hoy, la Fecha de finalización estimada es el 25 de septiembre (debe completarse después de 2 días, que es la mitad de la duración de la tarea).

* [Comprender cuándo se actualizan las fechas proyectadas en las tareas](#understand-when-projected-dates-update-on-tasks)
* [Comprender cuándo se actualizan las fechas estimadas en las tareas](#understand-when-the-estimated-dates-update-on-tasks)

### Comprender cuándo se actualizan las fechas proyectadas en las tareas {#understand-when-projected-dates-update-on-tasks}

Las fechas proyectadas pueden coincidir con otras fechas de tareas o son un cálculo realizado por Workfront que tiene en cuenta el progreso de la tarea en la vida real.

La siguiente lista muestra varios escenarios en los que las fechas previstas de las tareas se cambian durante la vida de un proyecto según lo que suceda en la vida real de la tarea:

* Cuando una tarea está marcada como Completa:

   *Fechas proyectadas = Fechas estimadas = Fechas reales*

* Cuando una tarea tiene una fecha de inicio real:

   *Fecha de inicio prevista = Fecha de inicio estimada = Fecha de inicio real*

* Cuando una tarea no tiene una fecha de inicio real, pero hay una restricción forzada en la fecha de inicio planeada (debe comenzar el) que está en el futuro:

   *Fecha de inicio prevista = Fecha de restricción*

   Para obtener información sobre la fecha de restricción, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Cuando una tarea no tiene una fecha de inicio real y la tarea no tiene una fecha de restricción forzada:

   *Fecha de inicio prevista = la siguiente fecha disponible en el futuro que se ajuste a la programación de trabajo*

* Cuando el usuario asignado actualiza la fecha de confirmación:

   *Fecha de finalización prevista = Fecha de confirmación*

   Para obtener información sobre la fecha de confirmación, consulte [Resumen de la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Cuando la tarea no tiene una fecha de confirmación actualizada y la tarea tiene una restricción forzada (debe finalizar el) para la fecha de finalización prevista que está en el futuro:

   *Fecha de finalización prevista = Fecha de restricción*

* Cuando una tarea no tiene una fecha de confirmación actualizada, una fecha de restricción forzada en el futuro o tiene una fecha de restricción en el pasado:

   *Fecha de Finalización Prevista = cálculo del sistema para la Fecha de Finalización basado en el progreso actual y el trabajo pendiente*

### Comprender cuándo se actualizan las fechas estimadas en las tareas {#understand-when-the-estimated-dates-update-on-tasks}

En comparación con los escenarios descritos anteriormente para las Fechas proyectadas, las Fechas estimadas siempre reflejan el análisis real de Workfront sobre cuándo se iniciará o completará la tarea, independientemente de las Fechas de restricción o de confirmación.

## Qué influye en la cronología de una tarea

A continuación se muestran algunos ejemplos de lo que puede influir en la cronología real de una tarea: 

* progreso de la tarea en relación con las fechas planificadas y el día actual
* porcentaje completado de la tarea hasta ahora
* relación predecesora
* progreso del predecesor
* asignación de usuarios

   >[!NOTE]
   >
   >La asignación de usuarios puede influir en la Fecha de finalización estimada de una tarea si afecta a la velocidad con la que se puede completar la tarea. Por ejemplo, si el tipo de duración de la tarea está impulsado por el esfuerzo, puede hacer que la tarea se complete antes de lo previsto añadiendo asignadores. Como resultado, cambia la Fecha de finalización estimada.
