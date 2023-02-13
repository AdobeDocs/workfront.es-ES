---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: Ver las horas disponibles, planificadas y reales o FTE en el Planificador de recursos al utilizar la vista Usuario
description: Ver Horario Disponible, Planificado y Real o FTE en el Planificador de Recursos cuando se utiliza la Vista de Usuario "Planificación" en el RP" - tal vez "Recursos de Presupuestación en el RP" o "Gestión de Recursos en el RP". etc... - ¡¿o podría ser necesario reutilizar desde otro PDV?!)"
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 1%

---

# Ver las horas disponibles, planificadas y reales o FTE en el Planificador de recursos al utilizar la vista Usuario

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

Además de presupuestar recursos en las vistas Proyecto y Función, puede utilizar la Vista de usuario del Planificador de recursos de Adobe Workfront para mostrar información sobre los valores de horas planificadas, disponibles y reales o FTE para proyectos y recursos.

## Información general sobre la vista del usuario en el planificador de recursos

Tenga en cuenta lo siguiente cuando vea la información de horas o de TLC en el Planificador de recursos:

* Puede ver la información Horario disponible y planificado o la información de FTE para usuarios, funciones de trabajo y proyectos en todas las vistas del Planificador de recursos.
* Solo puede ver la siguiente información en la Vista de usuario:

   * La diferencia entre la cantidad de horas planificadas o FTE y la cantidad de horas disponibles o FTE. A continuación, puede presupuestar la asignación de los usuarios según esta diferencia en las vistas Proyecto y Función.
   * Las horas reales o FTE.

