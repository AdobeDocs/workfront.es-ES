---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar las preferencias de tareas y problemas de todo el sistema
description: Puede configurar las preferencias de todo el sistema para tareas y problemas. Estas preferencias afectan a la forma en que los usuarios crean tareas y problemas en Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '2110'
ht-degree: 0%

---

# Configurar las preferencias de tareas y problemas de todo el sistema

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

Como administrador de [!DNL Adobe Workfront], puede configurar las preferencias de todo el sistema para tareas y problemas. Estas preferencias afectan la forma en que los usuarios crean tareas y problemas en [!DNL Workfront].

De forma predeterminada, las preferencias de tareas y problemas están bloqueadas y los administradores de grupos no pueden modificarlas en el nivel de grupo a menos que las desbloquee para todos los grupos del sistema. Para obtener más información, consulte la sección [Bloquear tareas y preferencias de problemas para grupos](#lock-task-and-issue-preferences-for-groups) en este artículo.


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   o
   <p>Actual: [!UICONTROL plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar las preferencias de tareas y problemas para todos en [!DNL Workfront]

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Preferencias del proyecto]** >**[!UICONTROL Tareas y problemas].**

1. En la página que aparece, continúe con una de las 5 secciones que se enumeran a continuación para configurar las opciones de [!UICONTROL Valores predeterminados de nueva tarea], [!UICONTROL Problemas], [!UICONTROL Eliminación], [!UICONTROL Fechas reales] y [!UICONTROL Acceso]:

   * [[!UICONTROL Valores predeterminados de nueva tarea]](#new-task-defaults)
   * [[!UICONTROL Problemas]](#issues)
   * [[!UICONTROL Eliminación]](#deletion)
   * [[!UICONTROL Fechas reales]](#actual-dates)
   * [[!UICONTROL Delegación]](#delegation)

   <!--
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Trabajar En Ello</a> </li>
  --&gt;

* [[!UICONTROL Acceso]](#access)

### [!UICONTROL Valores predeterminados de nueva tarea] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Fecha de inicio]</td> 
    <td> <p>Determina la fecha de comienzo predeterminada de las nuevas tareas para los jefes de proyecto. La fecha de inicio de las nuevas tareas puede ser la fecha de inicio planeada del proyecto o el día en que se crea la tarea.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Tipo de duración] </p> </td> 
    <td> <p>Determina la relación entre el número de recursos (y su porcentaje de asignación) y la duración o el esfuerzo total de la tarea. Para obtener más información, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Duración de la tarea y Tipos de duración</a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Tipo de ingresos]</td> 
    <td> <p>Calcula las estimaciones de ingresos planificadas y reales de una tarea. Cuando <strong>[!UICONTROL tipo de ingresos]</strong> se establece en <strong>[!UICONTROL no facturable]</strong>, las horas planificadas y las horas registradas no generan una estimación de ingresos para la tarea y el trabajo en la tarea no contribuye a los ingresos de nivel de proyecto.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Tipo de costo]</td> 
    <td> <p>Calcula las estimaciones de costos planificadas y reales de una tarea. Cuando se establece en <strong>[!UICONTROL Sin costo]</strong>, las horas planificadas y las horas registradas no generan una estimación de costo planificada o real para la tarea, y el trabajo en la tarea no contribuye a los costos en el nivel de proyecto.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Problemas {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Actualizar automáticamente el estado del problema solucionable cuando cambie el estado del objeto de resolución]</td> 
    <td> <p>Cuando alguien convierte un problema en un proyecto o tarea, tanto el problema original como el proyecto o tarea convertidos se convierten en objetos de resolución. Esta configuración le permite correlacionar la resolución del problema original con la resolución de su objeto solucionable. Para obtener más información sobre la resolución de objetos, vea <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y los objetos solucionables </a>.</p> <p>Para que esta configuración surta efecto, se debe seleccionar la opción <strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong>.</p> 
      <ul> 
      <li>Cuando esta configuración está habilitada, puede crear estados personalizados con la misma clave para problemas y proyectos o tareas. Cuando el proyecto o la tarea (como objeto solucionable) se convierte en el estado personalizado, el cambio también se refleja en el estado del problema. La clave de estado debe ser la misma para los estados de problema y proyecto o tarea.</li> 
      <li>Cuando esta configuración está desactivada, los estados de objetos de resolución se establecen automáticamente en el estado predeterminado en lugar de en los personalizados. Para obtener más información acerca de los estados predeterminados, vea <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acceso a la lista de estados de problemas del sistema</a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Al convertir un problema en una tarea]</td> 
    <td> <p>La configuración de esta sección determina qué sucede durante el proceso de conversión de un problema a una tarea:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Mantener el problema original y enlazar su resolución a la tarea]</strong>: Cuando convierta el problema, permanecerá visible como un problema hasta que se complete la tarea. El estado del problema cambia automáticamente a [!UICONTROL Cerrado] cuando finaliza la tarea. Si no selecciona esta opción, se elimina el problema.</p> <p><b>NOTA</b>:  <p>Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo vayan convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acceso a problemas</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Permitir que el contacto principal tenga acceso a la tarea]</strong>: otorga al contacto principal (creador del problema) acceso de vista a la tarea para revisar la tarea, mantenerse informado de su progreso y realizar comentarios en la sección Actualizaciones de la tarea.</li> 
      <li> <p><strong>[!UICONTROL Permitir cambiar esta configuración durante la conversión]</strong>: permite al usuario que está convirtiendo el problema cambiar estas opciones durante la conversión de un problema en una tarea.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Al convertir un problema en un proyecto]</td> 
    <td> <p>La configuración de esta sección determina qué sucede durante el proceso de conversión de un problema a un proyecto:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Mantener el problema original y enlazar su resolución al proyecto]</strong>: Cuando convierta el problema, permanecerá visible como un problema hasta que se complete el proyecto. El estado del problema cambia automáticamente a [!UICONTROL Cerrado] cuando finaliza el proyecto. Si no selecciona esta opción, se elimina el problema. </p> <p><b>NOTA</b>:  <p>Los usuarios sin acceso o permisos para eliminar problemas no podrán eliminar el problema a medida que lo vayan convirtiendo, independientemente del estado de esta configuración. Para obtener información sobre el acceso y los permisos a los problemas, consulte:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acceso a problemas</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Permitir que el contacto principal tenga acceso al proyecto]</strong>: otorga al contacto principal (creador del problema) acceso de vista al proyecto para revisar el proyecto, mantenerse informado de su progreso y realizar comentarios en la sección Actualizaciones del proyecto.</li> 
      <li><strong>[!UICONTROL Permitir cambiar esta configuración durante la conversión]</strong>: permite al usuario que está convirtiendo el problema cambiar las opciones de la lista durante la conversión de un problema en un proyecto.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Eliminación] {#deletion}

**[!UICONTROL Permitir que los usuarios eliminen tareas y problemas con las horas registradas]**: Permite determinar si permite la eliminación de tareas o problemas en los que se registran horas. Esta opción está seleccionada de forma predeterminada.

>[!TIP]
>
>Esta configuración también se aplica a la eliminación de proyectos que tienen tareas o problemas con horas registradas en ellos. Esta configuración no se aplica a los proyectos de eliminación en los que el tiempo se registra directamente en el proyecto.

* Cuando se selecciona, recibe una advertencia informativa cuando elimina una tarea o un problema. La advertencia le recuerda que si la tarea o el problema han registrado horas, se moverán al proyecto o se eliminarán. Puede configurar si las horas se eliminan o se mueven al proyecto en el área [!UICONTROL Preferencias de horas y hoja de horas] del [!UICONTROL programa de instalación]. Después de confirmar que ha visto la advertencia, la tarea o el problema se eliminan. Para obtener más información sobre cómo configurar las preferencias de horas y hojas de horas, consulte [Configurar las preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  >[!TIP]
  >
  >Cuando elimina un proyecto con tareas y problemas que han registrado horas, estas se eliminan o se conservan de acuerdo con la configuración del área [!UICONTROL Preferencias de hoja de horas y horas] de [!UICONTROL Configuración]. El mensaje de advertencia no se muestra al eliminar un proyecto.

* Si anula la selección de esta opción, recibe una advertencia prohibitiva cuando elimina una tarea o un problema con horas registradas, o cuando elimina un proyecto con horas registradas para sus tareas o problemas. La advertencia especifica que el administrador no permite que se eliminen tareas o problemas con horas registradas. Las tareas, problemas o proyectos que tienen horas registradas para tareas y problemas no se pueden eliminar.

### [!UICONTROL Fechas reales] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cuando una tarea o un problema pasen de "Nuevo" a "En curso", establecer la Fecha real de inicio en]</td> 
    <td> <p>Seleccione una de las siguientes opciones para cuándo se registra la fecha de inicio real en [!DNL Workfront] cuando una tarea o un problema pasa de <strong>[!UICONTROL Nuevo]</strong> a <strong>[!UICONTROL En curso]</strong>:</p> 
      <ul> 
      <li><strong>[!UICONTROL Ahora]:</strong> La fecha de inicio real está establecida en la fecha actual.</li> 
      <li><strong>[!UICONTROL Fecha planificada de inicio]:</strong> La fecha real de inicio se establece en la fecha planificada de inicio de la tarea o problema.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cuando se complete una tarea o un problema, establecer la Fecha real de finalización en]</td> 
    <td> <p>Seleccione una de las siguientes opciones para cuándo se registra la fecha real de finalización en [!DNL Workfront] cuando se completa una tarea o un problema:</p> 
      <ul> 
      <li><strong>[!UICONTROL Ahora]:</strong> La fecha real de finalización está establecida en la fecha actual.</li> 
      <li> <p><strong>[!UICONTROL Fecha planificada de finalización]:</strong> La fecha real de finalización está establecida en la fecha planificada de finalización de la tarea o problema.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Delegación

Habilitar la opción **[!UICONTROL Permitir que los usuarios deleguen sus tareas y problemas]** permite que todos los usuarios de deleguen temporalmente su trabajo a otros.

Cuando esta configuración está habilitada, los usuarios pueden ver lo siguiente:

* El vínculo [!UICONTROL **Delegar**] en sus widgets [!UICONTROL Mi trabajo], [!UICONTROL Mis tareas] o [!UICONTROL Mis problemas] en el área [!UICONTROL Inicio]. Pueden delegar asignaciones de tareas y problemas desde allí.

  >[!NOTE]
  >
  >  El vínculo [!UICONTROL **Delegar aprobaciones**] siempre está habilitado en el área de [!UICONTROL Inicio].

* Una indicación de que una tarea o un problema se ha delegado a otro usuario en el área [!UICONTROL Asignaciones y delegaciones] del encabezado de la tarea o el problema.
* Una indicación de que una tarea o un problema se ha delegado a otro usuario en su widget de [!UICONTROL Mi trabajo] en [!UICONTROL Inicio].

  Si deshabilita la opción [!UICONTROL Permitir que los usuarios deleguen sus tareas y problemas], las delegaciones programadas actualmente se detendrán y los usuarios delegados recibirán una notificación por correo electrónico avisando que la delegación se detuvo.

Para obtener información sobre cómo delegar el trabajo a otros, consulte los siguientes artículos:

* [Resumen del trabajo delegado](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Delegar tareas y problemas](../../../manage-work/delegate-work/how-to-delegate-work.md)


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
    <td role="rowheader">[!UICONTROL Cuando se asigna a alguien a una tarea]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Dar a ellos ... acceso a una tarea]</strong>: Define el permiso predeterminado que un usuario tiene para la tarea a la que está asignado. Para obtener más información acerca de los permisos de tareas, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</li> 
      <li> <p><strong>[!UICONTROL También concederles ... acceso al proyecto]</strong>: Define el permiso predeterminado que un usuario tiene para el proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cuando se asigna a alguien a un problema]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Dar a ellos ... acceso a una tarea]</strong>: Define el permiso predeterminado que un usuario tiene para la tarea a la que está asignado. Para obtener más información acerca de los permisos de tareas, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</li> 
      <li> <p><strong>[!UICONTROL También concederles ... acceso al proyecto]</strong>: Define el permiso predeterminado que un usuario tiene para el proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cuando alguien envía una solicitud]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Dar a ellos ... acceso al problema]</strong>: Define el permiso predeterminado que un usuario tiene en una solicitud que envió. Para obtener más información, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a>.</li> 
      <li> <p><strong>[!UICONTROL Las personas de la misma compañía heredarán los mismos permisos para todas las solicitudes]</strong>: permite a los usuarios ver las solicitudes enviadas por otros usuarios de la misma compañía que ellos. Tienen los mismos permisos en esas solicitudes que en sus propias solicitudes enviadas.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Haga clic en **[!UICONTROL Guardar]**.

