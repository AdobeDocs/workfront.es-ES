---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Información general del equilibrador de carga de trabajo
description: Una vez que los administradores de proyectos planifiquen el trabajo en proyectos y creen tareas, puede utilizar el equilibrador de carga de trabajo para asignar este trabajo a los usuarios de sus equipos.
author: Alina
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 11c87d8a97261c24d063fbc824f2e907d07f8217
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# Información general del equilibrador de carga de trabajo

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Una vez que los administradores de proyectos planifiquen el trabajo en proyectos y creen tareas, puede utilizar el equilibrador de carga de trabajo para asignar este trabajo a los usuarios.

>[!IMPORTANT]
>
>Puede utilizar el equilibrador de carga de trabajo para asignar el trabajo real (tareas y problemas) a los usuarios.
>
>Debe usar el Planificador de recursos y no el Equilibrador de carga de trabajo para estimar las asignaciones de funciones de trabajo para sus proyectos a un nivel superior. Para obtener más información acerca del planificador de recursos, consulte [Información general del planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

En este artículo se describe el propósito general del equilibrador de carga de trabajo y algunas de las prácticas recomendadas sobre cómo configurar los proyectos y recursos para utilizarlos correctamente.

## Localizar el equilibrador de carga de trabajo

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Se recomienda utilizar el equilibrador de carga de trabajo en las siguientes áreas para programar recursos:

* A nivel del sistema, en el área Recursos.
* En el nivel de proyecto, en la sección Equilibrador de carga de trabajo de un proyecto.
* A nivel de equipo, en la sección Equilibrador de carga de trabajo de un equipo.

Para obtener más información sobre cómo localizar el equilibrador de carga de trabajo, consulte [Localizar el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Ventajas del equilibrador de carga de trabajo

Tenga en cuenta las siguientes ventajas al utilizar el equilibrador de carga de trabajo:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Acceda a una clara asignación visual de la sobreasignación y la infrautilización de los recursos, que es transparente para todas las partes interesadas.
* Como administrador de personas, puede proteger a su gente de la excentricidad y capacitarla para que haga su mejor trabajo con mejor enfoque, calidad y compromiso. Puede garantizar su utilización completa, romper silos y permitir la alineación del trabajo entre equipos.
* Al asignar un trabajo en el nivel de tarea o problema, no tiene visibilidad sobre lo ocupado que puede estar un usuario. Al utilizar el equilibrador de carga de trabajo, puede ver qué usuarios tienen disponibilidad en su carga de trabajo para completar la tarea o el problema a tiempo. Esto incluye su tiempo libre y los detalles de las excepciones de programación.

   Para obtener más información, consulte [Información general sobre la asignación de trabajo en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

   También puede asignar elementos de trabajo de forma masiva, lo que facilita la distribución de un gran número de elementos de trabajo a la vez en varios proyectos. Para obtener más información, consulte [Asignar trabajo de forma masiva mediante el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* Los ejecutivos pueden tomar decisiones oportunas sobre la dotación de personal mediante la transparencia en la forma en que se utiliza a las personas de su organización.
* Los miembros del equipo se benefician de una mejor colaboración, ya que todos pueden ver en qué están trabajando sus colegas en cualquier momento. Para obtener información sobre el acceso necesario para ver o administrar recursos en el equilibrador de carga de trabajo, consulte [Acceso necesario para administrar los recursos en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Compártala con cualquier persona que no tenga acceso al área Recursos incrustando un vínculo a ella en una pestaña personalizada. Para obtener más información, consulte [Uso compartido de Workload Balancer con un vínculo](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualice y administre las cargas de trabajo y la demanda de las personas en una sola vista a nivel global, de proyecto o de equipo, según su función. Al administrar proyectos, esto incluye no solo la asignación de recursos para el proyecto, sino también la visualización de la asignación de recursos desde el planificador de escenarios de Adobe Workfront. Los administradores de Workfront Scenario Planner utilizan para administrar las habilidades laborales en toda la organización. El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront.

   >[!NOTE]
   >
   >  El planificador de escenarios requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte [Información general del planificador de escenarios](../../scenario-planner/scenario-planner-overview.md).


## Prácticas recomendadas para usar el equilibrador de carga de trabajo

Recomendamos las siguientes prácticas recomendadas para planificar proyectos, configurar usuarios y utilizar filtros antes de empezar a programar los recursos mediante el equilibrador de carga de trabajo.

* [Prácticas recomendadas para mostrar información en el equilibrador de carga de trabajo](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Prácticas recomendadas para configurar usuarios](#best-practices-for-setting-up-users)
* [Prácticas recomendadas para configurar tareas y problemas](#best-practices-for-setting-up-tasks-and-issues)

### Prácticas recomendadas para mostrar información en el equilibrador de carga de trabajo {#best-practices-for-displaying-information-in-the-workload-balancer}

Le recomendamos que utilice filtros para que pueda mostrar solamente la información que le interesa para los elementos de trabajo no asignados y asignados.

Para obtener información sobre la creación y el uso de filtros en el equilibrador de carga de trabajo, consulte [Filtrar información en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Prácticas recomendadas para configurar usuarios

* Como usuario que programa el trabajo para otros, debe tener el acceso y los permisos correctos para programar los recursos para el trabajo.

   Para obtener información sobre el acceso necesario para administrar la carga de trabajo de los recursos en el equilibrador de carga de trabajo, consulte [Acceso necesario para administrar los recursos en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Los usuarios cuya carga de trabajo desee administrar deben cumplir los siguientes criterios para que la información sobre su disponibilidad y habilidades sea precisa:

   * Tener programaciones y funciones de trabajo asociadas con su perfil.
   * Para obtener más información sobre cómo asociar programaciones y funciones de trabajo con usuarios, consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Si un usuario no está asociado con una programación, la programación predeterminada de su sistema Workfront se asocia al usuario de forma predeterminada con fines de administración de recursos.
   * Haga que las excepciones de programación se actualicen en sus programaciones.\
      Para obtener más información sobre la creación de programaciones, consulte [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Haga que se actualice el calendario de tiempo inactivo en su perfil.\
      Para obtener información sobre cómo actualizar el calendario de tiempo de espera de un usuario, consulte [Configuración del tiempo de espera personal en Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

      <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* El administrador de Workfront debe determinar cómo calcula Workfront la disponibilidad del usuario. Pueden decidir si Workfront utiliza la programación predeterminada del sistema o la programación del usuario para calcular el tiempo que el usuario está disponible para trabajar. Para obtener más información, consulte [Configurar las preferencias de Administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Prácticas recomendadas para configurar tareas y problemas {#best-practices-for-setting-up-tasks-and-issues}

Asegúrese de que existe la siguiente configuración de problemas y tareas antes de empezar a asignar trabajo a usuarios en el equilibrador de carga de trabajo:

* Las tareas principales no están asignadas a usuarios ni funciones. No se muestran en el equilibrador de carga de trabajo.
* Tareas y problemas tienen un valor para Horario planificado que es bueno que cero.

* Las tareas y los problemas tienen un valor para su duración que es buena a cero.
* Las fechas previstas de las cuestiones se encuentran dentro del calendario del proyecto.

## Antes de empezar a usar el equilibrador de carga de trabajo

* Puede utilizar el equilibrador de carga de trabajo para asignar trabajo y administrar asignaciones diarias para los usuarios de su organización.

   Este artículo le explica cómo navegar por el equilibrador de carga de trabajo para realizar estas acciones: [Navegar por el equilibrador de carga de trabajo](../workload-balancer/navigate-the-workload-balancer.md).

   Los siguientes artículos le explican cómo asigna trabajo y gestiona las asignaciones de usuario:

   * [Información general sobre la asignación de trabajo en el equilibrador de carga de trabajo](../workload-balancer/assign-work-in-workload-balancer.md).
   * [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../workload-balancer/manage-user-allocations-workload-balancer.md).

* El equilibrador de carga de trabajo se puede encontrar en varias áreas diferentes de Workfront. Para obtener información sobre dónde puede encontrar el equilibrador de carga de trabajo, consulte [Localizar el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Acceso necesario para utilizar el equilibrador de carga de trabajo

Debe tener el acceso y los permisos correctos de Workfront para proyectos específicos para poder ver y usar el equilibrador de carga de trabajo en Workfront. Para obtener información sobre el acceso necesario para utilizar el equilibrador de carga de trabajo, consulte el artículo [Acceso necesario para administrar los recursos en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
