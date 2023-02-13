---
product-area: projects
navigation-topic: update-work-in-a-project
title: Interacciones entre la fecha de confirmación y la fecha de finalización prevista
description: Tanto la Fechas de Finalización Planificada como la Fechas de Confirmación indican cuándo se debe completar la tarea. Pero difieren por quién establece cada fecha.
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---

# Interacciones entre la fecha de confirmación y la fecha de finalización prevista

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

Tanto la Fechas de Finalización Planificada como la Fechas de Confirmación indican cuándo se debe completar la tarea. Pero difieren por quién establece cada fecha.

## Descripción general de la fecha de confirmación y la fecha de finalización prevista

Las fechas de finalización y finalización previstas existen tanto en las tareas como en los problemas.

La siguiente tabla contiene información sobre la diferencia entre las fechas de finalización y finalización planificada:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Fecha de confirmación</td> 
   <td> <p>La fecha de confirmación es la fecha en la que la persona asignada a una tarea o emisión manualmente estima que habrá completado la tarea o el problema.</p> <p>Para obtener información sobre fechas de confirmación, consulte <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Resumen de la fecha de confirmación</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fecha planificada de finalización</td> 
   <td> <p>La Fecha de Finalización Planificada muestra cuándo el propietario del proyecto espera que se complete la tarea o el problema. El propietario del proyecto o cualquier persona con permisos de gestión de la tarea o el problema pueden configurarlo manualmente, o Adobe Workfront puede calcularlo automáticamente.</p> <p>Para obtener más información sobre las fechas de finalización planificadas, consulte <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Descripción general de la tarea Fecha de finalización planificada</a></p> </td> 
  </tr> 
 </tbody> 
</table>

## Interacciones entre la fecha de confirmación y la fecha de finalización prevista

Cuando el propietario del proyecto crea y asigna una tarea o un problema, la tarea o el problema tendrá lo siguiente:

* Una fecha de finalización prevista
* Sin fecha de confirmación

El usuario asignado que trabaje en la tarea o el problema puede actualizar manualmente la Fecha de confirmación o actualizarla automáticamente aceptando trabajar en ella. Esta es una forma visual de indicar al propietario del proyecto cuándo sería realista que completaran la tarea o el problema.

>[!TIP]
>
>Solo el usuario asignado puede actualizar la Fecha de confirmación de una tarea o problema.

El usuario asignado que cambia la fecha de confirmación no cambia automáticamente la fecha de finalización planeada. Lo contrario también es cierto: al cambiar la fecha de finalización planeada, no se cambiará la fecha de confirmación.

Cuando la fecha de finalización cambia a una fecha posterior a la fecha de finalización planeada, se notifica al propietario del proyecto que este cambio se produjo y podría afectar a la cronología del proyecto.

Si el propietario del proyecto acepta la fecha de confirmación ofrecida por el usuario asignado, deberá actualizar manualmente la fecha de finalización prevista de la tarea o el problema. Para obtener más información, consulte los siguientes artículos:

* [Resumen de la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [Actualizar fechas de confirmación en tareas y problemas](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