## Bloquear las preferencias de tareas y problemas para grupos {#lock-task-and-issue-preferences-for-groups}

Si los grupos de su organización necesitan una preferencia de tarea o problema configurada de forma diferente para sus flujos de trabajo únicos, puede desbloquear la preferencia de todos los grupos de la organización para que puedan configurarla por su cuenta. Cuando una preferencia está desbloqueada y el administrador del grupo la modifica, las tareas o problemas asociados con el grupo se ven afectados por la configuración de nivel de grupo para la preferencia en lugar de por la configuración de nivel de sistema.

Para obtener información sobre cómo un administrador de grupo configura las preferencias de tareas y problemas de un grupo, consulte [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Después de que un administrador de [!DNL Workfront] desbloquee una preferencia en el sistema, cualquier administrador de grupo puede configurarla y después bloquearla para asegurarse de que todos los miembros de su grupo y de los subgrupos que se muestran a continuación usan la misma configuración. Esto es paralelo a la capacidad que tiene un administrador de [!DNL Workfront] para configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, vea [Configurar las preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Bloquear o desbloquear una preferencia de proyecto, tarea o problema para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

Para bloquear o desbloquear una preferencia de tarea o problema para que los grupos puedan configurarla:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Preferencias del proyecto]** > **[!UICONTROL Tareas y problemas]**.

1. Realice una de las siguientes acciones:

   * Si desea que los administradores de los grupos que se encuentran debajo de su grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que su grupo y todos los grupos debajo de él utilicen su configuración para una preferencia, asegúrese de que esté bloqueada (este es el valor predeterminado).

     >[!IMPORTANT]
     >
     >Le recomendamos que se comunique con los administradores y usuarios de los grupos de todo el sistema para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando lo bloquea, la configuración para él la heredan todos los grupos del sistema. Y si la preferencia se ha desbloqueado durante cualquier período de tiempo, la configuración reemplaza las que los administradores del grupo puedan haber realizado.

1. Haga clic en **[!UICONTROL Guardar]**.
