---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Administrar el porcentaje de asignación de usuarios o funciones en tareas
description: El porcentaje de asignación representa la cantidad de tiempo que un recurso asignado está planificado para trabajar en una tarea en un día. Es el porcentaje de un día laborable (según la programación del usuario o del proyecto) en el que se asigna un recurso durante toda la tarea.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---

# Administrar el porcentaje de asignación de usuarios o funciones en tareas

El porcentaje de asignación representa la cantidad de tiempo que un recurso asignado está planificado para trabajar en una tarea en un día. Es el porcentaje de un día laborable (según la programación del usuario o del proyecto) en el que se asigna un recurso durante toda la tarea.

>[!NOTE]
>
>Al asignar usuarios al trabajo, su disponibilidad según sus programaciones afecta a las Fechas planificadas y proyectadas de las tareas y los problemas. Para obtener información sobre las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribute o permisos superiores para la tarea</p> <p>Editar permisos para actualizar el porcentaje de asignación en el cuadro Editar tarea</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre la modificación de las asignaciones porcentuales para las tareas

* De forma predeterminada, los usuarios tienen asignado un porcentaje de tiempo igual a las tareas a las que están asignados.
* Puede modificar manualmente el porcentaje de asignación para usuarios y las funciones de trabajo asignadas a tareas solo cuando el tipo de duración de la tarea es Trabajo calculado o Función del esfuerzo.

   Para obtener más información, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* No puede modificar la asignación porcentual para los equipos asignados a tareas.
* No puede modificar la asignación porcentual para usuarios y las funciones de trabajo asignadas a problemas.

## Modificación de la asignación de porcentaje de usuario o función para una tarea

1. Vaya a una tarea para cuyos recursos esté cambiando la asignación porcentual.
1. Haga clic en el **Más** menú ![](assets/qs-more-icon-on-an-object.png) junto al nombre de la tarea y, a continuación, haga clic en **Editar**.

   O

   Haga clic en el **Asignaciones** en el encabezado de la tarea y haga clic en **Avanzadas**.

1. Asegúrese de que la variable **Tipo de duración** de la tarea es una de las siguientes:

   * Trabajo calculado
   * Condicionada por el esfuerzo

   >[!TIP]
   >
   >* Para el Tipo de duración de asignación calculada, Workfront utiliza la fórmula siguiente para calcular el porcentaje de asignación de cada usuario asignado: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Para el tipo de duración simple, puede calcular las horas asignadas a cada recurso, no el porcentaje de asignación.


1. Haga clic en **Asignaciones** y, a continuación, modifique el **Asignaciones** para cada tarea asignada.

   Solo puede modificar el porcentaje de asignación para asignaciones de funciones de usuario y de trabajo.

   No puede modificar el porcentaje de asignación de un equipo asignado a una tarea.

   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. Haga clic en **Guardar**.
