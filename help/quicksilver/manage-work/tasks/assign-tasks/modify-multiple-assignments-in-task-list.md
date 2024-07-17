---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modificar varias asignaciones de usuario en una lista de tareas
description: Al administrar las asignaciones de tareas, puede modificarlas simultáneamente para varias tareas a la vez mediante la función de edición masiva en una lista de tareas.
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# Modificar varias asignaciones de usuario en una lista de tareas

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Al administrar las asignaciones de tareas, puede modificarlas simultáneamente para varias tareas a la vez mediante la función de edición masiva en una lista de tareas.

Este artículo hace referencia a la modificación de varias asignaciones de usuario para varias tareas en una lista de tareas. Consulte también los siguientes artículos para modificar asignaciones en varias tareas de otras áreas:

* Para obtener información acerca de cómo asignar tareas mediante el Distribuidor de cargas de trabajo, vea [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para obtener información acerca de cómo asignar una tarea a un recurso de una lista, vea [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

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
   <td> <p>Editar acceso a Proyectos y tareas</p> <p>Acceso de visualización o superior a los usuarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribute o permisos superiores para tareas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Modificar asignaciones para varias tareas

1. Vaya a la lista que contiene las tareas en las que desea modificar asignaciones.
1. (Opcional) Cree un filtro para mostrar solo las tareas asignadas al usuario asignado que desea modificar.

   Por ejemplo, si el proyecto contiene una función específica como el usuario asignado predeterminado para varias tareas, puede crear un filtro para mostrar solo las tareas con esa función como el usuario asignado. A continuación, puede reemplazar la función por un usuario específico.

   Para obtener información sobre cómo crear un filtro, consulte [Crear o editar filtros](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Para filtrar un rol, seleccione **Roles de asignación** y haga clic en **ID**.

   >[!TIP]
   >
   >No use el campo **Asignado a**. Esto solo encuentra el propietario principal de la tarea, en lugar de cualquiera de las funciones que se les pudieran asignar.

   O

   Para filtrar por un usuario, seleccione **Usuarios de asignación,** y luego haga clic en **ID.**

   >[!TIP]
   >
   >No use el campo **Asignado a**. Esto solo encuentra el Propietario principal de la tarea en lugar de cualquiera de los usuarios que se les podrían asignar.

1. Seleccione las tareas para las que desea modificar las asignaciones y, a continuación, haga clic en el icono **Editar** ![](assets/edit-icon.png).

   Se muestra la página Editar tareas. Los elementos que edite se mostrarán en la esquina superior izquierda de la página.

1. Vaya a la sección **Asignaciones**.
1. Realice una de las siguientes acciones para agregar o quitar usuarios asignados:

   >[!IMPORTANT]
   >
   >La eliminación de usuarios asignados puede afectar a las horas de tarea y a los porcentajes de asignación. Para obtener más información, vea la sección [Cómo afecta la eliminación de usuarios asignados a las horas de tareas y a los porcentajes de asignación](#how-removing-assignees-affects-task-hours-and-allocation-percentages) en este artículo.

   * Para agregar un nuevo usuario asignado:

      1. En la sección **Asignaciones**, seleccione **Usuario asignado**.

         Se muestra la información que es común en todas las tareas seleccionadas. Por ejemplo, si se asigna el mismo usuario a todas las tareas, ese usuario se muestra en la columna **Usuario asignado**. Si la información no es común en las tareas seleccionadas, no se muestra ninguna información.

      1. Empiece a escribir el nombre de un usuario, rol o equipo y, a continuación, selecciónelo cuando aparezca en la lista. La asignación se agrega y no reemplaza las asignaciones actuales en las tareas seleccionadas.


     >[!TIP]
     >
     > * Puede asignar varios usuarios, roles o equipos. Solo puede asignar usuarios activos, roles y equipos.
     >   
     > * Al agregar una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos un rol para verlo a medida que los agregue. Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Si se asignó un usuario, un rol o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
     >   
     >     * Reasignar el elemento de trabajo a los recursos activos.
     >     * Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.


   * Para eliminar usuarios asignados individuales:

      1. Haga clic en el **icono X** junto al nombre del usuario asignado que desee eliminar si este aparece en la lista Asignaciones.

         O

         (Condicional) Si el usuario asignado que desea eliminar no aparece en la sección Asignaciones porque el usuario asignado solo está asignado a algunas de las tareas que ha seleccionado, haga clic en **Quitar usuario asignado** y empiece a escribir el nombre del usuario asignado que desea eliminar; a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   * Para eliminar todas las personas asignadas actualmente:

      1. Haga clic en **Quitar todas las personas asignadas existentes** y, a continuación, haga clic en **Sí, eliminar todas las personas asignadas**.

         Esto elimina no solo los usuarios asignados comunes (los usuarios asignados que se muestran en el cuadro de diálogo de edición), sino también todos los usuarios asignados de todas las tareas seleccionadas.

     La eliminación de usuarios de las tareas puede afectar a las horas de tareas y a los porcentajes de asignación.

     Para obtener más información, vea [Información general sobre la modificación de asignaciones de tareas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Opcional) Modifique cualquiera de las siguientes opciones para los usuarios asignados:

   * (Condicional) **Porcentaje de asignación de horas**: especifique un nuevo porcentaje de asignación de horas.

     >[!NOTE]
     >
     >Esta opción solo se puede modificar si el Tipo de duración es el mismo en todas las tareas que se están editando. Si el tipo de duración es Trabajo calculado o Condicionado por el esfuerzo, puede actualizar el porcentaje de asignación. Cuando el Tipo de duración es Simple, puede actualizar las Horas. Para obtener información acerca del tipo de duración, vea [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >Si el campo está en blanco, significa que el valor es diferente en las tareas; sin embargo, aún puede modificarlo.

   * **Propietario de la tarea**: seleccione esta opción para que el usuario asignado sea el propietario de la tarea para todas las tareas que se están editando.
   * **Rol de asignado**: seleccione un rol de la lista desplegable. Si no se selecciona, Adobe Workfront selecciona automáticamente la función principal del usuario.

1. Haga clic en **Guardar cambios.**
