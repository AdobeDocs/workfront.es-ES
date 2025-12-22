---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Información general sobre la duración y el tipo de duración de la tarea
description: La duración de la tarea es la diferencia entre la fecha de finalización planificada y la fecha de inicio planificada de la tarea. La duración indica el lapso de tiempo disponible para que se complete la tarea.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1653'
ht-degree: 65%

---

# Información general sobre la duración y el tipo de duración de la tarea

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

La duración de la tarea es la diferencia entre la fecha de finalización planificada y la fecha de inicio planificada de la tarea. La duración indica el lapso de tiempo disponible para que se complete la tarea.

El tipo de duración de una tarea identifica la relación entre el número de recursos asignados a una tarea, el esfuerzo total y la duración total de la tarea.

## Información general sobre la duración de la tarea

Si las fechas de inicio y finalización reales de la tarea quedan fuera de la programación del proyecto, del usuario asignado principal o del horario predeterminado, la duración de la tarea es cero.

>[!BEGINSHADEBOX]

**EJEMPLO**
Si tiene una programación que comienza a las 9:00 AM y finaliza a las 12:00 PM y una tarea que está programada para comenzar a las 2:00 PM y finalizar a las 4:00 PM, la duración de la tarea es cero.


>[!ENDSHADEBOX]

A continuación se indican dos escenarios que existen al calcular la duración en Adobe Workfront:

* Si la tarea está asignada a un usuario:

   1. Workfront tiene en cuenta la programación del proyecto o la del usuario asignado a la tarea.

      El administrador de Workfront o del grupo determina qué programación utiliza Workfront cuando se asigna una tarea a un usuario. Para obtener más información, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Si el usuario o el proyecto no tienen una programación, Workfront utiliza la programación predeterminada del sistema.

      Los pasos son similares al primer escenario después de comprender qué programación utiliza Workfront para calcular la duración.

* Si la tarea está asignada a varios usuarios:

   1. Workfront tiene en cuenta la programación del proyecto o la del usuario asignado principal.

      El administrador de Workfront o del grupo determina qué programación utiliza Workfront cuando una tarea se asigna a varios usuarios. Para obtener más información, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Si el usuario principal asignado o el proyecto no tienen una programación, Workfront utiliza la programación predeterminada del sistema.

  Los pasos son similares al primer escenario después de comprender qué programación utiliza Workfront para calcular la duración.

>[!NOTE]
>
>Al tener en cuenta el tiempo libre de la persona asignada principal en un proyecto, las fechas planificadas de la tarea podrían ajustarse, pero la duración de la tarea sigue siendo la misma. Para obtener información sobre cómo tener en cuenta los días libres del usuario asignado principal al planificar un proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Unidades de tiempo para la duración de la tarea

Puede indicar la duración de la tarea tanto en el tiempo normal como en el tiempo transcurrido entre las fechas planificadas de inicio y finalización.

Al actualizar la duración de las tareas de una lista, puede utilizar las siguientes abreviaturas para indicar las unidades de tiempo en Workfront:

| Unidad de tiempo | Abreviatura |
|---|---|
| minutos | L |
| Horas | H |
| Días.Es la opción predeterminada. | D |
| Semanas | S |
| Meses | T, MO |
| Minutos transcurridos | MT |
| Horas transcurridas | HT |
| Días transcurridos | DT |
| Semanas transcurridas | ST |
| Meses transcurridos | ET |

{style="table-layout:auto"}

>[!BEGINSHADEBOX]

**EJEMPLO**

Si desea indicar que la duración de una tarea es de 3 días transcurridos, debe escribir &quot;3 ED&quot; en el campo Duración en una lista de tareas  También puede seleccionar la opción preferida para la Unidad de tiempo de duración en el menú desplegable disponible al editar una tarea o en la sección Detalles de la tarea. Para obtener información sobre la edición de tareas, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).


>[!ENDSHADEBOX]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Tenga en cuenta lo siguiente al indicar la duración de una tarea:

