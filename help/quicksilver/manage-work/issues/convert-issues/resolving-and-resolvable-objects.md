---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: Información general sobre la resolución y los objetos solucionables
description: Un objeto solucionable es un problema cuya resolución está vinculada a un objeto de resolución. Un objeto de resolución es un proyecto, una tarea u otro problema.
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '1771'
ht-degree: 3%

---

# Información general sobre la resolución y los objetos solucionables

Un objeto solucionable es un problema cuya resolución está vinculada a un objeto de resolución. Un objeto de resolución es un proyecto, una tarea u otro problema.

Cuando convierte un problema en una tarea o un proyecto, el problema se convierte en el objeto solucionable de la tarea o del proyecto.

También puede vincular manualmente un problema a un objeto de resolución, que puede ser una tarea, un proyecto o un problema. Para obtener más información, vea [Asociar manualmente la resolución de un problema a otros problemas, tareas o proyectos](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md).

El problema original se convierte en el objeto solucionable de la tarea, proyecto o problema, en este escenario.

## Configuración de Adobe Workfront para gestionar objetos solucionables {#set-up-adobe-workfront-to-handle-resolvable-objects}

Como administrador de Workfront o administrador de grupo, puede decidir cómo desea gestionar los objetos solucionables en el sistema o para el grupo.

Puede seleccionar conservar el objeto solucionable mientras lo está convirtiendo en una tarea o proyecto, o eliminarlo una vez creada la tarea o proyecto. Puede seleccionar permitir que esta configuración se cambie en el proceso de conversión de problemas, lo que permitirá al usuario convertir los problemas seleccionar si desea mantener o eliminar el problema a medida que lo estén convirtiendo.

>[!NOTE]
>
>Los objetos solucionables son siempre problemas cuya resolución y estado pueden depender de la resolución y el estado del objeto de resolución con el que están asociados. La resolución de objetos puede ser problemas, tareas o proyectos.

Para obtener información sobre la configuración de preferencias para la administración de objetos solucionables, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: drafted and just pointed the user to the article linked above)&nbsp;</p>
<p>To establish the system default for what happens to the issue as it is being converted to a task or a project:</p>
<ol>
<li value="1">Log in to Workfront as a Workfront administrator <span>or group administrator.</span></li>
<li value="2"> <p>  From the main menu, click <strong>Setup</strong>. </p> <p> <img src="assets/qs-main-menu-expanded-with-menu-highlight-350x521.png" style="width: 350;height: 521;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Expand <strong>Project Preferences</strong>.</li>
<li value="4">Click <strong>Tasks & Issues</strong>.</li>
<li value="5">Go to the <strong>Issues</strong> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings:
<ul>
<li><p><strong>Automatically update Resolvable Issue status when the status of the Resolving Object changes:</strong> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <strong>Keep the original issue and tie its resolution to the task</strong> or<strong>project</strong> must be selected.</p>
<ul>
<li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
<li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
</note></li>
</ul></li>
<li><strong>When converting an issue to a TASK...:</strong> The settings in this section determine what happens during the conversion process from issue to task:
<ul>
<li><strong>Keep the original issue and tie its resolution to the task:</strong> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
<li><strong>Allow Primary Contact to have access to the task:</strong> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
</ul></li>
<li><strong>When converting an issue to a PROJECT...:</strong> The settings in this section determine what happens during the conversion process from issue to project:
<ul>
<li><strong>Keep the original issue and tie its resolution to the project:</strong> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
<li><strong>Allow Primary Contact to have access to the project:</strong> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
</ul></li>
</ul></li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Controlar el objeto solucionable durante la conversión en un proyecto o una tarea

Según la forma en que el administrador de Workfront o del grupo haya configurado las preferencias de problemas a nivel de sistema o de grupo, es posible que pueda gestionar el objeto solucionable durante la conversión de un problema en un proyecto o una tarea.

Se dan los siguientes escenarios:

