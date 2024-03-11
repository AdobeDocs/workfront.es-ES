---
product-area: templates
navigation-topic: templates-navigation-topic
title: Editar plantillas de proyecto
description: Puede editar las plantillas de proyecto para reflejar los cambios en los procesos y la configuración del proyecto.
author: Alina
feature: Work Management
exl-id: da0fca31-6a50-4862-ad9a-a453ef968773
source-git-commit: a243094dc6bbbe71a6efdb4fe99f7365daae514d
workflow-type: tm+mt
source-wordcount: '4710'
ht-degree: 2%

---

# Editar plantillas de proyecto

<!-- Audited: 2/2024 -->

<!--The Resource Pools part also duplicates in the "Working with Resource Pools" article-->

Puede editar las plantillas de proyecto para reflejar los cambios en los procesos y la configuración del proyecto. Después de actualizar y guardar los cambios en una plantilla, los nuevos cambios serán visibles en los nuevos proyectos cuando los proyectos se creen con la plantilla. Los cambios que realice en la plantilla no se reflejarán en el proyecto que esté utilizando esa plantilla.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td>
      <p>Nuevo: estándar</p>
      <p>O</p>
      <p>Actual: plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Editar acceso a plantillas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> 
    <ul> 
     <li> <p>Permisos de contribución para editar una plantilla en la pestaña Detalles de la plantilla</p> </li> 
     <li> <p>Administre los permisos de una plantilla para editarla en el cuadro Editar plantilla</p> </li> 
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Edición de una plantilla {#edit-a-template}

<!--
Editing a template differs depending on what environment you choose. 

### Edit a template in the Production environment {#edit-a-template-in-the-production-environment} 

1. Go to the template you want to edit.
1. (Conditional) To edit limited information about the template,  click **Template Details** in the left panel, then go to the areas listed in the left panel to edit information for each area. 
1. To edit information in the Details section, click the **Edit** icon ![](assets/edit-icon.png), then select from any of the areas below, or click **Edit all** to edit information in all areas:

   * Overview
   * Custom Forms

     Names of customs forms display only if there are custom forms attached to the object.
   
   * Finance

   >[!TIP]
   >
   >For information about all fields that display in the Details area, continue with editing all fields using the Edit Template box below.

1. (Conditional) To edit all information about the template, click the **More** menu ![](assets/qs-more-icon-on-an-object.png) next to the name of the template, then click **Edit**.

   The **Edit Template** box opens. The sections in this box contain the same fields available in  the Template Details section .

1. Consider editing information in any of the following sections:

   * [Overview](#overview) 
   * [Finance](#finance) 
   * [Portfolio](#portfolio) 
   * [Settings](#settings) 
   * [Access](#access) 
   * [Custom Forms](#custom-forms) 
   * [Tasks](#tasks) 
   * [Issues](#issues) 
   * [Comment](#comment)

### Overview {#overview}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Overview**.

   ![](assets/edit-template-overview-with-tasks-and-issues-350x210.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong></td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong></td> 
      <td>Add additional information about the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Active</strong></td> 
      <td><p>Select this checkbox if you want the template to be active. Other users can find this template and attach it to projects when creating projects. Deselect this checkbox if you want to deactivate templates that are no longer used. Deactivated templates cannot be attached to projects. This is enabled by default. </p><p><b>TIP</b>
      
      You can deactivate a template from the template header as described in the [Activate or deactivate a template](#activate-or-deactivate-a-template) section in this article.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong></td> 
      <td>Specify a web link that relates to information about this template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule From</strong></td> 
      <td><p>Specify whether the project using this template is scheduled from the <strong>Start Date</strong>, or from the <strong>Completion Date</strong>. This selection determines the planned dates of the future tasks on the project using this template. </p><p>Select from the following: </p> 
       <ul> 
        <li><p><strong>Schedule From Start Date</strong>: The Start Date of the template is actually the Start Day. When you schedule a template from Start Date, Adobe Workfront calculates the Completion Day of the template based on the Duration of all the template tasks. The Start Day of the template becomes the Planned Start Date of the future project.</p></li> 
        <li><p><strong>Schedule from Completion Date</strong>: The Completion Date of the template is actually the Completion Day. When you schedule a template from Completion Date, Workfront calculates the Start Day of the template based on the Duration of all the template tasks. The Completion Day of the template becomes the Planned Completion Date of the future project. </p></li> 
       </ul><p>For more information about the Start and Completion Days of template tasks, see <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Overview of Start and Completion Days in a template</a>. </p><p>The Schedule From setting for templates is similar to that of projects. Your Workfront administrator selects the default Schedule From setting for the projects in your system. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition Type</strong></td> 
      <td><p>Select between the following Condition Types:</p> 
       <ul> 
        <li><strong>Manual:</strong> The project owner sets the Condition of the project on the project manually. <strong></strong></li> 
        <li><strong>Progress Status:</strong> Workfront automatically sets the Condition of the future project based on the Progress Status of tasks on the Critical Path. For more information about understanding Progress Status, see <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task Progress Status overview</a>.</li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong></td> 
      <td><p>This is just a visual flag for you which allows you to prioritize your future projects. Select from the following options:</p> 
       <ul> 
        <li><p><strong>None</strong></p></li> 
        <li><p><strong>Low</strong></p></li> 
        <li><p><strong>Normal</strong></p></li> 
        <li><p><strong>High</strong></p></li> 
        <li><p><strong>Urgent</strong></p></li> 
       </ul><p><p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Owner</strong></td> 
      <td><p>The user who is designated as the Template Owner must be a Workfront active user. </p><p>Consider the following about the user designated as the Template Owner: </p> 
       <ul> 
        <li>They are automatically given Manage permissions to the template. </li> 
        <li>They are added to the project team and are automatically given Manage permissions to the project created from the template. </li> 
        <li>They become the Project Owner, when the project is created from this template. </li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Sponsor</strong></td> 
      <td><p>The user specified in this field becomes the Project Sponsor, when the template is added to the project. This user is added to the project team and is automatically given view permissions to the project. The user who is designated as the Template Sponsor must be a Workfront active user. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Manager</strong></td> 
      <td><p>The specified users are automatically given manage permissions to the future projects and can assign resources to the tasks and issues of the projects. You can specify more than one Resource Manager. </p></td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Group</strong></td> 
      <td><p>In the drop-down list, select the group that you want to be associated with projects created from the template. It can be a group of any level. </p><p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p><b>NOTES</b>
      
    <ul> 
    <li><p>In the Projects area on a group's page, when someone creates a project using a template that doesn't have a group selected, the system associates the currently open group with the project.</p><p>This is different from other areas where the system associates a user's Home Group with the project when the user creates the project using a template that doesn't have a group selected.</p>
    </li> 
      <li><p>If a user selects a template that has a group selected while creating a project—or while converting a task or issue to a project—the user can choose a different group for the project.</p></li> 
      <li>Though this field is available in templates only in the new Adobe Workfront experience, you can see it in lists and reports both there and in Adobe Workfront Classic. </li> 
      </ul> </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Company</strong></td> 
      <td><p>Specify the Company that you want to associate with the template. Only active companies display in the list.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Finance {#finance}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Finance**.

   ![](assets/edit-template-finance-with-tasks-and-issues-350x259.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Performance Index Method</strong></td> 
      <td><p>Specify whether the Earned Value metrics of the future project are calculated using hours or costs. For more information about the Performance Index Method, see <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Set the Performance Index Method (PIM)</a>. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Budget</strong></td> 
      <td><p>Specify a Budget for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Cost</strong></td> 
      <td><p>Specify the Fixed Cost for the projects that are created from this template. This is different than the Labor Cost which comes from the hours on the project and the Expense Cost which comes from the amount of expenses on the project. The Fixed Cost of a project is taken into account when calculating the Net Value of a project and it is part of the Budgeted Cost.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Revenue</strong></td> 
      <td><p>Specify the Fixed Revenue for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Currency</strong></td> 
      <td><p>Specify the currency for the future project, if it is different than the default currency of your system. This field is not visible if you have only the default currency in the system.<br>For more information about currency, see <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Require time to be approved for this project</strong></td> 
      <td><p>Select this option to require the Project Owner of the future project created from this template to approve time logged on the project. If you are using Billing Records and you select this option, only the approved hours on the project appear as available billable hours for the Billing Records. Approving time on the project is independent of approving timesheets. For more information about requiring time to be approved on a project, see <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Require time to be approved for a project</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Portfolio {#portfolio}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Portfolio**.

   ![](assets/edit-template-portfolio-with-tasks-and-issues-350x228.png)

1. Update the following fields:

   <table style="table-layout:auto">
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Portfolio</strong></td> 
      <td><p>Specify a Portfolio for the projects that are created from this template. You must create a Portfolio first, before it appears in the drop-down list. </p><p>Only active portfolios display in the list. For more information about creating portfolios, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Create a portfolio </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Program</strong></td> 
      <td><p>If you selected a Portfolio for the template, specify a <strong>Program</strong> for the future project. Some Portfolios might not have Programs. You must create a Program first, before it appears in this drop-down list. Only active programs display in the list.</p><p>For more information about creating programs, see <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Create a program</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Benefit</strong></td> 
      <td><p>Specify the Planned Benefit of the projects that are created from this template. The Planned Benefit is used in the Business Case of the project and the Portfolio Optimizer. </p><p>For more information about the Planned Benefit of a project, see <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Overview of project Planned Benefit</a>. The Planned Benefit of a project is taken into account when the Net Value of a project is calculated. </p><p>For more information about using the Portfolio Optimizer, see <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Manage projects in the Portfolio Optimizer</a> </p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Settings {#settings}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Settings**.

   ![](assets/edit-template-settings-with-tasks-and-issues-350x336.png)

1. Update the following fields: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Milestone Path</strong> </td> 
      <td> <p>Select a Milestone Path for the template. Only active milestone paths display in the list.<br>For more information about Milestone Paths, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Create a milestone path</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Mode</strong> </td> 
      <td> <p>Controls how the future project will be marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The project is marked Complete when all the tasks and issues are completed.</p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually select the Complete status for the project, when all the tasks and issues are completed. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Summary Completion Mode</strong> </td> 
      <td> <p>Controls how the parent tasks on the future project are marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The parent tasks are marked Complete and they update their percent complete automatically, as the children tasks are completed and the percent complete of the children is updated. </p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually update the percent complete and the status of the parent tasks, independently of what changes are made to the children tasks. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Update Type</strong> </td> 
      <td> <p>Controls when the changes you make to the timeline of the future project are saved on the project. </p> 
       <b>EXAMPLE </b> 
        <p>The following changes to the project trigger an update to the timeline of the project:</p> 
        <ul> 
         <li> <p>update the dates of tasks</p> </li> 
         <li> <p>change predecessor relationships<br></p> </li> 
         <li> <p>change parent-child relationships</p> </li> 
         <li> <p>add or remove assignments in addition to changing the task constraint or duration type.</p> </li> 
        </ul> 
       </div> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Automatic and On Change</strong> (Default setting): The future project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on (On Change). The project timeline is also updated each night (Automatic).<br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you perform an action on a task or project that triggers a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer recalculations display briefly as a question mark (between 1 and 5 seconds, or up to a minute for large projects). This indicates that the recalculation is not yet finished, and the dates are subject to change.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Change Only</strong>: The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Automatic Only</strong>: The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on. However, be aware that you chose this setting, as the project will not update at the same time that the changes are made.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Manual Only</strong>: The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.<br></p> </li> 
       </ul> <p>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule</strong> </td> 
      <td> <p>Select a schedule for your template. This will become the schedule of the project that is created from this template. This should be the same schedule assigned to most people that are working on the project. You must create a schedule before you can assign it to a template.<br>For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>. <br>If you have not created custom schedules in your system, the Default Schedule is selected. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>User Time Off</strong> </td> 
      <td> <p>Determines whether the time off of the Primary Assignee of a task adjusts the task planned dates. When you attach the template to an existing project, and the template has a different setting for this field than the project, the setting on the project remains unchanged. The default option for this setting for a new template is the same as the system-level project preference. </p> <p>For information about the project preferences at the System level, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> <p>For information about how this setting affects the task dates on a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.<br>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Consider user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template adjust according to the time off of the Primary Assignee of the task, if the time off occurs during the duration of the task. </p> </li> 
        <li> <p><strong>Ignore user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template remain as originally planned, even if the Primary Assignee of the task has time off during the duration of the task. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Leveling Mode</strong> </td> 
      <td> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Manual</strong>: you must manually level your resources on the project created from this template (this is the default setting)</p> </li> 
        <li> <p><strong>Automatic:</strong> Workfront levels the resources on the future project. <br>For more information about Resource Leveling, see <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Level Resources in the Gantt Chart </a>. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Risk</strong> </td> 
      <td> <p>Define the level of risk of the projects created from this template. The risk is just an indicator of how risky a project can be. You can prioritize the execution of your projects based on the level of risk.<br>Consider selecting from the following levels of risk:<br></p> 
       <ul> 
        <li> <p><strong>Very Low</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p><strong>Medium</strong> </p> </li> 
        <li> <p><strong>High</strong> </p> </li> 
        <li> <p><strong>Very High</strong> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Pools</strong> </td> 
      <td> <p>Specify the resource pools associated with the template. Resource pools are collections of users that are needed at the same time for the completion of a project. For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> <p> <p><b>NOTE</b> 
      
      When you edit templates in bulk, only the resource pools that are common to all the templates selected appear in this field. If the templates selected have no shared resource pools, this field will be empty. The resource pools you specify here will overwrite the templates' individual resource pools.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template. Your Workfront administrator or a user with administrative access to Approval Processes must define system-level or group-level project approval processes before you can associate them with a template. For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
      <ul> 
      <li>Only active approval processes display in the list. </li> 
      <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the template does not display in the list.</p> <p><b>IMPORTANT</b> 
      
      If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
      <li> <p>If you added a single-use approval process, it displays as "Custom" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p> 
      </li> 
      <li> <p>When bulk-editing templates, the following scenarios exist:</p> 
      <ul> 
         <li> <p>When you select templates from the same group, both system-level and group-level approval processes display in this field.</p> </li> 
         <li> <p>When you select templates from different groups, only system-level approval processes display in this field.</p> </li> 
         <li> <p>When any of the templates has a single-use approval process attached, it is replaced by the system-level you select. </p> </li> 
      </ul> </li> 
      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Filter Hour Types</strong> </td> 
      <td> <p>Consider the following:</p> <p>Select <strong>No</strong> to make all project-specific hour types available on the future project. (This is the default selection)</p> <p>Or</p> <p>Select <strong>Yes</strong> to make only a subset of the project-specific hour types available on the future project, then select the hour types you want to make available. (Hold the Shift key to select multiple hour types.)</p> <p>If you select this option, only the hour types you select are made available to select when logging hours on the project (or on tasks and issues within the project). You must select at least one hour type; if you select this option and you do not select any hour types, all hour types are made available on the project.</p> <p>The same hour type selections must be made at the individual user level in order for the user to see these hour type options on the project. </p> <p>For more information about defining hour types at the user level, see the section <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Log time</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notification</strong> </td> 
      <td>Select the Reminder Notification that should be associated with the future project. You must configure Reminder Notifications for projects for this field to appear during editing a template. <br>For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.  
   Or
1. Click **Save Changes**.

### Access {#access}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Access**.

   ![](assets/edit-template-access-with-tasks-and-issues-350x241.png)

   The Access you specify for your template will become the Access of users associated with the project when the template is used to create a project.

   Specify the following **Access** information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to a task</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to a task. The user assigned to a task is automatically granted this access to the task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to a task is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to an issue</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to an issue. The user assigned to an issue is automatically granted this access to the issue. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to an issue is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone submits a request: Give them access</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the request. When they submit a request to the project, they are granted this access to the request they submitted. For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>People from the same company will inherit the same permissions for all requests</strong> </td> 
      <td> <p>Select this field if you want people from the same company to have the same access to all the requests on the project, whether they submitted them or not.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is given access to this project: Give them access to ...</strong> </td> 
      <td> <p>Select the access options that you want users to have on the project, if the project is shared with them. Select the specific options for their access, if they are designated as <strong>Viewers</strong>, <strong>Contributors</strong>, or <strong>Managers</strong> when sharing the project with them. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Custom Forms {#custom-forms}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Custom Forms**.

   ![edit_tempate_custom_forms.png](assets/edit-tempate-custom-forms-tasks-with-issues-sections-350x136.png)

1. Select the custom form or forms that you want to associate with the template. You must build the custom forms before they are available to select in this field.

   Only active custom forms display in the list. For more information about building custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   You can add up to ten custom forms to a template.

   The forms will be added to the project that is created from this template. 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Tasks {#tasks}

You can define the defaults that will be associated with all the new tasks when you add them to a project that is created from the template.

For information about how these settings affect creating new tasks, see [Create tasks overview](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Tasks**.

   ![](assets/edit-template-with-tasks-and-issue-sections-350x144.png)

1. In the **Task Default Approval Process** box, select the Approval Process you want to associate with all new tasks when you add them to a project created from this template. You must create an Approval Process for tasks before you can associate it with tasks. Only active approval processes display in the list. For more information about creating Approval Processes, see [Creating Approval Processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. In the **Task Default Custom Forms** box, select the custom form or forms that you want to associate with all new tasks when you add them to a project created from this template. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. For more information about building custom forms, see [Creating Custom Forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). You can associate up to ten custom forms with a task.
1. (Optional) **Select Use Work Effort to automatically calculate task Planned Hours** if you want to enable managing task effort by using&nbsp;Work Effort instead of Planned Hours in the project created from the template.
1. (Conditional and optional) If you selected Use Work Effort to automatically calculate task Planned Hours, click the drop-down menu to update the percentage for each level of Work Effort. The following percentage values are the defaults:
 
   | Work Effort level |Percentage value|
   |---|---|
   | Small |25% |
   | Medium |50% |
   | Large |75% |

  For information about using Work Effort to manage the effort on tasks on projects, see [Work Effort overview](../../../manage-work/tasks/task-information/work-effort.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Issues {#issues}

By editing issue settings, you can prevent users from adding issues inline in the future project created from the template.

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Issues**.

   ![](assets/edit-template-box-with-issues-nwe-350x171.png)

1. (Optional) Deselect the **Allow users to add issues inline** option. It is enabled by default.

   When disabling this option users cannot add issues inline to the project or the tasks in the Issues section, when the project is created from the template.

   >[!TIP]
   >
   >Disable this option if you want to enforce users to complete the New Issue Fields or the custom forms associated with new issues.

   When disabling this option, users with permissions to add issues to the project created from the template can do so by using the New Issue button or a request queue associated with the project.

   For more information about configuring issue settings on projects, see the [Issue Settings](../../../manage-work/projects/manage-projects/edit-projects.md#issue) section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

   For information about creating issues on projects, see [Create issues](../../../manage-work/issues/manage-issues/create-issues.md). 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Comment {#comment}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Comment**.

   ![edit_templates_comment.png](assets/edit-templates-comment-with-tasks-and-issues-350x177.png)

1. Specify a comment that you want to display in the updates stream of the template in the available field.

   This comment is visible for everyone with View access to the template and with access to view Notes.

1. Click **Save Changes**.

   Your changes will be submitted for this template.

   Now, when you use this template to create a project all these settings will transfer to the new project.


   <!--drafted section below for the edit template story: 
   remove this tag and add the Preview blurb at the top of this article in yellow, if it's not already there. Keep the "div class" tags below until 23.1 production: 


### Edit a template in the Preview environment {#edit-a-template-in-the-preview-environment}
-->

1. Vaya a la plantilla que desee editar.
1. (Condicional) Para editar información limitada sobre la plantilla, haga clic en **Detalles de plantilla** en el panel izquierdo, vaya a las áreas enumeradas en el panel izquierdo para editar la información de cada área.
1. Para editar información en la sección Detalles, haga clic en **Editar** icono ![](assets/edit-icon.png), seleccione una de las áreas siguientes o haga clic en **Editar todo** para editar información en todas las áreas:

   * Información general
   * Formularios personalizados

   Los nombres de los formularios personalizados solo se muestran si hay formularios personalizados adjuntos al objeto.

   * Finanzas

   >[!TIP]
   >
   >Para obtener información sobre todos los campos que se muestran en el área de Detalles, continúe editando todos los campos con el cuadro Editar plantilla que aparece a continuación.

1. (Condicional) Para editar toda la información acerca de la plantilla, haga clic en **Más** menú ![](assets/qs-more-icon-on-an-object.png) junto al nombre de la plantilla y haga clic en **Editar**.

   El **Editar plantilla** se abre el cuadro. Las secciones de este cuadro contienen los mismos campos disponibles en la sección Detalles de la plantilla

1. Considere la posibilidad de editar la información en cualquiera de las siguientes secciones:

   * [Nombre de plantilla](#template-name)
   * [Información general](#overview-preview)
   * [Finanzas](#finance-preview)
   * [Formularios personalizados](#custom-forms-preview)
   * [Configuración de proyecto](#project-settings)
   * [Configuración de tareas](#task-settings)
   * [Configuración de problema](#issue-settings)
   * [Acceso](#access-preview)


### Nombre de plantilla{#template-name}

1. Empiece a editar la plantilla como se ha descrito anteriormente.
1. En el **Editar plantilla** , haga clic en **Nombre de plantilla**.
1. (Opcional) Siga editando las secciones siguientes, según la información que desee modificar

   O

   Haga clic en **Guardar**.



### Información general {#overview-preview}

1. Empiece a editar la plantilla como se ha descrito anteriormente.
1. En el **Editar plantilla** , haga clic en **Información general**.

   ![](assets/edit-template-box-overview-section.png)

1. Actualice los campos siguientes:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
         <tr> 
         <td role="rowheader"><strong>Descripción</strong></td> 
         <td>Añada información adicional sobre la plantilla.</td> 
       </tr> 
         <tr> 
         <td role="rowheader"><strong>Prioridad</strong></td> 
         <td><p>Esto solo es un indicador visual para usted que le permite priorizar sus proyectos futuros. Seleccione entre las siguientes opciones:</p> 
         <ul> 
         <li><p><strong>Ninguno</strong></p></li> 
         <li><p><strong>Bajo</strong></p></li> 
         <li><p><strong>Normal</strong></p></li> 
         <li><p><strong>Alto</strong></p></li> 
         <li><p><strong>Urgente</strong></p></li> 
         </ul><p><p>Según las Preferencias del proyecto seleccionadas por el administrador de Workfront, los nombres de las prioridades pueden ser diferentes para usted. Para obtener más información sobre la edición de prioridades, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Creación y personalización de prioridades</a>.</p></p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>URL</strong></td> 
         <td>Especifique un vínculo web relacionado con la información sobre esta plantilla.</td> 
       </tr>
       <tr> 
       <td role="rowheader"><strong>Tipo de condición</strong></td> 
       <td><p>Seleccione entre los siguientes tipos de condición:</p> 
         <ul> 
         <li><strong>Manual:</strong> El propietario del proyecto establece manualmente la condición del proyecto en el proyecto. <strong></strong></li> 
         <li><strong>Estado de progreso:</strong> Workfront establece automáticamente la condición del proyecto futuro en función del estado de progreso de las tareas en la ruta crítica. Para obtener más información sobre el estado de progreso, consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Resumen del estado de progreso de tareas</a>.</li> 
       </ul>
         </td> 
         </tr> 
       <tr> 
         <td role="rowheader"><strong>Modo de programación</strong></td> 
         <td><p>Especifique si el proyecto que utiliza esta plantilla está programado desde el <strong>Fecha de inicio</strong>, o desde el <strong>Fecha de finalización</strong>. Esta selección determina las fechas planificadas de las tareas futuras del proyecto mediante esta plantilla. </p><p>Seleccione una de las siguientes opciones: </p> 
       <ul> 
       <li><p><strong>Programar desde la fecha de inicio</strong>: la fecha de inicio de la plantilla es en realidad el día de inicio. Cuando se programa una plantilla a partir de la fecha de inicio, Adobe Workfront calcula el día de finalización de la plantilla en función de la duración de todas las tareas de plantilla. El día de inicio de la plantilla se convierte en la fecha planificada de inicio del futuro proyecto.</p></li> 
       <li><p><strong>Programar desde fecha de finalización</strong>: la fecha de finalización de la plantilla es en realidad el día de finalización. Cuando se programa una plantilla a partir de la fecha de finalización, Workfront calcula el día de inicio de la plantilla en función de la duración de todas las tareas de plantilla. El día de finalización de la plantilla se convierte en la fecha planificada de finalización del futuro proyecto. </p></li> 
       </ul><p>Para obtener más información sobre los días de inicio y finalización de las tareas de plantilla, consulte <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Información general sobre los días de inicio y finalización de una plantilla</a>. </p><p>La configuración Programar a partir de las plantillas es similar a la de los proyectos. El administrador de Workfront selecciona la configuración predeterminada Programar desde para los proyectos del sistema. Para obtener información sobre cómo establecer los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p></td> 
       </tr>

   <tr> 
         <td role="rowheader"><strong>Portafolio</strong></td> 
         <td><p>Especifique un Portfolio para los proyectos creados a partir de esta plantilla. Primero debe crear un Portfolio para que aparezca en la lista desplegable. </p><p>En la lista solo se muestran los portafolios activos. Para obtener más información sobre la creación de portafolios, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Crear un portafolio </a>.</p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Programar</strong></td> 
         <td><p>Si seleccionó un Portfolio para la plantilla, especifique un <strong>Programa</strong> para el proyecto futuro. Es posible que algunos Portfolio no tengan programas. Primero debe crear un programa, antes de que aparezca en esta lista desplegable. En la lista solo se muestran los programas activos.</p><p>Para obtener más información sobre la creación de programas, consulte <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Creación de un programa</a>.</p></td> 
       </tr>  
       <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
         <td role="rowheader"><strong>Grupo</strong></td> 
         <td><p>En la lista desplegable, seleccione el grupo que desea asociar con los proyectos creados a partir de la plantilla. Puede ser un grupo de cualquier nivel. </p><p>Puede asegurarse de que está seleccionando el grupo correcto pasando el puntero sobre él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a ella. Se muestra información de objeto sobre el grupo, como la jerarquía de grupos por encima y sus administradores.</p> <p><b>NOTAS</b>

   <ul> 
       <li><p>En el área Proyectos de la página de un grupo, cuando alguien crea un proyecto con una plantilla que no tiene un grupo seleccionado, el sistema asocia el grupo abierto actualmente con el proyecto.</p><p>Esto es diferente a otras áreas en las que el sistema asocia el grupo de inicio de un usuario con el proyecto cuando el usuario crea el proyecto mediante una plantilla que no tiene un grupo seleccionado.</p></li> 
       <li><p>Si un usuario selecciona una plantilla que tiene un grupo seleccionado al crear un proyecto (o al convertir una tarea o un problema en un proyecto), el usuario puede elegir un grupo diferente para el proyecto.</p></li> 
       <li>Aunque este campo solo está disponible en plantillas en la nueva experiencia de Adobe Workfront, puede verlo en listas e informes tanto allí como en Adobe Workfront Classic. </li> 
         </ul> </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Compañía</strong></td> 
         <td><p>Especifique la Empresa que desea asociar con la plantilla. En la lista solo se muestran las empresas activas.</p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Propietario de plantilla</strong></td> 
         <td><p>El usuario designado como Propietario de la plantilla debe ser un usuario activo de Workfront. </p><p>Tenga en cuenta lo siguiente sobre el usuario designado como propietario de la plantilla: </p> 
         <ul> 
         <li>Se les otorgan automáticamente permisos de administración en la plantilla. </li> 
         <li>Se añaden al equipo del proyecto y se les otorgan automáticamente permisos de Administración al proyecto creado a partir de la plantilla. </li> 
         <li>Se convierten en Propietario del proyecto cuando el proyecto se crea a partir de esta plantilla. </li> 
         <li> Si el usuario designado como Propietario de la plantilla tiene acceso limitado a las plantillas o proyectos desde su nivel de acceso, sus permisos de Administración en la plantilla y en los proyectos estarán limitados. Por ejemplo, si solo tienen acceso de visualización para plantillas o proyectos en su nivel de acceso, recibirán automáticamente permisos de visualización en la plantilla y el proyecto cuando se designen como Propietario de la plantilla.</li>
         </ul></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Patrocinador de plantilla</strong></td> 
         <td><p>El usuario especificado en este campo se convierte en patrocinador del proyecto cuando la plantilla se agrega al proyecto. Este usuario se añade al equipo del proyecto y se le conceden automáticamente permisos de visualización para el proyecto. El usuario designado como patrocinador de la plantilla debe ser un usuario activo de Workfront. </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Gerente de recursos</strong></td> 
         <td><p>A los usuarios especificados se les otorgan automáticamente permisos de administración en los proyectos futuros y pueden asignar recursos a las tareas y problemas de los proyectos. Puede especificar más de un gerente de recursos. </p></td> 
       </tr> 
      </table>

1. (Opcional) Siga editando las secciones siguientes, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Finanzas {#finance-preview}

1. Empiece a editar la plantilla como se ha descrito anteriormente.
1. En el **Editar plantilla** , haga clic en **Finanzas**.

   ![](assets/edit-template-box-finance-section.png)

1. Actualice los campos siguientes:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody>
       <tr> 
         <td role="rowheader"><strong> Divisa</strong></td> 
         <td><p>Especifique la moneda para el proyecto futuro, si es diferente a la moneda predeterminada del sistema. Este campo no está visible si solo tiene la moneda predeterminada en el sistema.<br>Para obtener más información sobre la divisa, consulte <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tasas de cambio</a>.</p></td> 
       </tr>
       <tr> 
       <td role="rowheader"><strong>Presupuesto</strong></td> 
       <td><p>Especifique un presupuesto para los proyectos creados a partir de esta plantilla.</p></td> 
       </tr>  
       <tr> 
         <td role="rowheader"><strong>Método de índice de rendimiento</strong></td> 
         <td><p>Elija cómo calculará Workfront las métricas de valor ganado del proyecto futuro. Elija entre las siguientes opciones:
         <ul>
         <li>Basado en horas</li>
         <li>Basado en costos</li>
         </ul>

   Para obtener más información sobre el método de índice de rendimiento, consulte <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Establecer el método de índice de rendimiento (PIM)</a>. </p></td>
   </tr> 
         <tr> 
         <td role="rowheader"><strong>Beneficio planificado</strong></td> 
         <td><p>Especifique el beneficio planificado de los proyectos que se crean a partir de esta plantilla. El beneficio planificado se utiliza en el caso comercial del proyecto y en Portfolio Optimizer. </p><p>Para obtener más información sobre el beneficio planificado de un proyecto, consulte <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Visión General de Beneficio Planificado del Proyecto</a>. El beneficio planificado de un proyecto se tiene en cuenta cuando se calcula el valor neto de un proyecto. </p><p>Para obtener más información sobre el uso de Portfolio Optimizer, consulte <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Administrar proyectos en Portfolio Optimizer</a> </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Coste fijo</strong></td> 
         <td><p>Especifique el Coste fijo para los proyectos creados a partir de esta plantilla. Esto es diferente al costo de mano de obra que proviene de las horas en el proyecto y al costo de gasto que proviene de la cantidad de gastos en el proyecto. El costo fijo de un proyecto se tiene en cuenta al calcular su valor neto y forma parte del costo presupuestado.</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Ingresos fijos</strong></td> 
       <td><p>Especifique los ingresos fijos para los proyectos creados a partir de esta plantilla.</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Requerir tiempo de aprobación de este proyecto</strong></td> 
       <td><p>Seleccione esta opción para solicitar al propietario del proyecto del futuro proyecto creado a partir de esta plantilla que apruebe el tiempo de registro en el proyecto. Si está utilizando Registros de facturación y selecciona esta opción, solo las horas aprobadas en el proyecto aparecen como horas facturables disponibles para los Registros de facturación. La aprobación de las horas en el proyecto es independiente de la aprobación de plantillas de horas. Para obtener más información sobre cómo requerir tiempo para aprobarse en un proyecto, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Requerir tiempo de aprobación de un proyecto</a>.</p></td> 
       </tr> 
       </tbody> 
      </table>

1. (Opcional) Siga editando las secciones siguientes, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Formularios personalizados {#custom-forms-preview}

1. Empiece a editar la plantilla como se ha descrito anteriormente.
1. En el **Editar plantilla** , haga clic en **Forms personalizado**.

   ![](assets/edit-template-box-custom-forms-section.png)

   Los nombres de los formularios personalizados que ya están adjuntos a la plantilla se muestran en el panel izquierdo.

1. Haga clic dentro de **Añadir formulario personalizado** y seleccione el formulario o formularios personalizados que desee asociar a la plantilla. Debe crear los formularios personalizados antes de que estén disponibles para seleccionarlos en este campo.

   En la lista solo se muestran los formularios personalizados activos. Para obtener más información sobre la creación de formularios personalizados, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   Puede agregar hasta diez formularios personalizados a una plantilla.

   Los formularios se agregarán al proyecto creado a partir de esta plantilla.

1. (Opcional) Actualice la información en cualquiera de los campos de los formularios personalizados. La información se transferirá a los proyectos que se crearán a partir de la plantilla.

1. (Opcional) Haga clic en **x** a la derecha del nombre de un formulario personalizado y haga clic en **Eliminar** para eliminarlo de la plantilla.

1. (Opcional) Siga editando la sección siguiente, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Configuración de proyecto {#project-settings}

1. Empiece a editar la plantilla como se ha descrito anteriormente.
1. En el **Editar plantilla** , haga clic en **Configuración de proyecto**.

   ![](assets/edit-template-box-project-settings-section.png)

1. Actualice los campos siguientes:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
       <td role="rowheader"><strong>Ruta de hitos</strong> </td> 
       <td> <p>Seleccione una Ruta de hitos para la plantilla. En la lista solo se muestran las trayectorias de hitos activas.<br>Para obtener más información sobre las Rutas de hitos, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Creación de una trayectoria del hito</a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Modo de finalización</strong> </td> 
         <td> <p>Controla la manera en que el futuro proyecto se marcará como Completo. <br>Seleccione entre las siguientes opciones:</p> 
         <ul> 
         <li> <p><strong>Automático</strong>: el proyecto se marca como Completado cuando se completan todas las tareas y problemas.</p> </li> 
         <li> <p><strong>Manual</strong>: debe seleccionar manualmente el estado Completo del proyecto cuando se hayan completado todas las tareas y problemas. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Modo de finalización de resumen</strong> </td> 
       <td> <p>Controla la manera en que las tareas principales del futuro proyecto se marcan como Completadas. <br>Seleccione entre las siguientes opciones:</p> 
       <ul> 
       <li> <p><strong>Automático</strong>: las tareas principales se marcan como Completadas y actualizan el porcentaje completado automáticamente, a medida que se completan las tareas secundarias y se actualiza el porcentaje completado de las tareas secundarias. </p> </li> 
       <li> <p><strong>Manual</strong>: Debe actualizar manualmente el porcentaje completado y el estado de las tareas principales, independientemente de los cambios realizados en las tareas secundarias. </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Tipo de actualización</strong> </td> 
         <td> <p>Controla cuándo se guardan en el proyecto los cambios realizados en la escala de tiempo del futuro proyecto. </p> 
         <b>EJEMPLO </b> 
         <p>Los siguientes cambios en el déclencheur del proyecto pueden actualizar la cronología del proyecto:</p> 
         <ul> 
         <li> <p>actualizar las fechas de las tareas</p> </li> 
         <li> <p>cambiar relaciones de predecesoras<br></p> </li> 
         <li> <p>cambiar relaciones principal-secundario</p> </li> 
         <li> <p>agregar o quitar asignaciones además de cambiar la restricción de tarea o el tipo de duración.</p> </li> 
         </ul> 
         </div> <p>Seleccione entre las siguientes opciones:<br></p> 
         <ul> 
         <li> <p><strong>Automático y al cambiar</strong> (Configuración predeterminada): La escala de tiempo del proyecto futuro se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la escala de tiempo (Al cambiar). La cronología del proyecto también se actualiza cada noche (Automática).<br>Esta es la configuración recomendada para este campo porque garantiza que la cronología del proyecto siempre esté actualizada.<br>Cuando realiza una acción en una tarea o proyecto que almacena en déclencheur un cálculo de escala de tiempo, todas las fechas disponibles se muestran inmediatamente, lo que le permite continuar trabajando. En los proyectos con más de 100 tareas, las fechas que requieran recalculaciones más largas se muestran brevemente como signo de interrogación (entre 1 y 5 segundos, o hasta un minuto en los proyectos grandes). Esto indica que el cálculo aún no ha finalizado y que las fechas están sujetas a cambios.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Cambiar solo</strong>: la cronología del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la cronología. Es posible que desee seleccionar esta opción si los cambios rara vez se producen en el proyecto o en otros proyectos de los que depende la escala de tiempo.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Solo automático</strong>: la cronología del proyecto se actualiza cada noche; no se actualiza inmediatamente después de realizar cambios.<br>Es posible que desee seleccionar esta opción si se producen muchos cambios cada día en el proyecto o en otros proyectos de los que depende la escala de tiempo. Sin embargo, tenga en cuenta que ha elegido esta configuración, ya que el proyecto no se actualizará al mismo tiempo que se realizan los cambios.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Solo manual</strong>: la cronología del proyecto solo se actualiza cuando selecciona la opción Recalcular cronologías, tal como se describe en <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalcular escalas de tiempo del proyecto</a>.<br></p> </li> 
         </ul> <p>Es posible que desee seleccionar esta opción si realiza muchos cambios en el proyecto al mismo tiempo y desea que el cálculo de la escala de tiempo se produzca después de realizar todos los cambios (en lugar de después de cada cambio individual).</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Programación</strong> </td> 
         <td> <p>Seleccione una programación para la plantilla. Esto se convertirá en la programación del proyecto que se crea a partir de esta plantilla. Debe ser la misma programación asignada a la mayoría de las personas que trabajan en el proyecto. Debe crear una programación para poder asignarla a una plantilla.<br>Para obtener más información sobre la creación de programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creación de una programación</a>. <br>Si no ha creado programaciones personalizadas en el sistema, se seleccionará la Programación predeterminada. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Tiempo libre del usuario</strong> </td> 
         <td> <p>Determina si el tiempo libre de la persona asignada principal de una tarea ajusta las fechas planificadas de la tarea. Cuando adjunta la plantilla a un proyecto existente y la plantilla tiene una configuración para este campo diferente a la del proyecto, la configuración del proyecto permanece sin cambios. La opción predeterminada para esta configuración para una plantilla nueva es la misma que la preferencia de proyecto del sistema. </p> <p>Para obtener información sobre las preferencias del proyecto en el nivel de sistema, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>. </p> <p>Para obtener información sobre cómo afecta esta configuración a las fechas de las tareas de un proyecto, consulte <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar proyectos</a>.<br>Seleccione entre las siguientes opciones:<br></p> 
         <ul> 
         <li> <p><strong>Considere el tiempo libre del usuario en las duraciones de tareas</strong>: Al seleccionar esta opción, las fechas planificadas de las tareas del proyecto creadas a partir de esta plantilla se ajustan según el tiempo de espera de la persona asignada principal de la tarea, si el tiempo de espera se produce durante la duración de la tarea. </p> </li> 
         <li> <p><strong>Omitir tiempo libre del usuario en duraciones de tareas</strong>: Al seleccionar esta opción, las fechas planificadas de las tareas del proyecto creadas a partir de esta plantilla permanecen tal y como se planificaron originalmente, incluso si la persona asignada principal de la tarea tiene tiempo libre durante la duración de la tarea. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Modo de nivelación de recursos</strong> </td> 
         <td> <p>Seleccione entre las siguientes opciones:<br></p> 
         <ul> 
         <li> <p><strong>Manual</strong>: debe nivelar manualmente los recursos en el proyecto creado a partir de esta plantilla (esta es la configuración predeterminada)</p> </li> 
         <li> <p><strong>Automático:</strong> Workfront nivela los recursos en el proyecto futuro. <br>Para obtener más información sobre la nivelación de recursos, consulte <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Nivelar recursos en el gráfico Gantt </a>. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Riesgo</strong> </td> 
         <td> <p>Defina el nivel de riesgo de los proyectos creados a partir de esta plantilla. El riesgo es solo un indicador de lo riesgoso que puede ser un proyecto. Puede priorizar la ejecución de sus proyectos en función del nivel de riesgo.<br>Considere la posibilidad de seleccionar entre los siguientes niveles de riesgo:<br></p> 
         <ul> 
         <li> <p><strong>Muy baja</strong> </p> </li> 
         <li> <p><strong>Baja</strong> </p> </li> 
         <li> <p><strong>Mediana</strong> </p> </li> 
         <li> <p><strong>Alta</strong> </p> </li> 
         <li> <p><strong>Muy alto</strong> </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Conjuntos de recursos</strong> </td> 
         <td> <p>Especifique los conjuntos de recursos asociados a la plantilla. Los conjuntos de recursos son conjuntos de usuarios que se necesitan al mismo tiempo para completar un proyecto. Para obtener más información sobre los conjuntos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resumen de conjuntos de recursos </a>.</p> <p> <p><b>NOTA</b>

   Cuando edita las plantillas de forma masiva, solo aparecen en este campo los conjuntos de recursos que son comunes a todas las plantillas seleccionadas. Si las plantillas seleccionadas no tienen conjuntos de recursos compartidos, este campo estará vacío. Los conjuntos de recursos que especifique aquí sobrescribirán los conjuntos de recursos individuales de las plantillas.</p> </p> </td>
   </tr>
       <tr> 
         <td role="rowheader"><strong>Filtrar tipo de horas</strong> </td> 
         <td> <p>Tenga en cuenta lo siguiente:</p> <p>Seleccionar <strong>No</strong> para que todos los tipos de horas específicos del proyecto estén disponibles en el proyecto futuro. (Esta es la selección predeterminada)</p> <p>O</p> <p>Seleccionar <strong>Sí</strong> para que solo un subconjunto de los tipos de horas específicos del proyecto esté disponible en el proyecto futuro, seleccione los tipos de horas que desee poner a disposición. (Mantenga pulsada la tecla Mayús para seleccionar varios tipos de horas).</p> <p>Si selecciona esta opción, solo estarán disponibles para seleccionarlos los tipos de horas que seleccione al registrar horas en el proyecto (o en tareas y problemas dentro del proyecto). Debe seleccionar al menos un tipo de hora; si selecciona esta opción y no selecciona ningún tipo de hora, todos los tipos de horas estarán disponibles en el proyecto.</p> <p>Las mismas selecciones de tipo de hora deben realizarse en el nivel de usuario individual para que el usuario pueda ver estas opciones de tipo de hora en el proyecto. </p> <p>Para obtener más información sobre la definición de tipos de horas en el nivel de usuario, consulte la sección <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Registrar tiempo</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Registrar tiempo</a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Proceso de aprobación</strong> </td> 
         <td> <p>Seleccione el proceso de aprobación que desea asociar con la plantilla. El administrador de Workfront o un usuario con acceso administrativo a los procesos de aprobación deben definir los procesos de aprobación de proyectos de nivel de sistema o de grupo para poder asociarlos a una plantilla. Para obtener más información sobre la creación de procesos de aprobación, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Crear un proceso de aprobación para elementos de trabajo</a>.</p> <p>Tenga en cuenta lo siguiente al añadir procesos de aprobación: </p> 
         <ul> 
         <li>En la lista solo se muestran los procesos de aprobación activos. </li> 
         <li> <p>Los procesos de aprobación de todo el sistema y específicos del grupo se muestran en la lista. Un proceso de aprobación asociado a un grupo que no sea el de la plantilla no se muestra en la lista.</p> <p><b>IMPORTANTE</b>

   Si el grupo asociado a la plantilla cambia, el proceso de aprobación específico del grupo se convierte en un proceso de aprobación de un solo uso. Para obtener más información sobre cómo afectan los cambios en el grupo del proyecto o los cambios en el proceso de aprobación a la configuración de aprobación, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Cómo afectan los cambios en los procesos de aprobación y de grupo a los procesos de aprobación asignados</a>. </p> </li>
   <li> <p>Si agregó un proceso de aprobación de un solo uso, se mostrará como "Personalizado" en este campo. Para obtener más información, consulte <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Asociar un proceso de aprobación nuevo o existente con el trabajo</a>. </p> 
         </li> 
         <li> <p>Cuando se editan plantillas por lotes, existen los siguientes escenarios:</p> 
         <ul> 
            <li> <p>Al seleccionar plantillas del mismo grupo, en este campo se muestran tanto los procesos de aprobación de nivel de sistema como los de nivel de grupo.</p> </li> 
            <li> <p>Al seleccionar plantillas de diferentes grupos, solo se muestran en este campo los procesos de aprobación de nivel de sistema.</p> </li> 
            <li> <p>Cuando alguna de las plantillas tiene un proceso de aprobación de un solo uso adjunto, se reemplaza por el nivel de sistema que seleccione. </p> </li> 
         </ul> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Notificación de recordatorio</strong> </td> 
         <td>Seleccione la notificación de recordatorio que debe asociarse al proyecto futuro. Debe configurar las notificaciones de recordatorio de los proyectos para que este campo aparezca durante la edición de una plantilla. <br>Para obtener más información sobre la configuración de notificaciones de recordatorio, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configuración de notificaciones de recordatorio</a>.</td> 
       </tr> 
       </tbody> 
      </table>

1. (Opcional) Siga editando las secciones siguientes, según la información que desee modificar.\
   O
1. Haga clic en **Guardar**.

### Configuración de tarea {#task-settings}

Puede definir los valores predeterminados que se asociarán a todas las tareas nuevas cuando las agregue a un proyecto que se cree a partir de la plantilla.

Para obtener información sobre cómo afectan estos ajustes a la creación de nuevas tareas, consulte [Información general sobre Crear tareas](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Empiece a editar la plantilla como se ha descrito anteriormente.
1. En el **Editar plantilla** , haga clic en **Configuración de tarea**.

   ![](assets/edit-template-box-tax-settings-section.png)

1. En el **Proceso predeterminado de aprobación de tarea** , seleccione el Proceso de aprobación que desea asociar con todas las tareas nuevas cuando las agregue a un proyecto creado a partir de esta plantilla. Debe crear un Proceso de aprobación para las tareas antes de poder asociarlo a las tareas. En la lista solo se muestran los procesos de aprobación activos. Para obtener más información sobre la creación de procesos de aprobación, consulte [Creación de procesos de aprobación](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. En el **Forms personalizado predeterminado de tarea** , seleccione el formulario o formularios personalizados que desee asociar con todas las tareas nuevas cuando los agregue a un proyecto creado a partir de esta plantilla. Debe crear los formularios personalizados antes de que estén disponibles para seleccionarlos en este campo. En la lista solo se muestran los formularios personalizados activos. Para obtener más información sobre la creación de formularios personalizados, consulte [Crear Forms personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Puede asociar hasta diez formularios personalizados a una tarea.
1. (Opcional) Seleccione **Utilizar Esfuerzo de trabajo para calcular automáticamente las horas planificadas para la tarea** si desea habilitar la administración del esfuerzo de la tarea mediante el uso de Esfuerzo de trabajo en lugar de Horas planificadas en el proyecto creado a partir de la plantilla.
1. (Condicional y opcional) Si seleccionó Usar esfuerzo de trabajo para calcular automáticamente las horas planificadas para la tarea, haga clic en el menú desplegable para actualizar el porcentaje de cada nivel de esfuerzo de trabajo. Los siguientes valores de porcentaje son los predeterminados:

   | Nivel de esfuerzo de trabajo | Valor porcentual |
   |---|---|
   | Pequeño | 25 % |
   | Media | 50 % |
   | Grande | 75 % |

   Para obtener información sobre el uso de Esfuerzo de trabajo para administrar el esfuerzo en tareas en proyectos, consulte [Resumen de esfuerzo de trabajo](../../../manage-work/tasks/task-information/work-effort.md).

1. (Opcional) Siga editando la sección siguiente, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Configuración de problema {#issue-settings}

Al editar la configuración de problemas, puede evitar que los usuarios agreguen problemas en línea en el futuro proyecto creado a partir de la plantilla.

1. Empiece a editar la plantilla como se ha descrito anteriormente.
1. En el **Editar plantilla** , haga clic en **Configuración de problema**.

   ![](assets/edit-template-box-issue-settings-section.png)

1. (Opcional) Anule la selección del **Permitir que los usuarios agreguen problemas en línea** opción. Está activada de forma predeterminada.

   Al deshabilitar esta opción, los usuarios no pueden agregar problemas en línea al proyecto o a las tareas de la sección Problemas, cuando el proyecto se crea a partir de la plantilla.

   >[!TIP]
   >
   >Deshabilite esta opción si desea obligar a los usuarios a rellenar los campos de nuevo problema o los formularios personalizados asociados a nuevos problemas.

   Al deshabilitar esta opción, los usuarios con permisos para agregar problemas al proyecto creado a partir de la plantilla pueden hacerlo utilizando el botón Nuevo problema o una cola de solicitudes asociada al proyecto.

   Para obtener más información sobre la configuración de problemas en proyectos, consulte la [Configuración de problema](../../../manage-work/projects/manage-projects/edit-projects.md#issue) en el artículo [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

   Para obtener información sobre la creación de problemas en proyectos, consulte [Crear problemas](../../../manage-work/issues/manage-issues/create-issues.md).

1. (Opcional) Siga editando la sección siguiente, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Acceso {#access-preview}

1. Empiece a editar la plantilla como se ha descrito anteriormente.
1. En el **Editar plantilla** , haga clic en **Acceso**.

   ![](assets/edit-template-box-access-section.png)

   El acceso que especifique para la plantilla se convertirá en el acceso de los usuarios asociados al proyecto cuando la plantilla se utilice para crear un proyecto.

   Especifique lo siguiente **Acceso** información para la plantilla:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
         <td role="rowheader"><strong>Cada vez que se asigne a una persona a una tarea</strong> </td> 
         <td> <p>Seleccionar de <strong>Ver</strong>, <strong>Aportar,</strong> o <strong>Administrar</strong> acceso a una tarea. Al usuario asignado a una tarea se le concede automáticamente este acceso. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Conceder también acceso al proyecto</strong> </td> 
         <td> <p> Seleccionar de <strong>Ver</strong>, <strong>Contribute</strong>, o <strong>Administrar</strong> acceso al proyecto. Al usuario asignado a una tarea se le concede automáticamente este acceso al proyecto. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Cada vez que se asigne a una persona a un problema</strong> </td> 
         <td> <p>Seleccionar de <strong>Ver</strong>, <strong>Aportar,</strong> o <strong>Administrar</strong> acceso a un problema. Al usuario asignado a un problema se le concede automáticamente este acceso. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Conceder también acceso al proyecto</strong> </td> 
         <td> <p> Seleccionar de <strong>Ver</strong>, <strong>Contribute</strong>, o <strong>Administrar</strong> acceso al proyecto. Al usuario asignado a un problema se le concede automáticamente este acceso al proyecto. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Cada vez que alguien envíe una solicitud: Conceder acceso</strong> </td> 
         <td> <p> Seleccionar de <strong>Ver</strong>, <strong>Contribute</strong>, o <strong>Administrar</strong> acceso a la solicitud. Cuando envían una solicitud al proyecto, se les concede este acceso a la solicitud que han enviado. Para obtener más información, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Las personas de la misma compañía heredarán los mismos permisos en todas las solicitudes</strong> </td> 
         <td> <p>Seleccione este campo si desea que las personas de la misma compañía tengan el mismo acceso a todas las solicitudes del proyecto, tanto si las han enviado como si no.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Cada vez que alguien reciba acceso a este proyecto: Conceda acceso a...</strong> </td> 
         <td> <p>Seleccione las opciones de acceso que desea que tengan los usuarios en el proyecto, si el proyecto se comparte con ellos. Seleccione las opciones específicas para su acceso, si están designadas como <strong>Espectadores</strong>, <strong>Colaboradores</strong>, o <strong>Responsables</strong> al compartir el proyecto con ellos. </p> </td> 
       </tr> 
       </tbody> 
      </table>

1. (Opcional) Siga editando las secciones siguientes, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

   Los cambios se enviarán para esta plantilla.

   Ahora, cuando utilice esta plantilla para crear un proyecto, todos estos ajustes se transferirán al nuevo proyecto.


## Edición de plantillas por lotes

Puede editar las plantillas de forma masiva y actualizar toda su información al mismo tiempo.

Para editar plantillas de forma masiva:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Clic **Plantillas**.
1. Seleccione varias plantillas en la lista.
1. Clic **Editar**.

   El **Editar plantillas** se abre el cuadro de diálogo.

   ![](assets/edit-templates-in-bulk-box-nwe-350x327.png)

1. Haga clic en las secciones de la izquierda para editar todas las plantillas seleccionadas.

   Para obtener más información sobre la edición de información en plantillas, consulte la [Edición de una plantilla](#edit-a-template) de este artículo.

1. Haga clic en **Guardar cambios**.

   Todos los cambios realizados ahora están visibles en todas las plantillas seleccionadas.

## Adición de tareas a una plantilla

Una vez creada la plantilla y editada la información de la plantilla, puede agregarle tareas.

Agregar tareas a una plantilla es similar a agregar tareas a un proyecto.

Para obtener más información sobre cómo agregar tareas a un proyecto, consulte [Creación de tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Cuando se agregan tareas a una plantilla, la Duración de la plantilla y los Días de inicio y finalización de la plantilla cambian en consecuencia. Para obtener información sobre los días de inicio y finalización de la plantilla y de las tareas de plantilla, consulte [Información general sobre los días de inicio y finalización de una plantilla](../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md).

## Adición de elementos adicionales a una plantilla

Una vez creada la plantilla y editada su información, puede agregarle más elementos. Los elementos que agregue estarán disponibles para el proyecto cuando lo esté creando a partir de la plantilla.

Añadir los siguientes elementos a una plantilla es idéntico a agregarlos a un proyecto:

* Documentos
* Riesgos

  Para obtener más información sobre la creación de riesgos, consulte la [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md#create)  en el artículo [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

* Procesos de aprobación

  Para obtener información sobre cómo asociar procesos de aprobación con trabajo, consulte [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

* Tarifas de facturación

  Para obtener más información sobre la anulación de tarifas de facturación para un proyecto, consulte [Resumen de anulación de Tarifas de facturación de rol y cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Gastos

  Para obtener más información sobre cómo agregar gastos, consulte [Administrar gastos del proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Grupos de temas y temas de colas

  Para obtener más información sobre cómo agregar grupos de temas y temas de colas a un proyecto o plantilla, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Puede agregar los siguientes elementos a las tareas de la plantilla:

* Documentos
* Gastos

  Para obtener más información sobre cómo agregar gastos, consulte [Administrar gastos del proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Rutas de aprobación

  Para obtener más información sobre cómo asociar aprobaciones con trabajo, consulte [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).


## Activar o desactivar una plantilla

Puede desactivar una plantilla si desea que los usuarios no puedan encontrarla y crear proyectos a partir de ella. No puede adjuntar una plantilla desactivada a proyectos ni utilizarla para crear un proyecto.

Las plantillas desactivadas no afectan a los proyectos existentes creados con ellas.

Para desactivar una plantilla:

1. Vaya a una plantilla activa y haga clic en **Más** ![](assets/qs-more-icon-on-an-object.png) junto al nombre de la plantilla y haga clic en **Desactivar**.

   ![](assets/deactivate-template-link-in-more-menu.png)

   La plantilla ya no está activa y los usuarios ya no pueden encontrarla para crear proyectos a partir de ella.
1. (Opcional) Para activar la plantilla, haga clic en **Más** ![](assets/qs-more-icon-on-an-object.png) junto al nombre de la plantilla y haga clic en **Activar**.

   La plantilla ahora está activa y se puede adjuntar a proyectos o utilizar para crear proyectos.

