---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Introducción a la administración de recursos
description: La administración de recursos le permite configurar el sistema para prever con precisión el uso de los recursos en función de su disponibilidad, de modo que el trabajo que se debe realizar se complete a tiempo y según el presupuesto.
author: Lisa
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: a9d507bfcc0a602e71bcdd3142d63cc40175ebf4
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 0%

---

# Introducción a la administración de recursos

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

La administración de recursos le permite configurar el sistema para prever con precisión el uso de los recursos en función de su disponibilidad, de modo que el trabajo que se debe realizar se complete a tiempo y según el presupuesto.

## Información general sobre la administración de recursos en Adobe Workfront

Administración de recursos hace referencia a todas las actividades realizadas por el administrador de Adobe Workfront, el administrador de recursos y el propietario del proyecto para planificar (planificación de recursos o escenarios) y programar (Distribuidor de cargas de trabajo) los recursos de una organización y asignarlos al trabajo que se debe realizar, teniendo en cuenta su disponibilidad. Además, la administración de recursos también hace referencia a la visualización de información sobre las asignaciones de recursos planificadas y reales en una vista de informe (informe de utilización).

Workfront tiene varios conjuntos de herramientas para administrar recursos. Cada herramienta tiene un ámbito individual. Actualmente, puede utilizar las siguientes herramientas de administración de recursos en Workfront, según la etapa de administración de recursos en la que se encuentre:

