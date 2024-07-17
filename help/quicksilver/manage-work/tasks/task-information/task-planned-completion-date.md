---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre la fecha planificada de finalización de la tarea
description: La fecha planificada de finalización de una tarea es la fecha en la que la tarea está configurada para completarse.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 1%

---

# Información general sobre la fecha planificada de finalización de la tarea

La fecha planificada de finalización de una tarea es la fecha en la que la tarea está configurada para completarse.

Puede especificar la fecha planificada de finalización de una tarea o dejar que Adobe Workfront la calcule en función de determinados criterios. 

Las Fechas planificadas de finalización de las tareas de un proyecto determinan la Fecha planificada de finalización de un proyecto cuando el proyecto se programa a partir de la Fecha de inicio. Para obtener más información sobre la fecha planificada de finalización del proyecto, consulte [Establecer la fecha planificada de finalización del proyecto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La fecha planificada de finalización de una tarea difiere de la fecha de compromiso de la tarea o de la fecha proyectada de finalización de la tarea de las siguientes maneras:
>
>* La fecha de confirmación es la fecha en la que la persona asignada a la tarea calcula manualmente que habrá completado la tarea. Para obtener más información, consulte los siguientes artículos:
>
>   * [Resumen de fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interacciones entre la fecha de confirmación y la fecha planificada de finalización](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* La fecha proyectada de finalización es una fecha calculada por Workfront que tiene en cuenta los retrasos de las tareas, los plazos de la tarea o de sus predecesoras y otros factores para determinar una fecha real en la que se pueda completar la tarea de forma realista. Para obtener más información, vea [Información general sobre la fecha proyectada de finalización de proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Establecer manualmente la fecha planificada de finalización de una tarea

Debe tener acceso de edición a Tareas y permisos de administración en la tarea para poder actualizar la Fecha planificada de finalización de la tarea.

La configuración de la fecha planificada de finalización de una tarea depende del tipo de restricción de tarea que asigne a la tarea. 

Puede establecer manualmente la fecha planificada de finalización en las siguientes áreas de Workfront:

* En el cuadro Editar tarea, al crear o editar una tarea. Para obtener más información, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* En el área Detalles de la tarea. Para obtener más información, vea [Administrar información de tareas en el área Información general de detalles de tareas](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* En el área de Inicio, si se muestra la Fecha planificada de finalización al ver una tarea. Para obtener más información, vea [Actualizar o editar un elemento de trabajo en el área de inicio](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* En el encabezado de la tarea. Para obtener más información, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* En una lista de tareas o un informe cuando el campo Fecha planificada de finalización se muestra en la vista.

  Para obtener más información, vea [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

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
   <td> <p><span class="s1">La fecha planificada de inicio se ha ajustado para mantener la duración igual.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fechas fijas</p> </td> 
   <td> <p>La duración se ajusta para mantener la misma fecha planificada de inicio.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cómo Workfront calcula automáticamente la fecha planificada de finalización de una tarea

Cuando el sistema la calcula automáticamente, lo siguiente puede influir en la Fecha planificada de finalización de una tarea:

* Restricción de tarea

  Para obtener más información acerca de las restricciones de tarea, vea el artículo [Introducción a las restricciones de tarea](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relación de predecesoras de tareas

  Para obtener más información acerca de las tareas predecesoras, vea el artículo [Descripción general de las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Fecha de finalización del proyecto, cuando el proyecto está programado desde la fecha de finalización.
* El tiempo libre programado de la persona asignada principal de la tarea.

  Cuando el usuario asignado principal tiene tiempo libre programado durante la duración de la tarea, las fechas planificadas de la tarea se ajustan en consecuencia cuando se selecciona la configuración **Considerar el tiempo libre del usuario en las duraciones de la tarea** para el campo **Tiempo libre del usuario**. Los nuevos proyectos heredan esta configuración del área de Preferencias del proyecto, pero puede editarla en el nivel de proyecto.

  Por ejemplo, si una tarea con una delimitación de Lo antes posible está programada para comenzar el 1 de junio y finalizar el 3 de junio, y la persona asignada principal tiene marcado el 2 de junio como tiempo libre, la fecha planificada de finalización de la tarea pasará a ser el 4 de junio.

  Para obtener información acerca de la preferencia **Tiempo libre del usuario**, vea los artículos [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

* Cantidad de tiempo asociada con la Configuración de aprobación si la tarea está asociada con una aprobación. Para obtener más información, vea [Configurar la aprobación global](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Cuando se establece automáticamente, la fecha planificada de finalización se determina según el siguiente cálculo: 

```
Planned Completion Date = Planned Start Date + Duration
```

Por ejemplo, si la tarea tiene una fecha de inicio del 16 de septiembre y una duración de 10 días, la fecha planificada de finalización es el 26 de septiembre.

>[!NOTE]
>
> El tipo de actualización del proyecto debe establecerse en Automática y Al cambiar o Automáticamente para que las horas planificadas y la duración se ajusten automáticamente.\
>Para obtener más información acerca del tipo de actualización, vea el artículo [Seleccionar el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
