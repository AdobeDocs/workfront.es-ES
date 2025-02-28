---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Establecer la fecha planificada de finalización del proyecto
description: La fecha planificada de finalización de un proyecto es la fecha en la que está previsto que finalice.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 94%

---

# Establecer la fecha planificada de finalización del proyecto

La fecha planificada de finalización de un proyecto es la fecha en la que está previsto que finalice.

Las fechas de inicio y finalización planificadas de un proyecto dependen de las fechas de las tareas del proyecto. En este artículo se describe cómo se puede establecer de forma manual o automática la fecha planificada de finalización de un proyecto. Para obtener más información sobre la fecha planificada de finalización de una tarea, consulte [Información general sobre la fecha planificada de finalización de la tarea](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

La fecha planificada de finalización de un proyecto se puede establecer de forma manual o automática, dependiendo de si se programa el proyecto desde la fecha de inicio o desde la fecha de finalización.

## Requisitos de acceso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos del proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Establecer manualmente la fecha planificada de finalización de un proyecto

Debe establecer manualmente la fecha planificada de finalización de un proyecto al programar el proyecto desde la fecha de finalización.

>[!NOTE]
>
>Cuando se establece manualmente la fecha planificada de finalización de un proyecto, Workfront calcula automáticamente la fecha planificada de inicio del proyecto en función de la duración de todas las tareas.


Para programar un proyecto desde la fecha de finalización:

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y luego haga clic en **Proyectos**.

1. Haga clic en **Nuevo proyecto** y luego en **Nuevo proyecto**.

   Para obtener más información sobre la creación de proyectos, consulte el artículo [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

1. Seleccione **Detalles del proyecto** en el panel izquierdo y, a continuación, haga clic en el icono **Editar proyecto** en la esquina superior derecha.

1. En el campo **Modo de programación**, seleccione **Fecha de finalización**.

1. Especifique la **fecha planificada de finalización** del proyecto.
1. Haga clic en **Guardar cambios**.

   A medida que comienza a añadir tareas al proyecto, la **fecha planificada de inicio** del proyecto se calcula según la duración total de todas las tareas. 

## Establecer automáticamente la fecha planificada de finalización de un proyecto

Workfront calcula automáticamente la fecha planificada de finalización de un proyecto al programar el proyecto desde la fecha de inicio. 

Para programar un proyecto a partir de la fecha de inicio:

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y luego haga clic en **Proyectos**.

1. Haga clic en **Nuevo proyecto** y luego en **Nuevo proyecto**.

   Para obtener más información sobre la creación de proyectos, consulte el artículo [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

1. Seleccione **Detalles del proyecto** en el panel izquierdo y, a continuación, haga clic en el icono **Editar proyecto** en la esquina superior derecha.

1. En el campo **Modo de programación**, seleccione **Fecha de inicio**.

1. Especifique la **Fecha planificada de inicio** del proyecto.
1. Haga clic en **Guardar cambios**.

   A medida que comienza a añadir tareas al proyecto, la **fecha planificada de finalización** del proyecto se calcula según la duración total de todas las tareas. 

   Para obtener más información sobre la duración de la tarea, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   La fecha planificada de finalización del proyecto coincide, en este caso, con la fecha planificada de finalización de la última tarea del proyecto.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria.&nbsp;</p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task.&nbsp;</p>
<p>You can manually set the Planned Completion Date&nbsp;when creating a task, as described in&nbsp;the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints:&nbsp;</p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary&nbsp;Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date&nbsp;is determined based on the following calculation:&nbsp;</p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
&nbsp;The Update Type for the project must also be&nbsp;set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
