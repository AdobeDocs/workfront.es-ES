---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar condición para tareas y problemas
description: La condición de una tarea o problema es un indicador que se coloca en él para indicar cómo va. Es distinto del estado del elemento de trabajo, que indica la etapa actual del desarrollo del elemento.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Actualizar condición para tareas y problemas

La condición de una tarea o problema es un indicador que se coloca en él para indicar cómo va. Es distinto del estado del elemento de trabajo, que indica la etapa actual del desarrollo del elemento.

Puede establecer la condición de una tarea o un problema de forma automática o manual.

El administrador de Adobe Workfront puede crear condiciones personalizadas para su entorno, tal como se describe en [Creación o edición de una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## Requisitos de acceso {#access-requirements}

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>


   For legacy licenses:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Trabajo o superior para tareas</p>
   <p>Solicitar o superior para problemas</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver o acceder más a los proyectos</p> <p>Editar acceso a tareas y problemas </p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores en tareas y problemas para ver su condición</p>
   <p>Administrar permisos en tareas y problemas para actualizar la condición</p>
    <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Localización de la condición de las tareas y los problemas

Las condiciones se muestran como un indicador asociado a tareas o problemas. También pueden asociarse con un número que puede mostrarse en los informes en lugar de en la etiqueta. Para obtener más información sobre cómo asociar condiciones con números, consulte [Creación o edición de una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Puede localizar la condición de las tareas y los problemas en las siguientes áreas:

* Área de actualizaciones de tareas y problemas, dentro de una actualización, cuando se le asigna la tarea o el problema.
* Informes y listas cuando se muestra el campo Condición en una Vista o Grupo.

>[!NOTE]
>
>Cuando la palabra &quot;condición&quot; aparece en el campo Nombre de campo de un informe Entrada de diario, esto indica que se ha actualizado la condición de un elemento. Cuando se realiza el seguimiento del campo Condición en los informes Entradas en Journal, los Valores de Número Nuevo y Antiguo muestran el número asociado a la condición en lugar de su nombre. Si una condición no está definida originalmente para una tarea o un problema y posteriormente la actualiza, la entrada del asiento que captura la actualización mostrará el valor del número antiguo del campo Condición como -2.147.483.648.

## Actualizar automáticamente la condición actualizando el estado

Cuando se le asigna una tarea o un problema y hace clic en **Trabajar En Él** , Iniciar tarea o Iniciar problema, o actualizar su estado, la condición de la tarea o problema cambia automáticamente a la condición predeterminada asociada a **Suavemente**.

Para obtener información sobre el uso de una condición personalizada como condición predeterminada, consulte los artículos  [Establecer una condición personalizada como predeterminada para tareas y problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) y [Establecer una condición personalizada como predeterminada para los proyectos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Para obtener información sobre cómo cambiar el estado de la tarea, consulte [Actualizar estado de tarea](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Para obtener información sobre cómo cambiar el estado del problema, consulte [Actualizar estado del problema](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Para obtener información sobre cómo configurar el botón Trabajar en él como un botón Iniciar tarea o Iniciar problema, consulte [Reemplazar el botón Trabajar en él con un botón Inicio](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Actualizar manualmente la condición

Debe estar asignado a una tarea o al problema, o tener permisos de administración para poder establecer la condición en ella.

La actualización de la condición de una tarea o problema varía en función de si se le ha asignado o no:

* Puede actualizar la condición en la ficha Actualizaciones o en una lista de tareas o problemas si se le asigna.
* Puede actualizar la condición solo en una lista de tareas o problemas si no está asignado a ellas, pero tiene permisos de administración para ellas. En este caso, no puede actualizar la condición en la pestaña Update de la tarea o problema.

Para configurar manualmente la condición de una tarea o un problema:

1. Vaya a una tarea o problema asignado para el cual desea establecer la condición.

   O

   Vaya a una lista de tareas o problemas a los que tenga permisos de administración pero que no estén asignados.

1. Cambie la condición del problema o la tarea de la siguiente manera:

   * Si tiene asignado la tarea o el problema y tiene permisos de administración, en la variable **Actualizaciones** , haga clic en **Iniciar una nueva actualización**, seleccione **Condición** que mejor refleje cómo va la tarea, escriba el motivo para cambiar la condición en la variable **Iniciar una nueva actualización** área (opcional) y, a continuación, haga clic en **Actualizar**.

      ![](assets/change-condition-update-comment-350x141.png)

      >[!NOTE]
      >
      >Las condiciones se pueden personalizar para su entorno, por lo que puede encontrar más de tres opciones para Condición en su entorno. Los nombres de las Condiciones pueden ser diferentes de los indicados arriba. Para obtener información sobre la personalización de condiciones en Workfront, consulte [Creación o edición de una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

      Para obtener información sobre la funcionalidad adicional disponible al actualizar un elemento de trabajo, consulte [Actualizar trabajo](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
