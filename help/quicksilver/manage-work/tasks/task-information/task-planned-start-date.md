---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Descripción general de la tarea Fecha de inicio planificada
description: La Fecha de inicio planeada de una tarea es la fecha en la que, como creador de la tarea, decide que el trabajo de la tarea debe comenzar. Las fechas de las tareas planificadas influyen en las fechas y la cronología del proyecto. Para obtener información sobre la fecha de inicio planeada del proyecto, consulte Información general sobre la fecha de inicio planeada del proyecto.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 2%

---

# Descripción general de la tarea Fecha de inicio planificada

La Fecha de inicio planeada de una tarea es la fecha en la que, como creador de la tarea, decide que el trabajo de la tarea debe comenzar. Las fechas de las tareas planificadas influyen en las fechas y la cronología del proyecto. Para obtener información sobre la fecha de inicio planeada del proyecto, consulte [Descripción general de la fecha de inicio prevista del proyecto](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Fecha de inicio prevista de una tarea

Puede especificar la Fecha de inicio planeada de una tarea o dejarla en manos de Adobe Workfront para calcularla según ciertos criterios. 

* [Establecer manualmente la fecha de inicio prevista de una tarea](#manually-set-the-planned-start-date-of-a-task)
* [Cálculo de la fecha de inicio planeada para una tarea](#how-the-planned-start-date-is-calculated-for-a-task)

### Establecer manualmente la fecha de inicio prevista de una tarea {#manually-set-the-planned-start-date-of-a-task}

La configuración de la Fecha de Inicio Planificado de una tarea depende del tipo de Restricción de Tarea que asigne a la tarea. 

Puede establecer manualmente la fecha de inicio planeada al crear una tarea, tal como se describe en el artículo [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Puede especificar manualmente la Fecha de Inicio Planificado al seleccionar cualquiera de las siguientes Restricciones de Tarea: 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de restricción de tarea</strong> </p> </th> 
   <th> <p><strong>Efecto de cambiar manualmente la fecha de finalización planificada</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Debe iniciarse el</p> <p>No iniciar antes del</p> <p>No iniciar después del</p> </td> 
   <td> <p><span class="s1">La Fecha de Finalización Planificada se ajusta para mantener la Duración igual.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fechas fijas</p> </td> 
   <td> <p>La duración se ajusta para que la fecha de finalización prevista sea la misma.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Cálculo de la fecha de inicio planeada para una tarea {#how-the-planned-start-date-is-calculated-for-a-task}

Cuando el sistema lo calcula automáticamente, lo siguiente puede influir en la fecha de inicio planeada de una tarea:

* La configuración de preferencias Fecha de inicio en el área Tareas y problemas de Configuración

   El administrador de grupos o Workfront puede determinar si una nueva tarea se inicia en la misma fecha que la Fecha de inicio prevista del proyecto o en el día en que se crea la tarea.

   Para obtener información sobre las preferencias de Tareas y problemas, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Restricción de tarea

   Para obtener más información sobre las restricciones de tareas, consulte el artículo [Información general sobre la restricción de tareas](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* Relación predecesora de tareas

   Para obtener más información sobre las predecesoras de tareas, consulte el artículo [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Fecha de inicio del proyecto, cuando el proyecto está programado desde la Fecha de inicio.
* Tiempo fuera de la programación del usuario asignado principal de la tarea.

   Cuando el usuario asignado principal tiene un tiempo de espera programado durante la duración de la tarea, las fechas previstas de la tarea se ajustan en consecuencia cuando la función **Considere el tiempo de espera del usuario en las duraciones de las tareas** está seleccionada para la variable **Tiempo de espera del usuario desactivado** campo . Los nuevos proyectos heredan esta configuración del área Preferencias del proyecto , pero se puede editar la configuración en el nivel del proyecto.

   Por ejemplo, si una tarea con una Restricción de Tan pronto como sea posible está programada para empezar el 1 de junio y finalizarse el 3 de junio, y el usuario asignado principal tiene el 1 de junio marcado como Tiempo de espera, la tarea Fecha de inicio planeada pasa a ser el 2 de junio.

   Para obtener información sobre la variable **Tiempo de espera del usuario desactivado** preferencias, consulte los artículos  [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

Cuando se configura automáticamente, la Fecha de inicio planeada se determina en función del siguiente cálculo: 

```
Planned Start Date = Planned Completion Date - Task Duration
```

Por ejemplo, si la tarea tiene una fecha de finalización del 16 de septiembre y una duración de 10 días, la fecha de inicio planeada es el 6 de septiembre.

>[!NOTE]
>
> El tipo de actualización del proyecto también debe configurarse como &quot;Automático y en Cambio&quot; o &quot;Automáticamente&quot; para que las horas y la duración planificadas se ajusten automáticamente.\
Para obtener más información sobre el tipo de actualización, consulte el artículo [Seleccione el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
