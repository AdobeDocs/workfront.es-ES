---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Resumen del Distribuidor de cargas
description: Una vez que los administradores de proyecto hayan planificado el trabajo en los proyectos creando tareas y después de que los administradores de recursos asignen los recursos de funciones a los proyectos en el Planificador de recursos, los propietarios de proyecto y los jefes de equipo podrán utilizar el Distribuidor de cargas de trabajo para asignar elementos de trabajo a los usuarios.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 233e61c011cc87f49d0d4082a20b7790104c96c8
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 96%

---

# Información general del Distribuidor de cargas de trabajo

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Una vez que los administradores de proyecto hayan planificado el trabajo en los proyectos creando tareas y después de que los administradores de recursos asignen los recursos de funciones a los proyectos en el Planificador de recursos, los propietarios de proyecto y los jefes de equipo podrán utilizar el Distribuidor de cargas de trabajo para asignar elementos de trabajo a los usuarios.

>[!IMPORTANT]
>
>Puede utilizar el Distribuidor de cargas de trabajo para asignar trabajo real (tareas y problemas) a los usuarios.
>
>Debe utilizar el Planificador de recursos, y no el Distribuidor de cargas de trabajo, para calcular las asignaciones de funciones a sus proyectos en un nivel superior. Para obtener más información sobre el Planificador de recursos, consulte [Información general del Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Este artículo describe el propósito general del Distribuidor de cargas de trabajo y algunas de las prácticas recomendadas sobre cómo puede configurar sus proyectos y recursos para utilizarlo correctamente.

Para revisar los tutoriales en vídeo del Distribuidor de cargas de trabajo, vaya a la página [Tutorials de Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=es). En el menú de la izquierda, seleccione **Administrar recursos** > **Distribuidor de cargas de trabajo** y elija un tutorial.

## Buscar el Distribuidor de cargas de trabajo

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Se recomienda utilizar el Distribuidor de cargas de trabajo en las siguientes áreas para programar recursos:

* En el nivel del sistema, en el área Asignando recursos.
* En el nivel de proyecto, en la sección Distribuidor de cargas de trabajo de un proyecto.
* En el nivel de equipo, en la sección Distribuidor de cargas de trabajo de un equipo.

Para obtener más información sobre cómo localizar el Distribuidor de cargas de trabajo, consulte [Localizar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Ventajas del Distribuidor de cargas de trabajo

Tenga en cuenta las siguientes ventajas cuando utilice el Distribuidor de cargas de trabajo:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Acceso a una asignación visual clara de la sobreasignación y la infrautilización de los recursos que es transparente para todas las partes interesadas.
* Como administrador de personas, puede proteger a los trabajadores del agotamiento profesional y capacitarlos para que hagan un trabajo óptimo, con mejor enfoque, calidad y participación. Puede garantizar su plena utilización, romper los silos y habilitar la alineación del trabajo entre los equipos.
* Al asignar trabajo en el nivel de tarea o problema, no tiene visibilidad de la carga de trabajo de un usuario. Al utilizar el Distribuidor de cargas de trabajo, puede ver qué usuarios tienen disponibilidad en su carga de trabajo para completar la tarea o el problema a tiempo. Esto incluye los detalles de sus días libres y excepciones de horario.

  Para obtener más información, consulte [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  También puede asignar elementos de trabajo de forma masiva, lo que facilita la distribución de muchos elementos de trabajo al mismo tiempo en varios proyectos. Para obtener más información, consulte [Asignar trabajo de forma masiva mediante el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* Los ejecutivos pueden tomar decisiones oportunas sobre la dotación de personal a través de la transparencia en la forma en que se utilizan las personas de su organización.
* Los integrantes del equipo se benefician de una mejor colaboración, ya que todos pueden ver en qué están trabajando sus compañeros en cualquier momento determinado. Para obtener información sobre el acceso necesario para ver o administrar recursos en el Distribuidor de cargas de trabajo, consulte [Acceso necesario para administrar recursos en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Compártalo con cualquier persona que no tenga Recursos en el menú principal incrustando un vínculo en una pestaña personalizada. Para obtener más información, vea [Compartir el Distribuidor de cargas de trabajo con un vínculo](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
* Visualice y administre las cargas de trabajo y la demanda de las personas en una sola vista a nivel global, de proyecto o de equipo, según su función. Cuando se administran proyectos, esto incluye no solo la asignación de recursos para el proyecto, sino también la visualización de la asignación de recursos desde el Planificador de escenarios de Adobe Workfront. Los administradores de personas utilizan el Planificador de escenarios de Workfront para administrar las habilidades laborales en toda la organización. El Planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront.

  >[!NOTE]
  >
  >  El Planificador de escenarios requiere una licencia adicional. Para obtener información sobre el Planificador de escenarios de Workfront, consulte [Información general sobre el Planificador de escenarios](../../scenario-planner/scenario-planner-overview.md).


## Prácticas recomendadas para utilizar el Distribuidor de cargas de trabajo

Recomendamos las siguientes prácticas recomendadas para planificar proyectos, configurar usuarios y utilizar filtros antes de empezar a programar los recursos mediante el Distribuidor de cargas de trabajo.

* [Prácticas recomendadas para mostrar información en el Distribuidor de cargas de trabajo](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Prácticas recomendadas para configurar usuarios](#best-practices-for-setting-up-users)
* [Prácticas recomendadas para configurar tareas y problemas](#best-practices-for-setting-up-tasks-and-issues)

### Prácticas recomendadas para mostrar información en el Distribuidor de cargas de trabajo {#best-practices-for-displaying-information-in-the-workload-balancer}

Le recomendamos que utilice filtros para que pueda mostrar únicamente la información que le es relevante para los elementos de trabajo no asignados y asignados.

Para obtener información sobre cómo crear y usar filtros en el Distribuidor de cargas de trabajo, consulte [Información sobre filtros en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Prácticas recomendadas para configurar usuarios

* Como usuario que programa el trabajo para otros, debe tener el acceso y los permisos correctos para programar los recursos para el trabajo.

  Para obtener información sobre el acceso necesario para administrar la carga de trabajo de sus recursos en el Distribuidor de cargas de trabajo, consulte [Acceso necesario para administrar recursos en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Los usuarios cuya carga de trabajo desee administrar deben cumplir los siguientes criterios para que la información sobre su disponibilidad y aptitudes sea precisa:

   * Tener los horarios y los roles asociados a su perfil.

     Para obtener más información sobre cómo asociar horarios y roles a usuarios, consulte [Añadir usuarios](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Si un usuario no está asociado a un horario, el horario predeterminado de su sistema Workfront se asocia al usuario de forma predeterminada, a efectos de la gestión de recursos.
   * Tener las excepciones de horario actualizadas en sus horarios.

     Para obtener más información sobre la creación de programaciones, consulte [Crear programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Tener actualizado su calendario de días libres en el perfil.

     Para obtener información sobre la actualización del calendario de días libres de un usuario, consulte [Configurar los días libres personales](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* El administrador de Workfront debe determinar cómo calcula Workfront la disponibilidad del usuario. Puede decidir si Workfront utiliza el horario predeterminado del sistema o el horario del usuario para calcular el tiempo que el usuario está disponible para trabajar ajustando las preferencias de Administración de recursos en el área de Configuración de Workfront.

  Para obtener más información, consulte [Configurar las preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Prácticas recomendadas para configurar tareas y problemas {#best-practices-for-setting-up-tasks-and-issues}

Asegúrese de que existe la siguiente configuración de tareas y problemas antes de comenzar a asignar trabajo a los usuarios en el Distribuidor de cargas de trabajo:

* Las tareas principales no están asignadas a usuarios o roles. Las tareas principales no se muestran en el Distribuidor de cargas de trabajo.
* Las tareas y los problemas tienen un valor de horas planificadas mayor que cero.

* Las tareas y los problemas tienen un valor de Duración mayor que cero.
* Las fechas planificadas de los problemas se encuentran dentro de la cronología prevista del proyecto.

## Antes de empezar a utilizar el Distribuidor de cargas de trabajo

* Lea los siguientes artículos antes de empezar a utilizar el Distribuidor de cargas de trabajo:

   * En este artículo se explica cómo utilizar el Distribuidor de cargas de trabajo para realizar estas acciones: [Navegar por el Distribuidor de cargas de trabajo](../workload-balancer/navigate-the-workload-balancer.md).

   * En los siguientes artículos se explica cómo asignar trabajo y administrar asignaciones de usuarios:

      * [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../workload-balancer/assign-work-in-workload-balancer.md).
      * [Administrar asignaciones de usuario en el Distribuidor de cargas de trabajo](../workload-balancer/manage-user-allocations-workload-balancer.md).

* El Distribuidor de cargas de trabajo se puede encontrar en varias áreas diferentes de Workfront. Para obtener información sobre dónde puede encontrar el Distribuidor de cargas de trabajo, consulte [Buscar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Acceso necesario para utilizar el Distribuidor de cargas de trabajo

Para poder ver y utilizar el Distribuidor de cargas de trabajo en Workfront, debe tener el acceso correcto a Workfront y permisos para proyectos específicos. Para obtener información sobre el acceso necesario para utilizar el Distribuidor de cargas de trabajo, consulte el artículo [Acceso necesario para administrar recursos en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
