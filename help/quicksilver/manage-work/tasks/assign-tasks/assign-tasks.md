---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Asignar tareas
description: Puede asignar tareas a usuarios, funciones o equipos para indicar quién es el responsable de completar las tareas. Puede asignar una tarea a varios recursos a la vez.
author: Lisa
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '2156'
ht-degree: 83%

---

# Asignar tareas

<!--Audited: 10/2025-->

<!--remove production/ preview and old/ new experience references at prod-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Puede asignar tareas a usuarios, funciones o equipos para indicar quién es el responsable de completar las tareas. Puede asignar una tarea a varios recursos a la vez.

>[!TIP]
>
>Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos.
>
>Si se asignó un usuario, una función o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
>
>* Reasignar el elemento de trabajo a los recursos activos.
>* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.
>

El número de usuarios asignados a una tarea y la programación del propietario de la tarea pueden modificar las fechas planificadas de una tarea, lo que se traduce en un cambio de la línea de tiempo del proyecto. Para obtener información sobre el impacto de asignar varios usuarios a una tarea, consulte [Información general sobre la modificación de asignaciones de tareas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Además de este artículo, le recomendamos que lea los siguientes artículos para obtener más información sobre la asignación de tareas:

* [Información general sobre la modificación de asignaciones de tareas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Información general sobre asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Realizar asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Crear asignaciones avanzadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Modificar asignaciones de usuario en una lista de tareas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Información general sobre la planificación de un proyecto](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Información general sobre la fecha planificada de finalización de la tarea](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Establecer fecha planificada de finalización del proyecto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

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
   <td> <p>Editar acceso a proyectos y tareas</p> <p>Acceso de visualización o superior a los usuarios</p> </td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td>
   <td>Contribuir o permisos superiores para la tarea</td>
  </tr>
 </tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones para varias asignaciones a funciones, equipos y usuarios

Tenga en cuenta lo siguiente al asignar varios recursos a un elemento de trabajo:

* Los usuarios pueden tener más de una función asociada a su perfil. Para obtener información sobre la asociación de funciones de trabajo, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Si asigna más de un usuario a una tarea o un problema, el primer usuario que seleccione se designa automáticamente como el propietario de la tarea o el problema.
Para obtener instrucciones sobre cómo cambiar esto, consulte la información sobre la opción Convertir en principal en el artículo [Crear asignaciones avanzadas](create-advanced-assignments.md).

* Un equipo no puede ser un asignado principal de una tarea o un problema. Solo se puede designar a un usuario o función como principal en una tarea o un problema.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Las tareas y problemas de un proyecto podrían asignarse primero a uno o más equipos o funciones. Cuando el proyecto esté listo para comenzar, es posible que también se deban asignar a usuarios:

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Equipos</td>
   <td>Si asigna una tarea a un equipo y también asigna un usuario, la tarea permanece asignada al equipo y al usuario, incluso si el usuario no es integrante del equipo.</td>
  </tr>
  <tr>
   <td>Roles</td>
   <td><p>Si asigna una tarea o un problema a una o más funciones y, a continuación, también asigna un usuario, decida qué función asociar al usuario adicional (si corresponde) según las siguientes reglas:</p>
     <ul>
      <li>Si solo hay una función asignada y coincide con la función principal del usuario (configurada en su perfil), la tarea o el problema se asigna únicamente a ese usuario.</li>
      <li>Si se asignan varias funciones y al menos una de ellas coincide con una de las otras funciones del usuario, la tarea o el problema se asignan al usuario (la función se selecciona aleatoriamente si hay varias coincidencias), junto con cualquier función adicional asignada</li>
      <li>Si hay al menos una función asignada y no coinciden las funciones del usuario, la tarea o el problema se asignan a la función o funciones y al usuario.</li>
     </ul>
   <p>Para obtener información acerca de la función principal de un usuario y otras funciones, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Editar el perfil de un usuario</a>.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## Asignar una sola tarea

1. Vaya a la tarea que desee asignar.
1. Haga clic en **Asignar a** en el campo **Asignaciones** del encabezado de la tarea

   O

   Haga clic en el nombre de las asignaciones si la tarea ya está asignada.

   ![Asignaciones](assets/assignments-from-task-header-0825.png)

1. Realice una de las siguientes acciones:

   * Comience a escribir el nombre de un usuario, rol o equipo que desee asignar y, a continuación, haga clic en él cuando aparezca en la lista.

     >[!TIP]
     >
     >Al añadir una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.
     >
     >Debe tener habilitada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

     <!--When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md). -->

   * (Condicional) Haga clic en uno de los nombres de las listas **Usuarios y equipos** o **Funciones del puesto** cuando se muestren. Para obtener más información, consulte [Información general sobre las asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

     Puede empezar a escribir el nombre de cualquier usuario, equipo o función que desee asignar a la tarea y, a continuación, realizar la selección cuando se muestre en la lista.

   * Haga clic en **Opciones avanzadas**.

     Para obtener información sobre cómo realizar asignaciones avanzadas, consulte [Crear asignaciones avanzadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Haga clic en **Guardar**.
1. (Opcional y condicional) Si hizo clic en **Opciones avanzadadas**, haga clic en el icono **X** que aparece junto al nombre de la asignación en el panel derecho de la tarea para quitar una asignación.

## Asignar una tarea a una lista al editarla en línea

Puede asignar las tareas de una lista o un informe cuando cualquiera de los campos de asignación esté visible en la vista de la lista. Es una forma más rápida de asignar tareas. Este artículo describe cómo modificar las asignaciones para una tarea de una lista. Para obtener información sobre cómo modificar varias asignaciones para varias tareas de una lista, consulte [Modificar varias asignaciones de usuario en una lista de tareas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Según el campo que esté visible en la vista, puede asignar las siguientes entidades a la tarea:

| Campo | Entidades asignadas |
|---|---|
| **Asignar a** | Asignar un usuario |
| **Asignado** | Asignar un usuario |
| **Asignaciones** | Asignar usuarios, funciones o equipos |

Para asignar tareas de una lista:

1. Vaya a una lista de tareas que tenga los campos Asignado a, Asignado o Asignaciones en la vista.
1. (Opcional) Haga clic en el menú desplegable **Autoguardar** y seleccione una de las siguientes opciones:

   | Opción | Descripción de opción |
   |---|---| 
   | Autoguardar | Los cambios que realice en las tareas se guardan automáticamente y no puede revertirlos |
   | Guardado manual | Debe guardar manualmente los cambios. Puede revertir los cambios antes de guardarlos. |
   | Planificación de calendario | Debe guardar manualmente los cambios. Puede revertir los cambios antes de guardarlos. Guardar los cambios y todas las dependencias del proyecto es más rápido que cuando selecciona Guardar de forma manual. |

   Para obtener más información sobre cómo guardar tareas a medida que las edita en una lista, consulte [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Para asignar tareas, realice una de las siguientes acciones:

   * Haga clic dentro de los campos **Asignado a** o **Asignado** y empiece a escribir el nombre de un usuario activo que desee asignar a la tarea; a continuación, haga clic en él cuando se muestre en la lista.
   * Haga clic dentro del campo **Asignaciones** y empiece a escribir el nombre de un usuario, función o equipo activo que desee asignar a la tarea; a continuación, haga clic en él cuando se muestre en la lista.

     >[!TIP]
     >
     >Al añadir una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.
     >
     >Debe tener habilitada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)

     <!--<span class="preview">When adding a job role assignment, you can search for the job role or location. Select a Job role to use the default billing rate for the assignment, or select a Rate Card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. (Condicional) En el campo Asignaciones, haga clic en **Avanzadas** al final de la lista o en el **icono Personas** ![Icono Personas](assets/teams.png) en la esquina superior derecha del cuadro Asignaciones, para abrir el cuadro **Asignaciones avanzadas** y crear asignaciones avanzadas.

   Para obtener más información, consulte [Crear asignaciones avanzadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >No puede realizar asignaciones avanzadas desde los campos Asignado a o Asignado.

1. Después de añadir las personas asignadas a la tarea, pulse Intro o haga clic en cualquier lugar de la página para guardar los cambios si selecciona Autoguardar. De lo contrario, haga clic en **Guardar**.

## Asignar varias tareas de forma masiva desde una lista

1. Vaya a una lista de tareas que desee asignar en lotes.
1. (Condicional) Asegúrese de que la opción **Autoguardar** esté seleccionada si está en una lista de tareas de un proyecto.

   >[!IMPORTANT]
   >
   >No puede editar las tareas en lotes al guardar las tareas manualmente en un proyecto.

1. Seleccione varias tareas en la lista de tareas.
1. Haga clic en **Editar**.

   El cuadro de diálogo **Editar tareas** se abre en la nueva experiencia.

1. Continúe asignando las tareas con la nueva experiencia.

   Para obtener más información, consulte la sección [Asignar varias tareas de forma masiva desde una lista en la nueva experiencia](#assign-multiple-tasks-in-bulk-from-a-list-in-the-new-experience) en este artículo.

1. (Opcional) Haga clic en **Volver a la experiencia anterior** en la parte inferior del cuadro **Editar tareas** para abrir la experiencia anterior.

   >[!TIP]
   >
   >La asignación de tareas en el entorno de producción solo está disponible para la experiencia antigua.


1. (Condicional) Con la experiencia anterior, en el área **Asignaciones**, seleccione la casilla **Usuario asignado** y, a continuación, empiece a escribir el nombre de un usuario, rol o equipo que desee asignar a todas las tareas.

   >[!IMPORTANT]
   >
   >Si alguna de las tareas ya está asignada, los recursos que indique aquí se añaden a las tareas en lugar de reemplazar los recursos existentes en las tareas.

1. (Opcional) Seleccione el botón de opción de la columna **Propietario de la tarea** para indicar qué recurso es el principal asignado o el Propietario de la tarea, cuando asigne más de un recurso a la tarea. Esto no está disponible para equipos.
1. (Condicional) Especifique el **% de asignación** para cada recurso asignado a la tarea si todas las tareas seleccionadas tienen un tipo de duración de asignación calculada o condicionada por el esfuerzo. Esto indica la cantidad de tiempo que estos recursos deben dedicar a completar la tarea. Esto solo está disponible para usuarios y funciones.

   O

   Especifique la cantidad de **Horas** para cada recurso asignado a la tarea si todas las tareas que ha seleccionado tienen un Tipo de duración simple. El total de todas las horas de todos los recursos debe ser igual al número de horas planificadas para la tarea.

   >[!IMPORTANT]
   >
   >No puede especificar el porcentaje de asignación ni el número de horas por recurso si las tareas seleccionadas tienen diferentes tipos de duración o si las tareas seleccionadas tienen diferentes tipos de duración.

   Para obtener información acerca del tipo de duración de las tareas, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Opcional) Seleccione una función que el usuario debe cumplir en la tarea del menú desplegable **Elegir un rol** en la columna **Rol de asignado** cuando asigne usuarios a las tareas. Si no selecciona ninguna función, Workfront selecciona automáticamente la función principal del usuario.

1. (Opcional) Si desea quitar las personas asignadas existentes de todas las tareas, realice una de las siguientes acciones:

   1. Empiece a escribir el nombre del usuario, rol o equipo que desee quitar de la tarea, selecciónelo cuando aparezca en la lista y haga clic en **Quitar persona asignada** para quitar más personas asignadas.
   1. Haga clic en **Quitar todas las personas asignadas actualmente** para quitar todas las personas asignadas de todas las tareas seleccionadas.

1. Haga clic en **Guardar cambios**.
1. (Opcional y condicional) Cuando los campos Asignado a o Asignaciones se muestren en su lista de tareas, haga clic dentro de una de estas columnas para una tarea y luego haga clic en el **icono X** junto al nombre de un usuario asignado para quitarlo de la tarea.


### Asignar varias tareas por lotes desde una lista en la nueva experiencia

1. Vaya a una lista de tareas que desee asignar en lotes.
1. (Condicional) Asegúrese de que la opción **Autoguardar** esté seleccionada si está en una lista de tareas de un proyecto.

   >[!IMPORTANT]
   >
   >No puede editar las tareas en lotes al guardar las tareas manualmente en un proyecto.

1. Seleccione varias tareas en la lista de tareas.
1. Haga clic en **Editar**.

   Se abre el cuadro de diálogo **Editar tareas**.

1. En el área **Asignaciones**, empiece a escribir el nombre de los usuarios, equipos o roles en el campo **Buscar personas, roles o equipos** proporcionado y, a continuación, haga clic en ellos cuando se muestren en la lista

   O

   Haz clic en **Asignármelo** para asignártelo a ti mismo.

   >[!IMPORTANT]
   >
   >Si alguna de las tareas ya está asignada, los recursos que indique aquí se añaden a las tareas en lugar de reemplazar los recursos existentes en las tareas.

1. Haga clic dentro del campo **Tipo de duración** y elija un Tipo de duración.

   Para obtener información acerca del tipo de duración de las tareas, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Condicional) Según el **Tipo de duración** que haya seleccionado, actualice los campos siguientes:

   * Duración
   * Horas planificadas

     Para obtener más información, consulte [Editar tareas](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Opcional) Si desea quitar los usuarios asignados existentes de todas las tareas, haga clic en **x** junto a su nombre en el campo **Buscar personas, roles o equipos**.

1. Haga clic en **Guardar**.
1. (Opcional y condicional) Cuando los campos **Asignado a** o **Asignaciones** se muestren en su lista de tareas, haga clic dentro de una de estas columnas para una tarea y luego haga clic en el **icono X** junto al nombre de un usuario asignado para quitarlo de la tarea


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


