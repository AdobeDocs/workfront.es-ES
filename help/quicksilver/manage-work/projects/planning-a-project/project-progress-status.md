---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Resumen del estado del progreso del proyecto
description: Adobe Workfront determina el estado de progreso de un proyecto mirando la progresión del proyecto en su cronología. Puede configurar Workfront para determinar la condición de un proyecto en función del valor de estado de progreso de las tareas. Obtenga más información acerca del estado del progreso del proyecto en este artículo .
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 1%

---

# Resumen del estado del progreso del proyecto

<!--Audited: 12/2023-->

Adobe Workfront determina el estado de progreso de un proyecto mirando la progresión del proyecto en su cronología. Puede configurar Workfront para determinar la condición de un proyecto en función del valor de estado de progreso de las tareas. Para obtener más información sobre la configuración de la condición del proyecto, consulte el artículo [Descripción general de la condición y el tipo de condición del proyecto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

A continuación se muestran los estados de progreso de los proyectos en Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>A tiempo</td> 
   <td> El estado del progreso de un proyecto es <strong>Tiempo de activación</strong> si:<ul><li>Si las fechas de finalización proyectada y estimada son anteriores o iguales a la fecha planificada de finalización del proyecto</li></ul> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>En riesgo</td> 
   <td> El estado del progreso de un proyecto es <strong>En riesgo</strong> if <strong>todo</strong> de lo siguiente es verdadero:<ul><li>Las fechas de finalización estimada y proyectada son futuras</li><li> Las fechas de finalización estimada y proyectada son posteriores a la fecha planificada de finalización</li><li> La fecha estimada de finalización es posterior a la fecha proyectada de finalización</li></ul><p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Rezagado</td> 
   <td> El estado del progreso de un proyecto es <strong>Rezagado</strong> if <strong>todo</strong> de lo siguiente es verdadero:<ul><li>Las fechas de finalización estimada y proyectada son futuras</li><li> Las fechas de finalización estimada y proyectada son posteriores a la fecha planificada de finalización del proyecto</li><li> La fecha estimada de finalización no es posterior a la fecha proyectada de finalización</li></ul> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Retrasado</td> 
   <td> 
     El estado del progreso de un proyecto es <strong>Retrasado</strong> if <strong>o bien</strong> de lo siguiente es verdadero:<ul><li>El proyecto se ha completado y la fecha real de finalización es posterior a la fecha planificada de finalización <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>El proyecto no está completo y la fecha planificada de finalización del proyecto se encuentra en el pasado <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Tenga en cuenta lo siguiente:

* La fecha proyectada de finalización del proyecto está controlada por la tarea en la ruta crítica con la última fecha proyectada de finalización.
* La fecha estimada de finalización del proyecto está controlada por la tarea en la ruta crítica con la última fecha estimada de finalización.

Para obtener información sobre la ruta crítica del proyecto, consulte [Información general sobre la ruta crítica del proyecto](../../../manage-work/tasks/manage-tasks/critical-path.md).

Para obtener información sobre las fechas de finalización proyectadas, consulte [Información general sobre la fecha proyectada de finalización de proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
