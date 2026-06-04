---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Administrar horas de asignación de usuarios y funciones en las tareas
description: Al asignar usuarios o funciones a una tarea, se les asigna trabajar un determinado número de horas para completar la tarea. Puede modificar manualmente la cantidad de horas que se asigna a cada usuario o rol cuando se le asigna una tarea, cuando el tipo de duración de la tarea es simple.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Jx-D1MY9dopkps0UqnE7Mgu4vlYevFjzRjRGWXDaWQQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 559
ht-degree: 78%

---

# Administrar horas de asignación de usuarios y funciones en las tareas

<!--Audited: 10/2025-->

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->


<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

Las horas de asignación representan la cantidad total de tiempo que un recurso asignado está planificado para trabajar en una tarea. Las horas representan el tiempo que se asigna a un usuario en un día determinado o en un día de la semana, una semana o un mes a lo largo de la duración de la tarea.

Puede modificar las horas de asignación cuando realice asignaciones avanzadas en una tarea.

>[!NOTE]
>
>Al asignar usuarios para trabajar, su disponibilidad según sus programaciones afecta a las fechas planificadas y proyectadas de las tareas y problemas. Para obtener información acerca de las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
   <p>Trabajo o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Editar acceso a Tareas</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td>
   <td><p>Contribuir o permisos superiores para la tarea</p>
   <p>Edite los permisos para actualizar las horas de asignación en el cuadro Editar tarea.</p> 
   <!--
   Not true anymore:
   <p><b>NOTE</b></p>
   <p>
   You can no longer manage allocation hours in the Edit task box when editing tasks in the new experience.</p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a>.</p>
   -->
   </td>
  </tr>
 </tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones para modificar las horas de asignación de una tarea

>[!IMPORTANT]
>
>Después de modificar manualmente las asignaciones para cada tarea, las horas planificadas de las tareas podrían actualizarse en consecuencia. Para obtener más información, consulte la sección [Actualizar las horas planificadas de una tarea al administrar las asignaciones de usuario](../../../manage-work/tasks/task-information/planned-hours.md#update) en el artículo [Información general de Horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

* El total de horas asignadas a recursos individuales asignados a la tarea representa las horas planificadas de la tarea.
* Si hay un usuario o una asignación de rol en una tarea, la cantidad de horas asignadas al usuario o rol coincide con las Horas planificadas de la tarea.
* En el caso de múltiples asignaciones, a cada usuario o rol de trabajo se le asigna, de forma predeterminada, la misma cantidad de horas para trabajar en la tarea, si el tipo de duración de la tarea es simple. Para obtener más información, consulte los siguientes artículos:

   * [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Información general del tipo de duración: simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Cuando la tarea tiene un tipo de duración simple, puedes cambiar manualmente la cantidad de horas asignadas a cada usuario o rol de trabajo para indicar que algunos de los asignados a la tarea podrían tener más tiempo para trabajar en ella que otros.
* No se puede modificar la cantidad de horas asignadas a los equipos asignados a las tareas.
* No puede modificar manualmente la asignación de usuarios o funciones para los problemas.
* También puede administrar las asignaciones diarias, semanales o mensuales de usuarios a tareas o problemas mediante el Distribuidor de cargas de trabajo. Para obtener más información, consulte [Administrar asignaciones de usuario en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modificar las horas de asignación de usuarios o funciones de una tarea

1. Vaya a una tarea cuyas asignaciones desee cambiar las horas de asignación.
1. Haga clic en el área **Asignaciones** del encabezado de la tarea y, a continuación, haga clic en **Avanzadas**.
1. Asegúrese de que el **Tipo de duración** de la tarea sea **Simple**.
1. Modifique el campo **Asignaciones** para cada usuario asignado a la tarea. Son asignaciones generales para cada asignación a esta tarea, para toda la duración de la tarea. Esto también podría actualizar las **horas planificadas** generales de la tarea.

   Puede ver una de estas pantallas en función del paquete de flujo de trabajo o Workfront de su organización.

   ![Modificar asignaciones](assets/advanced-assignments-duration-type-allocations.png)

   ![Modificar asignaciones](assets/new-aa-allocation-by-hour.png)

1. Haga clic en **Guardar**.
