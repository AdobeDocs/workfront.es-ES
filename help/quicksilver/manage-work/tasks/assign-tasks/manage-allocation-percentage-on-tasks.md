---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Administrar porcentaje de asignación de usuarios o roles en tareas
description: El porcentaje de asignación representa la cantidad de tiempo que un recurso asignado está planificado para trabajar en una tarea en un día. Es el porcentaje de un día laborable (según la programación del usuario o proyecto) al que se asigna un recurso a lo largo de la duración de la tarea.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 18%

---

# Administrar porcentaje de asignación de usuarios o funciones en tareas

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<div class="preview">

La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Las mismas funciones también estarán disponibles en el entorno de producción para todos los clientes a partir de una semana desde la versión de vista previa.

Para obtener más información, vea [Modernización de la interfaz](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>


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
   <td>paquete de Adobe Workfront</td> 
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
   <p>Editar permisos para actualizar el porcentaje de asignación en el cuadro Editar tarea al <span class="preview"> editar tareas utilizando la experiencia anterior. Ya no puede administrar el porcentaje de asignación en el cuadro de diálogo Editar tarea al editar tareas en la nueva experiencia.</span></p> <p>Para obtener más información, consulte <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Editar tareas</a>.</p></td>
  </tr>
 </tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation percentage in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.
-->

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

   ![Modificar porcentaje de asignación](assets/advanced-assignments-allocation-percentage.png)

1. Haga clic en **Guardar**.
