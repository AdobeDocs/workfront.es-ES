---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Descripción general de la tarea Fecha de finalización planificada
description: La Fecha de Finalización Planificada de una tarea es la fecha en la que la tarea está configurada para completarse.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# Descripción general de la tarea Fecha de finalización planificada

La Fecha de Finalización Planificada de una tarea es la fecha en la que la tarea está configurada para completarse.

Puede especificar la Fecha de Finalización Planificada de una tarea o puede dejarla en manos de Adobe Workfront para calcularla según ciertos criterios. 

Las fechas de finalización previstas de las tareas de un proyecto determinan la fecha de finalización prevista de un proyecto cuando el proyecto está programado desde la fecha de inicio. Para obtener más información sobre la fecha de finalización prevista del proyecto, consulte [Establecer la fecha de finalización prevista del proyecto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La Fecha de Finalización Planificada de una tarea difiere de la Fecha de Finalización de la tarea o de la Fecha de Finalización Prevista de la tarea de las siguientes maneras:
>
>* La Fecha de confirmación es la fecha en la que la persona asignada a la tarea calcula manualmente que habrá completado la tarea. Para obtener más información, consulte los siguientes artículos:
   * [Resumen de la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [Interacciones entre la fecha de confirmación y la fecha de finalización prevista](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* La fecha de finalización prevista es una fecha calculada por Workfront y tiene en cuenta los retrasos de las tareas, las líneas de tiempo de la tarea o sus predecesores y otros factores para determinar una fecha de vida real para la fecha en la que la tarea se puede completar de forma realista. Para obtener más información, consulte [Información general sobre la fecha de finalización prevista para proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## Establecer manualmente la fecha de finalización planeada de una tarea

Debe tener acceso de edición a Tareas y permisos de administración en la tarea para poder actualizar la fecha de finalización planeada de la tarea.

La configuración de la Fecha de Finalización Planificada de una tarea depende del tipo de Restricción de Tarea que asigne a la tarea. 

Puede establecer manualmente la fecha de finalización planeada en las siguientes áreas de Workfront:

* En el cuadro Editar tarea, al crear o editar una tarea. Para obtener más información, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* En el área Detalles de la tarea . Para obtener más información, consulte [Administrar información de tarea en el área Información general de detalles de tarea](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* En el área de inicio si aparece la Fecha de finalización planeada al ver una tarea. Para obtener más información, consulte [Actualizar o editar un elemento de trabajo en el área principal](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* En el encabezado de la tarea. Para obtener más información, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* En una lista de tareas o informe, cuando se muestra en la vista el campo Fecha de finalización planeada .

   Para obtener más información, consulte [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Puede especificar manualmente la Fecha de Finalización Planificada cuando seleccione cualquiera de las siguientes Restricciones de Tarea: 

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
   <td> <p>Debe finalizarse el</p> <p>No terminar después de</p> <p>No terminar antes de</p> </td> 
   <td> <p><span class="s1">La Fecha de Inicio Planificado se ajusta para mantener la Duración igual.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Fechas fijas</p> </td> 
   <td> <p>La duración se ajusta para mantener la fecha de inicio planeada igual.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cómo calcula Workfront automáticamente la fecha de finalización prevista para una tarea

Cuando el sistema lo calcula automáticamente, lo siguiente puede influir en la fecha de finalización planeada de una tarea:

* Restricción de tarea

   Para obtener más información sobre las restricciones de tareas, consulte el artículo [Información general sobre la restricción de tareas](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relación predecesora de tareas

   Para obtener más información sobre las predecesoras de tareas, consulte el artículo [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Fecha de Finalización del Proyecto, cuando el proyecto está programado desde la Fecha de Finalización.
* Tiempo fuera de la programación del usuario asignado principal de la tarea.

   Cuando el usuario asignado principal tiene un tiempo de espera programado durante la duración de la tarea, las fechas previstas de la tarea se ajustan en consecuencia cuando la función **Considere el tiempo de espera del usuario en las duraciones de las tareas** está seleccionada para la variable **Tiempo de espera del usuario desactivado** campo . Los nuevos proyectos heredan esta configuración del área Preferencias del proyecto , pero se puede editar la configuración en el nivel del proyecto.

   Por ejemplo, si una tarea con una Restricción de Tan pronto como sea posible está programada para empezar el 1 de junio y finalizarse el 3 de junio, y el usuario asignado principal tiene el 2 de junio marcado como Tiempo de espera, la tarea Fecha de finalización planeada pasa a ser el 4 de junio.

   Para obtener información sobre la variable **Tiempo de espera del usuario desactivado** preferencias, consulte los artículos [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

* Cantidad de tiempo asociado con la Configuración de aprobación si la tarea está asociada con una aprobación. Para obtener más información, consulte [Configuración de la aprobación global](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Cuando se configura automáticamente, la fecha de finalización planeada se determina según el siguiente cálculo: 

```
Planned Completion Date = Planned Start Date + Duration
```

Por ejemplo, si la tarea tiene una fecha de inicio del 16 de septiembre y una duración de 10 días, la fecha de finalización planeada es el 26 de septiembre.

>[!NOTE]
 El tipo de actualización del proyecto debe establecerse en Automático y En Cambio o Automáticamente para que las horas y la duración planeadas se ajusten automáticamente.\
Para obtener más información sobre el tipo de actualización, consulte el artículo [Seleccione el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
