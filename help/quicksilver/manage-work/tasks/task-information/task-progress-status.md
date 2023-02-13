---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre el estado de progreso de la tarea
description: Adobe Workfront determina el estado de progreso de una tarea mirando el progreso de la tarea a lo largo de su cronología. Puede configurar Workfront para determinar la condición de un proyecto en función del valor del estado de progreso de las tareas. Para obtener más información sobre la configuración de la condición del proyecto, consulte el artículo Información general sobre la condición y el tipo de condición del proyecto.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 65f25a3b1198f491f7357efef11e2ae075e9721a
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 1%

---

# Información general sobre el estado de progreso de la tarea

Adobe Workfront determina el estado de progreso de una tarea mirando el progreso de la tarea a lo largo de su cronología. Puede configurar Workfront para determinar la condición de un proyecto en función del valor del estado de progreso de las tareas. Para obtener más información sobre la configuración de la condición del proyecto, consulte el artículo [Descripción general de la condición y el tipo de condición del proyecto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Criterios que determinan el estado de progreso de las tareas

Para obtener información sobre el estado de progreso de un proyecto, consulte [Resumen del estado del progreso del proyecto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Para obtener información sobre el seguimiento del progreso de las tareas, consulte [Información general sobre el modo de seguimiento de tareas](../../../manage-work/tasks/task-information/task-tracking-mode.md).

Los siguientes criterios determinan el estado de progreso de una tarea:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Estado de progreso</strong> </p> </th> 
   <th> <p><strong>Determinación de criterios</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>A tiempo</strong> </p> </td> 
   <td scope="col"> <p>Se considera una tarea <strong>Tiempo de activación</strong> cuando todas las fechas planeadas coinciden con las fechas proyectadas. Este estado de progreso también podría significar que el proyecto está por adelantado al calendario y que las fechas previstas podrían estar por encima de las fechas previstas.</p> <p>Para obtener más información sobre las fechas previstas, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Información general sobre la fecha de finalización prevista para proyectos, tareas y problemas</a>.</p> <p>Para obtener más información sobre la fecha de finalización planificada de la tarea, consulte los siguientes artículos:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Descripción general de la tarea Fecha de inicio planificada</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Descripción general de la tarea Fecha de finalización planificada</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>En riesgo</strong> </p> </td> 
   <td><p>Se considera una tarea <strong>En riesgo</strong> cuando la fecha de finalización estimada sea posterior a la fecha de finalización planeada y posterior a la fecha de finalización prevista. Esto puede ocurrir cuando una tarea tiene una restricción de <strong>Debe finalizar el</strong> o <strong>Debe comenzar el</strong> pero el porcentaje completado o las relaciones predecesoras de la tarea muestran que no puede terminar ni comenzar en las fechas especificadas. </p><p> Configuración de la restricción de tareas en <strong>Debe finalizar el</strong> establece manualmente la fecha de finalización planeada en una fecha específica. La Fecha de Finalización Prevista en este caso coincide con la Fecha de Finalización Planificada. En el caso de esta restricción, Workfront analiza la tarea para calcular cuándo finalizará en función del porcentaje completado. Este cálculo se almacena como Fecha de vencimiento estimada. Si la Fecha de vencimiento estimada es posterior a la Fecha de finalización prevista, se considera que la tarea corre el riesgo de llegar tarde. </p> <p> Configuración de la restricción de tareas en <strong>Debe comenzar el</strong> establece manualmente la fecha de inicio planeada en una fecha específica. En este caso, la Fecha de inicio prevista coincide con la Fecha de inicio planeada. En el caso de esta restricción, Workfront analiza la tarea para calcular cuándo comenzará en función de sus relaciones predecesoras. Este cálculo se almacena como Fecha de inicio estimada. Si hay un predecesor obligatorio que no permita que la tarea comience en la fecha de inicio especificada, entonces la fecha de inicio estimada puede ser posterior a la fecha de finalización prevista. Se considera que la tarea corre el riesgo de llegar tarde. </p> <p>Nota: Normalmente, las fechas estimadas coinciden con las fechas proyectadas excepto cuando <strong>Debe comenzar el</strong> o <strong>Debe finalizar el</strong> se utilizan. En estos casos, las fechas estimadas siguen calculándose en función del porcentaje completado y otros factores (relaciones predecesoras), mientras que las fechas proyectadas están obligadas a coincidir con las fechas planificadas que se han establecido manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rezagado</strong> </p> </td> 
   <td> <p>Se considera que una tarea es <strong>Detrás</strong> cuando la fecha de finalización estimada sea posterior o igual a la fecha de finalización planeada y anterior a la fecha de finalización prevista.</p> <p>La fecha de finalización prevista es una vista en tiempo real de cuándo se completará la tarea en función del progreso anterior. Aunque la tarea se inició con retraso, aún no se considera con retraso, ya que las fechas de finalización previstas y previstas siguen en el futuro y la tarea podría completarse a tiempo.</p> <p>Nota: La variable <strong>Detrás</strong> y <strong>En riesgo</strong> Los estados de progreso son casi idénticos. Sin embargo, <strong>En riesgo</strong> indica que hay algunas restricciones de tarea forzadas (debe terminar el, debe empezar el, fechas fijas) en una o ambas fechas planificadas. Si no hay restricciones forzadas en la tarea, las fechas proyectadas son las mismas que las fechas estimadas y reflejan el cálculo del sistema de la fecha de finalización en función del progreso actual de la tarea. La tarea aún no se considera tardía, ya que las fechas de finalización previstas y previstas siguen en el futuro y la tarea podría completarse a tiempo.<br>Para obtener más información sobre las fechas proyectadas y las fechas estimadas, consulte <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Diferenciación entre fechas proyectadas y estimadas </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Retrasado</strong> </p> </td> 
   <td> <p>Una tarea es <strong>Late</strong> cuando la fecha de finalización planeada es anterior a la fecha de hoy.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Cómo se actualiza el estado de progreso de la tarea a lo largo del tiempo

Los diferentes tipos de fechas de nuestros proyectos nos indican cómo progresan las tareas a lo largo del tiempo:

* A tiempo

   ![](assets/on-time-progress-status-350x233.png)

* En riesgo

   ![](assets/at-risk-progress-status-350x233.png)

* Rezagado

   ![](assets/behind-progress-status-350x233.png)

* Retrasado

   ![](assets/late-progress-status-350x233.png)
