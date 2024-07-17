---
title: Configurar las preferencias de tareas y problemas de un grupo
user-type: administrator
product-area: system-administration;user-management;setup
keywords: grupo, preferencias, tarea, problema, desbloquear
navigation-topic: create-and-manage-groups
description: Si los grupos de su organización necesitan configurar una preferencia de tarea o problema de forma independiente de la forma en que se configura en el sistema, un administrador de Adobe Workfront puede desbloquear la preferencia. A continuación, como administrador de grupo, puede configurar la preferencia de su grupo y esto afectará a todas las tareas o problemas asociados con su grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 4a9936b6bc034f2176167fc3939d647ee679a888
workflow-type: tm+mt
source-wordcount: '1895'
ht-degree: 2%

---

# Configurar las preferencias de tareas y problemas de un grupo

Si los grupos de su organización necesitan configurar una preferencia de tarea o problema de forma independiente de la forma en que se configura en el sistema, un administrador de Adobe Workfront puede desbloquear la preferencia. A continuación, como administrador de grupo, puede configurar la preferencia de su grupo y esto afectará a todas las tareas o problemas asociados con su grupo.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener información sobre cómo el administrador de Workfront desbloquea las preferencias, consulte [Bloquear o desbloquear las preferencias de proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>La configuración de nivel de grupo también es posible para las preferencias de proyecto. Para obtener más información, vea [Configurar las preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* Normalmente, una preferencia desbloqueada permanece desbloqueada indefinidamente. Si el administrador de Workfront vuelve a bloquearlo, la configuración del sistema vuelve a tener efecto y se pierde la configuración de las preferencias realizadas por los administradores del grupo.
>* Las preferencias establecidas para el grupo asociado a un proyecto tienen prioridad sobre las preferencias establecidas para el grupo de inicio del usuario que crea el proyecto.
>* Algunas preferencias de nivel de grupo afectan a las plantillas de proyecto que crea para el grupo. Para obtener más información, consulte la sección [Ver, trabajar y crear plantillas para su grupo desde el área de grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) en el artículo [Crear y modificar plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Una vez que un administrador de Workfront desbloquea una preferencia en el sistema, puede configurarla y, a continuación, bloquearla para garantizar que todos los miembros del grupo y de sus subgrupos estén utilizando la misma configuración. Esto es paralelo a la capacidad que tiene un administrador de Workfront para configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, vea [Bloquear o desbloquear las preferencias de proyecto, tarea o problema de los subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Configurar las preferencias de tareas y problemas desbloqueados para un grupo de nivel superior

>[!TIP]
>
>Si es administrador de Workfront, puede omitir los pasos 1-4 si va a Configuración > Preferencias de proyecto > Tareas y problemas y busca el nombre del grupo en el cuadro de la parte superior de la página.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea configurar las preferencias de tareas y problemas desbloqueados.
1. En la página que se muestra para el grupo, en el panel izquierdo, haga clic en **Preferencias de tarea y problema**.
1. En la página que aparece, continúe con una de las 5 secciones que se enumeran a continuación para configurar las opciones de las áreas Valores predeterminados de nueva tarea, Problemas, Eliminación, Fechas reales y Acceso, y luego haga clic en **Guardar**.

   Si pasa el ratón sobre el icono de candado ![](assets/lock-toggle-button-dimmed.png) para ver una preferencia que debe configurar y aparece información del objeto que le indica que está bloqueado, puede pedirle al administrador de Workfront que lo desbloquee para todos los grupos de la organización.

   Cuando está desbloqueado, usted y otros administradores del grupo pueden configurarlo por separado para sus propios grupos. Además, puede bloquearlo para su grupo y para cualquier subgrupo debajo de su grupo.

   * [Valores predeterminados de nueva tarea](#new-task-defaults)
   * [Problemas](#issues)
   * [Eliminación](#deletion)
   * [Fechas reales](#actual-dates)

     <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [Acceso](#access)

### Valores predeterminados de nueva tarea {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fecha de inicio en tareas nuevas</td> 
      <td> <p>Determina la fecha de comienzo predeterminada de las nuevas tareas para los jefes de proyecto. La fecha de inicio de las nuevas tareas puede ser la fecha de inicio planeada del proyecto o el día en que se crea la tarea.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tipo de duración </p> </td> 
      <td> <p>Determina la relación entre el número de recursos (y su porcentaje de asignación) y la duración o el esfuerzo total de la tarea. Para obtener más información, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Duración de la tarea y Tipos de duración: índice del artículo</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de ingresos</td> 
      <td> <p>Calcula las estimaciones de ingresos planificadas y reales de una tarea. Cuando el <strong>Tipo de ingresos</strong> se establece en<strong>No facturable</strong>, las horas planificadas y las horas registradas no generan una estimación de ingresos para la tarea y el trabajo en la tarea no contribuye a los ingresos en el nivel de proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de costo</td> 
      <td> <p>Calcula las estimaciones de costos planificadas y reales de una tarea. Cuando se establece en <strong>Sin costo</strong>, las horas planificadas y las horas registradas no generan una estimación de costo planificada o real para la tarea, y el trabajo en la tarea no contribuye a los costos de nivel de proyecto.</p> </td> 
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
      <td> <p>Cuando alguien convierte un problema en un proyecto o tarea, tanto el problema original como el proyecto o tarea convertidos se convierten en objetos de resolución. Esta configuración le permite correlacionar la resolución del problema original con la resolución de su objeto solucionable. Para obtener más información sobre la resolución de objetos, vea <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y los objetos solucionables </a>.</p> <p>Para que esta configuración surta efecto, debe estar seleccionada la opción de <strong>Mantener el problema original y enlazar su solución a la tarea</strong>.</p> 
       <ul> 
        <li>Cuando esta configuración está habilitada, puede crear estados personalizados con la misma clave para problemas y proyectos o tareas. Cuando el proyecto o la tarea (como objeto solucionable) se convierte en el estado personalizado, el cambio también se refleja en el estado del problema. La clave de estado debe ser la misma para los estados de problema y proyecto o tarea.</li> 
        <li>Cuando esta configuración está desactivada, los estados de objetos de resolución se establecen automáticamente en el estado predeterminado en lugar de en los personalizados. Para obtener más información acerca de los estados predeterminados, vea <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acceso a la lista de estados de problemas del sistema</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando se convierte un problema en una tarea</td> 
      <td> <p>La configuración de esta sección determina qué sucede durante el proceso de conversión de un problema a una tarea:</p> 
       <ul> 
        <li><strong>Conservar el problema original y enlazar su solución a la tarea</strong>: Cuando esté convirtiendo el problema, permanecerá visible como un problema hasta que se complete la tarea. El estado del problema cambia automáticamente a Cerrado cuando se completa la tarea.</li> 
        <li><strong>Permitir que el contacto principal tenga acceso a la tarea</strong>: otorga al contacto principal (creador del problema) acceso a la tarea para revisar la tarea, realizar actualizaciones y mantenerse informado de su progreso</li> 
        <li> <p><strong>Permitir cambiar esta configuración durante la conversión</strong>: permite al usuario que está convirtiendo el problema cambiar estas opciones durante la conversión de un problema en una tarea.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando se convierte un problema en un proyecto</td> 
      <td> <p>La configuración de esta sección determina qué sucede durante el proceso de conversión de un problema a un proyecto:</p> 
       <ul> 
        <li><strong>Conservar el problema original y enlazar su solución al proyecto</strong>: Cuando esté convirtiendo el problema, permanecerá visible como un problema hasta que se complete el proyecto. El estado del problema cambia automáticamente a Cerrado cuando se completa el proyecto.</li> 
        <li><strong>Permitir que el contacto principal tenga acceso al proyecto</strong>: otorga al contacto principal (creador del problema) acceso al proyecto para revisar el proyecto, realizar actualizaciones y mantenerse informado de su progreso.</li> 
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
      <td role="rowheader">Permitir que los usuarios eliminen tareas y problemas con las horas registradas</td> 
      <td> <p> Permite determinar si se permite eliminar tareas o problemas en los que se registran horas. Esta opción está seleccionada de forma predeterminada.</p> 
       <div> 
        <p><b>Sugerencia</b>: Esta configuración también se aplica a la eliminación de proyectos que tienen tareas o problemas con horas registradas en ellos. Esta configuración no se aplica a los proyectos de eliminación en los que el tiempo se registra directamente en el proyecto. </p> 
        <p>Tenga en cuenta lo siguiente:</p> 
        <ul> 
         <li> <p>Cuando se selecciona, recibe una advertencia informativa cuando elimina una tarea o un problema. La advertencia le recuerda que si la tarea o el problema han registrado horas, se moverán al proyecto o se eliminarán. Puede configurar si las horas se eliminan o se mueven al proyecto en la sección Hoja de horas y preferencias de horas de Configuración. Después de confirmar que ha visto la advertencia, la tarea o el problema se eliminan. Para obtener más información sobre cómo configurar las preferencias de horas y hojas de horas, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurar las preferencias de horas y hojas de horas</a>. </p> <p>Sugerencia: <span>Cuando elimina un proyecto con tareas y problemas que han registrado horas, estas se eliminan o se conservan de acuerdo con la configuración del área de Preferencias de horas y hojas de horas de Configuración</span>. </p> </li> 
         <li><span>Cuando anula la selección de esta opción, recibe una advertencia prohibitiva cuando elimina una tarea o un problema con horas registradas, o cuando elimina un proyecto con horas registradas para sus tareas o problemas</span> <span>.</span> La advertencia especifica que el administrador no permite que se eliminen tareas o problemas con horas registradas. No se pueden eliminar las tareas, problemas<span> o proyectos que tienen horas registradas para tareas y problemas</span>. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### Fechas reales {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Cuando una tarea o un problema pasen de "Nuevo" a "En curso", establecer la Fecha de inicio real en</td> 
      <td> <p>Seleccione una de las siguientes opciones para indicar cuándo se registra la fecha de inicio real en Workfront cuando una tarea o un problema pasa de <strong>Nuevo</strong> a <strong>En curso</strong>:</p> 
       <ul> 
        <li><strong>Ahora:</strong> La fecha real de inicio está establecida en la fecha actual.</li> 
        <li><strong>Fecha planificada de inicio:</strong> La fecha real de inicio se establece en la fecha planificada de inicio de la tarea o problema.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Una vez que se complete una tarea o un problema, establecer la Fecha real de finalización en</td> 
      <td> <p>Seleccione una de las siguientes opciones para cuándo se registra la fecha real de finalización en Workfront cuando se completa una tarea o un problema:</p> 
       <ul> 
        <li><strong>Ahora:</strong> La fecha real de finalización está establecida en la fecha actual.</li> 
        <li> <p><strong>Fecha planificada de finalización:</strong> la fecha real de finalización está establecida en la fecha planificada de finalización de la tarea o problema.</p> </li> 
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

### Acceso {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Cada vez que se asigne a una persona a una tarea</td> 
      <td> 
       <ul> 
        <li><strong>Concederles... acceso a una tarea</strong>: Define el permiso predeterminado que un usuario tiene para la tarea a la que está asignado. Para obtener más información acerca de los permisos de tareas, vea<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Conceder acceso a los usuarios</a>.</li> 
        <li> <p><strong>Concederles también... acceso al proyecto</strong>: Define el permiso predeterminado que un usuario tiene para acceder al proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cada vez que se asigne a una persona a un problema</td> 
      <td> 
       <ul> 
        <li><strong>Concederles... acceso a una tarea</strong>: Define el permiso predeterminado que un usuario tiene para la tarea a la que está asignado. Para obtener más información acerca de los permisos de tareas, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</li> 
        <li> <p><strong>Concederles también... acceso al proyecto</strong>: Define el permiso predeterminado que un usuario tiene para acceder al proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando alguien envía una solicitud</td> 
      <td> 
       <ul> 
        <li><strong>Concederles... acceso al problema</strong>: Define el permiso predeterminado que tiene un usuario sobre una solicitud que ha enviado. Para obtener más información, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema</a>.</li> 
        <li> <p><strong>Las personas de la misma compañía heredarán los mismos permisos para todas las solicitudes</strong>: permite a los usuarios ver las solicitudes enviadas por otros usuarios de la misma compañía que ellos. Tienen los mismos permisos en esas solicitudes que en sus propias solicitudes enviadas.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
