---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Administrar porcentaje de asignación de usuarios o roles en tareas
description: El porcentaje de asignación representa la cantidad de tiempo que un recurso asignado está planificado para trabajar en una tarea en un día. Es el porcentaje de un día laborable (según la programación del usuario o proyecto) al que se asigna un recurso a lo largo de la duración de la tarea.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/tpBEkOgTsJSJ-dk-gKZ6uLyCk4j4vP4nMIQ5-ciHMAI
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
source-wordcount: 444
ht-degree: 20%

---

# Administrar porcentaje de asignación de usuarios o funciones en tareas

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->


El porcentaje de asignación representa la cantidad de tiempo que un recurso asignado está planificado para trabajar en una tarea en un día. Es el porcentaje de un día laborable (según la programación del usuario o proyecto) al que se asigna un recurso a lo largo de la duración de la tarea.

Puede modificar el porcentaje de asignación cuando realice asignaciones avanzadas en una tarea.

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
   <p>Edite los permisos para actualizar el porcentaje de asignación en el cuadro Editar tarea.</p>
   <!--
   Not true anymore: 
   <p><b>NOTE</b></p>
   <p> You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a>.</p>
   -->
   </td>
  </tr>
 </tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones acerca de la modificación de asignaciones porcentuales para tareas

* De forma predeterminada, los usuarios tienen asignado el mismo porcentaje de tiempo a las tareas a las que están asignados.
* Solo puede modificar manualmente el porcentaje de asignación de los usuarios y las funciones de trabajo asignadas a las tareas cuando el tipo de duración de la tarea es Trabajo calculado o Condicionado por el esfuerzo.

  Para obtener más información, vea [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* No se puede modificar la asignación porcentual para los equipos asignados a tareas.
* No puede modificar la asignación porcentual para usuarios y roles asignados a problemas.

## Modificar la asignación de porcentaje de usuarios o roles para una tarea

1. Vaya a una tarea para cuyos recursos está cambiando la asignación porcentual.
1. Haga clic en el área **Asignaciones** del encabezado de la tarea y, a continuación, haga clic en **Avanzadas**.

1. Asegúrese de que el **Tipo de duración** de la tarea sea uno de los siguientes:

   * Trabajo calculado
   * Condicionada por el esfuerzo

   >[!TIP]
   >
   >* Para el tipo de duración de asignación calculada, Workfront usa la fórmula siguiente para calcular el porcentaje de asignación de cada usuario asignado: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Para el tipo de duración simple, puede estimar las horas asignadas a cada recurso, no el porcentaje de asignación.

1. Modifique el campo **Asignaciones** para cada usuario asignado a la tarea.

   Solo puede modificar el porcentaje de asignación para asignaciones de usuarios y funciones.

   No se puede modificar el porcentaje de asignación de un equipo asignado a una tarea.

   Puede ver una de estas pantallas en función del paquete de flujo de trabajo o Workfront de su organización.

   ![Modificar porcentaje de asignación](assets/advanced-assignments-allocation-percentage.png)

   ![Modificar porcentaje de asignación](assets/new-aa-allocation-by-percentage.png)

1. Haga clic en **Guardar**.