* El tiempo transcurrido es una unidad de tiempo de la duración de una tarea. Es el tiempo entre la fecha de inicio planificada y la fecha de finalización planificada de una tarea que incluye días festivos, fines de semana y días libres. En otras palabras, el tiempo transcurrido es el paso de los días del calendario.
* Los días representan los días laborables definidos en el sistema y se pueden configurar en el área de Configuración. En la mayoría de los casos, un día consta de 8 horas.
* El tiempo normal (días o días laborables) tiene en cuenta los días festivos, los fines de semana y los días libres, y los excluye de la duración de la tarea.
* Cuando se indica la duración de una tarea en semanas, Workfront calcula la duración en días y horas basándose en la configuración de Días laborables habituales por semana y Horas habituales por día laborable establecida por el administrador de Workfront en el área Preferencias de proyecto de Configuración.
* Workfront utiliza la duración predeterminada de 4 semanas para un mes al calcular la duración en meses.

## Información general sobre el tipo de duración de una tarea

Al administrar el tipo de duración de una tarea, puede establecer asignaciones de recursos coherentes en función de las necesidades de la tarea.

El tipo de duración ayuda a responder a las siguientes preguntas:

* ¿Hasta qué punto vamos a estar ocupados?
* ¿Qué envergadura tiene el trabajo?
* ¿Cuánto tiempo va a tardar?

![duration_type_triangle.png](assets/duration_type_triangle.png)

## Definir tipos de duración

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>Tipo de duración</strong></p></th> 
   <th scope="col"> <p><strong>Función</strong> </p> </th> 
   <th scope="col"> <p><strong>Cómo afectan los recursos</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Asignación calculada</strong> </p> </th> 
   <td scope="col"> <p>Calcula el porcentaje de asignación de cada persona asignada en una tarea. </p> <p>Cuando elige este tipo de duración, puede introducir la duración individual y las horas planificadas de la tarea. Workfront divide las horas planificadas por el número de horas dentro de la duración de la tarea y, a continuación, por el número de recursos asignados a la tarea para calcular la asignación de cada persona asignada.</p> <p>Para obtener información más detallada, consulte <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Información general sobre el tipo de duración: asignación calculada</a>.</p> </td> 
   <td scope="col">La duración y las horas planificadas no cambian cuando se añaden o eliminan personas asignadas a la tarea. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Trabajo calculado</strong> </p> </th> 
   <td scope="col"> <p>Determina las horas planificadas (cantidad de esfuerzo) necesarias para completar la tarea.</p> <p>Normalmente se utiliza cuando los recursos asignados a la tarea se asignan para toda la duración de la tarea.</p> <p>Al elegir este tipo de duración, tiene la posibilidad de introducir una duración individual para la tarea. Workfront calcula las horas planificadas de la tarea multiplicando el número de días de la duración por el número de horas de trabajo de la programación y por el número de personas asignadas a la tarea. </p> <p>Tiene la posibilidad de cambiar manualmente el porcentaje de asignación de cada persona asignada a la tarea, lo que acortará la cantidad de horas planificadas.</p> <p>Para obtener información más detallada, consulte <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Información general sobre el tipo de duración: trabajo calculado</a>.</p> </td> 
   <td scope="col"> <p>Las horas planificadas aumentan cuando se añaden personas asignadas a la tarea. </p> <p>Las horas planificadas disminuyen cuando las personas asignadas se eliminan de la tarea.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Condicionada por el esfuerzo</strong></p> </th> 
   <td scope="col"> <p>Determina las horas planificadas en función del número de recursos.</p> <p>Al elegir este tipo de duración, tiene la posibilidad de introducir una duración individual para la tarea. Workfront calcula las horas planificadas de la tarea multiplicando el número de días de la duración por el número de horas de trabajo de la programación y dividiendo ese número por el número de personas asignadas a la tarea. </p> <p>Tiene la posibilidad de cambiar manualmente el porcentaje de asignación de cada persona asignada a la tarea, pero el número de horas planificadas permanece igual.</p> <p>Para obtener información más detallada, consulte <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Información general sobre el tipo de duración: condicionada por el esfuerzo</a>.</p> </td> 
   <td scope="col"> <p>Las horas planificadas aumentan cuando las personas asignadas se eliminan de la tarea.</p> <p>Las horas planificadas disminuyen cuando se añaden personas asignadas a la tarea. </p> <p>La duración no cambia, independientemente de los cambios en el número de personas asignadas o su programación. </p> <p>La duración es igual a las horas planificadas. La duración planificada es igual a las horas planificadas divididas por el número de personas asignadas.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Simple</strong> </p> </th> 
   <td scope="col"> <p>Determina las horas planificadas y la duración (que son las mismas para este tipo de duración) en función del número de horas que se asignan a cada persona asignada. </p> <p>Workfront calcula las horas planificadas sumando las horas asignadas planificadas para cada persona asignada. </p> <p>Tiene la posibilidad de cambiar manualmente la cantidad de horas que se asignan a cada persona, y el número de horas planificadas, y la cantidad de la duración cambian en consecuencia. Si elige una cantidad total de horas asignadas para todos los usuarios asignados, ese número se divide a partes iguales entre cada usuario asignado.</p> <p>Para obtener información más detallada, consulte <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Información general del tipo de duración: Simple</a>.</p> </td> 
   <td scope="col"> <p>Las horas se distribuyen equitativamente entre las personas asignadas si elige una cantidad total de horas asignadas. Sin embargo, como jefe de proyecto, puede ajustar manualmente las horas de cada usuario asignado. </p> <p>Puede editar las horas planificadas y la duración de una tarea con un tipo de duración simple en línea o en el nivel de tarea. </p> <p>Si se asigna un equipo Agile a una tarea, el tipo de duración se establece automáticamente como Simple y no se puede cambiar. La duración de la tarea para un equipo Agile debe ser mayor que 0 minutos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## El tipo de duración de las nuevas tareas

