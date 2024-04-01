---
product-area: projects
navigation-topic: update-work-in-a-project
title: Interacciones entre la fecha de confirmación y la fecha planificada de finalización
description: Tanto la finalización planificada como las fechas de confirmación indican cuándo se debe completar la tarea. Pero difieren debido a quién establece cada fecha.
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
source-git-commit: ee957e319941fe5eabb9144eed184372e5402197
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---

# Interacciones entre la fecha de confirmación y la fecha planificada de finalización

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

Tanto la finalización planificada como las fechas de confirmación indican cuándo se debe completar la tarea. Pero difieren debido a quién establece cada fecha.

## Resumen de la fecha de compromiso y la fecha planificada de finalización

Existen fechas planificadas de finalización y confirmación tanto en tareas como en problemas.

La siguiente tabla contiene información sobre la diferencia entre las fechas de confirmación y finalización planificada:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Fecha de confirmación</td> 
   <td> <p>La fecha de confirmación es la fecha en la que la persona asignada manualmente a una tarea o problema estima que habrá completado la tarea o problema.</p> <p>Para obtener información sobre las fechas de confirmación, consulte <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Resumen de fecha de confirmación</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fecha planificada de finalización</td> 
   <td> <p>La fecha planificada de finalización indica cuándo espera el propietario del proyecto que se complete la tarea o el problema. Puede establecerlo manualmente el propietario del proyecto o cualquier persona con permisos de administración en la tarea o el problema, o Adobe Workfront puede calcularlo automáticamente.</p> <p>Para obtener más información sobre las fechas planificadas de finalización, consulte <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Información general sobre la fecha planificada de finalización de la tarea</a></p> </td> 
  </tr> 
 </tbody> 
</table>

## Interacciones entre la fecha de confirmación y la fecha planificada de finalización

Cuando el propietario del proyecto crea y asigna una tarea o un problema, la tarea o el problema presentan los siguientes elementos:

* Una fecha planificada de finalización
* Sin fecha de confirmación

El usuario asignado que trabaja en la tarea o el problema puede actualizar manualmente la fecha de confirmación o actualizarla automáticamente si acepta trabajar en ella. Es una forma visual de indicar al propietario del proyecto cuándo sería realista que completara la tarea o el problema.

>[!TIP]
>
>Solo el usuario asignado puede actualizar la fecha de confirmación de una tarea o problema.

El usuario asignado que cambia la fecha de compromiso no cambia automáticamente la fecha planificada de finalización. Lo contrario también es verdadero: al cambiar la fecha planificada de finalización, no se cambia la fecha de confirmación.

Cuando la fecha de compromiso cambia a una fecha posterior a la fecha planificada de finalización, se notifica al propietario del proyecto que este cambio se ha producido y podría afectar a la cronología del proyecto.

Si la fecha de confirmación ofrecida por el usuario asignado es aceptable para el propietario del proyecto, debe actualizar manualmente la fecha planificada de finalización de la tarea o el problema. Para obtener más información, consulte los siguientes artículos:

* [Resumen de fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [Actualizar fechas de confirmación en tareas y problemas](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
