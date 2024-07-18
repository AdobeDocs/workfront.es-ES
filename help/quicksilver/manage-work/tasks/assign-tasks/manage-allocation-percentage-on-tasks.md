---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Administrar porcentaje de asignación de usuarios o funciones en tareas
description: El porcentaje de asignación representa la cantidad de tiempo que un recurso asignado está planificado para trabajar en una tarea en un día. Es el porcentaje de un día laborable (según la programación del usuario o proyecto) al que se asigna un recurso a lo largo de la duración de la tarea.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: dd015fc356f65cc3d00a1c88ca0a8f2268283606
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---

# Administrar porcentaje de asignación de usuarios o funciones en tareas

El porcentaje de asignación representa la cantidad de tiempo que un recurso asignado está planificado para trabajar en una tarea en un día. Es el porcentaje de un día laborable (según la programación del usuario o proyecto) al que se asigna un recurso a lo largo de la duración de la tarea.

>[!NOTE]
>
>Al asignar usuarios para trabajar, su disponibilidad según sus programaciones afecta a las Fechas planificadas y proyectadas de las tareas y problemas. Para obtener información acerca de las programaciones, vea [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribute o permisos superiores para la tarea</p> <p>Editar permisos para actualizar el porcentaje de asignación en el cuadro Editar tarea</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones acerca de la modificación de asignaciones porcentuales para tareas

* De forma predeterminada, los usuarios tienen asignado el mismo porcentaje de tiempo a las tareas a las que están asignados.
* Solo puede modificar manualmente el porcentaje de asignación de los usuarios y las funciones de trabajo asignadas a las tareas cuando el tipo de duración de la tarea es Trabajo calculado o Condicionado por el esfuerzo.

  Para obtener más información, vea [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* No se puede modificar la asignación porcentual para los equipos asignados a tareas.
* No puede modificar la asignación porcentual para usuarios y roles asignados a problemas.

## Modificar la asignación de porcentaje de usuarios o roles para una tarea

1. Vaya a una tarea para cuyos recursos está cambiando la asignación porcentual.
1. Haga clic en el menú **Más** ![](assets/qs-more-icon-on-an-object.png) junto al nombre de la tarea y, a continuación, haga clic en **Editar**.

   O

   Haga clic en el área **Asignaciones** del encabezado de la tarea y, a continuación, haga clic en **Avanzadas**.

1. Asegúrese de que el **Tipo de duración** de la tarea sea uno de los siguientes:

   * Trabajo calculado
   * Condicionada por el esfuerzo

   >[!TIP]
   >
   >* Para el tipo de duración de asignación calculada, Workfront usa la fórmula siguiente para calcular el porcentaje de asignación de cada usuario asignado: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Para el tipo de duración simple, puede estimar las horas asignadas a cada recurso, no el porcentaje de asignación.

1. Haga clic en **Asignaciones** y, a continuación, modifique las **Asignaciones** para cada usuario asignado a la tarea.

   Solo puede modificar el porcentaje de asignación para asignaciones de usuarios y funciones.

   No se puede modificar el porcentaje de asignación de un equipo asignado a una tarea.

   ![Modificar porcentaje de asignación](assets/advanced-assignments-allocation-percentage.png)

1. Haga clic en **Guardar**.