El tipo de duración de una nueva tarea coincide con el tipo de duración configurado en el sistema. El tipo de duración predeterminado es Asignación calculada. El administrador de Workfront o de un grupo puede actualizar el tipo de duración predeterminado para el sistema o para el grupo asociado con el proyecto. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## La duración original de una tarea principal

La Duración original de una tarea es la Duración que una tarea tuvo originalmente antes de convertirse en una tarea principal, en minutos.

Cuando una tarea se convierte en principal, la Duración entre la Fecha planificada de inicio del primer elemento secundario y la Fecha planificada de finalización del último elemento secundario se acumula en la tarea principal y se convierte en la Duración de la tarea principal. Esto reemplaza la duración de la tarea original.

Cuando los elementos secundarios utilizan la unidad de duración de días transcurridos y su elemento principal utiliza la unidad de duración de días, puede haber discrepancias en la forma en que Workfront calcula la duración de la tarea principal.

Tenga en cuenta lo siguiente:

* La unidad de duración Días transcurridos representa días del calendario, que siempre consta de 24 horas al día.
* La unidad de duración Días representa el día laborable definido en el sistema y es configurable. En la mayoría de los casos, consta de 8 horas por día.
* La fórmula para calcular la duración de la tarea principal es la siguiente:

  `Parent task duration = Planned Completion Date of the child task that is planned to end the latest - Planned Start Date of the child task that starts the earliest`

* Al calcular la duración de la tarea principal, el sistema calcula primero la duración mediante la fórmula anterior y, a continuación, aplica la programación.


Para obtener más información, vea [Descripción general de la duración original de la tarea y Horas planificadas originales](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md).

## Cambiar el tipo de duración de una tarea

Para obtener información acerca de cómo cambiar el tipo de duración de una tarea, consulte [Actualizar el tipo de duración de una tarea](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
