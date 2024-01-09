---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Resumen del estado de progreso de tareas
description: Adobe Workfront determina el estado de progreso de una tarea mirando la progresión de la tarea en su cronología. Puede configurar Workfront para determinar la condición de un proyecto en función del valor de estado de progreso de las tareas. Para obtener más información sobre la configuración de la condición del proyecto, consulte el artículo Información general sobre la condición del proyecto y el tipo de condición.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 70d173ca3781d8d143a66ce7e963dcaf66bece19
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Resumen del estado de progreso de tareas

<!-- Audited: 1/2024 -->

Adobe Workfront determina el estado de progreso de una tarea mirando la progresión de la tarea en su cronología. Puede configurar Workfront para determinar la condición de un proyecto en función del valor de estado de progreso de las tareas. Para obtener más información sobre la configuración de la condición del proyecto, consulte el artículo [Descripción general de la condición y el tipo de condición del proyecto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Criterios que determinan el estado de progreso de las tareas

Para obtener información sobre el estado de progreso de un proyecto, consulte [Resumen del estado del progreso del proyecto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Para obtener información sobre el seguimiento del progreso de las tareas, consulte [Información general del modo de seguimiento de tareas](../../../manage-work/tasks/task-information/task-tracking-mode.md).

Los siguientes criterios determinan el estado de progreso de una tarea:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Estado de progreso</strong> </p> </th> 
   <th> <p><strong>Criterios determinantes</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>Tiempo de activación</strong> </p> </td> 
   <td scope="col"> <p>Se considera una tarea <strong>Tiempo de activación</strong> cuando todas las fechas planificadas coincidan con las fechas proyectadas. Este estado de progreso también podría significar que el proyecto está adelantado respecto a la programación y que las fechas proyectadas podrían ser anteriores a las fechas planificadas.</p> <p>Para obtener más información sobre las fechas proyectadas, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Información general sobre la fecha proyectada de finalización de proyectos, tareas y problemas</a>.</p> <p>Para obtener más información acerca de la fecha planificada de finalización de la tarea, consulte los siguientes artículos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Información general sobre la fecha planificada de inicio de la tarea</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Información general sobre la fecha planificada de finalización de la tarea</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>En riesgo</strong> </p> </td> 
   <td><p>Se considera una tarea <strong>En riesgo</strong> cuando la fecha estimada de finalización sea posterior a la fecha planificada de finalización y posterior a la fecha proyectada de finalización. Esto puede ocurrir cuando una tarea tiene una restricción de <strong>Debe finalizarse el</strong> o <strong>Debe comenzar el</strong> pero el porcentaje completado o las relaciones predecesoras de la tarea muestran que no puede finalizar o comenzar en las fechas especificadas. </p><p> Configuración de la restricción de tarea en <strong>Debe finalizarse el</strong> establece manualmente la fecha planificada de finalización en una fecha específica. La Fecha proyectada de finalización en este caso coincide con la Fecha planificada de finalización. En el caso de esta delimitación, Workfront analiza la tarea para calcular cuándo finalizará en función del porcentaje completado. Este cálculo se almacena como la fecha de vencimiento estimada. Si la fecha de vencimiento estimada es posterior a la fecha de finalización proyectada, la tarea se considera con riesgo de retrasarse. </p> <p> Configuración de la restricción de tarea en <strong>Debe comenzar el</strong> establece manualmente la fecha planificada de inicio en una fecha específica. La fecha de inicio proyectada en este caso coincide con la fecha de inicio planificada. En el caso de esta restricción, Workfront analiza la tarea para calcular cuándo comenzará en función de sus relaciones de predecesora. Este cálculo se almacena como la Estimated Start Date. Si hay una tarea predecesora forzada que no permite que la tarea comience en la fecha de inicio especificada, la fecha de inicio estimada puede ser posterior a la fecha proyectada de finalización. Se considera que la tarea está en riesgo de retrasarse. </p> <p>Nota: Por lo general, las fechas estimadas coinciden con las fechas proyectadas, excepto cuando <strong>Debe comenzar el</strong> o <strong>Debe finalizarse el</strong> se utilizan. En estos casos, las Fechas estimadas siguen calculándose en función del porcentaje completado y otros factores (relaciones de predecesoras), mientras que las Fechas proyectadas están obligadas a coincidir con las Fechas planificadas que se han establecido manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rezagado</strong> </p> </td> 
   <td> <p>Una tarea se considera <strong>Rezagado</strong> cuando la fecha estimada de finalización es posterior o igual a la fecha planificada de finalización y anterior a la fecha proyectada de finalización.</p> <p>La fecha proyectada de finalización es una vista en tiempo real de cuándo se completará la tarea en función del progreso anterior. Aunque la tarea se inició con retraso, aún no se considera que sea tarde, porque las fechas de finalización planificada y proyectada aún están en el futuro y es posible que la tarea se complete a tiempo.</p> <p>Nota: La <strong>Rezagado</strong> y <strong>En riesgo</strong> Los estados de progreso son casi idénticos. Sin embargo, <strong>En riesgo</strong> indica que hay algunas restricciones de tarea forzadas (debe finalizar el, debe comenzar el, fechas fijas) en una o ambas fechas planificadas. Si no hay delimitaciones forzadas en la tarea, las Fechas proyectadas son las mismas que las Fechas estimadas y reflejan el cálculo del sistema de la Fecha de finalización basado en el progreso actual de la tarea. La tarea aún no se considera tardía porque las fechas de finalización planificada y proyectada aún están en el futuro y es posible que la tarea se complete a tiempo.<br>Para obtener más información sobre las fechas proyectadas y estimadas, consulte <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Diferenciar entre fechas proyectadas y estimadas </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Retrasado</strong> </p> </td> 
   <td> <p>Una tarea es <strong>Retrasado</strong> cuando la fecha planificada de finalización sea anterior a la fecha actual.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![](assets/on-time-progress-status-350x233.png)

* At Risk

  ![](assets/at-risk-progress-status-350x233.png)

* Behind

  ![](assets/behind-progress-status-350x233.png)

* Late

  ![](assets/late-progress-status-350x233.png)

-->