* Puede mostrar la diferencia entre el Usuario disponible y la cantidad de horas planificadas o FTE como un número o como un valor de porcentaje en la vista Usuario.
* No puede mostrar la información en la vista Usuario por Coste.
* Adobe Workfront rellena las horas disponibles o los FTE según el tiempo de trabajo asociado a los usuarios en sus programaciones.\
   Los usuarios que no están asociados a una programación muestran disponibilidad según la programación predeterminada.\
   Para obtener información sobre la programación predeterminada, consulte [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront rellena las horas planificadas o los FTE a partir de la información de horas planificadas sobre las tareas y los problemas de los proyectos.
* Workfront rellena las horas reales con el tiempo real registrado en las tareas y los problemas por los usuarios asignados a ellas. Esto incluye el tiempo registrado en un proyecto.
* En la vista Usuario, puede hacer lo siguiente:

   * Expanda cada usuario para mostrar una lista de proyectos a los que se asigna ese usuario.

      >[!NOTE]
      >
      >Solo se pueden expandir los usuarios asociados a los proyectos incluidos en los filtros.

   * Expanda cada proyecto para mostrar una lista de las funciones de trabajo que el usuario puede desempeñar en esos proyectos.
   * Expanda cada función para mostrar una lista de las tareas a las que está asignado el usuario con esa función.

   Si los usuarios no tienen ninguna función de trabajo asociada a ellos, sus horas disponibles, programadas y reales o FTE se enumeran en el **Sin función** para obtener más información.\
   Para obtener información sobre los campos y elementos que se muestran al aplicar la vista Usuario al Planificador de recursos, consulte la sección &quot;Proyecto/Función/Selección de vista de usuario&quot; en [Información general sobre navegación del planificador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Descripción general de los campos visibles en la Vista del usuario del planificador de recursos

Consulte las siguientes tablas para comprender la información mostrada en la vista Usuario del Planificador de Recursos. La información se muestra en valores Horas o FTE.

* [La columna AVL (disponible)](#the-avl-available-column)
* [La columna PLN (Planificado)](#the-pln-planned-column)
* [La columna ACT (real)](#The%C2%A0ACT)
* [La columna DIF (Diferencia)](#the-dif-difference-column)
* [La columna % (porcentaje de asignación de horas planificadas)](#the-planned-hours-allocation-percentage-column)

### La columna AVL (disponible) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td> <p><strong>Descripción</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td>El total de horas disponibles o FTE para el usuario según su programación. </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>Esta información no está disponible para el proyecto al aplicar la vista Usuario al planificador de recursos. </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>El total de horas disponibles o FTE para la función según la programación del usuario y la <strong>Porcentaje de disponibilidad de FTE</strong> de la función.</p> </td> 
  </tr> 
  <tr> 
   <td>Tarea o problema</td> 
   <td>Esta información no está disponible para la tarea o el problema. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre cómo se calcula la disponibilidad de usuarios y funciones en función de la programación del usuario y el porcentaje de disponibilidad de FTE de la función, consulte [Descripción general del cálculo de horas y FTE para usuarios y funciones en el planificador de recursos](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### La columna PLN (Planificado) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td> <p><strong>Descripción</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> El total de horas planificadas o FTE de todas las tareas o problemas asignados al usuario en todos los proyectos.<br><p>Esto incluye tareas y problemas que están asignados al usuario pero no están asociados a ninguna función de trabajo ni tareas o problemas que no están en proyectos a los que tiene acceso en Administrar.</p><p>Cuando se modifica la asignación de usuario durante horas mediante el equilibrador de carga de trabajo, los datos del planificador de recursos pueden verse afectados si las fechas seleccionadas contienen solo una parte de una tarea o problema. Para obtener información sobre cómo modificar las asignaciones para los usuarios, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Administrar asignaciones de usuario en el equilibrador de carga de trabajo</a> . </p></td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td> El total de horas planificadas o FTE de todas las tareas y problemas asignados a un usuario específico del proyecto.<br><p>Nota: Esto no incluye el horario planificado ni el tiempo de espera de las tareas o problemas que no están asignados a ningún usuario. </p></td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>El total de horas planificadas o FTE de todas las tareas y problemas asignados al usuario en esta función del proyecto.</p> <p> <p>Nota: Esto no incluye las horas planificadas o los FTE de las tareas o problemas asignados a esta función, pero no a este usuario en esta función. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tarea o problema</td> 
   <td>Las horas planificadas o los FTE asociados con la tarea o el problema en el proyecto.</td> 
  </tr> 
 </tbody> 
</table>

Tenga en cuenta lo siguiente al ver las horas planificadas:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* Las horas planificadas se distribuyen de forma equitativa a cada día dentro de la Duración de las tareas y los problemas , para cada recurso que se les asigne. La duración de la tarea o del problema se basa en sus fechas de inicio y finalización planificadas e incluye todos los días del calendario dentro de ese período de tiempo.\
   Workfront tiene en cuenta la programación del usuario o del proyecto al distribuir Horario planificado a usuarios o proyectos. En este caso, las horas planificadas se distribuyen por igual a cada día dentro de la Duración de tareas o problemas, excluyendo los fines de semana, los días de descanso y las excepciones de programación.

   Si, por ejemplo, muestra el Planificador de recursos por semana y tiene tareas que abarcan varias semanas en los proyectos, el número de horas planificadas por semana depende de cuántos días dentro de esa semana formen parte de la duración de la tarea. Esto funciona de manera similar cuando se muestra el Planificador de recursos por mes o trimestre y cuando las tareas abarcan varios meses o trimestres.\
   Los días de fin de semana, las excepciones de programación y los días de tiempo libre se excluyen de esta distribución.

* Las siguientes categorías de tareas se incluyen en el cálculo de las horas planificadas para cada recurso:

   * tareas asignadas a usuarios en grupos de recursos, funciones de trabajo o equipos en el proyecto.

      >[!TIP]
      >
      >Si las tareas están asignadas a equipos, su asignación aparecerá en **Sin función** y **Sin usuario** secciones. Puede ver las horas planificadas asociadas con los equipos, pero no puede presupuestarlas, ya que no hay funciones ni usuarios asociados a las tareas.

* Las horas planificadas en el planificador de recursos no incluyen las horas planificadas asociadas con lo siguiente:

   * tareas principales
   * tareas no asignadas
   * problemas, cuando la variable **Incluir horas de problemas** está desactivado.

* Las horas planificadas no se muestran en el planificador de recursos si la tarea o el problema Duración es cero.
* Las horas planificadas asociadas con usuarios desactivados no se muestran.

Para obtener más información acerca de las horas planificadas y FTE en el planificador de recursos, consulte [Descripción general de las horas, los datos a tiempo completo y la información de costes en las vistas Proyecto y Función del planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### La columna ACT (real)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td> <p><strong>Descripción</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario </td> 
   <td> <p>Tiempo registrado por el usuario en todas las tareas o problemas asignados a ellos.</p> <p>Esto incluye lo siguiente:</p> 
    <ul> 
     <li>Tareas y problemas que están asignados al usuario pero no están asociados a ninguna función de trabajo.</li> 
     <li>Tareas y problemas que no están en proyectos para los que tiene acceso a Administrar. </li> 
    </ul> <p>Esto incluye el tiempo registrado en el proyecto solo cuando el usuario está asignado a tareas o problemas en ese proyecto.  </p> </td> 
  </tr> 
  <tr> 
   <td>Proyecto </td> 
   <td> <p>Tiempo registrado por el usuario en todas las tareas y problemas asignados al proyecto.</p> <p>Esto incluye el momento en que iniciaron sesión directamente en el proyecto.</p> <p>Esto no incluye lo siguiente:</p> 
    <ul> 
     <li> <p>Tiempo empleado en tareas y problemas que no están asignados a ningún usuario. </p> </li> 
     <li> <p>Tiempo registrado en las tareas principales. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>Tiempo registrado en todas las tareas o problemas asignados al usuario en esta función. </p> <p>Esto no incluye lo siguiente:</p> 
    <ul> 
     <li>Tiempo empleado en tareas y problemas asignados a esta función, pero no a este usuario en esta función.</li> 
     <li>Tiempo registrado directamente en el proyecto o en las tareas principales. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Tarea o problema </td> 
   <td> <p>El tiempo que el usuario que también se le asigna inicia sesión en las tareas y los problemas. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>El tiempo registrado se muestra en el intervalo de tiempo correspondiente a la fecha de entrada de la entrada de hora, independientemente del intervalo de tiempo de la tarea, el problema o el proyecto en el que se registran las horas.

Para obtener más información sobre las horas reales, consulte [Ver horas reales](../../manage-work/tasks/task-information/actual-hours.md).

### La columna DIF (Diferencia) {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td> <p><strong>Descripción</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>La diferencia entre las horas disponibles y planificadas o los FTE del usuario. </p> <p>La diferencia de hora o FTE se calcula mediante la fórmula siguiente:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Nota: Si el valor aparece en números rojos negativos, el usuario queda sobreasignado. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>Esta información no está disponible para el proyecto. </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>La diferencia entre las horas disponibles y planificadas o las horas de servicio a tiempo completo de la función de trabajo. </p> <p>La diferencia de hora o FTE se calcula mediante la fórmula siguiente:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Nota: Si el valor se muestra en números rojos negativos, la función se sobreasigna. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tarea o problema</td> 
   <td>Esta información no está disponible para la tarea, el problema o el proyecto. </td> 
  </tr> 
 </tbody> 
</table>

### La columna % (porcentaje de asignación de horas planificadas) {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Mostrado por</strong> </td> 
   <td> <p><strong>Descripción</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> <p>La asignación de las horas planificadas o FTE como porcentaje de las horas disponibles. El porcentaje de la asignación de horas planificadas se calcula mediante la fórmula siguiente:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>Se utiliza el mismo cálculo para los valores FTE. </p> </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>Esta información no está disponible para el proyecto al aplicar la variable <strong>Ver por usuario</strong> vista al planificador de recursos.</td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> La asignación de las horas planificadas o FTE como porcentaje de las horas disponibles. <p>El porcentaje de la asignación de horas planificadas se calcula mediante la fórmula siguiente:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>Se utiliza el mismo cálculo para los valores FTE.</p></td> 
  </tr> 
  <tr> 
   <td>Tarea o problema</td> 
   <td>Esta información no está disponible para la tarea, el problema o el proyecto. </td> 
  </tr> 
 </tbody> 
</table>

Si el valor de Horas planificadas o FTE es cero, la Asignación porcentual es 0%. Si el valor de las horas disponibles o FTE es cero, no se puede calcular la asignación porcentual.

Para obtener más información sobre las horas planificadas y los datos a tiempo completo y cómo se muestran en el planificador de recursos, consulte [Recursos presupuestarios en el planificador de recursos utilizando las vistas Proyecto y Función](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
