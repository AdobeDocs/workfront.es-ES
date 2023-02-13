---
product-area: projects
navigation-topic: plan-a-project
title: Ver las horas planificadas del proyecto en el panel Asignación de funciones
description: Puede ver la asignación de funciones para todas las funciones de trabajo asignadas a elementos de trabajo en un proyecto en el panel Asignación de funciones del proyecto.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Ver las horas planificadas del proyecto en el panel Asignación de funciones

Puede ver la asignación de funciones para todas las funciones de trabajo asignadas a elementos de trabajo en un proyecto en el panel Asignación de funciones del proyecto.

>[!NOTE]
>
>Este artículo se refiere a la visualización de las funciones de trabajo asociadas con tareas y problemas en un proyecto y sus horas planificadas asignadas en el panel Asignación de funciones de un proyecto. Para obtener información sobre la conciliación de horas planificadas con horas de iniciativas mediante el panel Asignación de funciones al utilizar el planificador de escenario de Adobe Workfront, consulte lo siguiente:
>
>* [Mostrar la asignación de funciones para proyectos e iniciativas en la lista de tareas](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Mostrar la asignación de funciones para proyectos e iniciativas en el equilibrador de carga de trabajo](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Debe tener una licencia de Planificador de escenario para ver las horas de iniciativa en el panel Asignación de funciones. Para obtener información sobre el planificador de escenarios, consulte [Introducción al planificador de escenarios](../../../scenario-planner/get-started-with-scenario-planning.md) .

## Requisitos de acceso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Debe tener lo siguiente:

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
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver o acceder más a Proyectos</p> <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores en el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe tener lo siguiente:

* Tareas o problemas asignados a funciones de trabajo o a usuarios asociados a una función de trabajo.

   >[!TIP]
   Si las tareas o los problemas no están asignados, asignados a equipos o están asignados a usuarios sin función de trabajo, las horas planificadas del proyecto son cero en el panel Asignación de funciones.

* Tareas y problemas con una duración mayor que cero.

## Ver las horas planificadas del proyecto en el panel Asignación de funciones

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Proyectos**.
1. Haga clic en el nombre de un proyecto para acceder a él. Se abre la página Proyecto .
1. Haga clic en una de las siguientes opciones del panel izquierdo:

   * **Tareas**
   * **Distribuidor de cargas de trabajo**

1. Haga clic en el **Mostrar asignación de funciones** icono ![](assets/show-role-allocation-icon.png).

   Se muestra el panel Asignación de funciones .

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Revise la siguiente información en la sección **Asignación de funciones** panel: |Campo | Descripción| |—|—| | **Función del trabajo** |Funciones de trabajo asignadas a tareas y problemas en el proyecto. Pueden ser funciones de trabajo asignadas directamente a tareas y problemas o funciones de trabajo asociadas con usuarios asignados a tareas y problemas en el proyecto.  | | **Horas planificadas** |El número total de horas planificadas de tareas y problemas asignados a funciones de trabajo o usuarios asociados a una función de trabajo en el proyecto. |



