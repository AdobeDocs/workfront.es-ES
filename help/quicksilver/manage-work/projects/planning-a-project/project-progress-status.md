---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Resumen del estado del progreso del proyecto
description: Adobe Workfront determina el estado de progreso de un proyecto observando la progresión del proyecto a lo largo de su cronología. Puede configurar Workfront para determinar la condición de un proyecto en función del valor del estado de progreso de las tareas. Para obtener más información sobre la configuración de la condición del proyecto, consulte el artículo Información general sobre la condición y el tipo de condición del proyecto.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# Resumen del estado del progreso del proyecto

Adobe Workfront determina el estado de progreso de un proyecto observando la progresión del proyecto a lo largo de su cronología. Puede configurar Workfront para determinar la condición de un proyecto en función del valor del estado de progreso de las tareas. Para obtener más información sobre la configuración de la condición del proyecto, consulte el artículo [Descripción general de la condición y el tipo de condición del proyecto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

A continuación se indican los estados de progreso de los proyectos en Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Tiempo de activación</td> 
   <td> <p>Si las fechas de finalización previstas y las previstas son anteriores o iguales a la fecha de finalización prevista del proyecto, el estado de progreso del proyecto es <strong>Tiempo de activación</strong>.</p> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>En riesgo</td> 
   <td> <p>Cuando las fechas de finalización previstas y las previstas se encuentran en el futuro, pero después de la fecha de finalización prevista del proyecto y la fecha de finalización estimada es posterior a la fecha de finalización prevista, el estado de progreso del proyecto es <strong>En riesgo</strong>. </p> <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Rezagado</td> 
   <td> <p>Cuando las fechas de finalización previstas y las previstas estén en el futuro, pero después de la fecha de finalización prevista del proyecto, pero la fecha de finalización estimada no sea posterior a la fecha de finalización prevista, el estado de progreso del proyecto será <strong>Detrás</strong>.</p> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Retrasado</td> 
   <td> 
    <ul> 
     <li> <p>Si el proyecto ha finalizado y la fecha de finalización real es posterior a la fecha de finalización prevista, el estado de progreso del proyecto es <strong>Late</strong>. </p> <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Si el proyecto no se ha completado y la fecha de finalización prevista del proyecto se encuentra en el pasado, el estado de progreso del proyecto es <strong>Late</strong>. </p> <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Tenga en cuenta lo siguiente:

* La fecha de finalización prevista del proyecto está impulsada por la tarea en la ruta crítica con la última fecha de finalización prevista.
* La fecha de finalización estimada del proyecto está impulsada por la tarea en la ruta crítica con la última fecha de finalización estimada.

Para obtener información sobre el proyecto Ruta crítica, consulte [Descripción general de la ruta crítica del proyecto](../../../manage-work/tasks/manage-tasks/critical-path.md).

Para obtener información sobre las fechas de finalización previstas, consulte [Información general sobre la fecha de finalización prevista para proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
