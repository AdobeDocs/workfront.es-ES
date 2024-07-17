---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Resumen del Planificador de recursos
description: Puede estimar y presupuestar la asignación de sus recursos a los proyectos a los que están asignados y prever su disponibilidad para el trabajo futuro mediante el Planificador de recursos.
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: 1c8d9a62f5582b0dbc3c72b5881bb5d8f0b790ba
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# Resumen del Planificador de recursos

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

Puede estimar y presupuestar la asignación de sus recursos a los proyectos a los que están asignados y prever su disponibilidad para el trabajo futuro mediante el Planificador de recursos.

Para obtener una descripción general de la planificación de recursos en Adobe Workfront, consulte el artículo [Introducción a la planificación de recursos](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Resumen del Planificador de recursos

Puede utilizar el Planificador de recursos para comprender fácilmente la disponibilidad de los usuarios y los roles, así como el tiempo planificado necesario para completar el trabajo en los proyectos. A continuación, puede decidir cómo asignar los usuarios y sus funciones en los proyectos a los que están asignados en función del tiempo disponible.

>[!IMPORTANT]
>
>No puede usar el Planificador de recursos para asignar trabajo real (tareas y problemas) a los usuarios. Solo puede calcular la cantidad de tiempo necesario para que los usuarios o los roles completen un proyecto, independientemente de las tareas y problemas a los que estén asignados.\
>Para asignar trabajo real a usuarios, debe utilizar el Distribuidor de cargas de trabajo. Para obtener más información sobre el Distribuidor de cargas de trabajo, consulte [Resumen del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Puede ver información en el Planificador de recursos utilizando tres vistas independientes. Puede utilizar cada vista para cumplir uno de los siguientes propósitos:

* Para presupuestar el tiempo o el costo de los recursos para el trabajo que debe realizarse, use las vistas Proyecto y Rol. Este es el propósito principal del Planificador de recursos.\
  Para obtener más información acerca de cómo presupuestar en el Planificador de recursos, consulte el artículo [Presupuesto de recursos en el Planificador de recursos mediante las vistas de proyecto y función](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* Para ver la siguiente información mediante la vista Usuario:

   * La disponibilidad de los usuarios según su programación
   * La cantidad de tiempo planificada necesaria para completar el trabajo según el plan del proyecto
   * Cantidad de tiempo que los usuarios ya han iniciado sesión en elementos de trabajo reales

  Para obtener más información sobre cómo ver las horas disponibles, planificadas y reales o FTE de los usuarios en el Planificador de recursos, consulte el artículo [Ver horas disponibles, planificadas y reales o FTE en el Planificador de recursos al usar la vista de usuario](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## Consideraciones del Planificador de recursos

* Puede priorizar los proyectos en los que está trabajando y presupuestar la asignación de recursos según su prioridad, para asegurarse de que primero tenga los recursos asignados a los proyectos más importantes.

  Para obtener información sobre cómo priorizar proyectos en el Planificador de recursos, consulte [Priorizar proyectos en el Planificador de recursos](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Puede mostrar información de horas, ETC y costos de las tareas y problemas de los proyectos.

  >[!NOTE]
  >
  >Las tareas y los problemas no se muestran en el Planificador de recursos. Sin embargo, la información de horas, ETC y costos de las asignaciones de recursos de las tareas se muestra en el Planificador de recursos como un número total para el proyecto.

* La información de horas, ETC y costos de las tareas principales se excluye de los proyectos que se muestran en el Planificador de recursos. Se recomienda asignar recursos únicamente a tareas secundarias si desea administrar el tiempo o el costo de esos recursos en el Planificador de recursos.

  Para obtener información sobre las tareas principales, consulte los siguientes artículos:

   * [Resumen de tareas](../../manage-work/tasks/task-information/tasks-overview.md)
   * [Creación de subtareas](../../manage-work/tasks/create-tasks/create-subtasks.md)

  >[!TIP]
  >
  >Las tareas principales muestran un total de las horas y los costes de las tareas secundarias. Debido a esto, contar las horas, el valor de FTE y el coste de las tareas secundarias y las tareas principales contaría estas cantidades dos veces. Por este motivo, la información de la tarea principal se excluye del Planificador de recursos.

* No puede administrar la asignación de equipos en los proyectos en los que tienen tareas o problemas en el Planificador de recursos.
* Puede presupuestar recursos para varios proyectos a la vez usando el Planificador de recursos o para un solo proyecto usando el área de Presupuestación de recursos del Caso comercial. La información presupuestada para un proyecto también se muestra en el Planificador de recursos.

  Para obtener información acerca de cómo puede presupuestar recursos para un solo proyecto, vea el artículo [Recursos de presupuesto en el caso comercial](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

  Para obtener información sobre cómo puede presupuestar recursos en el Planificador de recursos para varios proyectos a la vez, consulte la sección &quot;Presupuestar recursos en el Planificador de recursos&quot; en el artículo [Recursos presupuestarios en el Planificador de recursos mediante las vistas Proyecto y Rol](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## Requisitos previos para trabajar en el Planificador de recursos {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

Para utilizar correctamente el Planificador de recursos para presupuestar los recursos, primero debe asegurarse de que usted, sus proyectos y sus tareas cumplen con un conjunto de requisitos previos. Estos requisitos previos son obligatorios para mostrar la información correcta en el Planificador de recursos y para administrar con precisión los recursos.

>[!IMPORTANT]
>
>Si falta alguno de los siguientes requisitos previos, es posible que descubra que falta parte de la información sobre la asignación o la disponibilidad de los recursos o que tiene un valor cero.\
>Para obtener más información sobre por qué faltan datos en los campos o por qué tienen valores cero, pase el ratón sobre los campos.

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>Los siguientes requisitos previos solo son necesarios cuando se consulta el Planificador de recursos por proyecto, por rol o al presupuestar recursos en el caso comercial de un proyecto.

Se requieren los siguientes tipos de requisitos previos para la correcta funcionalidad del Planificador de recursos al visualizarlo por proyecto o por rol:

* [Requisitos previos del usuario](#user-prerequisites)
* [Requisitos previos del proyecto](#project-prerequisites)
* [Requisitos previos para tareas y problemas](#tasks-and-issues-prerequisites)
* [Requisitos previos de nivel de sistema](#system-level-prerequisites)

### Requisitos previos del usuario {#user-prerequisites}

Asegúrese de que exista la siguiente configuración de usuario antes de empezar a usar el Planificador de recursos:

* Tiene el acceso correcto a los recursos del presupuesto.

  Para obtener información sobre el acceso necesario para presupuestar recursos, consulte el artículo [Acceso necesario para presupuestar recursos en Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Los usuarios asignados a tareas se agregan a los conjuntos de recursos asociados con el proyecto.

  Para obtener información acerca de cómo agregar usuarios a los conjuntos de recursos, vea [Asociar conjuntos de recursos a los usuarios](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

  >[!NOTE]
  >
  >Cuando no se agregan usuarios a los conjuntos de recursos, pueden darse los siguientes escenarios:
  >
  >   
  >   
  >   * Los usuarios no aparecen en el Planificador de recursos, aunque podrían estar asignados a tareas de los proyectos.
  >   * Si las tareas con las que están asociadas tienen horas planificadas, esas horas no aparecen para el proyecto en el Planificador de recursos, a menos que el usuario también esté asociado a una función del trabajo en esas tareas.
  >   * Si los usuarios están asociados a un rol en una tarea del proyecto, las horas planificadas se muestran en el Planificador de recursos para el rol, pero el rol no se puede presupuestar.
  >   
  >

* Los usuarios asignados a conjuntos de recursos y de trabajo deben tener los programas y los roles asociados a su perfil.

  Para obtener información sobre cómo asociar horarios y roles con usuarios, consulte [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Los usuarios que no están asociados a una Programación pero que están en el fondo de recursos del proyecto no pueden presupuestarse en el Planificador de recursos.

* Para obtener información precisa sobre las horas disponibles, asegúrese de que las programaciones asociadas con los usuarios tengan actualizadas las excepciones de horario y los días libres.

  >[!NOTE]
  >
  >Si un usuario no está asociado a un Horario, el Horario por Defecto de su sistema Workfront está asociado al usuario por defecto, a los efectos del Planificador de Recursos.

  Para obtener información acerca de cómo crear programaciones, vea el artículo [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Si desea presupuestar los recursos por Coste, debe asociar los Roles con Coste/Hora. tarifas. El costo asociado con los roles asignados a los usuarios de los conjuntos de recursos se utiliza para calcular el costo de mano de obra presupuestado y el costo presupuestado del proyecto.\
  Para obtener información sobre cómo asociar roles con tasas, consulte el artículo [Crear y administrar roles](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
  Para obtener información sobre el cálculo del costo de mano de obra presupuestado, consulte el artículo [Comprender el costo de mano de obra presupuestado y las horas presupuestadas para proyectos](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
  Para obtener información acerca del cálculo del costo presupuestado, vea el artículo [Calcular costo presupuestado](../../manage-work/projects/project-finances/budgeted-cost.md).

### Requisitos previos del proyecto {#project-prerequisites}

Asegúrese de que exista la siguiente configuración de proyecto antes de empezar a usar el Planificador de recursos:

* Sus proyectos están asociados a conjuntos de recursos.\
  Para obtener más información acerca de cómo agregar conjuntos de recursos a proyectos, vea [Asociar conjuntos de recursos a proyectos y plantillas](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

  >[!IMPORTANT]
  >
  >Los proyectos sin conjuntos de recursos no muestran la información de horas planificadas o asignaciones en el Planificador de recursos.

### Requisitos previos de tareas y problemas {#tasks-and-issues-prerequisites}

Aunque no puede mostrar tareas y problemas en el Planificador de recursos, su información se transfiere a los proyectos que se muestran en el Planificador de recursos

Asegúrese de que exista la siguiente configuración de tarea y problema antes de iniciar los recursos de presupuesto en el Planificador de recursos:

* Las tareas o problemas de los proyectos para los que está presupuestando recursos se asignan a una de estas entidades:

   * Usuarios en los conjuntos de recursos del proyecto que también están asociados a Roles
   * Roles

  >[!NOTE]
  >
  >Las horas planificadas de las tareas y problemas asignados a los roles se muestran en el Planificador de recursos, pero estas horas no se pueden presupuestar a menos que un usuario asociado al rol aparezca en un conjunto de recursos asociado al proyecto.

* No debe asignar tareas principales a usuarios o funciones.

  Para mostrar información de horas en el Planificador de recursos para usuarios o roles asociados con tareas principales, también debe asignarlos a las tareas secundarias. El Planificador de recursos no muestra información de las tareas principales.

* Las tareas y los problemas tienen un valor de horas planificadas mayor que cero.
* Las tareas y los problemas tienen un valor de Duración mayor que cero.
* Las fechas planificadas de los problemas se encuentran dentro de los plazos previstos en el proyecto.

### Requisitos previos de nivel de sistema {#system-level-prerequisites}

Debe comprender cómo calcula la instancia de Workfront la disponibilidad del usuario según las Preferencias de administración de recursos del sistema. Workfront puede calcular la disponibilidad del usuario utilizando el horario del usuario definido en su página Perfil de usuario o el Horario predeterminado del sistema.

![](assets/resource-management-preferences-section-in-setup-350x89.png)

El administrador de Workfront configura las preferencias de administración de recursos.

Para obtener más información, consulte [Configurar las preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Busque el Planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

Puede ubicar el Planificador de recursos en dos áreas de Workfront, en función de si desea presupuestar los recursos para varios proyectos o para un solo proyecto.

Para obtener información sobre cómo encontrar el Planificador de recursos, consulte [Localizar el Planificador de recursos](../../resource-mgmt/resource-planning/locate-resource-planner.md).

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

## Las áreas del Planificador de recursos

Puede ver la siguiente información o realizar las siguientes acciones en el Planificador de recursos:

* Información sobre los recursos asignados a sus proyectos en el Planificador de recursos en una cronología general.
* Sobreasignación o infrautilización de los recursos en el Planificador de recursos.
* Presupueste los recursos para trabajar de forma manual o automática.

Para obtener más información sobre las áreas que se muestran en el Planificador de recursos y cómo configurar la información que se muestra en estas áreas, consulte el artículo [Información general sobre la navegación del Planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Limitaciones al mostrar información en el Planificador de recursos

Para mejorar el rendimiento, Workfront limita la cantidad de elementos que se pueden mostrar en el Planificador de recursos.

Para obtener más información sobre estas limitaciones, consulte el artículo [Limitaciones de visualización del Planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## Calcular FTE en el Planificador de recursos

Puede mostrar la disponibilidad, la asignación y los valores planificados en el Planificador de recursos en Horas, ETC o Coste.

Para obtener más información acerca de cómo cambiar la información que se muestra en el Planificador de recursos, vea la sección [Ver información por hora, ETC o costo](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) en el artículo [Revisar la disponibilidad y asignación de recursos mediante el Planificador de recursos de Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

Para obtener más información acerca de cómo se calculan las horas y el valor de FTE para los usuarios y las funciones en Workfront, vea el artículo [Información general sobre el cálculo de horas y el valor de FTE para los usuarios y las funciones en el Planificador de recursos](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Calcular costos en el Planificador de recursos

Para ver la información por costo en el Planificador de recursos, debe tener acceso de visualización a los datos financieros y de visualización de finanzas en los proyectos.

Además de mostrar la disponibilidad, la asignación y los valores planificados en el Planificador de recursos en horas y tiempo completo, también puede mostrarlos por costo.

>[!TIP]
>
>Debe asociar los usuarios y sus roles con las tasas de costo por hora para mostrar información por costos en el Planificador de recursos.

Para obtener más información acerca de cómo asociar tasas de costo por hora con roles de trabajo, vea el artículo [Crear y administrar roles](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
Para obtener más información acerca de cómo asociar tarifas de costo por hora con usuarios, vea el artículo [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Tenga en cuenta lo siguiente cuando visualice información por costo en el Planificador de recursos:

* El costo de cada tipo de horas (planificadas, disponibles, presupuestadas, reales para usuarios, roles o los proyectos) se calcula mediante una tasa de costo diferente.
* El costo planificado se ve afectado por el tipo de costo de las tareas de los proyectos.
* Al aplicar la Vista de usuario al Planificador de recursos, no puede mostrar la información de asignación y disponibilidad por costo.

Para obtener más información acerca de cómo se calculan los costos de los usuarios y las funciones en el Planificador de recursos, vea el artículo [Calcular costos en el Planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

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

## Filtrar información en el Planificador de recursos

Puede reducir el número de proyectos, funciones o usuarios que se muestran en el Planificador de recursos creando un filtro.\
Para obtener más información, vea el artículo [Filtrar información en el Planificador de recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).
