---
title: Configuración de las preferencias de tarea y problema para un grupo
user-type: administrator
product-area: system-administration;user-management;setup
keywords: grupo,preferencias,tarea,problema,desbloquear
navigation-topic: create-and-manage-groups
description: Si los grupos de su organización necesitan configurar una tarea o una preferencia de problema independientemente de la forma en que esté configurada en el sistema, un administrador de Adobe Workfront puede desbloquear la preferencia. A continuación, como administrador de grupos, puede configurar la preferencia del grupo y esto afectará a todas las tareas o problemas asociados con él.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 3%

---

# Configuración de las preferencias de tarea y problema para un grupo

Si los grupos de su organización necesitan configurar una tarea o una preferencia de problema independientemente de la forma en que esté configurada en el sistema, un administrador de Adobe Workfront puede desbloquear la preferencia. A continuación, como administrador de grupos, puede configurar la preferencia del grupo y esto afectará a todas las tareas o problemas asociados con él.

Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Para obtener información sobre cómo el administrador de Workfront desbloquea las preferencias, consulte [Bloquear o desbloquear las preferencias del proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>La configuración a nivel de grupo también es posible para las preferencias del proyecto. Para obtener más información, consulte [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* Normalmente, una preferencia desbloqueada permanece desbloqueada indefinidamente. Si el administrador de Workfront lo vuelve a bloquear, la configuración del sistema se aplica de nuevo y se pierde la configuración de las preferencias de los administradores del grupo.
>* Las preferencias establecidas para el grupo asociado a un proyecto tienen prioridad sobre las preferencias establecidas para el grupo principal del usuario que crea el proyecto.
>* Algunas preferencias de nivel de grupo afectan a las plantillas de proyecto que cree para el grupo. Para obtener más información, consulte la sección [Ver, trabajar con y crear plantillas para su grupo desde el área Grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) en el artículo [Creación y modificación de las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Una vez que un administrador de Workfront desbloquea una preferencia a nivel de sistema, puede configurarla y luego bloquearla para asegurarse de que todos los miembros del grupo y de sus subgrupos usen la misma configuración. Esto es paralelo a la capacidad que tiene un administrador de Workfront para configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, consulte [Bloquear o desbloquear un proyecto, tarea o preferencia de problemas para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o administrador de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Configurar las preferencias de problemas y tareas desbloqueadas para un grupo de nivel superior

>[!TIP]
>
>Si es administrador de Workfront, puede omitir los pasos del 1 al 4 accediendo a Configuración > Preferencias del proyecto > Tareas y problemas, y luego buscando el nombre del grupo en el cuadro de la parte superior de la página.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo para el que desea configurar las preferencias de problemas y tareas desbloqueadas.
1. En la página que aparece para el grupo, en el panel izquierdo, haga clic en **Preferencias de tareas y problemas**.
1. En la página que aparece, continúe con una de las 5 secciones enumeradas debajo de estos pasos para configurar las áreas Nuevos valores predeterminados de tarea, Problemas, Eliminación, Fechas reales y Acceso, y luego haga clic en **Guardar**.

   Si pasa el ratón por encima del icono de bloqueo ![](assets/lock-toggle-button-dimmed.png) para obtener una preferencia que debe configurar y se muestra información del objeto que le indica que está bloqueado, puede solicitar al administrador de Workfront que la desbloquee para todos los grupos de la organización.

   Cuando está desbloqueado, usted y los demás administradores del grupo pueden configurarlo por separado para sus propios grupos. Además, puede bloquearlo para su grupo y para cualquier subgrupo debajo de su grupo.

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
      <td role="rowheader">Fecha de inicio en nuevas tareas</td> 
      <td> <p>Determina la fecha de inicio predeterminada para las nuevas tareas de los jefes de proyecto. La fecha de inicio de las nuevas tareas puede ser la fecha de inicio planificada del proyecto o el día en el que se crea la tarea.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tipo de duración </p> </td> 
      <td> <p>Determina la relación entre el número de recursos (y su porcentaje de asignación) y la duración o el esfuerzo total de la tarea. Para obtener más información, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Duración de tarea y tipos de duración</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de ingresos</td> 
      <td> <p>Calcula las estimaciones de ingresos reales y planeados para una tarea. Cuando la variable <strong>Tipo de ingresos</strong> está configurado como<strong>No facturable</strong>, las horas planificadas y las horas reales registradas no generan una estimación de ingresos para la tarea y el trabajo en la tarea no contribuye a los ingresos a nivel de proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de costo</td> 
      <td> <p>Calcula las estimaciones de costes reales y planeadas de una tarea. Cuando se configura como <strong>Sin costo</strong>, las horas planificadas y las horas reales registradas no generan una estimación de coste planificada o real para la tarea y el trabajo en la tarea no contribuye a los costes a nivel de proyecto.</p> </td> 
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
      <td> <p>Cuando alguien convierte un problema en un proyecto o tarea, tanto el problema original como el proyecto o tarea convertido se convierten en objetos de resolución. Esta configuración le permite correlacionar la resolución del problema original con la resolución de su objeto resoluble. Para obtener más información sobre la resolución de objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y resolución de objetos </a>.</p> <p>Para que esta configuración tenga algún efecto, la opción <strong>Mantenga el problema original y vincule su resolución a la tarea</strong> debe estar seleccionado.</p> 
       <ul> 
        <li>Cuando esta configuración está habilitada, puede crear estados personalizados con la misma clave tanto para problemas como para proyectos o tareas. Cuando el proyecto o la tarea (como objeto resoluble) se convierte en un estado personalizado, el cambio también refleja el estado del problema. La clave de estado debe ser la misma para el problema y los estados de proyecto o tarea.</li> 
        <li>Cuando se deshabilita esta configuración, la resolución de estados de objeto se establece automáticamente en el estado predeterminado, no en los personalizados. Para obtener más información sobre los estados predeterminados, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acceda a la lista de estados de problemas del sistema</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Al convertir un problema en una tarea</td> 
      <td> <p>La configuración de esta sección determina lo que sucede durante el proceso de conversión de un problema a otro:</p> 
       <ul> 
        <li><strong>Mantenga el problema original y vincule su resolución a la tarea</strong>: Cuando se convierte el problema, permanece visible como un problema hasta que se complete la tarea. El estado del problema cambia automáticamente a Cerrado cuando se completa la tarea.</li> 
        <li><strong>Permitir que el contacto principal tenga acceso a la tarea</strong>: Proporciona al contacto principal (creador del problema) acceso a la tarea para revisar la tarea, realizar actualizaciones y mantenerse informado de su progreso</li> 
        <li> <p><strong>Permitir que esta configuración cambie durante la conversión</strong>: Permite al usuario que está convirtiendo el problema cambiar estas opciones durante la conversión de un problema en una tarea.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Al convertir un problema en un proyecto</td> 
      <td> <p>La configuración de esta sección determina lo que sucede durante el proceso de conversión de un problema a otro:</p> 
       <ul> 
        <li><strong>Mantener el problema original y enlazar su resolución con el proyecto</strong>: Cuando esté convirtiendo el problema, permanecerá visible como un problema hasta que se complete el proyecto. El estado del problema cambia automáticamente a Cerrado cuando el proyecto se completa.</li> 
        <li><strong>Permitir que el contacto principal tenga acceso al proyecto</strong>: Proporciona al contacto principal (creador del problema) acceso al proyecto para revisar el proyecto, realizar actualizaciones y mantenerse informado de su progreso.</li> 
        <li><strong>Permitir que esta configuración cambie durante la conversión</strong>: Permite al usuario que está convirtiendo el problema cambiar las opciones enumeradas durante la conversión de un problema en un proyecto.</li> 
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
      <td> <p> Permite determinar si se permite la eliminación de tareas o problemas en los que se registran horas. Esta opción está seleccionada de forma predeterminada.</p> 
       <div> 
        <p><b>Sugerencia</b>: Esta configuración también se aplica a la eliminación de proyectos que tengan tareas o problemas con horas registradas en ellos. Esta configuración no se aplica a la eliminación de proyectos en los que el tiempo se registra directamente para el proyecto. </p> 
        <p>Tenga en cuenta lo siguiente:</p> 
        <ul> 
         <li> <p>Cuando se selecciona, recibe una advertencia informativa al eliminar una tarea o problema. La advertencia le recuerda que si la tarea o el problema ha registrado horas, se moverán al proyecto o se eliminarán. Puede configurar si las horas se eliminan o se mueven al proyecto en el área Preferencias de horario y horario del programa de instalación. Después de confirmar que ha visto la advertencia, se elimina la tarea o el problema. Para obtener más información sobre la configuración de las preferencias de horario y horario, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configuración de las preferencias de horas y horas</a>. </p> <p>Sugerencia: <span>Cuando elimina un proyecto con tareas y problemas que tienen horas registradas, las horas registradas se eliminan o se conservan según la configuración del área Preferencias de horario y horario de la configuración</span>. </p> </li> 
         <li><span>Cuando anula la selección de esta opción, recibe una advertencia prohibitiva cuando elimina una tarea o problema con horas registradas, o cuando elimina un proyecto con horas registradas para sus tareas o problemas</span> <span>.</span> La advertencia especifica que el administrador no permite que se eliminen tareas o problemas con horas registradas. Tareas, problemas<span>o proyectos que tengan horas registradas para tareas y problemas</span> no se puede eliminar. </li> 
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
      <td role="rowheader">Cuando una tarea o problema pasa de "Nuevo" a "En curso", establezca la Fecha de inicio real en</td> 
      <td> <p>Seleccione una de las siguientes opciones para cuándo se registra la fecha de inicio real en Workfront cuando una tarea o problema proviene de <strong>Nuevo</strong> a <strong>En curso</strong>:</p> 
       <ul> 
        <li><strong>Ahora:</strong> La fecha de inicio real se establece en la fecha actual.</li> 
        <li><strong>La fecha de inicio planeada:</strong> La fecha de inicio real se establece en la fecha de inicio planeada de la tarea o el problema.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando se finalice una tarea o un problema, establecer la fecha de finalización real en</td> 
      <td> <p>Seleccione una de las siguientes opciones para cuándo se registra la fecha de finalización real en Workfront cuando se completa una tarea o problema:</p> 
       <ul> 
        <li><strong>Ahora:</strong> La fecha de finalización real se establece en la fecha actual.</li> 
        <li> <p><strong>La fecha de finalización prevista:</strong> La Fecha de Finalización Real se establece en la Fecha de Finalización Planificada de la tarea o la emisión.</p> </li> 
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
      <td role="rowheader">Cuando alguien está asignado a una tarea</td> 
      <td> 
       <ul> 
        <li><strong>Darles acceso ... a una tarea</strong>: Define el permiso predeterminado que un usuario tiene para la tarea a la que está asignado. Para obtener más información sobre los permisos de tareas, consulte<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Conceder acceso a los usuarios</a>.</li> 
        <li> <p><strong>También otorgarles ... acceso al proyecto</strong>: Define el permiso predeterminado que un usuario tiene para el proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando alguien está asignado a un problema</td> 
      <td> 
       <ul> 
        <li><strong>Darles acceso ... a una tarea</strong>: Define el permiso predeterminado que un usuario tiene para la tarea a la que está asignado. Para obtener más información sobre los permisos de tareas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</li> 
        <li> <p><strong>También otorgarles ... acceso al proyecto</strong>: Define el permiso predeterminado que un usuario tiene para el proyecto en el que tiene una tarea asignada. Para obtener más información sobre los permisos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cuando alguien envía una solicitud</td> 
      <td> 
       <ul> 
        <li><strong>Dales acceso ... al problema</strong>: Define el permiso predeterminado que tiene un usuario en una solicitud que envió. Para obtener más información, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema</a>.</li> 
        <li> <p><strong>Los usuarios de la misma empresa heredarán los mismos permisos para todas las solicitudes</strong>: Permite a los usuarios ver las solicitudes enviadas por otros usuarios desde la misma empresa que ellos. Tienen los mismos permisos en esas solicitudes que tienen en sus propias solicitudes enviadas.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
