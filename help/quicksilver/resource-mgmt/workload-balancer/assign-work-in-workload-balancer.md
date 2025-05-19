---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo
description: Como administrador de recursos, puede utilizar el Distribuidor de cargas de trabajo de Adobe Workfront para ver los elementos de trabajo que aún no se han asignado a los usuarios, así como asignarles estos elementos.
author: Lisa
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 92%

---

# Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo

<!-- Audited: 5/2025 -->

Como administrador de recursos, puede utilizar el Distribuidor de cargas de trabajo de Adobe Workfront para ver los elementos de trabajo que aún no se han asignado a los usuarios, así como asignarles estos elementos.

Para obtener información general sobre el Distribuidor de cargas de trabajo, consulte [Información general del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Puede asignar elementos de trabajo (tareas y problemas) a usuarios de otras áreas de Workfront. Sin embargo, al utilizar el Distribuidor de cargas de trabajo, puede conocer fácilmente la disponibilidad de los usuarios y ver claramente todos los demás elementos que tienen asignados antes de asignarles más trabajo.

Para obtener información sobre la asignación de elementos de trabajo en otras áreas de Workfront, consulte los siguientes artículos:

* [Asignar tareas](../../manage-work/tasks/assign-tasks/assign-tasks.md)
* [Asignar problemas](../../manage-work/issues/manage-issues/assign-issues.md)

## Disponibilidad de los usuarios en el Distribuidor de cargas de trabajo

Puede asignar trabajo en el Distribuidor de cargas de trabajo para que coincida con el tiempo disponible de los usuarios. Para asegurarse de que asigna la cantidad correcta de trabajo y no asigna en exceso al usuario, el total de horas planificadas de los elementos de trabajo asignados al usuario debe coincidir con las asignaciones diarias o semanales del usuario.

Es importante comprender cómo calcula Workfront el tiempo disponible para un usuario.

Workfront utiliza la siguiente información para calcular la capacidad del usuario en el Distribuidor de cargas de trabajo:

* Preferencias de la administración de recursos El administrador de Workfront determina cómo se calcula el tiempo disponible para el sistema seleccionando la opción para utilizar una de las siguientes opciones en el área Administración de recursos de Configuración:

   * El horario predeterminado del sistema Workfront y el EJC del usuario.
   * El horario del usuario, tal como se indica en el área Perfil de usuario.

     Calcula la disponibilidad diaria y semanal del usuario. Cualquier excepción de programación en la programación seleccionada se refleja en la capacidad del usuario en el Distribuidor de cargas de trabajo.

  Para obtener más información, consulte [Configurar las preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Para obtener información acerca de las programaciones, consulte [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* El tiempo libre del usuario. Indica los días que el usuario tiene previsto tomarse libres.

  Para obtener más información, consulte [Configurar días libres personales](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* El tiempo de trabajo del usuario. Indica el porcentaje de tiempo de EJC que el usuario tiene disponible para realizar el trabajo real relacionado con el proyecto, sin incluir las sobrecargas. Establezca el valor de Tiempo de trabajo en 1 para indicar que el usuario está disponible para realizar el trabajo relacionado con el proyecto en su equivalente a jornada completa.


## Asignación de trabajo en el Distribuidor de cargas de trabajo

Puede asignar elementos de trabajo que aún no se hayan asignado a un usuario o reasignar elementos que se hayan asignado a usuarios en el Distribuidor de cargas de trabajo.

Puede asignar trabajo en el Distribuidor de cargas de trabajo de las siguientes maneras:

* De uno en uno, asignando manualmente cada elemento.

  Puede realizar Asignaciones avanzadas cuando asigne elementos manualmente, de uno en uno.

  Para obtener más información, consulte [Asignar trabajo manualmente mediante el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

* De uno en uno, arrastrando y soltando elementos de trabajo para el usuario que necesita ser asignado.

  Para obtener más información, consulte [Asignar trabajo en el Distribuidor de cargas de trabajo arrastrando y soltando](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

* Varios elementos a la vez, utilizando la opción Asignaciones masivas. Puede definir reglas según las cuales los elementos se asignarán a varios usuarios a la vez.

  Para obtener más información, consulte [Asignar trabajo de forma masiva mediante el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

Para obtener información sobre cómo anular la asignación de trabajo, consulte [Anular la asignación de trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

## Áreas de asignación de trabajo en el Distribuidor de cargas de trabajo

Puede asignar trabajo a los usuarios mediante el Distribuidor de cargas de trabajo en el área de Recursos, en el proyecto o en el nivel de equipo. Para obtener más información sobre dónde se encuentra el Distribuidor de cargas de trabajo en Workfront, consulte [Buscar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Existen dos áreas en el Distribuidor de cargas de trabajo en las que puede ver elementos de trabajo:

* **Trabajo sin asignar**: muestra elementos que no están asignados a usuarios.
* **Trabajo asignado**: muestra elementos asignados a usuarios.

En la tabla siguiente se describen los elementos que se muestran en cada área en función de sus asignaciones:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Tipo de asignación</strong> </td> 
   <td colspan="2"><strong>Áreas en las que las asignaciones son visibles</strong> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>Trabajo sin asignar </td> 
   <td>Trabajo asignado </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;">Elemento sin asignar</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Equipo</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span data-mc-edit-date="2020-04-08T15:57:40.7175506-04:00" data-mc-editor="alinawilson" data-mc-comment="Drafted because role only is not displayed; first it will be displayed in Unassigned - 20.2 beta" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:24:04.5189150-05:00">Función</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Función y equipo</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Usuario y equipo</td> 
   <td> <p> </p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Usuario, función y equipo</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Usuario y función</p> </td> 
   <td><span data-mc-edit-date="2019-11-15T13:37:42.5435254-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted because it's not in the Unassigned" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:37:33.3097484-05:00">✔</span>*</td> 
   <td>✔**</td> 
  </tr> 
 </tbody> 
</table>

&#42;Al asignar un elemento de trabajo a un usuario y a una función, solo se mostrará en el área Trabajo no asignado cuando la función sea la persona asignada principal.

&#42;&#42;Al asignar un elemento de trabajo a un usuario y a otra entidad, solo se mostrará en el área Trabajo asignado cuando el usuario sea la persona asignada principal.

Para obtener más información sobre las áreas sin asignar y asignadas del equilibrador de cargas de trabajo, consulte [Navegar por el equilibrador de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Consideraciones para varias asignaciones a funciones, equipos y usuarios

Tenga en cuenta lo siguiente al asignar varios recursos a un elemento de trabajo:

* Los usuarios pueden tener más de una función asociada a su perfil. Para obtener información sobre cómo asociar usuarios con roles de trabajo, consulte [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Las tareas o problemas suelen asignarse primero a uno o varios roles de trabajo o a un equipo. Cuando los proyectos están listos para iniciarse, es posible que también deban asignarse a usuarios.\
  Si se asigna una tarea o un problema a una o varias funciones y, a continuación, también se asigna un usuario, Adobe Workfront decide qué función se asocia al usuario adicional (si corresponde) según las siguientes reglas:

   * Si solo hay una función asignada y coincide con la función principal del usuario, la tarea o el problema se asignan únicamente al usuario que desempeña su función principal.
   * Si hay varias funciones asignadas y al menos una de las funciones coincide con las funciones secundarias del usuario, la tarea o el problema se asigna al usuario que desempeña una de sus otras funciones (que Workfront selecciona aleatoriamente si hay varias coincidencias), así como cualquier función adicional asignada.
   * Si hay una o más funciones asignadas y no hay coincidencias con las funciones del usuario, la tarea o el problema se asignan tanto a la función o funciones como al usuario.

* Si se asigna una tarea o un problema a un equipo y también se asigna un usuario, la tarea o el problema permanecen asignados tanto al equipo como al usuario.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Manually assign one item at a time</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Moved manual assignment and drag-and-drop to their own articles) </p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <strong>Assigned Work</strong> area and expand the name of a user to view the work items assigned to them.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see
<a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
</note> </li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <strong>Assign this to</strong>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> <note type="tip">
<p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p>
<ul>
<li><span>In Windows: CTRL+click the task or issue bar.</span> </li>
<li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li>
</ul>
</note> </li>
<li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <strong>Search people, role or teams</strong> field, select it when it displays in the list, then click&nbsp;<strong>Save</strong>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer.</p> <note type="tip">
<p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
<p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p>
<ul>
<li> <p><span>Reassign the work item to active resources.</span> </p> </li>
<li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li>
</ul>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Assign an item by dragging and dropping</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider retitling this to "Assign one item at a time by dragging and dropping" when bulk assignments will come???)&nbsp;</p>
<p>You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.</p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area.</span>
</note> </li>
<li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <strong>Assigned</strong> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
</note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li>
<li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> <note type="tip">
<p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p>
<p>The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>. (NOTE: make sure these are still called this, and that the icon has not changed)</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol> 
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Assign items in bulk</h2>
<p>(NOTE: This is also a separate article. Should we keep this section or the separate article?) </p>
</div>
<p>&nbsp;</p>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Unassign work items in the Workload Balancer</h2>
<p>(NOTE: moved this section to a new article. Draft here at release to preview) </p>
<p>You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. </p>
<p>To unassign work items from users: </p>
<ol>
<li value="1">In the Workload Balancer, go to the <strong>Assigned Work</strong> area and expand a user.</li>
<li value="2">Do 
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
one of
</MadCap:conditionalText>
the following:
<ul>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. </p></li>
<li><p>Click the <strong>More</strong> icon <img src="assets/more-icon-task-list.png"> to the right of the name of a work item, click&nbsp;<strong>Assign this to</strong> , then remove the name of the entities assigned to the work item or enter another name and click&nbsp;<strong>Save</strong>.</p><p><img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"></p></li>
</ul><p>The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. </p><note type="tip">
Unassigned issues do not display in the Unassigned area.
</note><p>For information about filtering information in the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p></li>
</ol>
</div>
-->
