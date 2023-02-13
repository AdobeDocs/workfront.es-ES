---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar las preferencias de problemas y tareas de todo el sistema
description: Puede configurar las preferencias de todo el sistema para tareas y problemas. Estas preferencias afectan a la forma en que los usuarios crean las tareas y los problemas en Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 1%

---

# Configurar las preferencias de problemas y tareas de todo el sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

Como [!DNL Adobe Workfront] administrador, puede configurar las preferencias de todo el sistema para tareas y problemas. Estas preferencias afectan a la forma en que los usuarios crean las tareas y los problemas en [!DNL Workfront].

De forma predeterminada, las preferencias de tareas y problemas están bloqueadas y los administradores de grupos no pueden modificarlas a nivel de grupo a menos que las desbloquee para todos los grupos en el sistema. Para obtener más información, consulte la sección [Bloquear tareas y preferencias de problemas para grupos](#lock-task-and-issue-preferences-for-groups) en este artículo.

<!--SPLIT OUT BOTTOM SECTION TO NEW ARTICLE?-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure las preferencias de tareas y problemas para todos en [!DNL Workfront]

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Preferencias de proyecto]** >**[!UICONTROL Tareas y problemas].**

1. En la página que aparece, continúe con una de las 5 secciones enumeradas a continuación para configurar los parámetros de [!UICONTROL Nuevos valores predeterminados de tarea], [!UICONTROL Problemas], [!UICONTROL Eliminación], [!UICONTROL Fechas reales]y [!UICONTROL Acceso].
1. Haga clic en **[!UICONTROL Guardar]**.

