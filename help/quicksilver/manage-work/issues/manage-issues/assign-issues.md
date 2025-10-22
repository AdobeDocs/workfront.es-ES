---
product-area: projects
navigation-topic: manage-issues
title: Asignar problemas
description: Puede asignar problemas a usuarios, funciones y equipos para indicar quién es el responsable de completar los problemas. Para obtener información general sobre la asignación de problemas, consulte Información general sobre la modificación de asignaciones de problemas.
author: Lisa
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 6ded38ef130fbcdde8d680f77f6db38fbd81efb4
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 45%

---

# Asignar problemas

<!--Audited: 07/2024-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

Puede asignar problemas a usuarios, funciones y equipos para indicar quién es el responsable de completar los problemas. Para obtener información general sobre la asignación de problemas, consulte [Información general sobre la modificación de asignaciones de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos.
>
>Si un usuario, un rol o un equipo se han asignado antes de que se desactiven, permanecerán asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
>
>* Reasignar el elemento de trabajo a los recursos activos.
>* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.

Además de este artículo, le recomendamos que lea los siguientes artículos para obtener más información sobre la asignación de problemas:

* [Información general sobre la modificación de asignaciones de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Modificar asignaciones de usuarios para varios problemas en una lista](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Crear asignaciones avanzadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Realizar asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Información general sobre asignaciones inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

Puede asignar un problema a uno o varios recursos en el nivel de problema individual, o puede asignar varios recursos a varios problemas a la vez.

La asignación de problemas y tareas es similar en Adobe Workfront. Para obtener información general acerca de la asignación de tareas, vea [Información general sobre la modificación de asignaciones de tareas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td> <p>Colaborador o superior</p>
   <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Acceso de visualización o superior a proyectos y tareas para asignar un problema</p> </td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Permisos de administración para el problema</p> <p> Ver permisos o superiores al proyecto o tarea donde se encuentra el problema, al asignar un problema</p><p>Permisos de contribución o superiores para el proyecto o la tarea donde se encuentra el problema, al asignar varios problemas.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones para varias asignaciones a funciones, equipos y usuarios

Tenga en cuenta lo siguiente al asignar varios recursos a un elemento de trabajo:

* Los usuarios pueden tener más de una función asociada a su perfil. Para obtener información sobre cómo asociar usuarios con roles de trabajo, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Las tareas o los problemas suelen asignarse primero a uno o varios roles o equipos de trabajo. Cuando los proyectos están listos para iniciarse, es posible que también deban asignarse a usuarios.

  Si se asigna una tarea o un problema a una o varias funciones y, a continuación, también se asigna un usuario, Adobe Workfront decide qué función se asocia al usuario adicional (si corresponde) según las siguientes reglas:

   * Si solo hay una función asignada y coincide con la función principal del usuario, la tarea o el problema se asignan únicamente al usuario que desempeña su función principal.
   * Si hay varias funciones asignadas y al menos una de las funciones coincide con las funciones secundarias del usuario, la tarea o el problema se asigna al usuario que desempeña una de sus otras funciones (que Workfront selecciona aleatoriamente si hay varias coincidencias), así como cualquier función adicional asignada.
   * Si hay una o más funciones asignadas y no hay coincidencias con las funciones del usuario, la tarea o el problema se asignan tanto a la función o funciones como al usuario.

* Si se asigna una tarea o un problema a un equipo y también se asigna un usuario, la tarea o el problema permanecen asignados tanto al equipo como al usuario.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## Asignar un solo problema

1. Vaya al problema que desee asignar.
1. Haga clic en **Asignar a** en la esquina superior derecha del encabezado del problema, en el área de **Asignaciones**

   O

   Haga clic en el nombre de las asignaciones actuales, si el problema ya está asignado.

   ![Asignar a botón](assets/assign-to-button-in-header.png)

1. Realice una de las siguientes acciones:

   * Comience a escribir el nombre del usuario, función o equipo que desea asignar y, a continuación, haga clic en él cuando aparezca en la lista.

     ![Búsqueda de asignaciones](assets/smart-assignments-issue-header.png)

   * (Condicional) Haga clic en uno de los nombres, roles o equipos de las listas disponibles
   * Haz clic en **Asignármelo** para asignártelo a ti mismo
   * Haga clic en **Avanzadas**.

     Crear asignaciones avanzadas es similar para tareas y problemas. Para obtener información sobre cómo realizar asignaciones avanzadas, consulte [Crear asignaciones avanzadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >Al añadir una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos.
     >
     >Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.
     >
     >Debe tener habilitada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >

     <!-- this doesn't apply to issues; if it does, add this to the TIP above: 
      ><span class="preview">When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. Haga clic en **Guardar** para completar la asignación del problema.
1. (Opcional) Haga clic en el **icono X** junto al nombre de las asignaciones en el área Asignaciones del encabezado del problema para quitar una asignación.

## Asignar un problema en una lista

Puede asignar problemas en una lista o un informe cuando cualquiera de los campos de asignaciones esté visible en la vista de la lista. Esta es una forma más rápida de asignar problemas.

Según el campo visible en la vista, puede asignar las siguientes entidades al problema:

| Opción | Entidades asignadas |
|---|---|
| **Asignar a** | Asignar un usuario |
| **Asignado** | Asignar un usuario |
| **Asignaciones** | Asigne usuarios, funciones o equipos. |

Para asignar problemas en una lista:

1. Vaya a una lista de problemas que tenga los campos Asignado a, Asignado o Asignaciones en la vista.
1. Para asignar problemas, realice una de las siguientes acciones:

   * Haga clic dentro de los campos **Asignado a** o **Asignado** y empiece a escribir el nombre de un usuario activo que desee asignar al problema; a continuación, haga clic en él cuando se muestre en la lista.

     ![Asignado a campo](assets/assigned-to-field-task-list-nwe.png)

   * Haga clic dentro del campo **Asignaciones** y empiece a escribir el nombre de un usuario, rol o equipo activo que desee asignar al problema; a continuación, haga clic en él cuando se muestre en la lista.

     ![Campo de asignaciones](assets/assignments-field-0825.png)

   >[!TIP]
   >
   >Al añadir una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos.
   >
   >Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.
   >
   >Debe tener habilitada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. (Condicional) En el campo Asignaciones, haga clic en **Avanzadas** en la parte inferior de la lista o en el **icono Personas** ![Icono Personas](assets/teams.png) en la esquina superior derecha del cuadro Asignaciones, para abrir el cuadro Asignaciones avanzadas y crear asignaciones avanzadas. Para obtener más información, consulte [Crear asignaciones avanzadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >No puede realizar asignaciones avanzadas desde los campos Asignado a o Asignado.

1. Después de agregar los usuarios asignados al problema, presione Intro o haga clic en cualquier lugar de la página para guardar los cambios.

## Asignar problemas de forma masiva

<!--
Assigning issues in bulk is different depending on what environment you choose to do this. 

### Assign issues in bulk in the Production environment -->

1. Vaya a una lista de problemas que desee asignar de forma masiva.
1. Seleccione varios problemas en la lista.
1. Haga clic en el **icono Editar** ![icono Editar](assets/qs-edit-icon.png).

   Se abre el cuadro de diálogo **Editar problemas**.

1. En el área **Asignaciones**, seleccione la casilla **Usuario asignado** y, a continuación, empiece a escribir el nombre de un usuario, rol o equipo que desee asignar a todos los problemas.

   >[!IMPORTANT]
   >
   >Si alguno de los problemas ya está asignado, los recursos que indique aquí se agregan a los problemas en lugar de reemplazar los recursos existentes en los problemas.

1. (Opcional) Seleccione el botón de opción en la columna **Propietario del problema** para indicar qué recurso es el principal asignado o el propietario del problema, cuando asigne más de un recurso al problema. Esto no está disponible para equipos.
1. (Opcional) Seleccione un rol que el usuario deba cumplir en el problema desde el menú desplegable **Elegir un rol** en la columna **Rol de asignado** cuando asigne usuarios a los problemas. Si no selecciona ninguna función, Workfront selecciona automáticamente la función principal del usuario.

1. (Opcional) Si desea quitar los usuarios asignados existentes de todos los problemas, realice una de las siguientes acciones:

   1. Empiece a escribir el nombre de un usuario, rol o equipo que desee eliminar del problema y, a continuación, selecciónelo cuando aparezca en la lista y haga clic en **Quitar usuario asignado** para agregar usuarios asignados adicionales que eliminar.
   1. Haga clic en **Quitar todas las personas asignadas existentes** para quitar todas las personas asignadas de todos los problemas seleccionados.

1. Haga clic en **Guardar cambios**.
1. (Opcional y condicional) Cuando los campos Asignado a o Asignaciones se muestren en su lista de problemas, haga clic dentro de una de estas columnas para un problema y luego haga clic en el **icono X** junto al nombre de un usuario asignado para quitarlo del problema.

<!--
<div class="preview">

### Assign issues in bulk in the Preview environment

1. Go to a list of issues that you want to assign in bulk. 
1. Select several issues in the list. 
1. Click the **Edit icon** ![Edit icon](assets/qs-edit-icon.png).

   The **Edit Issues** dialog box opens.

1. Click **Assignments** in the left panel, and in the **Assignments** area, start typing the name of a user, role, or team in the **Search people, roles, or teams** field, then click it when it displays in the list

   Or

   Click **Assign to me** to assign the issues to yourself.

   >[!IMPORTANT]
   >
   >If any of the issues is already assigned, the resources you indicate here are added to the issues instead of replacing the existing resources on the issues. 
   
1. (Optional) If you want to remove existing assignees from all issues, click the **x** next to their name.

1. (Optional) Update the Planned Hours field. For more information, see [Edit issues](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md). 

1. Click **Save**.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of issues, click inside one of these columns for an issue, then click the **X icon** next to the name of an assignee to remove it from the issue.

</div>
-->
