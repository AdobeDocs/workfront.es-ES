---
product-area: projects
navigation-topic: manage-issues
title: Modificar asignaciones de usuarios para varios problemas en una lista
description: Modificar asignaciones de usuarios para varios problemas en una lista
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 8f7249e08268a8cb784d4c0ecc8c534542fa80cf
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 51%

---

# Modificar asignaciones de usuarios para varios problemas en una lista

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Puede modificar simultáneamente las asignaciones de usuarios a varios problemas. Para obtener información sobre cómo editar problemas o asignarlos de uno en uno, consulte los siguientes artículos:

* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Asignar problemas](../../../manage-work/issues/manage-issues/assign-issues.md)

Para obtener información general sobre la asignación de problemas, consulte [Información general sobre la modificación de asignaciones de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Debe tener al menos permisos de aportación para resolver un problema y poder realizar asignaciones al mismo.

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
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Acceso de visualización o superior a proyectos y tareas para asignar un problema</p> </td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Permisos de administración para el problema</p> <p>Permisos de contribución o superiores para el proyecto o la tarea donde se encuentra el problema, al asignar varios problemas.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modificar asignaciones para varios problemas

1. Vaya a la lista de problemas que contiene los problemas cuyas asignaciones desea modificar.
1. (Opcional) Cree un filtro para mostrar solo los problemas asignados al usuario asignado que desee modificar.

   Por ejemplo, puede crear un filtro para mostrar solo los problemas con una función específica como usuario asignado.  A continuación, puede reemplazar la función por un usuario específico. Haga lo siguiente:

   1. Haga clic en la lista desplegable **Filtros** y luego haga clic en **Nuevo filtro**.

   1. En el primer campo, empiece a escribir **Roles de asignación** y elija **Roles de asignación: Nombre** en la lista.
   1. Seleccione **Es cualquiera de** en el menú desplegable de modificadores y, a continuación, empiece a escribir el nombre de un rol y selecciónelo cuando se muestre en la lista. Puede escribir varias funciones.

      >[!TIP]
      >
      >No use **Asignado a** porque este campo hace referencia solamente al Propietario del problema y no a todas las personas asignadas.

      La lista de problemas filtra automáticamente los criterios de filtro.
   1. (Opcional) Haga clic en **Guardar como nuevo** y después en **Guardar**.

1. Seleccione los problemas para los que desea modificar las asignaciones y, a continuación, haga clic en el icono **Editar** ![Editar icono](assets/qs-edit-icon.png).

   Se muestra la opción **Editar problemas**. El número de elementos seleccionados se muestra en la esquina superior izquierda de la página.

1. Haga clic en **Asignaciones** en el panel izquierdo y, a continuación, haga clic en el icono **x** junto al usuario asignado que desee eliminar.

   >[!TIP]
   >
   >Solo se muestran las personas asignadas a todos los problemas seleccionados en el área **Asignaciones**.

   ![Área de asignaciones en problemas de edición masiva](assets/assignments-area-on-bulk-edit-issues.png)

1. Empiece a escribir el nombre de un usuario, rol o equipo para agregar usuarios asignados a todos los problemas seleccionados.

   >[!TIP]
   >
   >Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos.
   >
   >Si se asignó un usuario, una función o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >
   >* Reasignar el elemento de trabajo a los recursos activos.
   >* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.

   Los usuarios asignados añadidos se añaden a los existentes. No reemplazan a los existentes para cada problema seleccionado.

1. (Opcional) Haga clic en **Asignármelo** para asignarse a sí mismo todos los problemas.
1. Haga clic en **Guardar**.


   <!--Old functionality for assignments for issues - before November 2025:
   1. (Conditional) In the Production environment, do the following: 
   1. Go to the **Assignments** section, then select **Assignee**.
      ![Assignments area](assets/classic-assignmens-area-on-edit-box-350x119.png)
   1. Do one of the following:
      1. To add a new assignee:
         1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues.
         >[!TIP]
         >
         >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
         >
         >If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
         >
         >* Reassign the work item to active resources.
         >* Associate the users in a deactivated team with an active team and reassign the work item to the active team.
          Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the **Assignee**  column. If information is not common across the issues selected, no information displays.
      1. To remove individual assignees:
         1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.
            Or
            If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.
         1. Click  **Remove Assignee** again to add another assignee to remove.
      1. To remove all existing assignees:
         1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.
            This removes not only common assignees (assignees that are displayed in the edit  dialog box), but also all assignees on all the selected issues.
         1. (Optional) Modify any of the following options for the assignees you selected to associate with the issues:
          * **Issue Owner:**  Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, Adobe Workfront designates the first assignee as the Issue Owner. This is not available for team assignments. 
            * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Workfront automatically selects the Primary Role of the user.
      1. Click **Save Changes**.-->




