---
product-area: projects
navigation-topic: plan-a-project
title: Ver horas planificadas del proyecto en el panel Asignación de funciones
description: Puede ver la asignación de funciones para todos los roles asignados a elementos de trabajo en un proyecto en el panel Asignación de funciones del proyecto.
author: Alina, Lisa
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 14%

---

# Ver horas planificadas del proyecto en el panel Asignación de funciones

Puede ver la asignación de funciones para todos los roles asignados a elementos de trabajo en un proyecto en el panel Asignación de funciones del proyecto.

>[!NOTE]
>
>Este artículo hace referencia a la visualización de las funciones del puesto asociadas con las tareas y los problemas de un proyecto y a las horas planificadas asignadas en el panel Asignación de funciones de un proyecto. Para obtener información sobre la reconciliación de horas planificadas con horas de iniciativas mediante el panel Asignación de funciones cuando se utiliza el planificador de escenarios de Adobe Workfront, consulte lo siguiente:
>
>* [Mostrar la asignación de funciones para proyectos e iniciativas en la lista de tareas](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Mostrar la asignación de funciones para proyectos e iniciativas en el Distribuidor de cargas de trabajo](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Debe tener una licencia de Scenario Planner para ver las horas de iniciativa en el panel Asignación de funciones. Para obtener información acerca del Planificador de escenarios, vea [Introducción al Planificador de escenarios](../../../scenario-planner/get-started-with-scenario-planning.md).
>
>Si su empresa ha comprado el Scenario Planner de Adobe en el pasado, se le ha otorgado la licencia de propietario. El planificador de escenarios ya no está disponible para adquirir.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Adobe Workfront Ultimate</p>
   <p>Adobe Workflow Ultimate</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Ligero o superior</p>
   <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a los proyectos</p>
   <p>Editar acceso al Scenario Planner para actualizar las horas de las iniciativas</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores en el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

able style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
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
</table>-->

## Requisitos previos

Debe tener lo siguiente:

* Tareas o problemas asignados a roles o usuarios asociados a un rol.

  >[!TIP]
  >
  >Si las tareas o los problemas no están asignados, están asignados a equipos o están asignados a usuarios sin un rol, las horas planificadas del proyecto son cero en el panel Asignación de rol.

* Tareas y problemas con una duración superior a cero.

## Ver horas planificadas del proyecto en el panel Asignación de funciones

1. Haga clic en el icono **Menú principal** ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Proyectos**.
1. Haga clic en el nombre de un proyecto para acceder a él. Se abrirá la página Proyecto.
1. Haga clic en una de las siguientes opciones del panel izquierdo:

   * **Tareas**
   * **Distribuidor de cargas de trabajo**

1. Haga clic en el icono **Mostrar asignación de funciones** ![Mostrar icono de asignación de funciones](assets/show-role-allocation-icon.png).

   Se muestra el panel Asignación de funciones.

   ![Panel de asignación de funciones con solo horas planificadas](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Revise la siguiente información en el panel **Asignación de funciones**:

   | Campo | Descripción |
   |---|---|
   | **Función** | Funciones del puesto asignadas a tareas y problemas del proyecto. Pueden ser funciones del puesto asignadas directamente a tareas y problemas o funciones del puesto asociadas a usuarios asignados a tareas y problemas del proyecto. |
   | **Horas planificadas** | Número total de horas planificadas de tareas y problemas asignados a roles de trabajo o usuarios asociados a un rol en el proyecto. |

