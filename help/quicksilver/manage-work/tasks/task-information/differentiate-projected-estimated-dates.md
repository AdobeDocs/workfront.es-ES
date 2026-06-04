---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general de las fechas proyectadas y estimadas
description: Existen varios tipos de fechas que muestran la cronología de las tareas entre el momento en que pueden comenzar y el momento en que pueden finalizar.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
TQID: https://experienceleague.adobe.com/H-lO-an4TrEuwNx-l76JFpACJfyM22g36F3pa3aP6EY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 925
ht-degree: 100%

---

# Información general de las fechas proyectadas y estimadas

<!--Audited: 07/2024-->

Existen varios tipos de fechas que muestran la cronología de las tareas entre el momento en que pueden comenzar y el momento en que pueden finalizar. A continuación se muestran algunas fechas que muestran la cronología de las tareas:

* Fechas de inicio planificado y finalización planificada
* Fechas proyectadas de inicio y finalización
* Fechas estimadas de inicio y de vencimiento
* Fechas reales de inicio y finalización

Este artículo describe las diferencias entre las fechas estimadas y proyectadas para los proyectos.

Cuando se crea la tarea por primera vez, las fechas planificadas, proyectadas y estimadas suelen coincidir. Existen algunas excepciones.

Para obtener más información sobre el proyecto, las tareas y las fechas de los problemas en Adobe Workfront, consulte [Información general sobre las fechas de los proyectos, las tareas y los problemas en Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Información general de las fechas planificadas

Las fechas planificadas son las fechas que el propietario del proyecto define como fechas de inicio y finalización de las tareas. Usted o el propietario del proyecto pueden modificar manualmente las fechas planificadas de una tarea.

## Información general de las fechas reales

Cuando se crea una tarea por primera vez, no tiene fechas reales porque aún no se ha iniciado ni completado.

## Información general de las fechas proyectadas y estimadas

Durante la duración de un proyecto, las fechas proyectadas y estimadas se acercan más a la realidad del proyecto, ya que tienen en cuenta lo que puede influir en el inicio y el final reales de una tarea. Esto hace que cambien con respecto a las fechas planificadas.

Tenga en cuenta lo siguiente cuando trabaje con fechas proyectadas y estimadas en tareas:

* No puede modificar manualmente las fechas estimadas o proyectadas de las tareas. Adobe Workfront calcula ambas opciones.
* Al crear una tarea, las fechas proyectadas y estimadas deben ser idénticas y deben ilustrar las horas reales en que las tareas pueden comenzar o finalizar.\
  Ciertas actualizaciones que se aplican a las tareas afectan directamente a los valores de las fechas proyectadas y estimadas.

  Por ejemplo, si el usuario inicia o completa una tarea, la tarea muestra las fechas de inicio y finalización reales que influyen en las fechas proyectadas y estimadas de la tarea. Además, si un usuario asignado a la tarea modifica la fecha de compromiso, esta fecha influye en la fecha proyectada de la tarea.

## Diferencia entre fechas proyectadas y estimadas

La diferencia entre las fechas proyectadas y estimadas es:

* Las fechas proyectadas se ven afectadas cuando un usuario realiza las siguientes actualizaciones en la tarea:

   * Añadir una fecha de restricción añadiendo una restricción de tarea fija
   * Añadir una fecha de compromiso

* Las fechas estimadas solo tienen en cuenta el progreso real de una tarea en un momento determinado.

**Ejemplo:** si tenemos una tarea con una fecha de inicio planificada del 20 de septiembre y una fecha de finalización planificada del 24 de septiembre y debe finalizar con la restricción, la fecha proyectada de finalización del 24 de septiembre. Esta tarea tiene una duración de 4 días.

La fecha estimada de finalización se calcula según el progreso actual del trabajo en la tarea. Por lo tanto, si hoy es 23 de septiembre y la tarea aún no ha comenzado, la fecha estimada de finalización es el 27 de septiembre (debe completarse al cabo de 4 días, suponiendo que el trabajo se inicie hoy).

Si la tarea se completa hoy al 50 %, la fecha estimada de finalización es el 25 de septiembre (debe completarse al cabo de 2 días, lo que equivale a la mitad de la duración de la tarea).


### Comprender cuándo se actualizan las fechas proyectadas en las tareas {#understand-when-projected-dates-update-on-tasks}

Las fechas proyectadas pueden coincidir con otras fechas de la tarea o son un cálculo realizado por Workfront que tiene en cuenta el progreso en tiempo real de la tarea.

La siguiente lista muestra varios escenarios en los que las fechas proyectadas de las tareas se cambian durante la duración de un proyecto dependiendo de lo que le ocurra a la tarea en la vida real:

* Cuando una tarea se marca como Completa:

  `Projected Dates = Estimated Dates = Actual Dates`

* Cuando una tarea tiene una fecha de inicio real:

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* Cuando una tarea no tiene una fecha de inicio real, pero existe una restricción forzada en la fecha de inicio planificada (debe comenzar el) futura:

  `Projected Start Date = Constraint Date`

  Para obtener información acerca de la fecha de restricción, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Cuando una tarea no tiene una fecha de inicio real y la tarea no tiene una fecha de restricción forzada:

  `Projected Start Date = the next available date in the future that falls within working schedule`

* Cuando el usuario asignado actualiza la fecha de confirmación:

  `Projected Completion Date = Commit Date`

  Para obtener información sobre la fecha de confirmación, consulte [Información general de la fecha de compromiso](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Cuando la tarea no tiene una fecha de compromiso actualizada y la tarea tiene una restricción forzada (debe finalizar el) para la fecha planificada de finalización futura:

  `Projected Completion Date = Constraint Date`

* Cuando una tarea no tiene una fecha de compromiso actualizada, una fecha de restricción forzada en el futuro o tiene una fecha de restricción en el pasado:

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### Comprenda cuándo se actualizan las fechas estimadas en las tareas {#understand-when-the-estimated-dates-update-on-tasks}

En comparación con los escenarios descritos anteriormente para las fechas proyectadas, las fechas estimadas siempre reflejan el análisis real de Workfront de cuándo comenzará o finalizará la tarea, independientemente de las fechas de restricción o de compromiso.

## Qué influye en la cronología de una tarea

A continuación se muestran algunos ejemplos de lo que puede influir en la cronología real de una tarea:

* Progreso de la tarea en relación a las fechas planificadas y al día actual
* Porcentaje completado de la tarea hasta el momento
* Relación de predecesoras
* Progreso de predecesora
* Asignación de usuarios

  >[!NOTE]
  >
  >La asignación de usuarios puede influir en la fecha estimada de finalización de una tarea si afecta a la velocidad con la que se puede finalizar la tarea. Por ejemplo, si el tipo de duración de la tarea es condicionada por el esfuerzo, puede finalizar la tarea antes añadiendo usuarios asignados. Como resultado, cambia la fecha estimada de finalización.
