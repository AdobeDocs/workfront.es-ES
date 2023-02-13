---
product-area: projects
navigation-topic: convert-issues
title: Información general sobre la conversión de problemas en Adobe Workfront
description: Si es necesario trabajar más para completar un problema después de que se envíe el problema, puede convertir el problema en un proyecto o en una tarea.
author: Alina
feature: Work Management
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 2%

---

# Información general sobre la conversión de problemas en Adobe Workfront

Si es necesario trabajar más para completar un problema después de que se envíe el problema, puede convertir el problema en un proyecto o en una tarea.

Para obtener información sobre la conversión de problemas en tareas, consulte [Conversión de un problema en una tarea en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md).

Para obtener información sobre la conversión de problemas en proyectos, consulte [Convertir un problema en un proyecto en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Consideraciones al convertir problemas

* El administrador de Workfront o el administrador de grupo ya han establecido las preferencias para lo que sucede con un problema, su resolución y el acceso de su contacto principal cuando se convierte en un proyecto o una tarea, tal como se describe en [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Workfront elimina las aprobaciones que estén asociadas con problemas durante la conversión.
* Workfront sobrescribe el objeto resuelto del problema al convertirlo en una tarea o un proyecto. La nueva tarea o problema se convierte en el nuevo objeto resuelto del problema después de la conversión.
* Tenga en cuenta lo siguiente:

   * Durante la conversión, es posible que se le pregunte si desea mantener el problema y su resolución relacionados con el proyecto o la tarea que está creando.
   * Si mantiene el problema, el estado y el porcentaje completado del proyecto o tarea actualizan automáticamente el estado y el porcentaje completado del problema cuando se produce algún cambio en el proyecto, la tarea o el problema, o cuando Workfront vuelve a calcular la cronología.

* Al convertir un problema en un proyecto mediante una plantilla, la mayoría de la información de la plantilla se transfiere al nuevo proyecto. Sin embargo, parte de la información del tema también puede transferirse al nuevo proyecto. Para obtener más información, consulte la [Resumen de los campos del proyecto al convertir un problema en un proyecto mediante una plantilla](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) en este artículo.
* Al convertir un problema, no todos los documentos o su información se mueven al nuevo objeto al que se convierte el problema. Los siguientes elementos se incluyen al convertir un problema que tiene documentos o vínculos de documento adjuntos:

   * Documento
   * El documento vincula a servicios de terceros, como Google Drive o SharePoint.
   * Versiones
   * Las pruebas solo se incluyen cuando la opción **Mantener el problema original y enlazar su resolución a esta tarea** no está seleccionado.
   * Las aprobaciones de documentos no se incluyen cuando se convierte un problema que tiene documentos y vínculos de documentos adjuntos.

* Si ha decidido mantener el problema en la conversión y tiene documentos adjuntos, el documento y sus versiones se copian en el proyecto o en la tarea. Las pruebas y las aprobaciones de documento no se copian en el proyecto ni en la tarea.
* Si ha decidido no mantener el problema en la conversión y tiene documentos adjuntos, el documento, sus versiones y la transferencia de pruebas al proyecto o a la tarea. Las aprobaciones de documento no se transferirán al proyecto ni a la tarea.
* Si tiene documentos y carpetas vinculados al problema original desde servicios de terceros, como Google Drive, independientemente de si mantiene el problema o no durante la conversión, esos vínculos se copiarán en el nuevo objeto.
* Los comentarios del problema también se copian en la tarea o proyecto convertido desde el problema, pero los usuarios etiquetados no se transferirán.
* Si desea transferir información de formulario personalizada del problema al proyecto o tarea al que lo está convirtiendo, asegúrese de que tiene un formulario personalizado de proyecto o tarea que incluya los mismos campos que desea transferir del problema. Para obtener más información, consulte [Transferir datos de formulario personalizados al convertir un objeto](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

## Resumen de los campos del proyecto al convertir un problema en un proyecto mediante una plantilla {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

Al convertir un problema en un proyecto, puede convertirlo en un proyecto en blanco o utilizar una plantilla.

Para obtener más información, consulte [Convertir un problema en un proyecto en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

Al utilizar una plantilla, algunos campos rellenados en la plantilla se transfieren al proyecto creado a partir del problema convertido. Otros campos se transfieren al proyecto desde el número convertido.

En la tabla siguiente se muestra la información del proyecto y si se transfiere desde la plantilla o desde el problema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Descripción</td> 
   <td> <p>La Descripción de la emisión se transfiere al nuevo proyecto. </p> <p> Si no hay descripción del problema, la descripción de la plantilla se transfiere al proyecto. </p> <p>Si el campo Description está vacío tanto para el problema como para la plantilla, el campo está vacío en el proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>Estado</td> 
   <td>Estado predeterminado seleccionado para el grupo en la plantilla. Si la plantilla no está asociada al grupo, el estado del proyecto se establece en el estado predeterminado establecido por el administrador de Workfront en el área Preferencias del proyecto de Configuración. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</td> 
  </tr> 
  <tr> 
   <td>Prioridad</td> 
   <td>Transferencias de la plantilla. </td> 
  </tr> 
  <tr> 
   <td>Dirección URL</td> 
   <td> <p>La URL del problema se transfiere al nuevo proyecto. </p> <p> Si no se especifica ninguna dirección URL sobre el problema, la dirección URL de la plantilla se transfiere al proyecto. </p> <p>Si el campo URL está vacío tanto para el problema como para la plantilla, el campo está vacío en el proyecto. </p> </td> 
  </tr> 
  <tr> 
   <td>Tipo de condición del proyecto</td> 
   <td>Transferencias de la plantilla.</td> 
  </tr> 
  <tr> 
   <td>Condición del proyecto</td> 
   <td>Coincide con la preferencia predeterminada de nivel de sistema determinada por el administrador de Workfront en el área Configuración. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Establecer una condición personalizada como predeterminada para los proyectos</a></td> 
  </tr> 
  <tr> 
   <td>Programar desde</td> 
   <td>Transferencias de la plantilla.</td> 
  </tr> 
  <tr> 
   <td>Fechas del proyecto</td> 
   <td> 
    <ul> 
     <li> <p><b>Fecha de inicio planeada</b>: El tiempo de trabajo más cercano basado en el tiempo de trabajo de la plantilla debe preseleccionarse, según la zona horaria de la programación de la plantilla. Este campo está desactivado si el campo Programar desde está definido como Desde la finalización. </p> </li> 
     <li> <p><b>Fecha de finalización planeada</b>: El tiempo de trabajo más cercano basado en el tiempo de trabajo de la plantilla debe preseleccionarse, según la zona horaria de la programación de la plantilla. Este campo está desactivado si el campo Programar desde está definido como Desde el inicio. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Portafolio</td> 
   <td>Transferencias de la plantilla. De lo contrario, este campo está vacío.</td> 
  </tr> 
  <tr> 
   <td>Programar</td> 
   <td>Transferencias de la plantilla. De lo contrario, este campo está vacío.</td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>Transferencias de la plantilla. Si no hay ningún grupo en la plantilla, se establece en el grupo del proyecto al que pertenece el problema.</td> 
  </tr> 
  <tr> 
   <td>Compañía</td> 
   <td>Transferencias de la plantilla. De lo contrario, este campo está vacío.</td> 
  </tr> 
  <tr> 
   <td>Propietario del proyecto</td> 
   <td>Se transfiere desde el campo Propietario de plantilla de la plantilla. De lo contrario, se establece en el usuario que ha iniciado sesión y que está realizando la conversión. </td> 
  </tr> 
  <tr> 
   <td>Patrocinador de proyecto</td> 
   <td>Se transfiere desde el campo Patrocinador de plantilla de la plantilla. De lo contrario, este campo está vacío.</td> 
  </tr> 
  <tr> 
   <td>Administrador de recursos</td> 
   <td>Transferencias de la plantilla. De lo contrario, este campo está vacío.</td> 
  </tr> 
  <tr> 
   <td>Configuración de tarea</td> 
   <td>Se transfiere desde la plantilla .</td> 
  </tr> 
  <tr> 
   <td>Configuración de problema</td> 
   <td>Se transfiere desde la plantilla . </td> 
  </tr> 
  <tr> 
   <td>Acceso</td> 
   <td> <p>Transferencias desde la sección Acceso de la plantilla. </p> </td> 
  </tr> 
  <tr> 
   <td>Rutas de aprobación</td> 
   <td>Se transfiere desde la plantilla . Las aprobaciones asociadas con el problema se eliminan durante la conversión. </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-issues-icon-highlighted-on-project.png"> </p> </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p> <p> <img src="assets/qs-issue-more-menu-highlighted-350x469.png" style="width: 350;height: 469;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p> <p> <img src="assets/qs-issue-more-menu-highlighted-350x469.png" style="width: 350;height: 469;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## Ver la información del problema original en proyectos y tareas {#view-original-issue-information-on-projects-and-tasks}

Puede ver la información del problema original en listas e informes de proyectos y tareas o en el área Detalles del proyecto . Para obtener información sobre la creación de informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

La siguiente tabla ilustra qué campos de problema son visibles desde los proyectos y tareas convertidos.

| Campos de problema | Campo de proyecto o tarea | Lista de proyectos o informe | Área Detalles del proyecto | Lista de tareas o informe | Área Detalles de la tarea |
|---|---|---|---|---|---|
| Nombre de problema | Nombre de problema convertido | š | ✔ | ✔ | ✔ |
| Contacto primario | Nombre del creador del problema convertido | ✔ | `✔` | ✔ |   |
| Fecha de entrada | Fecha de entrada de emisión convertida | ✔ |   | ✔ |   |


>[!CAUTION]
>
>Si el Contacto principal de un problema cambia o si el problema se desvincula del proyecto o la tarea después de que se haya convertido el problema, el Nombre del creador del problema convertido no se actualiza y muestra el Contacto principal original del problema en el momento en que se convirtió el problema.
