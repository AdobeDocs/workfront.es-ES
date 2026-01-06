---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre la fecha planificada de inicio de la tarea
description: La fecha de inicio planificada de una tarea es la fecha en la que usted, como creador de la tarea, decide que debe empezar el trabajo sobre la tarea. Las fechas de las tareas planificadas influyen en las fechas y en la cronología del proyecto. Para obtener información sobre la fecha de inicio planificada del proyecto, consulte Información general sobre la fecha de inicio planificada del proyecto.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 43%

---

# Información general sobre la fecha de inicio planificada de la tarea

<!-- Audited: 6/2025 -->

La fecha de inicio planificada de una tarea es la fecha en la que usted, como creador de la tarea, decide que debe empezar el trabajo sobre la tarea. Las fechas de las tareas planificadas influyen en las fechas y en la cronología del proyecto. Para obtener información sobre la fecha de inicio planificada del proyecto, consulte [Información general sobre la fecha de inicio planificada del proyecto](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Fecha de inicio planificada de una tarea

Puede especificar la fecha planificada de inicio de la tarea o dejar que Adobe Workfront la calcule en función de determinados criterios.

* [Establecer manualmente la fecha de inicio planificada de una tarea](#manually-set-the-planned-start-date-of-a-task)
* [Cómo se calcula la fecha de inicio planificada de una tarea](#how-the-planned-start-date-is-calculated-for-a-task)

### Establecer manualmente la fecha de inicio planificada de una tarea {#manually-set-the-planned-start-date-of-a-task}

La configuración de la fecha planificada de inicio de una tarea depende del tipo de restricción de tarea que asigne a la tarea.

Puede establecer manualmente la Fecha planificada de inicio al crear una tarea. Para obtener más información, vea [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Puede especificar manualmente la Fecha planificada de inicio al seleccionar cualquiera de las siguientes restricciones de tarea:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de restricción de tarea</strong> </p> </th> 
   <th> <p><strong>Efecto de cambiar manualmente la fecha planificada de finalización</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Debe iniciarse el</p> <p>No iniciar antes del</p> <p>No iniciar después del</p> </td> 
   <td> <p><span class="s1">La fecha planificada de finalización se ha ajustado para mantener la duración igual.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fechas fijas</p> </td> 
   <td> <p>La duración se ajusta para mantener la misma fecha planificada de finalización.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Cómo se calcula la fecha de inicio planificada de una tarea {#how-the-planned-start-date-is-calculated-for-a-task}

Cuando el sistema la calcula automáticamente, lo siguiente puede influir en la fecha de inicio planificada de una tarea:

* La configuración de la preferencia Fecha de inicio en el área Tareas y problemas de la Configuración

  El administrador del grupo o de Workfront puede determinar si una nueva tarea se inicia en la misma fecha que la fecha planificada de inicio del proyecto o en el día en que se crea la tarea.

  Para obtener información acerca de las preferencias de tareas y problemas, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Restricción de tarea

  Para obtener más información acerca de las restricciones de tarea, vea [Información general sobre las restricciones de tarea](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relación de predecesoras de tareas

  Para obtener más información acerca de las tareas predecesoras, vea [Información general sobre las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Fecha de inicio del proyecto, cuando el proyecto está programado a partir de la fecha de inicio.
* El tiempo libre programado de la persona principal asignada a la tarea.

  Cuando el usuario asignado principal tiene tiempo libre programado durante la duración de la tarea, las fechas planificadas de la tarea se ajustan en consecuencia cuando la configuración Considerar el tiempo libre del usuario en las duraciones de la tarea se selecciona para el campo Tiempo libre del usuario. Los nuevos proyectos heredan esta configuración del área de Preferencias del proyecto, pero puede editarla en el nivel de proyecto.

  Por ejemplo, si una tarea con una delimitación de Lo antes posible está programada para empezar el 1 de junio y finalizar el 3 de junio, y el usuario principal asignado tiene el 1 de junio marcado como tiempo libre, la fecha planificada de inicio de la tarea pasará a ser el 2 de junio.

  Para obtener información acerca de la preferencia Tiempo libre del usuario, vea [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

Cuando se establece automáticamente, la fecha planificada de inicio se determina según el siguiente cálculo:

```
Planned Start Date = Planned Completion Date - Task Duration
```

Por ejemplo, si la tarea tiene una fecha de finalización del 16 de septiembre y una duración de 10 días, la fecha de inicio planificada es el 6 de septiembre.

>[!NOTE]
>
> El tipo de actualización del proyecto también debe establecerse en Automática y Al cambiar o Automáticamente para que las horas planificadas y la duración se ajusten automáticamente.\
>Para obtener más información sobre el tipo de actualización, vea [Seleccionar el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
