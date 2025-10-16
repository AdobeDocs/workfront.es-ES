---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre la duración original de la tarea y las horas planificadas originales
description: Como parte de la planificación de un proyecto, debe determinar los valores de las horas planificadas y de la duración (o duración planificada) de cada tarea del proyecto.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 1%

---

# Información general sobre la duración original de la tarea y las horas planificadas originales

Como parte de la planificación de un proyecto, debe determinar los valores de las horas planificadas y de la duración (o duración planificada) de cada tarea del proyecto.

Para obtener más información sobre las horas planificadas en las tareas, consulte [Resumen de horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

Para obtener más información acerca de la duración de la tarea, vea [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Puede ver estos valores en la pestaña Detalles de la tarea o mientras edita una tarea.

Si genera una vista para una lista de tareas o un informe de tareas, también puede ver los campos Horas planificadas originales y Duración original de las tareas.

## Horas planificadas originales

Las horas planificadas originales de una tarea representan el número de horas planificadas que una tarea tenía originalmente antes de convertirse en una tarea principal. Cuando una tarea se convierte en una tarea principal, las horas planificadas de las tareas secundarias se acumulan en la tarea principal para indicar las horas planificadas de la tarea principal.

Al mostrar el campo Horas planificadas originales en un informe de tareas o una lista, puede ver el número original de horas planificadas antes de que la tarea herede el número de horas planificadas de sus tareas secundarias.

>[!NOTE]
>
>Al crear una tarea, el número de horas planificadas originales es cero. Si la tarea se convierte en una tarea principal, el valor de este campo se rellena con el número de horas planificadas de la tarea antes de que se cambie a una tarea principal. Este valor permanece en este campo incluso cuando la tarea vuelve a ser una tarea independiente.

## Duración original

La Duración original de una tarea es la Duración que una tarea tuvo originalmente antes de convertirse en una tarea principal, en minutos. Cuando una tarea se convierte en principal, la Duración entre la Fecha planificada de inicio del primer elemento secundario y la Fecha planificada de finalización del último elemento secundario se acumula en la tarea principal y se convierte en la Duración de la tarea principal. Esto reemplaza la duración de la tarea original.

Al mostrar el campo Duración original en un informe o lista de tareas, puede ver el número original de días de la Duración de la tarea antes de que herede la Duración de sus tareas secundarias.

>[!NOTE]
>
>Cuando crea una tarea, la Duración original es cero. Si la tarea se convierte en una tarea principal, el valor de este campo se rellena con la Duración de la tarea antes de que se cambie a una tarea principal. Este valor permanece en este campo incluso cuando la tarea vuelve a ser una tarea independiente. Este valor se muestra en minutos.

## Ejemplo

Por ejemplo, cuando dos tareas son tareas independientes, su Duración original y Horas planificadas originales son cero.

![original_planned_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

Cuando la primera tarea se convierte en la principal de la segunda tarea, los campos Duración original y Horas planificadas originales se rellenan con los valores de Duración y Horas planificadas de la tarea antes de que se convierta en principal. La duración original se muestra en minutos. La duración y las horas planificadas del hijo se convierten en la duración y las horas planificadas del padre.

![original_and_planned_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

Cuando el principal vuelve a ser una tarea independiente, las horas planificadas y de duración vuelven a los valores originales, mientras que las horas planificadas originales y de duración original permanecen rellenadas. No vuelven a cero.

![duración_original_y_horas_planificadas_después_de_la_reversión_de_un_padre.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
