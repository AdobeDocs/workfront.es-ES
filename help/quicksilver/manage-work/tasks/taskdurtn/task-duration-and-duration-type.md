---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Información general sobre la duración y el tipo de duración de la tarea
description: Duración de la tarea es la diferencia entre la Fecha de Finalización Planificada y la Fecha de Inicio Planificada de la tarea. La duración indica el lapso de tiempo disponible para que se complete la tarea.
author: Alina
feature: Work Management
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 2%

---

# Información general sobre la duración y el tipo de duración de la tarea

Duración de la tarea es la diferencia entre la Fecha de Finalización Planificada y la Fecha de Inicio Planificada de la tarea. La duración indica el lapso de tiempo disponible para que se complete la tarea.

El tipo de duración de una tarea identifica la relación entre el número de recursos asignados a una tarea, el esfuerzo total y la duración total de la tarea.

## Información general sobre la duración de la tarea

>[!NOTE]
>
>Si se tiene en cuenta el tiempo de espera del Asignado principal en un proyecto, las fechas previstas de la tarea podrían ajustarse, pero la duración de la tarea sigue siendo la misma. Para obtener información sobre cómo tener en cuenta el tiempo de espera del usuario asignado principal al planificar un proyecto, consulte  [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Si las fechas de inicio y finalización reales de la tarea están fuera de la programación del proyecto, del usuario asignado principal o de la programación predeterminada, la duración de la tarea es cero.

**Ejemplo:** Si tiene una programación que comienza a las 9:00 a.m. y termina a las 23:00 y una tarea que está programada para empezar a las 2:00 p.m. y termina a las 4:00 p.m., la Duración de la tarea es cero.

Los siguientes son dos escenarios que existen al calcular la duración en Adobe Workfront.

* Si la tarea está asignada a un usuario Workfront utiliza una de las siguientes programaciones, en este orden exacto para calcular la Duración:

   1. Workfront tiene en cuenta la programación del usuario.
   1. Si el usuario no está asociado a una programación, Workfront tiene en cuenta la programación del proyecto.
   1. Si el proyecto no está asociado a una programación, Workfront tiene en cuenta la programación predeterminada del sistema. Para obtener información sobre las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Si la tarea está asignada a varios usuarios:

   Workfront tiene en cuenta la programación del proyecto o la del usuario asignado principal.

   El administrador de Workfront determina la programación que utiliza Workfront cuando se asigna una tarea a varios usuarios. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Los pasos son similares al primer escenario después de saber qué programación utiliza Workfront para calcular la duración.

## Unidades de tiempo para la duración de la tarea

Puede indicar la duración de la tarea tanto en el tiempo normal como en el tiempo transcurrido entre las fechas de inicio planeado y finalización planeada.

Al actualizar la duración de las tareas en una lista, puede utilizar las siguientes abreviaciones para indicar las unidades de tiempo en Workfront:

| Unidad de tiempo | Abreviación |
|---|---|
| minutos | L |
| Horas | H |
| Días. Este es el valor predeterminado. | D |
| Semanas | M |
| Meses | M |
| Minutos transcurridos | EM |
| Horas transcurridas | EH |
| Días transcurridos | ED |
| Semanas transcurridas | EW |
| Meses transcurridos | ET |

{style="table-layout:auto"}

**Ejemplo:** Si desea indicar que la duración de una tarea es de 3 días transcurridos, escriba &quot;3 ED&quot; en el campo Duración de una lista de tareas .  También puede seleccionar la opción preferida para la unidad de tiempo de duración en el menú desplegable disponible al editar una tarea o en la sección Detalles de la tarea . Para obtener información sobre la edición de tareas, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Tenga en cuenta lo siguiente al indicar la Duración de una tarea:

* El tiempo transcurrido es una unidad de tiempo para la duración de una tarea. Es la hora entre la Fecha de Inicio Planificado y la Fecha de Finalización Planificada de una tarea que incluye festivos, fines de semana y tiempo libre. En otras palabras, el tiempo transcurrido es el paso de días naturales.
* El tiempo regular tiene en cuenta los festivos, los fines de semana y el tiempo libre, y los excluye de la Duración de la tarea.

* Cuando se indica la duración de una tarea en semanas, Workfront calcula la duración en días y horas en función de los días de trabajo típicos por semana y las horas por día de trabajo típicas establecidas por el administrador de Workfront en el área Preferencias del proyecto de configuración.
* Workfront utiliza la duración predeterminada de 4 semanas para un mes al calcular la duración en meses.

## Información general sobre el tipo de duración de la tarea

La administración del tipo de duración de una tarea permite establecer asignaciones de recursos coherentes en función de las necesidades de la tarea.

El tipo de duración ayuda a responder a las siguientes preguntas:

* ¿Qué tan ocupados vamos a estar?
* ¿Qué tan grande es el trabajo?
* ¿Cuánto tiempo va a tardar?

![duration_type_triangle.png](assets/duration-type-triangle-350x245.png)

## Definir tipos de duración

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row">Tipo de duración </th> 
   <th scope="col"> <p><strong>Función</strong> </p> </th> 
   <th scope="col"> <p><strong>Cómo afectan los recursos</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Asignación calculada</strong> </p> </th> 
   <td scope="col"> <p>Calcula el porcentaje de asignación para cada usuario asignado en una tarea. </p> <p>Al elegir este Tipo de duración, puede introducir la duración y las horas planificadas individuales para la tarea. Workfront divide las horas planificadas por el número de horas dentro de la duración de la tarea y, a continuación, por el número de recursos asignados a la tarea para calcular la asignación de cada usuario asignado.</p> <p>Para obtener información más detallada, consulte <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Información general del tipo de duración: Asignación calculada</a>.</p> </td> 
   <td scope="col">La duración y las horas planificadas no cambian al agregar o eliminar asignadores a la tarea. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Trabajo calculado</strong> </p> </th> 
   <td scope="col"> <p>Determina las horas planificadas (cantidad de esfuerzo) necesarias para completar la tarea.</p> <p>Normalmente se utiliza cuando los recursos asignados a la tarea se asignan a toda la duración de la tarea.</p> <p>Al elegir este Tipo de duración, tiene la capacidad de introducir una duración individual para la tarea. Workfront calcula las horas previstas para la tarea multiplicando el número de días de la duración por el número de horas de trabajo de la programación y por el número de personas asignadas a la tarea. </p> <p>Tiene la capacidad de cambiar manualmente el porcentaje de asignación de cada usuario asignado a la tarea, lo que acortará la cantidad de horas planificadas.</p> <p>Para obtener información más detallada, consulte <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Información general del tipo de duración: Trabajo calculado</a>.</p> </td> 
   <td scope="col"> <p>Las horas planificadas aumentan cuando se añaden asignadores a la tarea. </p> <p>Las horas planificadas disminuyen cuando se eliminan de la tarea los usuarios asignados.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p>Condicionada por el esfuerzo</p> </th> 
   <td scope="col"> <p>Determina el horario planificado en función del número de recursos.</p> <p>Al elegir este Tipo de duración, tiene la capacidad de introducir una duración individual para la tarea. Workfront calcula las horas planificadas para la tarea multiplicando el número de días de la duración por el número de horas de trabajo de la programación y dividiendo ese número por el número de personas asignadas a la tarea. </p> <p>Tiene la capacidad de cambiar manualmente el porcentaje de asignación de cada usuario asignado a la tarea, pero el número de horas planificadas sigue siendo el mismo.</p> <p>Para obtener información más detallada, consulte <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Información general del tipo de duración: Impulsado por el esfuerzo</a>.</p> </td> 
   <td scope="col"> <p>Las horas planificadas aumentan cuando se eliminan los usuarios asignados de la tarea.</p> <p>Las horas planificadas disminuyen cuando se añaden asignadores a la tarea. </p> <p>La duración no cambia, independientemente de los cambios en el número de personas asignadas o en su programación. </p> <p>La duración es igual a horas planificadas. La duración planeada es igual a las horas planificadas divididas por el número de personas asignadas.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Sencilla</strong> </p> </th> 
   <td scope="col"> <p>Determina las horas planificadas y la duración (que son las mismas, para este tipo de duración) en función del número de horas para las que se asigna cada usuario asignado. </p> <p>Workfront calcula las horas planificadas añadiendo las horas asignadas planificadas para cada usuario asignado. </p> <p>Tiene la capacidad de cambiar manualmente la cantidad de horas asignadas a cada usuario asignado, y el número de horas planificadas y la cantidad de la duración cambian en consecuencia. Si elige un número total de horas asignadas para todos los usuarios asignados, ese número se divide equitativamente entre cada usuario asignado.</p> <p>Para obtener información más detallada, consulte <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Información general del tipo de duración: Sencilla</a>.</p> </td> 
   <td scope="col"> <p>Las horas se distribuyen de manera uniforme entre los usuarios asignados si se elige un número total de horas asignadas. Sin embargo, como administrador de proyectos, puede ajustar manualmente las horas de cada usuario asignado. </p> <p>Puede editar horas planificadas y duración de una tarea con un tipo de duración simple en línea o en el nivel de tarea. </p> <p>Si se asigna un equipo ágil a una tarea, el tipo de duración se establece automáticamente como Simple y no se puede cambiar. La duración de la tarea para un equipo ágil debe ser buena a 0 minutos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## El tipo de duración de las nuevas tareas

El tipo de duración de una nueva tarea coincide con el tipo de duración configurado en el sistema. El tipo de duración predeterminado es Asignación calculada. El administrador de Workfront o un administrador de grupo pueden actualizar el tipo de duración predeterminado para su sistema o para el grupo asociado al proyecto. Para obtener más información, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Cambiar el tipo de duración de una tarea

Para obtener información sobre cómo cambiar el tipo de duración de una tarea, consulte [Actualizar el tipo de duración de una tarea](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
