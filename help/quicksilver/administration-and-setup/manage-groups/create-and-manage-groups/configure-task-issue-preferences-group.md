---
title: Configurar las preferencias de tareas y problemas de un grupo
user-type: administrator
product-area: system-administration;user-management;setup
keywords: grupo, preferencias, tarea, problema, desbloquear
navigation-topic: create-and-manage-groups
description: Si los grupos de su organización necesitan configurar una preferencia de tarea o problema de forma independiente de la forma en que se configura en el sistema, un administrador de Adobe Workfront puede desbloquear la preferencia. A continuación, como administrador de grupo, puede configurar la preferencia de su grupo, lo cual afectará a todas las tareas o problemas asociados con su grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '2185'
ht-degree: 88%

---

# Configurar las preferencias de tareas y problemas de un grupo

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Si los grupos de su organización necesitan configurar una preferencia de tarea o problema de forma independiente de la forma en que se configura en el sistema, un administrador de Adobe Workfront puede desbloquear la preferencia. A continuación, como administrador de grupo, puede configurar la preferencia de su grupo, lo cual afectará a todas las tareas o problemas asociados con su grupo.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener información sobre cómo el administrador de Workfront desbloquea las preferencias, consulte [Bloquear o desbloquear las preferencias de proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>La configuración de nivel de grupo también es posible para las preferencias de proyecto. Para obtener más información, vea [Configurar las preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* Normalmente, una preferencia desbloqueada permanecerá desbloqueada indefinidamente. Si el administrador de Workfront volviese a bloquearla, la configuración del sistema volverá a tener efecto y se perderá la configuración de las preferencias realizadas por los administradores del grupo.
>* Las preferencias establecidas para el grupo asociado a un proyecto tendrán prioridad sobre las preferencias establecidas para el grupo de inicio del usuario que cree el proyecto.
>* Algunas preferencias de nivel de grupo afectarán a las plantillas de proyecto que cree para el grupo. Para obtener más información, consulte la sección [Ver, trabajar y crear plantillas para grupos desde el área Grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) en el artículo [Crear y modificar plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Una vez que un administrador de Workfront desbloquee una preferencia en el sistema, podrá configurarla y, a continuación, bloquearla para garantizar que todos los miembros del grupo y los subgrupos usen la misma configuración. Esto es similar a la capacidad que tiene un administrador de Workfront para configurar y bloquear preferencias para todos los miembros del sistema. Para obtener más información, vea [Bloquear o desbloquear las preferencias de proyecto, tarea o problema de los subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar las preferencias de tareas y problemas desbloqueados para un grupo de nivel superior

>[!TIP]
>
>Si es administrador de Workfront, puede omitir los pasos 1-4 si va a Configuración > Preferencias de proyecto > Tareas y problemas y busca el nombre del grupo en el cuadro de la parte superior de la página.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos**![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea configurar las preferencias de tareas y problemas desbloqueados.
1. En la página que se muestra para el grupo, en el panel izquierdo, haga clic en **Preferencias de tarea y problema**.
1. En la página que aparece, continúe con una de las 5 secciones que se enumeran a continuación para configurar las opciones de las áreas Valores predeterminados de nueva tarea, Problemas, Eliminación, Fechas reales y Acceso, y luego haga clic en **Guardar**.

   Si pasa el ratón sobre el icono de candado ![](assets/lock-toggle-button-dimmed.png) para ver una preferencia que debe configurar y aparece información del objeto que le indica que está bloqueado, puede pedirle al administrador de Workfront que lo desbloquee para todos los grupos de la organización.

   Cuando está desbloqueado, usted y otros administradores del grupo pueden configurarlo por separado para sus propios grupos. Además, puede bloquearlo para su grupo y para cualquier subgrupo debajo de su grupo.

   * [Valores predeterminados de nueva tarea](#new-task-defaults)
   * [Problemas](#issues)
   * [Eliminación](#deletion)
   * [Mover](#move)
   * [Fechas reales](#actual-dates)
   * [Delegación](#delegation)
   * [Acceso](#access)

### Valores predeterminados de nueva tarea {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fecha de inicio en tareas nuevas</td> 
      <td> <p>Determina la fecha de comienzo predeterminada de las nuevas tareas para los jefes de proyecto. La fecha de inicio de las nuevas tareas puede ser la fecha de inicio planificada del proyecto o el día en que se crea la tarea.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tipo de duración </p> </td> 
      <td> <p>Determina la relación entre el número de recursos (y su porcentaje de asignación) y la duración o el esfuerzo total de la tarea. Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Duración y tipos de duración de la tarea: índice de artículos</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de ingresos</td> 
      <td> <p>Calcula las estimaciones de ingresos planificados y reales de una tarea. Cuando el <strong>Tipo de ingresos</strong> se establece en <strong>No facturable</strong>, las horas planificadas y las horas reales registradas no generan una estimación de ingresos para la tarea, y el trabajo de la tarea no contribuye a los ingresos del nivel de proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de costo</td> 
      <td> <p>Calcula las estimaciones de costes planificados y reales de una tarea. Cuando se establece en <strong>Sin coste</strong>, las horas planificadas y las horas reales registradas no generan una estimación de costes planificados o reales para la tarea, y el trabajo de la tarea no contribuye a los costes del nivel de proyecto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

### Problemas {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Actualizar automáticamente el estado del problema solucionable cuando cambie el estado del objeto de resolución</td> 
      <td> <p>Cuando alguien convierte un problema en un proyecto o tarea, tanto el problema original como el proyecto o tarea convertidos se convierten en objetos de resolución. Esta configuración permite correlacionar la resolución del problema original con la resolución del nuevo objeto que se puede resolver. Para obtener más información sobre la resolución de objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y los objetos solucionables </a>.</p> <p>Para que esta configuración tenga algún efecto, la opción <strong>Mantener el problema original y vincular su resolución a la tarea</strong> debe estar seleccionada.</p> 
       <ul> 
        <li>Cuando esta configuración está habilitada, puede crear estados personalizados con la misma clave para problemas y proyectos o tareas. Cuando el proyecto o la tarea (como objeto solucionable) cambia al estado personalizado, el cambio también se refleja en el estado del problema. La clave de estado debe ser la misma para los estados de problema y proyecto o tarea.</li> 
        <li>Cuando esta configuración está desactivada, los estados de objetos de resolución se establecen automáticamente en el estado predeterminado en lugar de hacerlo en los personalizados. Para obtener más información acerca de los estados predeterminados, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acceder a la lista de estados de problemas del sistema</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando se convierte un problema en una tarea</td> 
      <td> <p>La configuración de esta sección determina qué sucede durante el proceso de conversión de un problema a una tarea:</p> 
       <ul> 
        <li><strong>Conservar el problema original y vincular su resolución a la tarea</strong>: cuando esté convirtiendo el problema, permanecerá visible como problema hasta que se complete la tarea. El estado del problema cambiará automáticamente a Cerrado cuando se complete la tarea.</li> 
        <li><strong>Permitir que el contacto principal tenga acceso a la tarea</strong>: otorga al contacto principal (creador del problema) acceso a la tarea para revisarla, realizar actualizaciones y mantenerse al corriente de su progreso</li> 
        <li> <p><strong>Permitir cambiar esta configuración durante la conversión</strong>: permite al usuario que está convirtiendo el problema cambiar estas opciones durante la conversión de un problema en una tarea.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando se convierte un problema en un proyecto</td> 
      <td> <p>La configuración de esta sección determina qué sucede durante el proceso de conversión de un problema a un proyecto:</p> 
       <ul> 
        <li><strong>Conservar el problema original y vincular su resolución al proyecto</strong>: cuando esté convirtiendo el problema, permanecerá visible como problema hasta que se complete el proyecto. El estado del problema cambiará automáticamente a Cerrado cuando se complete el proyecto.</li> 
        <li><strong>Permitir que el contacto principal tenga acceso al proyecto</strong>: otorga al contacto principal (creador del problema) acceso al proyecto para revisarlo, realizar actualizaciones y mantenerse al corriente de su progreso.</li> 
        <li><strong>Permitir cambiar esta configuración durante la conversión</strong>: permite al usuario que está convirtiendo el problema cambiar las opciones enumeradas durante la conversión de un problema en un proyecto.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Eliminación {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Permitir que los usuarios eliminen tareas y problemas con horas registradas</td> 
      <td> <p> Permite determinar si se permite la eliminación de tareas o problemas en los que se registran horas. Esta opción está desactivada de forma predeterminada.</p> 
       <div> 
        <p><b>Sugerencia</b>: Esta opción de configuración también se aplica a la eliminación de proyectos que tienen tareas o problemas con horas registradas. Esta configuración no se aplica a los proyectos de eliminación en los que el tiempo se registra directamente en el proyecto. </p> 
        <p>Tenga en cuenta lo siguiente:</p> 
        <ul> 
         <li> <p>Cuando se selecciona, recibe una advertencia informativa cuando elimina una tarea o un problema. La advertencia le recuerda que si la tarea o el problema han registrado horas, se moverán al proyecto o se eliminarán. Puede configurar si las horas se eliminan o se mueven al proyecto en el área Preferencias de horas y plantillas de horas de Configuración. Después de confirmar que ha visto la advertencia, la tarea o el problema se eliminan. Para obtener más información sobre cómo configurar las preferencias de horas y plantillas de horas, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurar las preferencias de horas y plantillas de horas</a>. </p> <p>Sugerencia: <span>Cuando se elimina un proyecto con tareas y problemas que han registrado horas, estas se eliminan o se conservan de acuerdo con la configuración del área Preferencias de horas y plantillas de horas de Configuración</span>. </p> </li> 
         <li><span>Cuando anula la selección de esta opción, recibe una advertencia de prohibición al eliminar una tarea o un problema con horas registradas, o al eliminar un proyecto con horas registradas para sus tareas o problemas</span> <span>.</span> La advertencia especifica que la persona con la función de administrador no permite que se eliminen tareas o problemas con horas registradas. No se pueden eliminar las tareas, problemas<span> o proyectos que tienen horas registradas para tareas y problemas</span>. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>


### Mover

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Permitir que los usuarios muevan tareas y problemas con horas registradas</td> 
      <td> <p> Permite determinar si permite el movimiento de tareas o problemas donde se registran las horas. Esta opción está desactivada de forma predeterminada.</p> 
       <p>Tenga en cuenta lo siguiente:</p> 
        <ul> 
         <li> Cuando está seleccionada, puede mover tareas y problemas que tengan tiempo registrado. Las horas también se mueven con las tareas o problemas. </li>
      <li>Si anula la selección de esta opción, recibe una advertencia prohibitiva cuando mueve una tarea o un problema con horas registradas. La advertencia especifica que el administrador no permite mover tareas o problemas con horas registradas. Las tareas o los problemas que tienen horas registradas no se pueden mover a otro proyecto. Puede mover tareas con horas registradas dentro del mismo proyecto, incluso con esta opción sin seleccionar.  </li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

### Fechas reales {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Cuando una tarea o un problema pasen de “Nuevo” a “En curso”, establecer la fecha de inicio real en</td> 
      <td> <p>Seleccione una de las siguientes opciones para indicar cuándo desea que se registre la fecha de inicio real en Workfront cuando una tarea o un problema pase de <strong>Nuevo</strong> a <strong>En curso</strong>:</p> 
       <ul> 
        <li><strong>Ahora:</strong> la fecha de inicio real se establece en la fecha actual.</li> 
        <li><strong>Fecha de inicio planificada:</strong> la fecha de inicio real se establece en la fecha planificada de inicio de la tarea o problema.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando se complete una tarea o un problema, establecer la fecha de finalización real en</td> 
      <td> <p>Seleccione una de las siguientes opciones cuando la fecha de finalización real esté registrada en Workfront cuando se complete una tarea o un problema:</p> 
       <ul> 
        <li><strong>Ahora:</strong> la fecha de finalización real se establece en la fecha actual.</li> 
        <li> <p><strong>Fecha planificada de finalización:</strong> la fecha real de finalización se establece en la fecha planificada de finalización de la tarea o problema.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### Delegación

Habilitar la opción **[!UICONTROL Permitir que los usuarios deleguen sus tareas y problemas]** permite que todos los usuarios del grupo deleguen temporalmente su trabajo a otros.

Cuando esta configuración está habilitada, los usuarios del grupo pueden ver lo siguiente:

* El vínculo [!UICONTROL **Delegar**] en sus widgets [!UICONTROL Mi trabajo], [!UICONTROL Mis tareas] o [!UICONTROL Mis problemas] en el área [!UICONTROL Inicio]. Pueden delegar asignaciones de tareas y problemas desde allí.

  >[!NOTE]
  >
  >  El vínculo [!UICONTROL **Delegar aprobaciones**] siempre está habilitado en el área de [!UICONTROL Inicio].

* Una indicación de que una tarea o un problema se ha delegado a otro usuario en el área [!UICONTROL Assignments and delegations] del encabezado de la tarea o el problema.
* Una indicación de que una tarea o un problema se ha delegado a otro usuario en su widget de [!UICONTROL Mi trabajo] en [!UICONTROL Inicio].

  Si deshabilita la opción [!UICONTROL Permitir que los usuarios deleguen sus tareas y problemas], las delegaciones programadas actualmente se detendrán y los usuarios delegados recibirán una notificación por correo electrónico de que la delegación se ha detenido.

Para obtener información sobre la delegación del trabajo a otras personas, consulte los siguientes artículos:

* [Información general sobre la delegación de trabajo](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Delegar tareas y problemas](../../../manage-work/delegate-work/how-to-delegate-work.md)

### Acceso {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Cuando se asigna a una persona una tarea</td> 
      <td> 
       <ul> 
        <li><strong>Concederles... acceso a una tarea</strong>: define el permiso predeterminado que un usuario tiene para la tarea que tiene asignada. Para obtener más información sobre los permisos de la tarea, consulte<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Conceder acceso a los usuarios</a>.</li> 
        <li> <p><strong>Concederles también... acceso al proyecto</strong>: define el permiso predeterminado que un usuario tiene para acceder al proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando se asigna a una persona un problema</td> 
      <td> 
       <ul> 
        <li><strong>Concederles... acceso a una tarea</strong>: define el permiso predeterminado que un usuario tiene para la tarea que tiene asignada. Para obtener más información sobre los permisos de la tarea, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</li> 
        <li> <p><strong>Concederles también... acceso al proyecto</strong>: define el permiso predeterminado que un usuario tiene para acceder al proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando alguien envía una solicitud</td> 
      <td> 
       <ul> 
        <li><strong>Concederles... acceso al problema</strong>: Define el permiso predeterminado que tiene un usuario sobre una solicitud que ha enviado. Para obtener más información, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema</a>.</li> 
        <li> <p><strong>Las personas de la misma compañía heredarán los mismos permisos para todas las solicitudes</strong>: permite a los usuarios ver las solicitudes enviadas por otros usuarios de la misma compañía que ellos. Tienen los mismos permisos sobre esas solicitudes que los que tienen sobre sus propias solicitudes enviadas.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
