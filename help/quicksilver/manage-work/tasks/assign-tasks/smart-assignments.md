---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Información general sobre las asignaciones inteligentes
description: Al administrar asignaciones de tareas y problemas, puede utilizar asignaciones inteligentes para identificar quién es el mejor usuario para completar el trabajo. Las asignaciones inteligentes son sugerencias que Adobe Workfront presenta al asignar elementos de trabajo a recursos en función de un algoritmo que determina el recurso más adecuado para el trabajo.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '1255'
ht-degree: 95%

---

# Información general sobre las asignaciones inteligentes

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">La información resaltada en esta página hace referencia a la funcionalidad disponible solamente en el entorno de producción para los clientes que habilitaron versiones rápidas.</span>

<span class="preview">Para obtener información acerca de las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> Esta funcionalidad se eliminará del entorno de producción para los clientes que habilitaron la versión rápida con la versión 25.1 en enero de 2025. Para obtener más información sobre la versión 25.1, consulte [Información general sobre la versión del primer trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

Al administrar las asignaciones de tareas y problemas, puede utilizar asignaciones inteligentes para identificar quién es el mejor recurso para completar el trabajo. Las asignaciones inteligentes son sugerencias que Adobe Workfront presenta al asignar elementos de trabajo a recursos en función de un algoritmo que determina el recurso más adecuado para el trabajo. Las asignaciones inteligentes pueden ser usuarios, funciones o equipos.

>[!NOTE]
>
>Al sugerir usuarios, las asignaciones inteligentes no tienen en cuenta la disponibilidad del usuario. Sin embargo, su disponibilidad según sus programaciones afecta a las fechas planificadas y proyectadas de las tareas y problemas cuando se asignan. Para obtener información acerca de las programaciones, consulte el artículo [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Este artículo contiene información general sobre las asignaciones inteligentes. Para obtener información sobre cómo usar asignaciones inteligentes para asignar tareas y problemas a los usuarios, consulte [Realizar asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Información general sobre las asignaciones inteligentes

Tenga en cuenta lo siguiente al trabajar con asignaciones inteligentes:

* <span class="preview">El algoritmo funciona de forma independiente para tareas y problemas. Esto significa que la lista de usuarios sugeridos para los problemas puede diferir de la lista de usuarios sugeridos para una tarea, ya que Workfront crea las listas de acuerdo con los criterios pertenecientes a los problemas y las tareas por separado. </span>
<!--not sure this is accurate: * Smart assignments do not recommend job roles or teams. Instead, they are suggestions of users who are best fit to complete a task or an issue. -->
* Las asignaciones sugeridas siempre son usuarios activos, funciones o equipos.
* El recurso que aparezca en primer lugar debe ser el más adecuado para la tarea.

## Localizar las sugerencias de asignación inteligente

Puede ver las asignaciones inteligentes en las áreas siguientes, donde puede asignar tareas o problemas:

* Lista o informe de problemas en la columna Asignaciones

  ![](assets/smart-assignments-issue-list.png)

* <span class="preview">Una lista de tareas o un informe en la columna Asignaciones</span>

  ![](assets/smart-assignments-task-list.png)

* <span class="preview">Un encabezado de tarea en el campo Asignaciones</span>

  ![](assets/smart-assignments-task-header-nwe-350x302.png)

* Un encabezado de problema en el campo Asignaciones

  ![](assets/smart-assignments-issue-header.png)

* El panel Resumen de tareas o problemas del área Asignaciones

  ![](assets/issue-assignments-summary-panel.png)

* <span class="preview">El campo Asignaciones en el cuadro Nueva tarea, al añadir una tarea a un proyecto</span>

  ![](assets/smart-assignments-new-task-modal.png)

<!--this is not possible in the new home  - we have Summary there: 
* The Assignments field for an item listed in the Home area, when you open a task or issue

  ![](assets/smart-assignments-in-home-nwe-350x216.png)
-->

* <span class="preview">Distribuidor de cargas de trabajo en el área Asignado a al asignar una tarea o un problema</span>

  ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## Criterios de las asignaciones inteligentes

Las asignaciones inteligentes funcionan de forma diferente para las tareas y para los problemas.

### Criterios de las asignaciones inteligentes para tareas

El cálculo de asignaciones inteligentes de tareas funciona en <span class="preview">dos fases que utilizan dos algoritmos diferentes.</span>

<span class="preview">Según el algoritmo que encuentre la asignación inteligente, las asignaciones se enumerarán en dos secciones independientes del campo Asignaciones.</span> Para obtener más información, consulte [Realizar asignaciones inteligentes](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md).

![](assets/smart-assignments-task-list.png)

<div class="preview">

#### Primera fase del cálculo de asignación inteligente para tareas

En la primera fase del cálculo de las asignaciones inteligentes, Workfront calcula una puntuación de similitud para cada asignación.

>[!NOTE]
>
>La primera fase del cálculo de asignaciones inteligentes no se aplica a las siguientes áreas de tareas:
>
>* Asignaciones en lotes en el Distribuidor de cargas de trabajo.
>* Tarjetas conectadas en tableros.


El cálculo de la puntuación de similitud y el orden en que se enumeran las asignaciones tienen en cuenta lo siguiente:

* Se asigna una puntuación del 100 % a una asignación existente en la que los nombres de las tareas, proyectos y portafolios son idénticos a los de la tarea que intenta asignar. Los nombres de proyecto y portafolios de la tarea de una asignación existente también deben coincidir con el proyecto y portafolios de la tarea que intenta asignar.

* Si sólo parte de esta información de otras asignaciones coincide con las tareas existentes, la puntuación podría ser inferior al 100 %.

  Por ejemplo, si asigna una tarea denominada “Mi segunda tarea” a un proyecto denominado “Mi proyecto” en un portafolio denominado “Mi portafolio” y ya tiene una tarea denominada “Mi tarea” en otro proyecto denominado “Mi proyecto” en un portafolio denominado “Mi portafolio”, el usuario asignado a “Mi tarea” podría obtener una puntuación del 95 % porque el nombre de la tarea existente y la tarea que está intentando asignar ahora son similares, pero no idénticos.

  >[!TIP]
  >
  >  Workfront busca coincidencias únicamente en los campos Nombre de tareas, proyectos y portafolios y no en ningún otro campo.

* Una asignación podría obtener una puntuación más alta cuando se le asignan muchas tareas en el sistema que tienen nombres similares. Por ejemplo, si se asigna un equipo llamado “Desarrollo” al 50 % de las tareas del sistema que contienen “IA” en el nombre y ahora se asigna otra tarea con “AI” en el nombre, la puntuación del equipo “Desarrollo” es mayor. En este caso, los nombres de los proyectos y portafolios no son tan importantes.

* Teniendo en cuenta este sistema de puntuación, las primeras siete sugerencias se enumeran como asignaciones inteligentes, en orden descendente según sus puntuaciones. No se muestran las asignaciones con puntuaciones inferiores al 40 %.

* Si varias asignaciones tienen puntuaciones idénticas, se muestran en orden de fecha en que se realizaron las asignaciones, empezando por la fecha más reciente.

  Por ejemplo, si se asignó a Rick una tarea similar durante el día de hoy, y a Jennifer se le asignó una tarea similar hace dos días, Rick aparece primero.

* Las asignaciones identificadas en esta fase se enumeran en la sección **Asignaciones recomendadas** del campo Asignaciones para tareas.

* Si no se obtienen coincidencias al usar este cálculo, se inicia la segunda fase de las asignaciones inteligentes, que se calcula con un algoritmo diferente.

</div>

#### Segunda fase del cálculo de asignaciones inteligentes para tareas

Si no se encuentran coincidencias en el primer paso de las asignaciones inteligentes de tareas, Workfront calcula las asignaciones inteligentes de las tareas de la misma manera que las calcula para los problemas.

Para obtener más información, consulte la sección [Criterios de asignaciones inteligentes para tareas y problemas](#smart-assignments-criteria-for-tasks-and-issues) en este artículo.

Las asignaciones identificadas en esta fase se enumeran en las secciones **Usuarios y equipos**, **Asignaciones de funciones** y <span class="preview">**Funciones de tarjeta de tarifas**</span> del campo Asignaciones. <span class="preview">Para obtener más información sobre las tarjetas de tarifas, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)</span>. <!--keep the rate cards roles in yellow after the release of assignments to Prod-->

### Criterios de asignaciones inteligentes para tareas y problemas


>[!NOTE]
>
>Los siguientes criterios se aplican a las tareas solo cuando la primera fase del cálculo de asignación inteligente de tareas no encontró ninguna coincidencia. Para obtener más información, consulte la sección [Primera fase del cálculo de asignaciones inteligentes para tareas](#first-phase-of-smart-assignment-calculation-for-tasks) en este artículo. Los siguientes criterios siempre se aplican a los problemas de forma predeterminada.

![](assets/smart-assignments-issue-header.png)

Las recomendaciones se dan a los usuarios en la lista desplegable de asignaciones inteligentes en función de una combinación de los siguientes criterios (enumerados en orden de lo más importante a lo menos importante):

1. Usuarios asignados a otros elementos de trabajo en los últimos 30 días por el usuario que realiza la asignación. Se muestran los 50 primeros usuarios que coinciden con este criterio. El usuario que se asigna con mayor frecuencia se muestra primero.

2. Si el elemento de trabajo se asigna a un equipo o a una función, la lista de usuarios recomendados se filtra aún más teniendo en cuenta las asignaciones existentes a continuación. En este caso, solo se muestran los siguientes usuarios en la lista de sugerencias:

   * Usuarios cuyo equipo local es el equipo asignado al elemento de trabajo.
   * Usuarios cuya función principal es la función asignada al elemento de trabajo.

>[!TIP]
>
>* Si no hay ninguna función o equipo asignado para la tarea o el problema, Workfront muestra todos los usuarios asignados durante los últimos 30 días, hasta 50 usuarios.
>
>* Si no ha realizado ninguna asignación en los últimos 30 días, solo se mostrarán en la lista de asignaciones inteligentes los usuarios que pertenezcan al equipo asignado o que tengan la función asignada al elemento de trabajo.



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
