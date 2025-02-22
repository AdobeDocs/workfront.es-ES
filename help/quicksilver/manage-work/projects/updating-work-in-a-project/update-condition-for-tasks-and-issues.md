---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar la condición para tareas y problemas
description: La condición de una tarea o problema es un indicador colocado en él para indicar cómo va. Esto es diferente al Estado del elemento de trabajo, que indica la fase actual de desarrollo del elemento.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 2def8297fe606adaeaef6cc079b718531377919d
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---

# Actualizar condición para tareas y problemas

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

La condición de una tarea o problema es un indicador colocado en él para indicar cómo va. Esto es diferente al Estado del elemento de trabajo, que indica la fase actual de desarrollo del elemento.

Puede establecer la condición de una tarea o un problema de forma automática o manual.

Los valores de Condición a los que nos referimos en este artículo están disponibles en Workfront de forma predeterminada. El administrador de Adobe Workfront puede crear condiciones personalizadas para su entorno, tal como se describe en [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Requisitos de acceso {#access-requirements}

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
   Nuevo:
   <ul><li><p>Estándar para tareas</p></li>
   <li><p>Colaborador o superior para problemas</p></li></ul>
   Actual:
   <ul><li><p>Trabajo o superior para tareas</p></li>
   <li><p>Solicitud de problemas o superior</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a los proyectos</p> <p>Editar acceso a tareas y problemas </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores en tareas y problemas para ver su condición</p>
   <p>Permisos de Contribute en tareas y problemas para actualizar la condición</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Se le debe asignar una tarea o un problema para poder actualizar manualmente su condición.

## Busque la Condición de tareas y problemas

Las condiciones se muestran como un indicador asociado a tareas o problemas. También pueden asociarse con un número que se puede mostrar en los informes en lugar de en la etiqueta. Para obtener más información acerca de cómo asociar condiciones con números, vea [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Puede localizar la Condición de las tareas y problemas en las siguientes áreas de Workfront:

* La página Detalles, después de que un administrador de Workfront o de un grupo la añada a la plantilla de diseño. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

* Encabezado de una tarea o problema, después de que un administrador de Workfront o de grupo lo añada a la plantilla de diseño. Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

* El panel Resumen, después de que un administrador de Workfront o de grupo lo añada a la plantilla de diseño. Para obtener más información, consulte [Personalizar el panel de resumen con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

* Informes y listas cuando se muestra el campo Condición en una vista o agrupación.

  >[!NOTE]
  >
  >Cuando la palabra &quot;condición&quot; aparece en el campo Nombre de campo de un informe de Entrada de cuaderno, esto indica que se ha actualizado la condición de un artículo. Cuando se realiza el seguimiento del campo Condición en los informes de entradas de diario, los valores de número nuevo y antiguo muestran el número asociado a la condición en lugar de su nombre. Si originalmente una condición no está definida para una tarea o un problema y posteriormente la actualiza, la entrada de diario que captura la actualización mostrará el valor del número anterior del campo Condición como -2.147.483.648.

## Actualizar automáticamente la condición al actualizar el estado

Cuando se le asigna una tarea o un problema y hace clic en **Trabajar en ello** , Iniciar tarea o Iniciar problema o actualizar su estado, la condición de la tarea o el problema cambia automáticamente a la condición predeterminada asociada con **Avanzar sin problemas**.

Para obtener información acerca de cómo usar una condición personalizada como condición predeterminada, vea los artículos [Establecer una condición personalizada como predeterminada para tareas y problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) y [Establecer una condición personalizada como predeterminada para proyectos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Para obtener información acerca de cómo cambiar el estado de la tarea, vea [Actualizar el estado de la tarea](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Para obtener información sobre cómo cambiar el estado del problema, consulte [Actualizar estado del problema](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Para obtener información acerca de cómo establecer el botón Trabajar en ello en un botón Iniciar tarea o Iniciar problema, vea [Reemplazar el botón Trabajar en ello por un botón Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Actualizar manualmente la condición

Debe tener asignada una tarea o el problema o tener permisos de administración para poder establecer la condición en él.

Puede actualizar manualmente la condición de una tarea o problema en un informe o lista de tareas o problemas al mostrar el campo Condición en la vista.

>[!NOTE]
>
>Puede pedir al administrador del sistema o del grupo que agregue el campo Condición al Panel de resumen, al encabezado de tarea o problema o a las páginas Detalles.
>
>Para obtener más información, consulte los siguientes artículos:
>
>* [Resumen](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personalizar el panel de resumen mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Puede actualizar de forma manual la Condición de las tareas y los problemas en varias áreas de Workfront. En las siguientes secciones se describe cómo actualizar de forma manual la Condición de las tareas y los problemas.

### Actualizar la condición de una tarea o problema en el encabezado de tarea o problema

1. (Condicional) Si el administrador del grupo o de Workfront agregó el campo Condición al encabezado de tarea o problema de la plantilla de diseño, haga clic en el campo **Condición** del encabezado y seleccione una de las siguientes opciones:
   * Sin problemas
   * Algunas preocupaciones
   * Impedimentos mayores

   ![](assets/condition-in-task-header.png)
1. Haga clic en Entrar para guardar la condición.

### Actualizar la condición de una tarea o un problema en la sección Detalles de la tarea o el problema

1. (Condicional) Si el administrador del grupo o de Workfront agregó el campo Condición a la sección Detalles de una tarea o problema de la plantilla de diseño, haga clic en **Detalles** en el panel izquierdo y, a continuación, haga clic en **Condición de la tarea** o **Condición del problema** y seleccione una de las siguientes opciones:
   * Sin problemas
   * Algunas preocupaciones
   * Impedimentos mayores
1. Haga clic en **Guardar cambios**. Se actualiza la condición de la tarea o el problema.

### Actualizar la condición de una tarea o un problema en un informe o una lista

1. Vaya a una lista de tareas o problemas para los que tenga permisos de administración. Asegúrese de que el campo **Condición** esté visible en la vista de la lista.

1. Actualice la **condición** del problema o tarea en línea, haciendo doble clic en la condición existente y seleccionando un nuevo valor en el menú desplegable.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >Las condiciones se pueden personalizar para su entorno, por lo que puede encontrar más de tres opciones para Condición en su entorno. Los nombres de las condiciones pueden ser diferentes a los enumerados anteriormente. Para obtener información acerca de cómo personalizar condiciones en Workfront, vea [Crear o editar una condición personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. Presione **Enter** en el teclado o haga clic fuera del campo Condición para guardar la nueva condición de tarea o problema.

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


