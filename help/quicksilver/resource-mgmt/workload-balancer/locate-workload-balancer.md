---
product-area: resource-management
keywords: trabajo,equipo,dotación de personal,recursos
navigation-topic: the-workload-balancer
title: Localizar el equilibrador de carga de trabajo
description: Puede utilizar el equilibrador de carga de trabajo para programar recursos para el trabajo o revisar su disponibilidad y las asignaciones actuales.
author: Alina
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 87f02f3908c86575ca2dfacd7d88146b9967a804
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 1%

---

# Localizar el equilibrador de carga de trabajo


Puede utilizar el equilibrador de carga de trabajo para programar recursos para el trabajo o revisar su disponibilidad y las asignaciones actuales.

Puede acceder al equilibrador de carga de trabajo de las siguientes maneras:

* Desde varias áreas predefinidas por Adobe Workfront
* Añadirlo a una sección personalizada

Este artículo describe las áreas en las que puede acceder al equilibrador de carga de trabajo.

>[!NOTE]
>
>Independientemente del método que utilice para acceder al equilibrador de carga de trabajo, navegarlo y administrar recursos es idéntico.
>
>Para obtener información sobre el equilibrador de carga de trabajo y cómo utilizarlo para administrar y programar sus recursos para el trabajo, consulte los siguientes artículos:
>
>* [Información general del equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [Información general sobre la asignación de trabajo en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)
>


## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, al utilizar el equilibrador de carga de trabajo para un equipo o en el área de recursos </p>
   <p>Trabajar, al utilizar el equilibrador de carga de trabajo de un proyecto </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver o acceso superior a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Tareas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p><b> NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos o superiores de proyectos, tareas y problemas </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Acceso al equilibrador de carga de trabajo en áreas predefinidas

Las siguientes secciones ilustran dónde puede acceder al equilibrador de carga de trabajo dentro de Workfront.

### Acceso al equilibrador de carga de trabajo para varios proyectos en el área de recursos

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)y haga clic en **Recurso**.
1. Haga clic en **Equilibrador de carga de trabajo** en el panel izquierdo.

   ![](assets/nwe-balancer-global.png)

   El equilibrador de carga de trabajo muestra lo siguiente por información en el área Recursos, de forma predeterminada:

   * **Trabajo no asignado**: No hay elementos de trabajo sin asignar.
   * **Trabajo asignado**: Todos los usuarios activos del sistema.

      Se recomienda utilizar filtros al mostrar a los usuarios en el área Trabajo asignado . Para obtener más información, consulte [Filtrar información en el equilibrador de carga de trabajo](../workload-balancer/filter-information-workload-balancer.md).

### Acceso al equilibrador de carga de trabajo para un equipo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)y, a continuación, haga clic en Equipos.
Se muestra la página de su equipo de inicio.

   El equilibrador de carga de trabajo del equipo se muestra de forma predeterminada.

   ![](assets/nwe-balancer-team-350x172.png)

   El equilibrador de carga de trabajo de un equipo muestra la siguiente información de forma predeterminada:

   * **Trabajo no asignado**: Elementos asignados al equipo y no asignados a usuarios.
   * **Trabajo asignado**: Todos los miembros del equipo con todas sus tareas.

      >[!TIP]
      >
      >Los integrantes del equipo podrían asignarse a trabajos también asignados al equipo o a trabajos asignados a otros equipos o funciones.



### Acceso al equilibrador de carga de trabajo para un proyecto

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)y haga clic en **Proyectos**.
1. Haga clic en el nombre de un proyecto para abrir la página del proyecto.
1. Haga clic en **Equilibrador de carga de trabajo** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más**, luego **Equilibrador de carga de trabajo**.

   Se muestra el equilibrador de carga de trabajo para el proyecto.

   ![](assets/nwe-balancer-project-350x152.png)

   El equilibrador de carga de trabajo de un proyecto muestra lo siguiente por información, de forma predeterminada:

   * **Trabajo no asignado**: Los elementos del proyecto que están asignados a roles de trabajo o equipos y no están asignados a usuarios.
   * **Trabajo asignado**: Usuarios asignados a elementos del proyecto.

      >[!TIP]
      >
      >Puede mostrar todos los usuarios del sistema en lugar de solo los del proyecto (en el área Trabajo asignado) activando la opción Mostrar todos los usuarios . Para obtener más información, consulte [Navegar por el equilibrador de carga de trabajo](../workload-balancer/navigate-the-workload-balancer.md).


## Agregar el equilibrador de carga de trabajo a una sección personalizada

Puede agregar el equilibrador de carga de trabajo a cualquier sección personalizada.

La mayoría de las personalizaciones que ya ha aplicado al equilibrador de carga de trabajo se conservan al agregarlo a una sección personalizada.

1. Acceda al equilibrador de carga de trabajo yendo a cualquiera de las siguientes áreas:

   * El área de recursos
   * Un equipo
   * Un proyecto

1. Obtenga un vínculo que se pueda compartir y cópielo en el portapapeles como se describe en [Uso compartido de Workload Balancer con un vínculo](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. Cree un tablero con una página externa como se describe en [Incrustar una página web externa en un panel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Utilice el vínculo que se puede compartir en el paso 2 para la página externa.

   <!--
      (NOTE: ensure this stays correct)
      -->

1. Cree una sección personalizada como se describe en [Crear fichas o secciones personalizadas](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) para colocar el tablero en la ficha personalizada.

   Al acceder al equilibrador de carga de trabajo desde la sección personalizada, puede verlo como si estuviera accediendo a él directamente desde una de sus áreas originales enumeradas en el paso 1.

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (Opcional) Comparta la ficha personalizada en una plantilla de diseño como se describe en  [Personalización del panel izquierdo mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) .


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->