* Para planificar cómo se asignan los recursos a un nivel superior, antes de que comience el trabajo real en los proyectos, utilice las siguientes herramientas:

   * **El Planificador de recursos**: puede usar el Planificador de recursos en la primera etapa de la administración de recursos para presupuestar el tiempo de proyecto de los recursos según su disponibilidad programada. Durante la fase de planificación de los recursos, puede organizar a los usuarios en conjuntos de recursos y asignar varios conjuntos de recursos a un proyecto.

     Para obtener más información acerca de Planificación de recursos, vea [Planificación de recursos: índice de artículo](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **El planificador de escenarios**: se trata de una planificación de recursos de nivel superior que le permite administrarlos en varias iniciativas que pueden abarcar un plan de uno, tres o cinco años e incluir varios proyectos. Puede utilizar el mejor escenario para aprovechar al máximo su disponibilidad y su presupuesto.

     El Scenario Planner requiere una licencia independiente, además de la licencia de Workfront. Para obtener información sobre el Scenario Planner de Workfront, consulte [Información general sobre el Scenario Planner](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* Para programar o asignar recursos a trabajo real (tareas y problemas), utilice la siguiente herramienta:

   * **Distribuidor de cargas de trabajo**: pertenece a una etapa de nivel inferior de la administración de recursos, en la que puede asignar los recursos al trabajo real (tareas y problemas) que deben completar, según la cantidad de horas necesarias para completarlos y su disponibilidad. Con el Distribuidor de cargas de trabajo, puede asignar usuarios a trabajo real que no esté asignado o asignado a roles actualmente.

     Para obtener información acerca del Distribuidor de cargas de trabajo de Workfront, consulte [El Distribuidor de cargas de trabajo: índice de artículos](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Para analizar las asignaciones presupuestadas, planificadas y reales en varios proyectos, utilice la siguiente herramienta:

   * **Informe de utilización**: Use este informe para ver la utilización de los recursos de los proyectos. Puede comparar las asignaciones presupuestadas, planificadas y reales de los proyectos y su impacto en el coste y en los ingresos.

     Para obtener información sobre el informe de utilización, vea [Ver información sobre la utilización de los recursos](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Los componentes del proceso de gestión de recursos

>[!NOTE]
>
>La administración de recursos nunca es un proceso estancado en Workfront. A medida que cambian las programaciones de los proyectos, la disponibilidad de los usuarios o sus funciones, debe ajustar continuamente la información sobre los recursos, sus asignaciones y sus asignaciones a los proyectos, tareas y problemas.

El proceso de administración de recursos en Workfront incluye las siguientes etapas:

* **Configuración**: como administrador del sistema, administrador de recursos o propietario del proyecto, debe configurar ciertos campos y objetos en la instancia de Workfront antes de administrar los recursos. Para obtener más información sobre los requisitos previos necesarios para empezar a administrar recursos en Workfront, consulte la sección [Requisitos previos para una administración precisa de los recursos](#prerequisites-for-accurate-resource-management) en este artículo.\
  Además de tener proyectos con elementos de trabajo, debe configurar los siguientes elementos en Workfront:

   * Usuarios\
     Para obtener más información acerca de cómo crear usuarios, vea el artículo [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * Roles\
     Para obtener más información sobre cómo crear roles, consulte el artículo [Crear y administrar roles](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * Horarios\
     Para obtener más información acerca de cómo crear programaciones, vea el artículo [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * Preferencias de proyecto

     >[!TIP]
     >
     >Solamente un administrador de sistema o de grupo puede modificar las Preferencias del proyecto para su sistema o para su grupo.

     Para obtener más información acerca de la definición de Preferencias de proyecto, vea el artículo [Configurar las preferencias de proyecto de todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * Conjuntos de recursos

     Para obtener más información acerca de cómo crear conjuntos de recursos, vea [Crear conjuntos de recursos](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * Preferencias de administración de recursos

     Como sistema, debe decidir cómo calcula Workfront la disponibilidad de los usuarios en el nivel del sistema, ya sea mediante la programación del usuario o mediante la programación predeterminada del sistema.

     Para obtener más información, consulte [Configurar las preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Asignación de recursos**: como administrador de recursos o propietario de un proyecto, puede definir la asignación de recursos para sus proyectos, así como asignar trabajo. Para este paso, puede administrar la estimación de la asignación de los recursos mediante el Planificador de recursos o el Planificador de escenarios, y asignar el trabajo real a los usuarios en el Distribuidor de cargas de trabajo.

  Para obtener más información sobre la planificación de recursos y la asignación de trabajo, vea las secciones siguientes:

   * [Planificación de recursos: índice de artículos](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Planificador de escenarios de Adobe Workfront](../../scenario-planner/scenario-planning.md)
   * [Índice de artículos del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Workload Balancer overview](../workload-balancer/overview-workload-balancer.md). 
-->

* **Análisis**: como gerente de recursos, propietario de proyecto o gerente de personas, revise el informe de utilización para comprender cómo se comparan las asignaciones presupuestadas y planificadas de sus recursos con las asignaciones reales. Revise la información por horas, coste o ingresos. Para obtener información acerca del informe Utilización, vea [Ver información sobre la utilización de los recursos](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Acceso necesario para ver y administrar los recursos mediante las herramientas de administración de recursos de Workfront

Los siguientes usuarios tienen acceso a las herramientas de administración de recursos de Workfront:

Debe ser uno de los siguientes usuarios y tener los siguientes permisos y acceso a las herramientas de administración de recursos:

* El administrador del sistema.
* Un usuario con una licencia estándar o de planificación.

  Un usuario con una licencia de trabajo puede utilizar el Distribuidor de cargas de trabajo de un proyecto y administrar asignaciones y asignaciones.

  Además de tener una licencia de trabajo o superior (o una licencia estándar), debe tener lo siguiente para utilizar herramientas específicas de administración de recursos:

   * Editar el acceso a la administración de recursos (no es necesario para realizar asignaciones en el Distribuidor de cargas de trabajo)
   * Editar acceso a datos financieros para mostrar información de costos en el Planificador de recursos
   * Consulte el acceso a los datos financieros para ver la información de costes e ingresos en el informe Utilización (sólo usuarios con licencia de planificación)

* Permisos de Contribute o superiores que incluyen Realización de asignaciones en los proyectos para los que desea administrar recursos.

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

Para obtener información sobre el acceso necesario para presupuestar recursos, consulte el artículo [Acceso necesario para presupuestar recursos](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Para obtener información sobre el acceso necesario para administrar recursos en el Distribuidor de cargas de trabajo, consulte [Acceso necesario para administrar recursos en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Requisitos previos para una administración precisa de los recursos  {#prerequisites-for-accurate-resource-management}

Debe cumplir una serie de requisitos para poder utilizar de forma eficaz las herramientas de administración de recursos de Workfront.

Para obtener información sobre los requisitos de cada herramienta de administración de recursos en Workfront, consulte lo siguiente:

* La sección [Requisitos previos para trabajar en el Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) del artículo [Información general del Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
* La sección [Prácticas recomendadas para usar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) del artículo [Información general del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Acceso necesario para presupuestar recursos en Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Acceso necesario para administrar recursos en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
