---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Descripción general de la tarea Duración original y Horario planeado original
description: Como parte de la planificación de un proyecto, debe determinar los valores de las horas planificadas y de la duración (o duración prevista) de cada tarea del proyecto.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 1%

---

# Descripción general de la tarea Duración original y Horario planeado original

Como parte de la planificación de un proyecto, debe determinar los valores de las horas planificadas y de la duración (o duración prevista) de cada tarea del proyecto.

Para obtener más información sobre las horas planificadas en las tareas, consulte [Información general sobre las horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

Para obtener más información sobre la duración de la tarea, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Puede ver estos valores en la pestaña Detalles de la tarea o durante la edición de una tarea.

Si crea una vista para una lista de tareas o un informe de tareas, también puede ver los campos Horario planeado original y Duración original para las tareas.

## Trabajo original planificado

Las horas planificadas originales de una tarea representan el número de horas planificadas que tenía una tarea originalmente antes de convertirse en una tarea principal. Cuando una tarea se convierte en una tarea principal, las horas planificadas de las tareas secundarias se acumulan en la tarea principal para indicar las horas planificadas del elemento principal.

Al mostrar el campo Horario planeado original en un informe o lista de tareas, puede ver el número original de horas planeadas antes de que la tarea heredara el número de horas planeadas de sus hijos.

>[!NOTE]
>
>Cuando crea una tarea, el número de horas planeadas originales es cero. Si la tarea se convierte en una tarea principal, el valor de este campo se rellena con el número de horas planificadas de la tarea antes de cambiarse a una tarea principal. Este valor se mantiene en este campo incluso cuando la tarea vuelve a ser una tarea independiente.

## Duración original

La duración original de una tarea es la duración que tenía una tarea originalmente antes de convertirse en una tarea principal, en minutos. Cuando una tarea pasa a ser una tarea principal, la duración entre la fecha de inicio planeada del elemento secundario más temprano y la fecha de finalización planeada del último elemento secundario se resume en la tarea principal y se convierte en la duración de la tarea principal. Esto reemplaza la Duración de la tarea original.

Al mostrar el campo Duración original en un informe o lista de tareas, puede ver el número original de días para la Duración de la tarea antes de que herede la Duración de sus elementos secundarios.

>[!NOTE]
>
>Cuando crea una tarea, la Duración original es cero. Si la tarea se convierte en una tarea principal, el valor de este campo se rellena con la Duración de la tarea antes de cambiarse a una tarea principal. Este valor se mantiene en este campo incluso cuando la tarea vuelve a ser una tarea independiente. Este valor se muestra en minutos.

## Ejemplo

Por ejemplo, cuando dos tareas son tareas independientes, la duración original y las horas planeadas originales son cero.

![original_scheduled_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

Cuando la primera tarea pasa a ser la principal de la segunda tarea, los campos Duración original y Horario planeado original se rellenan con los valores de Duración y Horario planificado de la tarea antes de convertirse en la tarea principal. La Duración original se muestra en minutos. La duración y las horas previstas del niño se convierten en la duración y las horas previstas del progenitor.

![original_and_scheduled_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

Cuando el elemento principal vuelve a ser una tarea independiente, la duración y las horas planificadas vuelven a los valores originales, mientras que la duración original y las horas planificadas originales siguen rellenadas. No vuelven a cero.

![original_duration_and_scheduled_hours_after_reversal_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
