---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Información general del planificador de recursos
description: Puede estimar y presupuestar la asignación de sus recursos a los proyectos a los que están asignados y predecir su disponibilidad para el trabajo futuro mediante el planificador de recursos.
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: ec49a7d3adeb24c1b8df0ff5fafe650d18d92280
workflow-type: tm+mt
source-wordcount: '2077'
ht-degree: 0%

---

# Información general del planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

Puede estimar y presupuestar la asignación de sus recursos a los proyectos a los que están asignados y predecir su disponibilidad para el trabajo futuro mediante el planificador de recursos.

Para obtener una descripción general de la planificación de recursos en Adobe Workfront, consulte el artículo [Introducción a la planificación de recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Información general del planificador de recursos

Puede utilizar el planificador de recursos para comprender fácilmente la disponibilidad de los usuarios y las funciones de trabajo, así como el tiempo planificado necesario para completar el trabajo en los proyectos. A continuación, puede decidir cómo asignar a los usuarios y sus funciones de trabajo en los proyectos a los que están asignados en función de su tiempo disponible.

>[!IMPORTANT]
>
>No puede utilizar el planificador de recursos para asignar el trabajo real (tareas y problemas) a los usuarios. Solo puede calcular la cantidad de tiempo necesario para que los usuarios o las funciones de trabajo completen un proyecto, independientemente de las tareas y los problemas a los que estén asignados.\
>Para asignar el trabajo real a los usuarios, debe utilizar el equilibrador de carga de trabajo. Para obtener más información sobre el equilibrador de carga de trabajo, consulte [Información general del equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Puede ver información en el Planificador de recursos utilizando tres vistas independientes. Puede utilizar cada vista para realizar una de las siguientes finalidades:

* Para presupuestar el tiempo o el coste de los recursos para el trabajo que debe realizarse mediante las vistas Proyecto y Función. Este es el propósito principal del planificador de recursos.\
   Para obtener más información sobre la presupuestación en el Planificador de recursos, consulte el artículo [Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* Para ver la siguiente información mediante la vista Usuario:

   * la disponibilidad de los usuarios según su programación
   * el tiempo previsto necesario para completar el trabajo de acuerdo con el plan del proyecto.
   * cantidad de tiempo que los usuarios ya han iniciado sesión en elementos de trabajo reales.

   Para obtener más información sobre la visualización de horas disponibles, planificadas y reales o horas FTE para los usuarios en el planificador de recursos, consulte el artículo [Ver las horas disponibles, planificadas y reales o FTE en el Planificador de recursos al utilizar la vista Usuario](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## Consideraciones del planificador de recursos

* Puede priorizar los proyectos en los que está trabajando y presupuestar la asignación de recursos según su prioridad para asegurarse de que primero tenga recursos asignados a los proyectos más importantes.

   Para obtener información sobre cómo priorizar proyectos en el planificador de recursos, consulte [Priorizar los proyectos en el planificador de recursos](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Puede mostrar información sobre horas, FTE y costes de las tareas y problemas de los proyectos.

   >[!NOTE]
   >
   >Las tareas y los problemas no se muestran en el Planificador de recursos. Sin embargo, la información de horas, FTE y costes de las asignaciones de recursos en las tareas se muestra en el Planificador de recursos como un número total para el proyecto.

* La información de hora, tiempo de espera y coste de las tareas principales se excluye de los proyectos que se muestran en el Planificador de recursos. Se recomienda asignar recursos únicamente a tareas secundarias si se desea administrar el tiempo o el coste de esos recursos en el Planificador de recursos.

   Para obtener información sobre las tareas principales, consulte los siguientes artículos:

   * [Información general sobre tareas](../../manage-work/tasks/task-information/tasks-overview.md)
   * [Crear subtareas](../../manage-work/tasks/create-tasks/create-subtasks.md)

   >[!TIP]
   >
   >Las tareas principales muestran un total de las horas y los costes de las tareas secundarias. Debido a esto, el recuento de horas, FTE y el coste de las tareas secundarias y las tareas principales contarían estas cantidades dos veces. Por este motivo, la información de la tarea principal se excluye del Planificador de recursos.

* No puede administrar la asignación de equipos en los proyectos en los que tienen tareas o problemas en el Planificador de recursos.
* Puede presupuestar recursos para varios proyectos a la vez mediante el planificador de recursos o para un solo proyecto mediante el área de presupuestación de recursos del caso empresarial. La información que presupuestó para un proyecto también se muestra en el Planificador de recursos.

   Para obtener información sobre cómo se pueden presupuestar recursos para un solo proyecto, consulte el artículo [Recursos presupuestarios en el caso empresarial](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   Para obtener información sobre cómo puede presupuestar recursos en el Planificador de recursos para varios proyectos a la vez, consulte la sección &quot;Recursos presupuestarios en el Planificador de recursos&quot; en el artículo [Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## Requisitos previos para trabajar en el planificador de recursos {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

Para utilizar correctamente el planificador de recursos para presupuestar sus recursos, primero debe asegurarse de que usted, sus proyectos y las tareas cumplan un conjunto de requisitos previos. Estos requisitos previos son obligatorios para mostrar la información correcta en el Planificador de recursos y para administrar con precisión sus recursos.

>[!IMPORTANT]
>
>Si falta alguno de los siguientes requisitos previos, es posible que descubra que falta parte de la información sobre la asignación o la disponibilidad de los recursos o que tiene un valor cero.\
>Para obtener más información sobre por qué faltan datos en los campos o tienen valores cero, pase el ratón sobre los campos.

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>Los siguientes requisitos previos solo son necesarios cuando se visualiza el Planificador de recursos por proyecto o función de trabajo o cuando se presupuestan recursos en el caso de negocio de un proyecto.

Se requieren los siguientes tipos de requisitos previos para la funcionalidad correcta del Planificador de recursos al visualizarlo por proyecto o función:

* [Requisitos previos de usuario](#user-prerequisites)
* [Requisitos previos del proyecto](#project-prerequisites)
* [Requisitos previos de tareas y problemas](#tasks-and-issues-prerequisites)
* [Requisitos previos de nivel de sistema](#system-level-prerequisites)

### Requisitos previos de usuario {#user-prerequisites}

Asegúrese de que existe la siguiente configuración de usuario antes de empezar a usar el Planificador de recursos:

* Tiene el acceso correcto a los recursos presupuestarios.

   Para obtener información sobre el acceso necesario a los recursos presupuestarios, consulte el artículo [Acceso necesario para presupuestar recursos en Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Los usuarios asignados a tareas se añaden a los grupos de recursos asociados al proyecto.

   Para obtener información sobre cómo agregar usuarios a grupos de recursos, consulte [Asociación de grupos de recursos con usuarios](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

   >[!NOTE]
   >
   >Cuando los usuarios no se agregan a los grupos de recursos, pueden darse los siguientes escenarios:
   >
   >   
   >   
   >   * Los usuarios no aparecen en el planificador de recursos, aunque podrían asignarse a tareas de los proyectos.
   >   * Si las tareas a las que están asociadas tienen Horario planificado, esas horas no aparecen para el proyecto en el Planificador de recursos, a menos que el usuario también esté asociado con una función de trabajo en esas tareas.
   >   * Si los usuarios están asociados a una función de trabajo en una tarea del proyecto, el horario planificado se muestra en el Planificador de recursos para la función de trabajo, pero la función de trabajo no se puede presupuestar.


* Los usuarios asignados a grupos de trabajo y recursos deben tener programas y funciones de trabajo asociados a su perfil.

   Para obtener información sobre cómo asociar programaciones y funciones de trabajo con usuarios, consulte [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Los usuarios que no están asociados a un programa pero que están en el grupo de recursos del proyecto no pueden presupuestarse en el Planificador de recursos.

* Para obtener información precisa sobre las horas disponibles, asegúrese de que las programaciones asociadas con los usuarios tengan las excepciones de programación y el tiempo de espera actualizado.

   >[!NOTE]
   >
   >Si un usuario no está asociado a una programación, la programación predeterminada de su sistema Workfront se asocia al usuario de forma predeterminada, a los efectos del Planificador de recursos.

   Para obtener información sobre la creación de programaciones, consulte el artículo [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Si desea presupuestar los recursos por costo, debe asociar las funciones de trabajo con costo/hora. tasas. El coste asociado con las funciones de trabajo asignadas a los usuarios en los grupos de recursos se utiliza para calcular el Coste de trabajo presupuestado y el Coste presupuestado del proyecto.\
   Para obtener información sobre cómo asociar roles de trabajo con tasas, consulte el artículo [Crear y administrar funciones de trabajo](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
   Para obtener información sobre el cálculo del costo de trabajo presupuestado, consulte el artículo [Comprender el costo presupuestado del trabajo y las horas presupuestadas para los proyectos](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
   Para obtener información sobre el cálculo del coste presupuestado, consulte el artículo [Calcular costo presupuestado](../../manage-work/projects/project-finances/budgeted-cost.md).

### Requisitos previos del proyecto {#project-prerequisites}

Asegúrese de que existe la siguiente configuración de proyecto antes de empezar a usar el Planificador de recursos:

* Los proyectos están asociados a grupos de recursos.\
   Para obtener más información sobre cómo agregar grupos de recursos a proyectos, consulte [Asociación de grupos de recursos con proyectos y plantillas](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

   >[!IMPORTANT]
   >
   >Los proyectos sin grupos de recursos no muestran la información de horas planificadas o asignaciones en el Planificador de recursos.

### Requisitos previos de tareas y problemas {#tasks-and-issues-prerequisites}

Aunque no puede mostrar tareas y problemas en el Planificador de recursos, su información se transfiere a los proyectos que se muestran en el Planificador de recursos .

Asegúrese de que existe la siguiente configuración de problemas y tareas antes de iniciar los recursos de presupuesto en el Planificador de recursos:

* Las tareas o los problemas de los proyectos para los que está presupuestando recursos se asignan a una de estas entidades:

   * Usuarios de los grupos de recursos del proyecto que también están asociados a Funciones de trabajo
   * Roles

   >[!NOTE]
   >
   >Las horas planificadas de tareas y los problemas asignados a funciones de trabajo se muestran en el Planificador de recursos, pero estas horas no se pueden presupuestar a menos que un usuario asociado a la función de trabajo aparezca en un grupo de recursos asociado al proyecto.

* No debe asignar tareas principales a usuarios o funciones.

   Para mostrar información de hora en el Planificador de recursos para usuarios o funciones asociadas con tareas principales, también debe asignarlas a las tareas secundarias. El planificador de recursos no muestra información de tareas principales.

* Tareas y problemas tienen un valor para Horario planificado que es bueno que cero.
* Las tareas y los problemas tienen un valor para su duración que es buena a cero.
* Las fechas previstas de las cuestiones se encuentran dentro del calendario del proyecto.

### Requisitos previos de nivel de sistema {#system-level-prerequisites}

Debe comprender cómo la instancia de Workfront calcula la disponibilidad de los usuarios según las preferencias de administración de recursos de su sistema. Workfront puede calcular la disponibilidad del usuario según la programación del usuario definida en su página Perfil del usuario o en la programación predeterminada de su sistema.

![](assets/resource-management-preferences-section-in-setup-350x89.png)

El administrador de Workfront configura las preferencias de administración de recursos.

Para obtener más información, consulte [Configurar las preferencias de Administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Localizar el planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

Puede ubicar el Planificador de recursos en dos áreas de Workfront, en función de si desea presupuestar los recursos para varios proyectos o solo para un proyecto.

Para obtener información sobre cómo localizar el planificador de recursos, consulte [Localizar el planificador de recursos](../../resource-mgmt/resource-planning/locate-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(this is drafted and moved to its own article: locate-resource-planner) </p>
<p>Ensure that all prerequisites are met before starting to use the Resource Planner. This way, you ensure that the Resource Planner displays the correct information before you start budgeting your resources.<br>For information about the prerequisites that must be met before you can start using the Resource Planner, see the <a href="#prerequisites-for-working-in-the-resource-planner" class="MCXref xref">Prerequisites for working in the Resource Planner</a> section in this article. </p>
<p>You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.</p>
<ul>
<li><a href="#use-the-resource-planner-for-multiple-projects" class="MCXref xref">Use the Resource Planner for multiple projects</a> </li>
<li> <p><a href="#use-the-resource-planner-for-one-project" class="MCXref xref">Use the Resource Planner for one project</a> </p> </li>
</ul>
<p><strong>Use the Resource Planner for multiple projects</strong></p>
<p>When using the Resource Planner for multiple projects, the allocation numbers for your resources represent numbers across multiple projects. </p>
<p>To access the  Planner section  in the  Resourcing area: </p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.  </li>
<li value="2"> <p>  Click <strong>Resourcing</strong>. The Resource Planner displays by default.  For information about budgeting resources in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> <p> <img src="assets/qs-resource-management-area-with-planner-as-default-350x152.png" style="width: 350;height: 152;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">  Hover over the left panel, and click <strong>Resource Pools</strong>. <br>For information about creating new resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</li>
</ol>
<p><strong>Use the Resource Planner for one project</strong></p>
<p>When using the Resource Planner for one project, the allocation numbers for your resources represent numbers for the selected project. </p>
<ol>
<li value="1"> <p>Go to a project you want to budget resources for.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Business Case</strong> in the left panel.</p> </li>
<li value="3"> <p>Scroll to the <strong>Resource Budgeting</strong> section of the Business Case.</p> </li>
<li value="4"> <p>Click <strong>Edit Resource Budgeting</strong> to add resource pools to your project and start budgeting your resources. </p> <note type="tip">
You can only add a resource pool in the Resource Budgeting area of the Business Case when the project has no resource pools associated with it. When the project already has a resource pool, the users in the pool and their job roles display in the Resource Budgeting area by default.
</note> <p> <img src="assets/resource-budgeting-area-on-project-350x70.png" style="width: 350;height: 70;"> </p> <p>For information about budgeting resources for one project, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</p> </li>
</ol>
</div>
-->

## Las áreas del planificador de recursos

Puede ver la siguiente información o realizar las siguientes acciones en el Planificador de recursos:

* Información sobre los recursos asignados a sus proyectos en el Planificador de recursos en una cronología general.
* Sobreasignación o infrautilización de sus recursos en el Planificador de Recursos.
* Asigne un presupuesto a los recursos para que funcionen de forma manual o automática.

Para obtener más información sobre las áreas que se muestran en el Planificador de recursos y cómo configurar la información que se muestra en estas áreas, consulte el artículo [Información general sobre navegación del planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Limitaciones en la visualización de la información en el planificador de recursos

Para mejorar el rendimiento, Workfront limita la cantidad de elementos que puede mostrar en el Planificador de recursos.

Para obtener más información sobre estas limitaciones, consulte el artículo [Limitaciones de visualización del Planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## Calcular FTE en el planificador de recursos

Puede mostrar los valores de disponibilidad, asignación y planificación en el Planificador de recursos en Horas, FTE o Coste.

Para obtener más información sobre cómo cambiar la información que se muestra en el Planificador de recursos, consulte la sección [Ver información por hora, tiempo de espera o costo](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) en el artículo [Revisar la disponibilidad y asignación de recursos con el planificador de recursos de Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

Para obtener más información sobre cómo se calculan las horas y los datos a tiempo completo para los usuarios y las funciones en Workfront, consulte el artículo [Descripción general del cálculo de horas y FTE para usuarios y funciones en el planificador de recursos](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Calcular los costes en el planificador de recursos

Para ver la información por Coste en el Planificador de recursos, debe tener permisos de Vista a Datos Financieros y Ver Finanzas en los proyectos.

Además de mostrar los valores de disponibilidad, asignación y planeados en el Planificador de recursos en Horas y FTE, también puede mostrarlos por Coste.

>[!TIP]
>
>Debe asociar los usuarios y las funciones de su trabajo con las tasas de Costo por hora para mostrar la información por Costes en el Planificador de Recursos.

Para obtener más información sobre la asociación de tasas de costo por hora con funciones de trabajo, consulte el artículo [Crear y administrar funciones de trabajo](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
Para obtener más información sobre cómo asociar las tasas de costo por hora con los usuarios, consulte el artículo [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Tenga en cuenta lo siguiente cuando consulte la información por Coste en el Planificador de Recursos:

* El coste de cada tipo de horas (Planificado, Disponible, Presupuestado, Real para Usuarios, Funciones o Proyectos) se calcula mediante una tasa de coste diferente.
* El coste planeado se ve afectado por el tipo de coste de las tareas en los proyectos.
* Al aplicar la Vista de usuario al planificador de recursos, no puede mostrar la información de asignación y disponibilidad por costo.

Para obtener más información sobre cómo se calculan los costes en el planificador de recursos para usuarios y funciones, consulte el artículo [Calcular los costes en el planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the User View to view Available, Planned, and Actual Hours or FTE </h2>
<p>(this information is repeated from above where it exists in shorter form. Drafted to simplify the amount of info of this article.) </p>
<p>You can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. </p>
<p>For information about using the Resource Planner to review the Available, Planned, and Actual Hours and FTE for resources, see the article <a href="../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md" class="MCXref xref">View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view</a>.</p>
<p><strong>Use the Project and Role Views to budget resources </strong></p>
<p> The main function of the Resource Planner is to budget your resources for the work that needs to be completed on the projects that you can manage. </p>
<p> You can budget your resources only if you apply the <strong>View by Project</strong> or <strong>View by Role</strong> views to the Resource Planner.</p>
<p>For information about budgeting resources using the Project and Role views in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md"><a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a></a>.</p>
</div>
-->

## Filtrar información en el planificador de recursos

Puede reducir el número de proyectos, funciones o usuarios que se muestran en el Planificador de recursos creando un filtro.\
Para obtener más información, consulte el artículo [Filtrar información en el planificador de recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).
