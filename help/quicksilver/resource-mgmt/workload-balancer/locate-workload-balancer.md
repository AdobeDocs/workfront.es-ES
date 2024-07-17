---
product-area: resource-management
keywords: trabajo, equipo, plantilla, recursos
navigation-topic: the-workload-balancer
title: Localización del Distribuidor de cargas de trabajo
description: Puede utilizar el Distribuidor de cargas de trabajo para programar los recursos para el trabajo o revisar su disponibilidad y las asignaciones actuales.
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# Localización del Distribuidor de cargas de trabajo


Puede utilizar el Distribuidor de cargas de trabajo para programar los recursos para el trabajo o revisar su disponibilidad y las asignaciones actuales.

Puede acceder al Distribuidor de cargas de trabajo de las siguientes maneras:

* De varias áreas predefinidas por Adobe Workfront
* Añadiéndolo a una sección personalizada

Este artículo describe las áreas en las que puede acceder al Distribuidor de cargas de trabajo.

>[!NOTE]
>
>Independientemente del método que utilice para acceder al Distribuidor de cargas de trabajo, es idéntico navegar por él y administrar recursos.
>
>Para obtener información sobre el Distribuidor de cargas de trabajo y cómo utilizarlo para administrar y programar los recursos para el trabajo, consulte los siguientes artículos:
>
>* [Resumen del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [Navegar por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)
>

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, al utilizar el Distribuidor de cargas de trabajo en el área de Recursos</p>
   <p>Trabaje con el Distribuidor de cargas de trabajo de un equipo o proyecto</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Vea o acceda a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Tareas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p><b> NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos o superiores de los proyectos, tareas y problemas </p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Acceso al Distribuidor de cargas de trabajo en áreas predefinidas

Las secciones siguientes ilustran dónde puede acceder al Distribuidor de cargas de trabajo dentro de Workfront.

### Acceso al Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) y luego haga clic en **Recursos**.
1. Haga clic en **Distribuidor de cargas de trabajo** en el panel izquierdo.

   ![](assets/nwe-balancer-global.png)

   El Distribuidor de cargas de trabajo muestra, de forma predeterminada, lo siguiente según la información del área de Recursos:

   * **Trabajo sin asignar**: no hay elementos de trabajo sin asignar.
   * **Trabajo asignado**: todos los usuarios activos en el sistema.

     Se recomienda utilizar filtros al mostrar los usuarios en el área de Trabajo asignado. Para obtener más información, consulte [Filtrar información en el Distribuidor de cargas de trabajo](../workload-balancer/filter-information-workload-balancer.md).

### Acceso al Distribuidor de cargas de trabajo para un equipo

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) y, a continuación, haga clic en Equipos.
Se muestra la página de su equipo de inicio.

   El Distribuidor de cargas de trabajo del equipo se muestra de forma predeterminada.

   ![](assets/nwe-balancer-team-350x172.png)

   El Distribuidor de cargas de trabajo de un equipo muestra la siguiente información de forma predeterminada:

   * **Trabajo sin asignar**: elementos asignados al equipo y no asignados a usuarios.
   * **Trabajo asignado**: todos los miembros del equipo con todas sus asignaciones.

     >[!TIP]
     >
     >Los integrantes del equipo pueden estar asignados a trabajos que también están asignados al equipo o a trabajos asignados a otros equipos o roles.



### Acceso al Distribuidor de cargas de trabajo para un proyecto

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) y luego haga clic en **Proyectos**.
1. Haga clic en el nombre de un proyecto para abrir su página.
1. Haga clic en **Distribuidor de cargas de trabajo** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más** y luego en **Distribuidor de cargas de trabajo**.

   Se muestra el Distribuidor de cargas de trabajo para el proyecto.

   ![](assets/nwe-balancer-project-350x152.png)

   El Distribuidor de cargas de trabajo de un proyecto muestra lo siguiente a modo de información de forma predeterminada:

   * **Trabajo sin asignar**: elementos del proyecto que están asignados a roles o equipos de trabajo y no están asignados a usuarios.
   * **Trabajo asignado**: usuarios asignados a elementos del proyecto.

     >[!TIP]
     >
     >Puede mostrar todos los usuarios del sistema en lugar de solo los del proyecto (en el área de Trabajo asignado) activando la opción Mostrar todos los usuarios. Para obtener más información, consulte [Navegar por el Distribuidor de cargas de trabajo](../workload-balancer/navigate-the-workload-balancer.md).


## Añadir el Distribuidor de cargas de trabajo a una sección personalizada

Puede agregar el Distribuidor de cargas de trabajo a cualquier sección personalizada.

La mayoría de las personalizaciones que ya se han aplicado al Distribuidor de cargas de trabajo se conservan al agregarlo a una sección personalizada.

1. Acceda al Distribuidor de cargas de trabajo en cualquiera de las siguientes áreas:

   * El área de recursos
   * Un equipo
   * Un proyecto

1. Obtenga un vínculo que se puede compartir y cópielo en el portapapeles tal como se describe en [Compartir el Distribuidor de cargas de trabajo con un vínculo](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. Cree un panel con una página externa como se describe en [Incrustar una página web externa en un panel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Utilice el vínculo que se puede compartir obtenido en el paso 2 para la página externa.

   <!--
      (NOTE: ensure this stays correct)
      -->

1. Cree una sección personalizada tal como se describe en [Cree fichas o secciones personalizadas](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) para colocar el tablero en la ficha personalizada.

   Al acceder al Distribuidor de cargas de trabajo desde la sección personalizada, puede verlo como si estuviera accediendo directamente desde una de sus áreas originales enumeradas en el paso 1.

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (Opcional) Comparta la pestaña personalizada en una plantilla de diseño como se describe en [Personalice el panel izquierdo con una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)


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