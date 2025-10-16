---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Información general de tipo de duración: asignación calculada'
description: La asignación calculada es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte Información general sobre la duración de la tarea y el tipo de duración.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 89%

---

# Información general del tipo de duración: Asignación calculada

<!-- Audited: 5/2025 -->

La asignación calculada es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general acerca de los tipos de duración en Workfront, consulte [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Descripción general del tipo de duración de asignación calculada

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* Cuando utilice un tipo de duración de asignación calculada, debe especificar tanto una duración como un número de horas planificadas para la tarea. A continuación, Workfront divide la cantidad de horas planificadas por la cantidad de horas de duración y, a continuación, por el número de recursos asignados a la tarea para calcular el porcentaje de asignación (calcula la asignación) de cada recurso. Cada recurso tendrá igualmente el mismo valor para su porcentaje de asignación. En este caso, no puede modificar los valores de asignación para cada recurso.
* Su Workfront o un administrador de grupo pueden establecer el tipo de duración predeterminado de su sistema o grupo como asignación calculada.En este caso, todas las tareas nuevas se crearán con este tipo de duración. Para obtener información sobre cómo cambiar las preferencias de tareas y problemas como parte de las preferencias de proyectos de nivel de sistema o de grupo, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  En este caso, la tarea tiene una Duración predeterminada de un día y un valor predeterminado de 0 horas de Horas planificadas. A menos que el gestor del proyecto establezca una duración más precisa y rellene el campo de horas planificadas con una estimación realista, los recursos parecerán infrautilizados.

Asignación calculada es el tipo de duración preferido en las siguientes situaciones:

* Cuando las asignaciones tienen una ventana de actividad pero no tardan toda la duración asignada en completar su trabajo. Por ejemplo, se le asigna la tarea de enviar un informe a su supervisor antes del final de la semana. Tiene una duración de cinco días, pero solo le llevará 10 horas redactar el borrador del documento.
* Cuando se asigna un único recurso a una tarea, el gestor del proyecto puede estimar la duración planificada y la cantidad de esfuerzo planificado de manera independiente entre sí.

  Puedes usar el tipo de duración de trabajo calculada para obtener el mismo resultado, pero el gestor del proyecto debe introducir un porcentaje de asignación para el recurso con el fin de afectar el valor calculado de las horas planificadas. Esto hace que la planificación de proyectos sea más difícil y lleve más tiempo.

El porcentaje de asignación de cada recurso se calcula de la siguiente manera:

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

Por ejemplo, en el escenario que se describe a continuación, cada tarea tiene una Duración de 3 días. El gestor del proyecto introduce manualmente tanto la Duración (3 días o 24 horas) como las Horas Planificadas, y como resultado, se calcula el porcentaje de asignación (o porcentaje de tarea asignada):

![](assets/calcassign-350x80.png)

## Cambiar el tipo de duración de una tarea a Asignación calculada

Para obtener información acerca de cómo cambiar el tipo de duración de una tarea, consulte [Actualizar el tipo de duración de una tarea](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
