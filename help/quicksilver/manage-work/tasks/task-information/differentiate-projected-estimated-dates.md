---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Diferenciar entre fechas proyectadas y estimadas
description: Existen varios tipos de fechas que muestran la cronología de las tareas entre el momento en que pueden comenzar y el momento en que pueden finalizar.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 0%

---

# Diferenciar entre fechas proyectadas y estimadas

Existen varios tipos de fechas que muestran la cronología de las tareas entre el momento en que pueden comenzar y el momento en que pueden finalizar. A continuación se muestran algunas fechas que muestran la cronología de las tareas:

* Fechas planificadas de inicio y finalización planificada
* Fechas proyectadas de inicio y finalización
* Fechas estimadas de inicio y de vencimiento
* Fechas reales de inicio y finalización

Este artículo describe las diferencias entre las fechas estimadas y proyectadas para los proyectos.

Cuando se crea la tarea por primera vez, las fechas planificadas, proyectadas y estimadas suelen coincidir. Existen algunas excepciones. 

Para obtener más información sobre el proyecto, las tareas y las fechas de los problemas en Adobe Workfront, consulte [Información general sobre las fechas de los proyectos, las tareas y los problemas en Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Resumen de las fechas planificadas

Las Fechas planificadas son las fechas que el propietario del proyecto define como las fechas de inicio y finalización de las tareas. Usted o el propietario del proyecto pueden modificar manualmente las fechas planificadas de una tarea.

## Resumen de las fechas reales

Cuando se crea una tarea por primera vez, no tiene fechas reales porque aún no se ha iniciado ni completado.

## Resumen de las fechas proyectadas y estimadas

Durante la duración de un proyecto, las fechas proyectadas y estimadas están más en línea con la realidad del proyecto, ya que tienen en cuenta lo que puede influir en el inicio y el final reales de una tarea. Esto hace que cambien de las Fechas planificadas.

Tenga en cuenta lo siguiente cuando trabaje con fechas proyectadas y estimadas en tareas:

* No puede modificar manualmente las fechas estimadas o proyectadas de las tareas. Adobe Workfront calcula ambas opciones.
* Al crear una tarea, las fechas proyectadas y estimadas deben ser idénticas y deben ilustrar las horas reales en que las tareas pueden comenzar o finalizar.\
  Ciertas actualizaciones que realiza en las tareas afectan directamente a los valores de las Fechas proyectadas y estimadas. 

  Por ejemplo, si el usuario inicia o completa una tarea, la tarea muestra las fechas de inicio y finalización reales que influyen en las fechas proyectadas y estimadas de la tarea. Además, si un usuario asignado a la tarea modifica la fecha de compromiso, esta fecha influye en la fecha proyectada de la tarea.

## Diferencia entre fechas proyectadas y estimadas

La diferencia entre las fechas proyectadas y estimadas es:

* Las fechas proyectadas se ven afectadas por el hecho de que un usuario realice las siguientes actualizaciones en la tarea:

   * Agregar una fecha de restricción agregando una restricción de tarea fija
   * Añadir una fecha de confirmación

* Las fechas estimadas solo tienen en cuenta el progreso real de una tarea en un momento determinado.

**Ejemplo:** Si tenemos una tarea que tiene una Fecha planificada de inicio del 20 de septiembre y una Fecha planificada de finalización del 24 de septiembre y debe finalizar con la restricción, la Fecha proyectada de finalización del 24 de septiembre. Esta tarea tiene una duración de 4 días.

La Fecha estimada de finalización se calcula según el progreso actual del trabajo en la tarea. Por lo tanto, si hoy es 23 de septiembre y la tarea aún no ha comenzado, la fecha estimada de finalización es el 27 de septiembre (debe completarse después de 4 días, suponiendo que el trabajo se inicie hoy).

Si la tarea se completa hoy al 50 %, la fecha estimada de finalización es el 25 de septiembre (debe completarse después de 2 días, lo que equivale a la mitad de la duración de la tarea).


### Comprender cuándo se actualizan las fechas proyectadas en las tareas {#understand-when-projected-dates-update-on-tasks}

Las Fechas proyectadas pueden coincidir con otras fechas de la tarea o son un cálculo realizado por Workfront que tiene en cuenta el progreso en tiempo real de la tarea.

La siguiente lista muestra varios escenarios en los que las Fechas proyectadas de las tareas se cambian durante la duración de un proyecto dependiendo de lo que suceda en la vida real a la tarea:

* Cuando una tarea se marca como Completada:

  *Fechas proyectadas = Fechas estimadas = Fechas reales*

* Cuando una tarea tiene una fecha de inicio real:

  *Fecha proyectada de inicio = Fecha estimada de inicio = Fecha real de inicio*

* Cuando una tarea no tiene una fecha de inicio real, pero existe una restricción forzada en la fecha de inicio planificada (debe comenzar el) que es futura:

  *Fecha proyectada de inicio = Fecha de restricción*

  Para obtener información acerca de la fecha de restricción, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Cuando una tarea no tiene una fecha de inicio real y la tarea no tiene una fecha de delimitación forzada:

  *Fecha proyectada de inicio = la próxima fecha disponible en el futuro que se encuentre dentro del horario de trabajo*

* Cuando el usuario asignado actualice la fecha de confirmación:

  *Fecha proyectada de finalización = Fecha de confirmación*

  Para obtener información sobre la fecha de confirmación, consulte [Resumen de la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Cuando la tarea no tiene una fecha de confirmación actualizada y la tarea tiene una delimitación forzada (Debe finalizar el) para la fecha planificada de finalización futura:

  *Fecha proyectada de finalización = Fecha de restricción*

* Cuando una tarea no tiene una fecha de compromiso actualizada, una fecha de restricción forzada en el futuro o tiene una fecha de restricción en el pasado:

  *Fecha proyectada de finalización = cálculo del sistema para la fecha de finalización basado en el progreso actual y el trabajo que queda por hacer*

### Comprenda cuándo se actualizan las fechas estimadas en las tareas {#understand-when-the-estimated-dates-update-on-tasks}

En comparación con los escenarios descritos anteriormente para las Fechas Proyectadas, las Fechas Estimadas siempre reflejan el análisis real de Workfront de cuándo comenzará o finalizará la tarea, independientemente de las Fechas de Restricción o de Confirmación.

## Qué influye en la cronología de una tarea

A continuación se muestran algunos ejemplos de lo que puede influir en la cronología real de una tarea: 

* Progreso de la tarea en relación con las fechas planificadas y el día actual
* Porcentaje completado de la tarea hasta el momento
* Relación de predecesoras
* Progreso de predecesora
* Asignación de usuarios

  >[!NOTE]
  >
  >La asignación de usuarios puede influir en la Fecha estimada de finalización de una tarea si afecta a la velocidad con la que se puede finalizar la tarea. Por ejemplo, si el tipo de duración de la tarea es Condicionada por el esfuerzo, puede finalizar la tarea antes agregando usuarios asignados. Como resultado, cambia la Fecha estimada de finalización.
