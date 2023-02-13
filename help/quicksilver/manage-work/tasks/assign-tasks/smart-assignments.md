---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Información general sobre asignaciones inteligentes
description: Al administrar asignaciones de tareas y problemas, puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo. Las asignaciones inteligentes son sugerencias que Adobe Workfront le presenta cuando asigna elementos de trabajo a recursos en función de un algoritmo que determina el recurso más adecuado para el trabajo.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 7e220e496aff2675910416bd86e3ddf7b9231afa
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Información general sobre asignaciones inteligentes

Al administrar asignaciones de tareas y problemas, puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo. Las asignaciones inteligentes son sugerencias que Adobe Workfront le presenta cuando asigna elementos de trabajo a recursos en función de un algoritmo que determina el recurso más adecuado para el trabajo.

>[!NOTE]
>
>Las asignaciones inteligentes no tienen en cuenta la disponibilidad del usuario. Sin embargo, su disponibilidad según sus programaciones afecta a las fechas planificadas y previstas de las tareas y problemas cuando se les asigna. Para obtener información sobre las programaciones, consulte el artículo [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Este artículo contiene información general sobre las asignaciones inteligentes. Para obtener información sobre el uso de asignaciones inteligentes para asignar tareas y problemas a los usuarios, consulte [Realización de asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Información general sobre asignaciones inteligentes

Tenga en cuenta lo siguiente al trabajar con asignaciones inteligentes:

* El algoritmo funciona de forma independiente para tareas y problemas. Esto significa que la lista de usuarios sugeridos para problemas puede diferir de la lista de usuarios sugeridos para una tarea porque Workfront crea las listas de acuerdo con criterios pertenecientes a problemas y tareas por separado.
* Las asignaciones inteligentes no recomiendan funciones de trabajo ni equipos. En su lugar, son sugerencias de usuarios que son los más adecuados para completar una tarea o un problema.
* Las asignaciones sugeridas siempre son usuarios activos.
* El usuario que aparece primero debe ser la mejor coincidencia para la tarea.

## Buscar sugerencias de asignación inteligente

Puede ver las asignaciones inteligentes en las siguientes áreas, donde puede asignar tareas o problemas:

* Una tarea, una lista de problemas o un informe

   ![](assets/smart-assignments-task-list-nwe-350x280.png)

* Una tarea o un encabezado de problema

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

* La tarea o el panel Resumen del problema

   ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* El campo Asignaciones de un elemento enumerado en el área principal

   ![](assets/smart-assignments-in-home-nwe-350x216.png)


<!--removed for scheduling deprecation: 

* Resource Scheduling

  ![](assets/smart-assignments-scheduling-350x219.png)

  >[!CAUTION]
  >
  >Resource Scheduling is a deprecated feature. For more information, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Distribuidor de cargas de trabajo

   ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## Criterios de asignación inteligente

Las asignaciones inteligentes muestran las 50 recomendaciones principales en función de un algoritmo propietario.

Se recomienda a los usuarios en la lista desplegable de asignaciones inteligentes en función de una combinación de los siguientes criterios (enumerados en orden de más importante a menos importante):

* Usuarios asignados a otros elementos de trabajo en los últimos 30 días por el usuario que realiza la asignación. Se muestran los 50 primeros usuarios que coinciden con estos criterios. El usuario que se asigna con más frecuencia aparece primero.

   Si el elemento de trabajo está asignado a un equipo o a una función, la lista de usuarios sugeridos se filtra aún más teniendo en cuenta las asignaciones existentes a continuación. En este caso, solo los siguientes usuarios se muestran en la lista de sugerencias:

   * Usuarios cuyo equipo principal es el equipo asignado al elemento de trabajo.
   * Usuarios cuya función principal es la función asignada al elemento de trabajo.

      >[!TIP]
      >
      >* If <!--you're not part of any team and --> no hay ninguna función o equipo asignado en la tarea o el problema, Workfront muestra todos los usuarios asignados durante los últimos 30 días, hasta 50 usuarios.
      >* Si no ha realizado ninguna asignación en los últimos 30 días, solo los usuarios que pertenezcan al equipo asignado o que tengan la función asignada al elemento de trabajo se mostrarán en la lista de asignaciones inteligentes.


<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