* Si el administrador de Workfront o del grupo tiene **Mantener el problema original y enlazar su solución a la tarea** y **Mantener el problema original y enlazar su solución al proyecto** seleccionado y la opción **Permitir que esta configuración se cambie durante la conversión** no seleccionada, no podrá cambiar esta configuración cuando esté convirtiendo problemas en tareas o proyectos.\
  ![](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* Si el administrador de Workfront o del grupo tiene **Mantener el problema original y enlazar su solución a la tarea** y **Mantener el problema original y enlazar su solución al proyecto** seleccionado o no seleccionado y **Permitir que esta configuración se cambie durante la conversión** seleccionado, podrá cambiar esta configuración a medida que esté convirtiendo problemas en tareas o proyectos.\
  ![](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

Para obtener más información acerca de la conversión de problemas en tareas y proyectos, vea [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Tie the resolution of an issue to a project, task or </h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: created new article for this section; draft when the article is live and see if you need to make a link from this one to the new article) </p>
<div>
<p>You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue. <br>For more information about how the status of the Resolving Object affects the Resolvable Object, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p>
<p>You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this. </p>
<p>To tie the resolution of an issue to the resolution of a project, task, or issue:</p>
<ol>
<li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li>
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p>  </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li>
<li value="4">At the bottom of the form,  click in the <strong>Resolved By</strong> field,  and select from the following types of resolving objects:
<ul>
<li><strong>Project</strong></li>
<li><strong>Task</strong></li>
<li><p><strong>Issue</strong></p></li>
</ul><p>The field for the resolving object displays. </p></li>
<li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li>
<li value="6">Click <strong>Save</strong>&nbsp;<strong>Changes</strong>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
One project, task, or issue may have multiple issues as Resolvable Objects.
</note></li>
</ol>
</div>
</div>
-->

## Sincronizar el estado del objeto solucionable con el del objeto de resolución {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* [Sincronizar estados cuando el objeto de resolución es un problema](#synchronize-statuses-when-the-resolving-object-is-an-issue)
* [Sincronizar estados cuando el objeto de resolución sea una tarea o un proyecto](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### Sincronizar estados cuando el objeto de resolución sea un problema {#synchronize-statuses-when-the-resolving-object-is-an-issue}

Cuando un problema se vincula manualmente a otro, el estado del segundo problema (objeto de resolución) déclencheur un cambio en el estado del primer problema (objeto solucionable). El estado del primer problema coincide con el estado al que se cambia el segundo problema. Esto se aplica a los estados de problema predeterminados y personalizados.

### Sincronizar estados cuando el objeto de resolución sea una tarea o un proyecto {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

Cuando un problema es el objeto solucionable de una tarea o un proyecto, los cambios en el estado de las tareas y el déclencheur de los proyectos cambian en el estado del problema. Los estados predeterminados se activan de forma diferente a los estados personalizados, en este caso.

Cuando el estado personalizado del proyecto equivale a un estado predeterminado que no déclencheur un cambio en el estado del problema, no déclencheur un cambio en el estado del problema.

* [Sincronizar el estado predeterminado del objeto de resolución con el estado predeterminado del objeto solucionable](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [Sincronizar el estado personalizado del objeto de resolución con el estado personalizado del objeto solucionable](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### Sincronizar el estado predeterminado del objeto de resolución con el estado predeterminado del objeto solucionable {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

Independientemente de si la opción &quot;Actualizar automáticamente el estado del problema solucionable cuando cambia el estado del objeto de resolución&quot; está seleccionada, cada vez que cambia el estado predeterminado en los objetos de resolución (proyectos o tareas), el estado del objeto solucionable (problemas) cambia en consecuencia. Solo los estados predeterminados ya están asignados al déclencheur para este cambio.

Los siguientes estados predeterminados para las tareas almacenan en déclencheur los siguientes cambios en los estados predeterminados para los problemas, cuando el problema se establece como objeto de resolución de una tarea:

| **ESTADO DE LA TAREA** | **ESTADO DEL PROBLEMA** |
|---|---|
| Nuevo | Nuevo |
| En curso | En curso |
| Completar | Cerrado |

Los siguientes estados predeterminados de los proyectos almacenan en déclencheur los siguientes cambios en los estados predeterminados de los problemas, cuando el problema se establece como objeto solucionable de un proyecto. Algunos estados de los proyectos no almacenan en déclencheur los cambios de estado de los problemas. Los problemas permanecen en el estado en que estaban antes de que el proyecto se convirtiera en uno de estos estados:

| **ESTADO DEL PROYECTO** | **ESTADO DEL PROBLEMA** |
|---|---|
| Planificación | Nuevo |
| Al día | En curso |
| En espera | En espera |
| Solicitud | No almacena en déclencheur un cambio en el estado del problema |
| Aprobado | No almacena en déclencheur un cambio en el estado del problema |
| Rechazado | No almacena en déclencheur un cambio en el estado del problema |
| Idea | No almacena en déclencheur un cambio en el estado del problema |
| Inactivo | Cerrado |
| Finalizado | Cerrado |

>[!NOTE]
>
>Una vez que el estado del problema pasa a ser Cerrado (como resultado del cierre de la tarea o del proyecto), independientemente del estado en que cambie la tarea o el proyecto después de cerrarlos, el problema permanece Cerrado.

#### Sincronizar el estado personalizado del objeto de resolución con el estado personalizado del objeto solucionable {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

Cuando cambia el estado de la tarea o del proyecto a un estado personalizado, el estado del problema cambia a un estado de problema personalizado solo si se cumplen las dos condiciones siguientes:

* La opción &quot;Actualizar automáticamente el estado del problema solucionable cuando cambia el estado del objeto de resolución&quot; está seleccionada. Para obtener más información acerca de cómo habilitar esta configuración, vea [Configurar Adobe Workfront para controlar objetos solucionables](#set-up-adobe-workfront-to-handle-resolvable-objects).

* El estado personalizado del proyecto o la tarea tiene el mismo código de tres letras que el estado personalizado del problema.

Puede crear estados personalizados con la misma clave tanto para problemas como para proyectos o tareas. Cuando el proyecto o la tarea (como objeto de resolución) cambian al estado personalizado, el cambio también se refleja en el estado del problema. La clave de estado debe ser la misma para los estados de problema y proyecto o tarea.

Por ejemplo, cree un estado personalizado de proyecto llamado &quot;Iniciado&quot; con el código de tres letras &quot;LCD&quot; que equivale a &quot;Actual&quot;. Además, cree un estado personalizado de problema denominado &quot;Proyecto iniciado&quot;, también con el código de letra &quot;LCD&quot; que equivale a &quot;En curso&quot;. Cuando marca el proyecto como &quot;Iniciado&quot;, el problema cambia automáticamente el estado a &quot;Proyecto iniciado&quot;. Si la variable &quot;
Actualizar automáticamente el estado del problema solucionable cuando el estado de la configuración &quot;Cambios en el objeto de resolución&quot; no esté habilitado, el estado del problema cambiaría a &quot;En curso&quot; en su lugar (el estado predeterminado).

Para obtener más información sobre cómo crear un estado personalizado, vea [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Sincronizar el porcentaje completado de un objeto de resolución con el del objeto solucionable

Si un problema se resuelve mediante una tarea o un proyecto, el porcentaje completado del problema se actualiza en el problema solucionable cuando se produce cualquiera de las siguientes cosas: 

* Cada vez que alguien guarde un cambio en la tarea o el proyecto.
* Se vuelve a calcular la cronología del proyecto.

Si un problema se resuelve mediante otro problema, el porcentaje completado se actualiza cuando se actualiza cualquiera de los problemas.

## Localizar el objeto solucionable en una tarea o un proyecto

La ubicación del objeto de resolución es idéntica para tareas y proyectos.

1. Desplácese hasta un proyecto o una tarea que haya creado convirtiendo un problema en el proyecto o la tarea.
1. Haga clic en **Detalles del proyecto** o en el icono **Detalles de la tarea** y luego haga clic para expandirlo.
1. Haga clic en **Información general**.
1. En la parte inferior de la pestaña, localice en **Este campo resuelve**: el problema que es el objeto solucionable del proyecto o la tarea se enumera en este campo.

   >[!NOTE]
   >
   >Los problemas no se pueden convertir en otros problemas, pero se pueden asociar manualmente a una solución. Un proyecto, tarea o problema puede tener varios problemas como objetos solucionables. Cuando se resuelve el proyecto, la tarea o el problema, también se resuelve el objeto solucionable (problema). El problema solucionable permanece cerrado aunque se vuelva a abrir el proyecto, la tarea o el problema que lo resolvió.

## Identificar un problema con un objeto de resolución en una lista

En una lista de problemas, puede identificar los que estén etiquetados como objetos de resolución mediante iconos de estado ubicando este icono en las columnas **Iconos de estado** o **Indicadores**:

![](assets/ro1.png)

## Ver información de objetos solucionables y de resolución en un informe

Puede mostrar información sobre los objetos que se pueden resolver o resolver en la vista o el informe de proyectos, tareas o problemas.\
En la tabla siguiente se muestran los campos que se pueden mostrar y en qué vistas se pueden mostrar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Campo en la vista</strong> </th> 
   <th><strong>Vista de problemas</strong> </th> 
   <th><strong>Vista de tareas</strong> </th> 
   <th><strong>Vista de proyecto</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Tiene elementos solucionables</strong>: muestra un valor <strong>Verdadero</strong> si el proyecto o la tarea tiene problemas solucionables asociados a ellos, y un valor <strong>Falso</strong> si no los tienen.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong>Nombre del problema original, Fecha de entrada del problema original, Nombre del creador</strong>: muestra el nombre y la fecha de entrada del problema original, así como el nombre del usuario que creó el problema en una vista personalizada en modo de texto.<br>Para obtener más información acerca de cómo crear una vista personalizada en modo de texto para un proyecto, informe de tareas o lista para mostrar información sobre el problema original, vea <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref">Ver: mostrar información del problema original en listas de tareas o proyectos</a>.<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Objetos solucionables:</strong> muestra una lista de todos los objetos solucionables en una vista personalizada de modo de texto para un informe o lista de proyecto o tarea.</p> <p>Para obtener más información acerca de cómo crear esta vista, vea <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref">Vista: objetos solucionables en un informe de tarea o proyecto</a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong>Creador de problema convertido</strong>: muestra información sobre el usuario que registró originalmente el problema y que posteriormente se convirtió en la tarea. </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Resolver proyecto</strong>: muestra información sobre el proyecto de resolución que se convirtió a partir del problema original o que se designó manualmente como el objeto de resolución de un problema.</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Resolver tarea</strong>: muestra información sobre la tarea de resolución que se convirtió a partir del problema original o que se designó manualmente como el objeto de resolución de un problema.</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Resolver problema</strong>: muestra información sobre el problema que se designó manualmente como el objeto de resolución de un problema.</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
