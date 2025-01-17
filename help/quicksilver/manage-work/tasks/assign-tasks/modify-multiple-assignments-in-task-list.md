---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modificar varias asignaciones de usuario en una lista de tareas
description: Al administrar las asignaciones de tareas, puede modificarlas simultáneamente para varias tareas a la vez mediante la función de edición masiva en una lista de tareas.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 259fd0e3fdaa07bfdb0301d60bf0d9b1090b4ef7
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 100%

---

# Modificar varias asignaciones de usuario en una lista de tareas

<!--Audited: 07/2024-->

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Al administrar las asignaciones de tareas, puede modificarlas simultáneamente para varias tareas a la vez mediante la función de edición masiva en una lista de tareas.

Este artículo hace referencia a la modificación de varias asignaciones de usuario para varias tareas de una lista de tareas. Consulte también los siguientes artículos para modificar asignaciones en varias tareas de otras áreas:

* Para obtener información sobre la asignación de tareas mediante el Distribuidor de cargas de trabajo, consulte [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para obtener información sobre la asignación de una tarea a un recurso de una lista, consulte [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar</p>
   <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a proyectos y tareas</p> <p>Acceso de visualización o superior a los usuarios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de aportación o superiores a las tareas</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
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
1. (Opcional) Cree un filtro para mostrar solo las tareas asignadas al asignado que desea modificar.

   Por ejemplo, si el proyecto contiene una función específica como asignado predeterminado para varias tareas, puede crear un filtro para mostrar solo las tareas con esa función como asignado. A continuación, puede reemplazar la función por un usuario específico.

   Para obtener información sobre la creación de un filtro, consulte [Crear o editar filtros](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Para filtrar una función, seleccione **Funciones de asignación** y haga clic en **ID**.

   >[!TIP]
   >
   >No use el campo **Asignado a**. Encontrará el propietario principal de la tarea, en lugar de cualquiera de las funciones que se les pudieran asignar.

   O

   Para filtrar por un usuario, seleccione **Usuarios de asignación,** y luego haga clic en **ID.**

   >[!TIP]
   >
   >No use el campo **Asignado a**. Solo encontrará el propietario principal de la tarea en lugar de cualquiera de los usuarios que se les pudieran asignar.

1. Seleccione las tareas para las que desea modificar las asignaciones y, a continuación, haga clic en el icono de **Editar** ![](assets/edit-icon.png).

   Se muestra la página Editar tareas. Los elementos que edite se mostrarán en la esquina superior izquierda de la página.

1. Vaya a la sección **Asignaciones**.
1. Realice una de las siguientes acciones para añadir o quitar asignados:

   >[!IMPORTANT]
   >
   >La eliminación de asignados puede afectar a las horas de la tarea y a los porcentajes de asignación. Para obtener más información, consulte la sección [Cómo afecta la eliminación de asignados a las horas de la tarea y a los porcentajes de asignación](#how-removing-assignees-affects-task-hours-and-allocation-percentages) en este artículo.

   * Para añadir un nuevo usuario asignado:

      1. En la sección **Asignaciones**, seleccione **Asignado**.

         Se muestra la información que es común en todas las tareas seleccionadas. Por ejemplo, si se asigna el mismo usuario a todas las tareas, ese usuario se muestra en la columna **Asignado**. Si la información no es común en las tareas seleccionadas, no se muestra ninguna información.

      1. Empiece a escribir el nombre de un usuario, función o equipo y, a continuación, selecciónelo cuando aparezca en la lista. La asignación se añade y no reemplaza las asignaciones actuales en las tareas seleccionadas.


     >[!TIP]
     >
     > * Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos.
     >   
     > * Al añadir una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función para verla a medida que los añade. Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Si se asignó un usuario, una función o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
     >   
     >     * Reasignar el elemento de trabajo a los recursos activos.
     >     * Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.


   * Para quitar usuarios asignados individuales:

      1. Haga clic en el **icono X** junto al nombre del usuario asignado que desee eliminar si este aparece en la lista Asignaciones.

         O

         (Condicional) Si el usuario asignado que desea eliminar no aparece en la sección Asignaciones porque solo está asignado a algunas de las tareas que ha seleccionado, haga clic en **Quitar usuario asignado** y empiece a escribir el nombre del usuario asignado que desea eliminar; a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   * Para quitar todos los usuarios asignados existentes:

      1. Haga clic en **Quitar todos los usuarios asignados existentes** y, a continuación, en **Sí, eliminar todos los usuarios asignados**.

         De este modo se eliminan no solo los usuarios asignados comunes (los usuarios asignados que se muestran en el cuadro de diálogo de edición), sino también todos los usuarios asignados de todas las tareas seleccionadas.

     Eliminar usuarios de las tareas puede afectar a las horas de las tareas y a los porcentajes de asignación.

     Para obtener más información, consulte [Información general sobre la modificación de asignaciones de tareas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Opcional) Modifique cualquiera de las siguientes opciones para los usuarios asignados:

   * (Condicional) **Porcentaje de asignación de horas**: especifique un nuevo porcentaje de asignación de horas.

     >[!NOTE]
     >
     >Esta opción solo se puede modificar si el Tipo de duración es el mismo en todas las tareas que se están editando. Si el tipo de duración es Trabajo calculado o Condicionado por el esfuerzo, puede actualizar el porcentaje de asignación. Cuando el Tipo de duración es Simple, puede actualizar las Horas. Para obtener más información sobre los tipos de duración, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >Si el campo está en blanco, significa que el valor es diferente en las tareas; sin embargo, aún puede modificarlo.

   * **Propietario de la tarea**: seleccione esta opción para que el usuario asignado sea el propietario de la tarea para todas las tareas que se están editando.
   * **Función de usuario asignado**: seleccione una función de la lista desplegable. Si no se selecciona, Adobe Workfront selecciona automáticamente la función principal del usuario.

1. Haga clic en **Guardar cambios.**
