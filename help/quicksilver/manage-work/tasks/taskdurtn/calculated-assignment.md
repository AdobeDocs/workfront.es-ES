---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Descripción general del tipo de duración: Asignación calculada'''
description: Asignación calculada es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte Información general sobre la duración de la tarea y el tipo de duración.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Información general del tipo de duración: Asignación calculada

Asignación calculada es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Descripción general del tipo de duración de asignación calculada

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* Al utilizar un Tipo de duración de asignación calculada, debe especificar una duración y una cantidad de horas planificadas para la tarea. A continuación, Workfront divide la cantidad de horas planificadas por la cantidad de horas en Duración y, a continuación, por el número de recursos asignados a la tarea para calcular el porcentaje de asignación (calcula la asignación) de cada recurso. Cada recurso tendrá el mismo valor para su porcentaje de asignación. En este caso, no se pueden modificar los valores de asignación de cada recurso.
* El administrador de Workfront o de un grupo puede establecer el tipo de duración predeterminado del sistema o del grupo como Asignación calculada. En este caso, todas las tareas nuevas se crearán con este tipo de duración. Para obtener información sobre cómo cambiar las preferencias de problemas y tareas como parte de las preferencias de proyecto de nivel de sistema o de grupo, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   En este caso, la tarea tiene un valor predeterminado de Duración de un día y un valor predeterminado de 0 horas de horas planificadas. A menos que el administrador de proyectos establezca una Duración más precisa y rellene el campo Horario planificado con una estimación realista, los recursos aparecerán subasignados.

Asignación calculada es el tipo de duración preferido en las siguientes situaciones:

* Cuando las asignaciones tienen una ventana de actividad, pero no toman toda la duración asignada para completar su trabajo. Por ejemplo, se le asigna que envíe un informe a su supervisor antes del final de la semana. Tiene una duración de cinco días, pero sólo le llevará diez horas redactar el documento.
* Cuando se asigna un solo recurso a una tarea porque el administrador del proyecto puede estimar la duración planificada y la cantidad de esfuerzo planeada independientemente de la otra.

   Puede utilizar el Tipo de duración de trabajo calculada para el mismo resultado, pero el administrador de proyectos debe introducir una asignación porcentual para el recurso para afectar al valor calculado para horas planificadas. Esto hace que la planificación de proyectos sea más difícil y lleve más tiempo.

El porcentaje de asignación de cada recurso se calcula de la siguiente manera:

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

Por ejemplo, en el escenario que se describe a continuación, cada tarea tiene una duración de 3 días. El administrador de proyectos introduce manualmente la Duración (3 días o 24 horas) y el Horario planificado y, como resultado, se calcula el porcentaje de asignación (o el porcentaje de asignación):

![](assets/calcassign-350x80.png)

## Cambiar el tipo de duración de una tarea a Asignación calculada

Para obtener información sobre cómo cambiar el tipo de duración de una tarea, consulte [Actualizar el tipo de duración de una tarea](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