* [[!UICONTROL Valores predeterminados de nueva tarea]](#new-task-defaults)
* [[!UICONTROL Problemas]](#issues)
* [[!UICONTROL Eliminación]](#deletion)
* [[!UICONTROL Fechas reales]](#actual-dates)
* [[!UICONTROL Delegación]](#delegation)

   <!--
  <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>
  -->

* [[!UICONTROL Acceso]](#access)

### [!UICONTROL Valores predeterminados de nueva tarea] {#new-task-defaults}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de inicio en nuevas tareas]</td> 
   <td> <p>Determina la fecha de inicio predeterminada para las nuevas tareas de los jefes de proyecto. La fecha de inicio de las nuevas tareas puede ser la fecha de inicio planificada del proyecto o el día en el que se crea la tarea.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de duración] </p> </td> 
   <td> <p>Determina la relación entre el número de recursos (y su porcentaje de asignación) y la duración o el esfuerzo total de la tarea. Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Duración de tarea y tipos de duración</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de ingresos]</td> 
   <td> <p>Calcula las estimaciones de ingresos reales y planeados para una tarea. Cuando la variable <strong>[!UICONTROL Tipo de ingresos]</strong> está configurado como<strong>[!UICONTROL No facturable]</strong>, las horas planificadas y las horas reales registradas no generan una estimación de ingresos para la tarea y el trabajo en la tarea no contribuye a los ingresos a nivel de proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de coste]</td> 
   <td> <p>Calcula las estimaciones de costes reales y planeadas de una tarea. Cuando se configura como <strong>[!UICONTROL Sin costo]</strong>, las horas planificadas y las horas reales registradas no generan una estimación de coste planificada o real para la tarea y el trabajo en la tarea no contribuye a los costes a nivel de proyecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Problemas {#issues}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actualizar automáticamente el estado del problema resuelto cuando cambia el estado del objeto resuelto]</td> 
   <td> <p>Cuando alguien convierte un problema en un proyecto o tarea, tanto el problema original como el proyecto o tarea convertido se convierten en objetos de resolución. Esta configuración le permite correlacionar la resolución del problema original con la resolución de su objeto resoluble. Para obtener más información sobre la resolución de objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y resolución de objetos </a>.</p> <p>Para que esta configuración tenga algún efecto, la opción <strong>[!UICONTROL Mantenga el problema original y vincule su resolución a la tarea]</strong> debe estar seleccionado.</p> 
    <ul> 
     <li>Cuando esta configuración está habilitada, puede crear estados personalizados con la misma clave tanto para problemas como para proyectos o tareas. Cuando el proyecto o la tarea (como objeto resoluble) se convierte en un estado personalizado, el cambio también refleja el estado del problema. La clave de estado debe ser la misma para el problema y los estados de proyecto o tarea.</li> 
     <li>Cuando se deshabilita esta configuración, la resolución de estados de objeto se establece automáticamente en el estado predeterminado, no en los personalizados. Para obtener más información sobre los estados predeterminados, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acceda a la lista de estados de problemas del sistema</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader" [!UICONTROL>Al convertir un problema en una tarea]</td> 
   <td> <p>La configuración de esta sección determina lo que sucede durante el proceso de conversión de un problema a otro:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mantenga el problema original y vincule su resolución a la tarea]</strong>: Cuando se convierte el problema, permanece visible como un problema hasta que se complete la tarea. El estado del problema cambia automáticamente a [!UICONTROL Cerrado] cuando se completa la tarea. Cuando se anula la selección, se elimina el problema.</p> <p><b>NOTA</b>:  <p>Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo estén convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concesión de acceso a problemas</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL Permitir que el contacto principal tenga acceso a la tarea]</strong>: Proporciona al contacto principal (creador del problema) acceso a la tarea para revisar la tarea, realizar actualizaciones y mantenerse informado de su progreso</li> 
     <li> <p><strong>[!UICONTROL Permitir que esta configuración cambie durante la conversión]</strong>: Permite al usuario que está convirtiendo el problema cambiar estas opciones durante la conversión de un problema en una tarea.</p> <!--
       Screenshot when possible</p>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Al convertir un problema en un proyecto]</td> 
   <td> <p>La configuración de esta sección determina lo que sucede durante el proceso de conversión de un problema a otro:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mantenga el problema original y vincule su resolución al proyecto]</strong>: Cuando esté convirtiendo el problema, permanecerá visible como un problema hasta que se complete el proyecto. El estado del problema cambia automáticamente a [!UICONTROL Cerrado] cuando el proyecto se completa. Cuando se anula la selección, se elimina el problema. </p> <p><b>NOTA</b>:  <p>Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo estén convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concesión de acceso a problemas</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL Permitir que el contacto principal tenga acceso al proyecto]</strong>: Proporciona al contacto principal (creador del problema) acceso al proyecto para revisar el proyecto, realizar actualizaciones y mantenerse informado de su progreso.</li> 
     <li><strong>[!UICONTROL Permitir que esta configuración cambie durante la conversión]</strong>: Permite al usuario que está convirtiendo el problema cambiar las opciones enumeradas durante la conversión de un problema en un proyecto.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminación] {#deletion}

**[!UICONTROL Permitir que los usuarios eliminen tareas y problemas con las horas registradas]**: Permite determinar si se permite la eliminación de tareas o problemas en los que se registran horas. Esta opción está seleccionada de forma predeterminada.

>[!TIP]
>
>Esta configuración también se aplica a la eliminación de proyectos que tengan tareas o problemas con horas registradas en ellos. Esta configuración no se aplica a la eliminación de proyectos en los que el tiempo se registra directamente para el proyecto.

* Cuando se selecciona, recibe una advertencia informativa al eliminar una tarea o problema. La advertencia le recuerda que si la tarea o el problema ha registrado horas, se moverán al proyecto o se eliminarán. Puede configurar si las horas se eliminan o se mueven al proyecto en el [!UICONTROL Preferencias de horario y horario] del [!UICONTROL Configuración]. Después de confirmar que ha visto la advertencia, se elimina la tarea o el problema. Para obtener más información sobre la configuración de las preferencias de horario y horario, consulte [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   >[!TIP]
   >
   >Cuando elimina un proyecto con tareas y problemas que han registrado horas, las horas registradas se eliminan o se conservan según la configuración de la [!UICONTROL Preferencias de horario y horario] área de [!UICONTROL Configuración]. El mensaje de advertencia no se muestra al eliminar un proyecto.

* Cuando anula la selección de esta opción, recibe una advertencia prohibitiva cuando elimina una tarea o problema con horas registradas, o cuando elimina un proyecto con horas registradas para sus tareas o problemas. La advertencia especifica que el administrador no permite que se eliminen tareas o problemas con horas registradas. Las tareas, los problemas o los proyectos que tienen horas registradas para tareas y problemas no se pueden eliminar.

### [!UICONTROL Fechas reales] {#actual-dates}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuando una tarea o problema pasa de "Nuevo" a "En curso", establezca la Fecha de inicio real en]</td> 
   <td> <p>Seleccione una de las siguientes opciones para cuándo se registra la fecha de inicio real en [!DNL Workfront] cuando una tarea o un problema provienen de <strong>[!UICONTROL Nuevo]</strong> a <strong>[!UICONTROL In Progress]</strong>:</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> La fecha de inicio real se establece en la fecha actual.</li> 
     <li><strong>[!UICONTROL La Fecha De Inicio Planificada]:</strong> La fecha de inicio real se establece en la fecha de inicio planeada de la tarea o el problema.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuando finaliza una tarea o problema, establezca la fecha de finalización real en]</td> 
   <td> <p>Seleccione una de las siguientes opciones para cuándo se registra la fecha de finalización real en [!DNL Workfront] cuando se complete una tarea o un problema:</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> La fecha de finalización real se establece en la fecha actual.</li> 
     <li> <p><strong>[!UICONTROL La Fecha De Finalización Planificada]:</strong> La Fecha de Finalización Real se establece en la Fecha de Finalización Planificada de la tarea o la emisión.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Delegación

Al habilitar la variable [!UICONTROL Permitir que los usuarios deleguen sus tareas y problemas] permite a todos los usuarios en delegar temporalmente su trabajo a otros.

Cuando esta configuración está habilitada, los usuarios pueden ver lo siguiente:

* La variable [!UICONTROL Delegar] vínculo en su [!UICONTROL Página principal] . Pueden delegar aprobaciones o tareas y emitir asignaciones desde aquí.
* Una indicación de que una tarea o un problema se delega a otro usuario en la variable [!UICONTROL Funciones y delegaciones] en el encabezado de la tarea o del problema.

Si desactiva el [!UICONTROL Permitir que los usuarios deleguen sus tareas y problemas] , las delegaciones programadas actualmente se detendrán y los usuarios delegados recibirán una notificación por correo electrónico de que la delegación se detuvo.

Para obtener información sobre la delegación de trabajo a otros, consulte los siguientes artículos:

* [Resumen del trabajo de los delegados](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Administrar delegación de tareas y problemas](../../../manage-work/delegate-work/how-to-delegate-work.md)

<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL Acceso] {#access}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuando alguien está asignado a una tarea]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Darles acceso a una tarea]</strong>: Define el permiso predeterminado que un usuario tiene para la tarea a la que está asignado. Para obtener más información sobre los permisos de tareas, consulte<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</li> 
     <li> <p><strong>[!UICONTROL Conceda también ... acceso al proyecto]</strong>: Define el permiso predeterminado que un usuario tiene para el proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuando alguien está asignado a un problema]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Darles acceso a una tarea]</strong>: Define el permiso predeterminado que un usuario tiene para la tarea a la que está asignado. Para obtener más información sobre los permisos de tareas, consulte<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</li> 
     <li> <p><strong>[!UICONTROL Conceda también ... acceso al proyecto]</strong>: Define el permiso predeterminado que un usuario tiene para el proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuando alguien envía una solicitud]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Denles acceso al problema]</strong>: Define el permiso predeterminado que tiene un usuario en una solicitud que envió. Para obtener más información, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a>.</li> 
     <li> <p><strong>[!UICONTROL Las personas de la misma empresa heredarán los mismos permisos para todas las solicitudes]</strong>: Permite a los usuarios ver las solicitudes enviadas por otros usuarios desde la misma empresa que ellos. Tienen los mismos permisos en esas solicitudes que tienen en sus propias solicitudes enviadas.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Bloquear tareas y preferencias de problemas para grupos {#lock-task-and-issue-preferences-for-groups}

Si los grupos de la organización necesitan una tarea o preferencias de problemas configurados de forma diferente para sus flujos de trabajo únicos, puede desbloquear la preferencia de todos los grupos de la organización para que puedan configurarla por su cuenta. Cuando se desbloquea una preferencia y el administrador del grupo la modifica, las tareas o los problemas asociados con el grupo se ven afectados por la configuración de nivel de grupo de la preferencia en lugar de por la configuración de nivel del sistema.

Para obtener información sobre cómo un administrador de grupo configura las preferencias de problemas y tareas de un grupo, consulte [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Después de un [!DNL Workfront] administrador desbloquea una preferencia a nivel de sistema, cualquier administrador de grupo puede configurarla y luego bloquearla para asegurarse de que todos los miembros de su grupo y los subgrupos siguientes usen la misma configuración. Esto es paralelo a la capacidad de que una [!DNL Workfront] El administrador debe configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, consulte [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Bloquear o desbloquear un proyecto, tarea o preferencia de problemas para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

Bloquear o desbloquear una tarea o emitir preferencias para que los grupos puedan configurarla

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Tareas y problemas]**.

1. Realice una de las siguientes acciones:

   * Si desea que los administradores de los grupos situados debajo del grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que su grupo y todos los grupos debajo utilicen su configuración para una preferencia, asegúrese de que esté bloqueado (este es el valor predeterminado).

      >[!IMPORTANT]
      >
      >Le recomendamos que se comunique con los administradores y usuarios en grupos de todo el sistema para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando lo bloquea, la configuración para él la heredan todos los grupos del sistema. Y si la preferencia se ha desbloqueado durante cualquier periodo de tiempo, la configuración sustituye a las que pueden haber realizado los administradores del grupo.

1. Haga clic en **[!UICONTROL Guardar]**.
