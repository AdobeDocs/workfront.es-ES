---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre la fecha planificada de finalización de la tarea
description: La fecha planificada de finalización de una tarea es la fecha en la que está previsto que finalice.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 73%

---

# Información general sobre la fecha planificada de finalización de la tarea

La fecha planificada de finalización de una tarea es la fecha en la que está previsto que finalice.

Puede especificar la fecha planificada de finalización de una tarea o dejar que Adobe Workfront la calcule en función de determinados criterios.

Las Fechas planificadas de finalización de las tareas de un proyecto determinan la Fecha planificada de finalización de un proyecto cuando el proyecto se programa a partir de la Fecha de inicio. Para obtener más información sobre la fecha planificada de finalización del proyecto, consulte [Establecer la fecha planificada de finalización del proyecto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La fecha planificada de finalización de una tarea difiere de la fecha de confirmación de la tarea o de la fecha proyectada de finalización de la tarea de las siguientes maneras:
>
>* La fecha de confirmación es la fecha en la que la persona asignada a la tarea calcula manualmente que habrá completado la tarea. Para obtener más información, consulte los siguientes artículos:
>
>   * [Información general sobre la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interacciones entre la fecha de confirmación y la fecha planificada de finalización](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* La fecha proyectada de finalización es una fecha calculada por Workfront que tiene en cuenta los retrasos de las tareas, las líneas de tiempo de la tarea o de sus predecesoras y otros factores para determinar una fecha real en la que se pueda completar la tarea de forma realista. Para obtener más información, consulte [Información general sobre la fecha proyectada de finalización para proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## No se puede cambiar establecer la fecha planificada de finalización de una tarea

Debe tener acceso de edición a tareas y permisos de administración sobre la tarea para poder actualizar la fecha planificada de finalización de la misma.

La configuración de la fecha planificada de finalización de una tarea depende del tipo de restricción de tarea que asigne a la tarea.

Puede establecer manualmente la fecha planificada de finalización en las siguientes áreas de Workfront:

* En el cuadro Editar tarea, al crear o editar una tarea. Para obtener más información, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* En el área Detalles de la tarea. Para obtener más información, consulte [Administrar información de tarea en el área Información general de detalles de la tarea](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* En el área de Inicio, si se muestra la Fecha planificada de finalización al ver una tarea en el panel Resumen. Para obtener más información, consulte [Actualizar o editar un elemento de trabajo en el área de inicio](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* El encabezado de la tarea. Para obtener más información, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* En una lista de tareas o un informe cuando el campo Fecha planificada de finalización se muestra en la vista.

  Para obtener más información, consulte [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Puede especificar manualmente la Fecha planificada de finalización al seleccionar cualquiera de las siguientes restricciones de tarea:

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
   <td> <p>Debe finalizarse el</p> <p>No terminar después de</p> <p>No terminar antes de</p> </td> 
   <td> <p><span class="s1">La fecha de inicio planificada se ha ajustado para mantener la duración igual.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fechas fijas</p> </td> 
   <td> <p>La duración se ha ajustado para mantener la misma fecha de inicio planificada.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cómo Workfront calcula automáticamente la fecha planificada de finalización de una tarea

Cuando el sistema la calcula automáticamente, lo siguiente puede influir en la Fecha planificada de finalización de una tarea:

* Restricción de tarea

  Para obtener más información sobre las restricciones de tarea, consulte el artículo [Información general sobre la restricción de tarea](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relación de predecesoras de tareas

  Para obtener más información acerca de las predecesoras de tareas, consulte el artículo [Descripción general sobre las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Fecha de finalización del proyecto, cuando el proyecto está programado desde la fecha de finalización.
* El tiempo libre programado de la persona asignada principal de la tarea.

  Cuando el principal asignado tiene tiempo libre programado durante la duración de la tarea, las fechas planificadas de la tarea se ajustan en consecuencia cuando se selecciona la configuración **Tenga en cuenta el tiempo libre del usuario en las duraciones de la tarea** para el campo **Tiempo libre del usuario**. Los nuevos proyectos heredan esta configuración del área de Preferencias del proyecto, pero puede editarla en el nivel de proyecto.

  Por ejemplo, si una tarea con una delimitación de Lo antes posible está programada para empezar el 1 de junio y finalizar el 3 de junio, y el principal asignado tiene marcado el 2 de junio como tiempo libre, la fecha planificada de finalización de la tarea pasará a ser el 4 de junio.

  Para obtener información acerca de la preferencia **Tiempo libre del usuario**, consulte los artículos [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

* Cantidad de tiempo asociada con la Configuración de aprobación si la tarea está asociada con una aprobación. Para obtener más información, consulte [Configuración de la aprobación global](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Cuando se establece automáticamente, la fecha planificada de finalización se determina según el siguiente cálculo:

```
Planned Completion Date = Planned Start Date + Duration
```

Por ejemplo, si la tarea tiene una fecha de inicio del 16 de septiembre y una duración de 10 días, la fecha planificada de finalización es el 26 de septiembre.

>[!NOTE]
>
> El tipo de actualización del proyecto debe establecerse en Automática y Al cambiar o Automáticamente para que las horas planificadas y la duración se ajusten automáticamente.\
>Para obtener más información acerca del tipo de actualización, consulte el artículo [Seleccionar el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
