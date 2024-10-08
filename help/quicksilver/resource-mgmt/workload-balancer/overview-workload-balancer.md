---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Resumen del Distribuidor de cargas
description: Una vez que los jefes de proyecto hayan planificado el trabajo en los proyectos creando tareas y después de que los jefes de recursos asignen los recursos de roles a los proyectos en el Planificador de recursos, los propietarios de proyecto y los jefes de equipo podrán utilizar el Distribuidor de cargas de trabajo para asignar elementos de trabajo a los usuarios.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 0%

---

# Resumen del Distribuidor de cargas

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Una vez que los jefes de proyecto hayan planificado el trabajo en los proyectos creando tareas y después de que los jefes de recursos asignen los recursos de roles a los proyectos en el Planificador de recursos, los propietarios de proyecto y los jefes de equipo podrán utilizar el Distribuidor de cargas de trabajo para asignar elementos de trabajo a los usuarios.

>[!IMPORTANT]
>
>Puede utilizar el Distribuidor de cargas de trabajo para asignar trabajo real (tareas y problemas) a los usuarios.
>
>Debe utilizar el Planificador de recursos, y no el Distribuidor de cargas de trabajo, para calcular las asignaciones de roles de sus proyectos en un nivel superior. Para obtener más información sobre el Planificador de recursos, consulte [Resumen del Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Este artículo describe el propósito general del Distribuidor de cargas de trabajo y algunas de las prácticas recomendadas sobre cómo puede configurar sus proyectos y recursos para utilizarlo correctamente.

Para ver los tutoriales en vídeo del Distribuidor de cargas de trabajo, ve a la página [Tutorials de Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=es). En el menú de la izquierda, seleccione **Administrar recursos** > **Distribuidor de cargas de trabajo** y elija un tutorial.

## Localización del Distribuidor de cargas de trabajo

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Se recomienda utilizar el Distribuidor de cargas de trabajo en las siguientes áreas para programar recursos:

* En el nivel del sistema, en el área de Recursos.
* En el nivel de proyecto, en la sección Distribuidor de cargas de trabajo de un proyecto.
* En el nivel de equipo, en la sección Distribuidor de cargas de trabajo de un equipo.

Para obtener más información sobre cómo encontrar el Distribuidor de cargas de trabajo, consulte [Localizar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Ventajas del Distribuidor de cargas de trabajo

Tenga en cuenta las siguientes ventajas al utilizar el Distribuidor de cargas de trabajo:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Acceda a una asignación visual clara de la sobreasignación y la infrautilización de recursos que sea transparente para todas las partes interesadas.
* Como gerente de personas, puede proteger a sus empleados del agotamiento profesional y empoderarlos para que hagan su mejor trabajo con mejor enfoque, calidad y participación. Puede garantizar su utilización completa, romper los silos y habilitar la alineación del trabajo entre equipos.
* Al asignar trabajo en el nivel de tarea o problema no tiene visibilidad de cuán ocupado podría estar un usuario. Al utilizar el Distribuidor de cargas de trabajo, puede ver qué usuarios tienen disponibilidad en su carga de trabajo para completar la tarea o el problema a tiempo. Esto incluye los detalles de sus días libres y excepciones de horario.

  Para obtener más información, vea [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  También puede asignar elementos de trabajo de forma masiva, lo que facilita la distribución de muchos elementos de trabajo al mismo tiempo en varios proyectos. Para obtener más información, consulte [Asignar trabajo de forma masiva mediante el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* Los ejecutivos pueden tomar decisiones oportunas sobre la dotación de personal a través de la transparencia en la forma en que se utilizan las personas de su organización.
* Los miembros del equipo se benefician de una mejor colaboración, ya que todos pueden ver en qué están trabajando sus compañeros en un momento determinado. Para obtener información sobre el acceso necesario para ver o administrar recursos en el Distribuidor de cargas de trabajo, consulte [Acceso necesario para administrar recursos en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Compártalo con cualquier persona que no tenga acceso al área de Recursos incrustando un vínculo a ella en una pestaña personalizada. Para obtener más información, vea [Compartir el Distribuidor de cargas de trabajo con un vínculo](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualice y administre las cargas de trabajo y la demanda de las personas en una sola vista a nivel global, de proyecto o de equipo, según su función. Al administrar proyectos, esto incluye no solo la asignación de recursos para el proyecto, sino también la visualización de la asignación de recursos desde el Scenario Planner de Adobe Workfront. Los administradores de personas utilizan el planificador de escenarios de Workfront para administrar las habilidades laborales en toda la organización. El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront.

  >[!NOTE]
  >
  >  El Scenario Planner requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte [Información general sobre el Scenario Planner](../../scenario-planner/scenario-planner-overview.md).


## Prácticas recomendadas para utilizar el Distribuidor de cargas de trabajo

Recomendamos las siguientes prácticas recomendadas para planificar proyectos, configurar usuarios y utilizar filtros antes de empezar a programar recursos mediante el Distribuidor de cargas de trabajo.

* [Prácticas recomendadas para mostrar información en el Distribuidor de cargas de trabajo](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Prácticas recomendadas para configurar usuarios](#best-practices-for-setting-up-users)
* [Prácticas recomendadas para configurar tareas y problemas](#best-practices-for-setting-up-tasks-and-issues)

### Prácticas recomendadas para mostrar información en el Distribuidor de cargas de trabajo {#best-practices-for-displaying-information-in-the-workload-balancer}

Le recomendamos que utilice filtros para que pueda mostrar únicamente la información que le interesa para los elementos de trabajo no asignados y asignados.

Para obtener información sobre cómo crear y usar filtros en el Distribuidor de cargas de trabajo, consulte [Información sobre filtros en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Prácticas recomendadas para configurar usuarios

* Como el usuario que programa el trabajo para otros, debe tener el acceso y los permisos correctos para programar recursos para el trabajo.

  Para obtener información sobre el acceso necesario para administrar la carga de trabajo de sus recursos en el Distribuidor de cargas de trabajo, consulte [Acceso necesario para administrar recursos en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Los usuarios cuya carga de trabajo desee gestionar deben cumplir los siguientes criterios para que la información sobre su disponibilidad y aptitudes sea precisa:

   * Tienen los horarios y los roles asociados a su perfil.

     Para obtener más información sobre cómo asociar horarios y roles con usuarios, consulte [Agregar usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Si un usuario no está asociado a un Horario, el Horario por Defecto de su sistema Workfront se asocia al usuario por defecto, a efectos de la gestión de recursos.
   * Hacer que las excepciones de horario se actualicen en sus horarios.

     Para obtener más información acerca de cómo crear programaciones, vea [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Actualice su calendario de días libres en el perfil.

     Para obtener información sobre cómo actualizar el calendario de días libres de un usuario, consulte [Configurar los días libres personales](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* El administrador de Workfront debe determinar cómo calcula Workfront la disponibilidad del usuario. Pueden decidir si Workfront utiliza el horario predeterminado del sistema o el horario del usuario para calcular el tiempo que el usuario está disponible para trabajar ajustando las preferencias de Administración de recursos en el área de Configuración de Workfront.

  Para obtener más información, consulte [Configurar las preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Prácticas recomendadas para configurar tareas y problemas {#best-practices-for-setting-up-tasks-and-issues}

Asegúrese de que exista la siguiente configuración de tareas y problemas antes de comenzar a asignar trabajo a los usuarios en el Distribuidor de cargas de trabajo:

* Las tareas principales no están asignadas a usuarios o roles. Las tareas principales no se muestran en el Distribuidor de cargas de trabajo.
* Las tareas y los problemas tienen un valor de horas planificadas mayor que cero.

* Las tareas y los problemas tienen un valor de Duración mayor que cero.
* Las fechas planificadas de los problemas se encuentran dentro de los plazos previstos en el proyecto.

## Antes de empezar a utilizar el Distribuidor de cargas de trabajo

* Lea los siguientes artículos antes de empezar a utilizar el Distribuidor de cargas de trabajo:

   * Este artículo explica cómo usar el Distribuidor de cargas de trabajo para realizar estas acciones: [Usar el Distribuidor de cargas de trabajo](../workload-balancer/navigate-the-workload-balancer.md).

   * En los siguientes artículos se explica cómo asignar trabajo y administrar asignaciones de usuarios:

      * [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../workload-balancer/assign-work-in-workload-balancer.md).
      * [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../workload-balancer/manage-user-allocations-workload-balancer.md).

* El Distribuidor de cargas de trabajo se puede encontrar en varias áreas diferentes de Workfront. Para obtener información sobre dónde encontrar el Distribuidor de cargas de trabajo, consulte [Localizar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Acceso necesario para utilizar el Distribuidor de cargas de trabajo

Debe tener el acceso a Workfront y los permisos correctos para proyectos específicos para poder ver y utilizar el Distribuidor de cargas de trabajo en Workfront. Para obtener información acerca del acceso necesario para usar el Distribuidor de cargas de trabajo, consulte el artículo [Acceso necesario para administrar recursos en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
