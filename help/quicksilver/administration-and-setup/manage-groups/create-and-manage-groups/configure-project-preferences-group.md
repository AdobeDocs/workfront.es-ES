---
title: Configuración de las preferencias de un proyecto para un grupo
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Si es un administrador de grupos y un administrador de Adobe Workfront desbloquea una preferencia de proyecto para todos los grupos del sistema, puede configurar esa preferencia para que su grupo afecte a todos los proyectos subsiguientes que cree su grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '2643'
ht-degree: 3%

---

# Configuración de las preferencias de un proyecto para un grupo

Si es un administrador de grupos y un administrador de Adobe Workfront desbloquea una preferencia de proyecto para todos los grupos del sistema, puede configurar esa preferencia para que su grupo afecte a todos los proyectos subsiguientes que cree su grupo.

Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>* Normalmente, una preferencia desbloqueada permanece desbloqueada indefinidamente. Si el administrador de Workfront lo vuelve a bloquear, la configuración del sistema se aplica de nuevo y se pierde la configuración de las preferencias de los administradores del grupo.
>* Las preferencias establecidas para el grupo asociado a un proyecto tienen prioridad sobre las preferencias establecidas para el grupo principal del usuario que crea el proyecto.
>* Algunas preferencias de nivel de grupo afectan a las plantillas de proyecto que cree para el grupo. Para obtener más información, consulte la sección [Ver, trabajar con y crear plantillas para su grupo desde el área Grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) en el artículo [Creación y modificación de las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Una vez que un administrador de Workfront desbloquea una preferencia a nivel de sistema, puede configurarla y luego bloquearla para asegurarse de que todos los miembros del grupo y de sus subgrupos usen la misma configuración. Esto es paralelo a la capacidad que tiene un administrador de Workfront para configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, consulte [Bloquear o desbloquear un proyecto, tarea o preferencia de problemas para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


La configuración a nivel de grupo también es posible para las preferencias de tareas y problemas, así como para las preferencias de parte de horas y hora. Para obtener más información, consulte [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) y [Configuración de las preferencias de horas y horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Para obtener información sobre cómo un administrador de Workfront desbloquea una preferencia de proyecto, consulte [Bloquear o desbloquear las preferencias del proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

## Configurar una preferencia de proyecto desbloqueado para un grupo

>[!TIP]
>
>Si es administrador de Workfront, puede omitir los pasos del 1 al 4 accediendo a Configuración > Preferencias de proyecto > Proyectos y luego buscando el nombre del grupo en el cuadro de la parte superior de la página.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo cuyas preferencias de proyecto desee configurar.
1. En el panel izquierdo, haga clic en **Preferencias de proyecto**.
1. En la página que aparece, continúe con una de las 4 secciones enumeradas a continuación para configurar las preferencias de Estado del proyecto, Líneas de tiempo, Casos de negocio y Vida después de la muerte.

   >[!TIP]
   >
   >Si pasa el ratón sobre una preferencia y aparece un aviso para decirle que está bloqueado, puede solicitar al administrador de Workfront que la desbloquee para todos los grupos de la organización.

* [Estado del proyecto](#project-status)
* [Escalas de tiempo](#timelines)
* [Casos comerciales](#business-cases)
* [Vida después de la muerte](#life-after-death)

### Estado del proyecto {#project-status}

Configure cualquiera de las siguientes preferencias para los proyectos recién creados asociados al grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Permitir a los usuarios crear proyectos sin usar una plantilla</td>
<td><p>Esta preferencia permite a los usuarios crear proyectos sin usar una plantilla al crear un proyecto desde las siguientes áreas:</p>
<ul>
<li><p>Utilizar la opción Nuevo proyecto en una lista de proyectos</p></li>

<li><p>Convertir un problema en un proyecto desde la página del problema</p></li>
</ul>

<p>Esta preferencia está habilitada de forma predeterminada en el nivel del sistema.</p>
<p><b>NOTA</b></p>
<p>Cuando un usuario pertenece a varios grupos con preferencias diferentes, se le permitirá crear un proyecto sin plantilla si al menos uno de sus grupos tiene habilitada esta preferencia.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Establecer estado de nuevo proyecto en</td> 
   <td> <p>Determine el estado de los nuevos proyectos.</p> <p><b>NOTA</b>   
     <ul> 
      <li>Si usted u otro administrador de Workfront oculta el estado seleccionado aquí, el estado predeterminado cambia al primer estado de la lista de estado.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Para las preferencias de proyecto de grupo, solo se puede seleccionar un estado bloqueado o un estado requerido como estado predeterminado.</li> 
      <li> <p>Si un sistema bloqueado o un estado de grupo se establece como estado predeterminado y más tarde alguien lo desbloquea, el sistema intenta reemplazarlo por un estado bloqueado del mismo tipo de estado.</p> <p>Si no encuentra una, busca un estado obligatorio:</p> 
       <ul> 
        <li>Si hay un estado requerido que equivale al estado predeterminado desbloqueado, el estado requerido se convierte en el estado predeterminado, aunque esté desbloqueado.</li> 
        <li>Si ninguno de los estados requeridos equivale al estado predeterminado desbloqueado, el primer estado requerido en la lista de estado se convierte en el estado predeterminado.</li> 
       </ul> <p>Para obtener información sobre los estados necesarios, consulte los artículos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de proyectos del sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de tareas del sistema</a>y <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceda a la lista de estados de problemas del sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calcular porcentaje completado en función de</td> 
   <td> <p>El porcentaje completado de un proyecto o tarea principal se basa en el progreso general de las tareas. Esta información se puede calcular en función de la duración o del horario planificado de las tareas de un proyecto.</p> <p>Si selecciona Duración, la Duración de cada tarea de un proyecto determina el porcentaje total completado del proyecto y la Duración de cada subtarea determina el porcentaje total completado de la tarea principal.</p> <p>Si selecciona Duración, asegúrese de especificar las horas típicas por día laboral y los días laborables típicos por semana en la sección Líneas de tiempo . Workfront utiliza esta información para calcular el porcentaje completado de una tarea en función de la duración. </p> <p>Si selecciona Horario planificado, asegúrese de que todas las tareas de cada proyecto tengan definida la cantidad de horas planificadas y de que la cantidad no sea cero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Establecer automáticamente Condición de proyecto según el estado de Progreso</td> 
   <td> <p>Esta preferencia permite a los usuarios establecer la condición de un proyecto manualmente (en Target, en riesgo, en problemas) o hacer que Workfront establezca la condición (estado de progreso) automáticamente en función de la progresión del proyecto en la cronología. Para obtener más información sobre la condición de los proyectos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Descripción general de la condición y el tipo de condición del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Crear automáticamente líneas base</p> </td> 
   <td> <p>Esta preferencia crea automáticamente una línea de base (instantánea) de los detalles de la tarea y el proyecto cuando el estado del proyecto cambia a Actual. Para obtener información sobre la creación de líneas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Crear líneas de base del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Método de índice de rendimiento </p> </td> 
   <td> <p>El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Workfront para calcular las métricas de valor obtenido, como Índice de rendimiento de costes (CPI) y Estimación al finalizar (EAC). Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular el índice de rendimiento de costes (CPI)</a>y <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular estimación al finalizar (CAO)</a></p> 
    <ul> 
     <li><strong>Basado en horas</strong>: Workfront utiliza Horario planificado para calcular métricas de rendimiento como EAC y CPI. Cuando el PIM se calcula en función de las horas, el EAC se muestra como un número de horas. Asegúrese de que tiene un valor para Horario planificado, distinto de cero.</li> 
     <li> <p><strong>Basado en los costes</strong>: Workfront utiliza Costo laboral planificado para calcular métricas de rendimiento como EAC y CPI. Asegúrese de que las funciones de su trabajo o los usuarios estén asociados con las tasas de costo por hora. Cuando el PIM se calcula en función de los costes, el EAC se muestra como un valor de moneda.</p> <p>El administrador de proyectos puede modificar esta configuración a nivel de proyecto mediante el área Finanzas de Detalles del proyecto . Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área de finanzas del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Estimar al finalizar </p> </td> 
   <td> <p>Determine qué datos utiliza Workfront para calcular la estimación al finalizar (EAC) que representa el coste total proyectado de un proyecto.</p> 
    <ul> 
     <li><strong>Calcular en el nivel de proyecto</strong>:EAC para la tarea principal y el proyecto se determina introduciendo horas reales o costo laboral real en las fórmulas de EAC. Este cálculo incluye horas reales o costes y gastos añadidos directamente a la tarea o proyecto principal.</li> 
     <li> <p><strong>Resumen de tareas/subtareas</strong>: Las CAO para la tarea principal y el proyecto se determinan sumando la CAO para cada tarea secundaria. Este cálculo excluye las horas reales o los costes y gastos reales añadidos directamente a la tarea o proyecto principal.</p> <p>El administrador de proyectos puede modificar esta configuración a nivel de proyecto mediante el área Finanzas de Detalles del proyecto . Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área de finanzas del proyecto</a>.</p> </li> 
    </ul> <p>Para obtener más información sobre cómo se calcula la CAO, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular estimación al finalizar (CAO)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Escalas de tiempo {#timelines}

Configure cualquiera de las siguientes preferencias para los proyectos recién creados asociados al grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Programar desde</td> 
   <td> <p>Determine si los nuevos proyectos están programados desde la fecha de inicio o desde la fecha de finalización cuando se crean.</p> 
    <ul> 
     <li><strong>Fecha de inicio</strong>: Las nuevas tareas se configuran de forma predeterminada como Restricción de tareas lo antes posible y se solicita a los administradores de proyectos que proporcionen una Fecha de inicio planificada para el proyecto.</li> 
     <li><strong>Fecha de finalización</strong>: Las nuevas tareas se configuran de forma predeterminada como lo más tarde posible Restricción de tareas y se solicita a los administradores de proyectos que proporcionen una Fecha de finalización planificada para el proyecto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tiempo libre del usuario</td> 
   <td> <p>Determine si el tiempo de espera del Asignado principal de una tarea ajusta las fechas planificadas para esa tarea en un proyecto.</p> 
    <ul> 
     <li> <p><strong>Considere el tiempo de espera del usuario en las duraciones de las tareas</strong>: Cualquier tiempo libre programado para el Asignado Principal de una tarea ajusta las fechas planificadas de la tarea si el tiempo de espera se produce durante la duración de la tarea. Esta es la configuración predeterminada. </p> <p>Por ejemplo, si una tarea con una Restricción de Tan pronto como sea posible está programada para empezar el 1 de junio y finalizarse el 3 de junio, y el usuario asignado principal tiene la Marca de tiempo de espera del 2 de junio, las fechas programadas para la tarea se ajustan al 1 al 4 de junio.</p> <p><b>IMPORTANTE</b>: La duración de la tarea no cambia al seleccionar esta configuración. Solo cambian las fechas planificadas, dependiendo de la restricción de tareas.</p> </li> 
     <li><strong>Ignorar el tiempo de espera del usuario en duraciones de tareas</strong>: Las fechas previstas de cada tarea en un proyecto permanecen como estaba planeado originalmente, incluso si el Asignado Principal de una tarea tiene tiempo libre durante su duración.</li> 
    </ul> <p>Tenga en cuenta lo siguiente al seleccionar opciones para esta configuración:</p> 
    <ul> 
     <li>Cuando cambia esta configuración, solo los proyectos y las plantillas creados después del cambio heredan la configuración actualizada. </li> 
     <li> <p>El valor Restricción de tareas de la tarea determina qué fechas de tareas planificadas se deben ajustar: </p> 
      <ul> 
       <li>Fecha planificada de inicio</li> 
       <li>Fecha planificada de finalización</li> 
       <li>Ambas fechas</li> 
       <li>Ninguna fecha. </li> 
      </ul> <p>Por ejemplo, si una tarea tiene una Restricción de Fechas Fijas, las fechas no se ajustan cuando el Destinatario Principal tiene tiempo libre, aunque la opción Tenga en cuenta el tiempo de espera del usuario en la duración de la tarea esté seleccionada. Para obtener información sobre las restricciones de tareas, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Información general sobre la restricción de tareas</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Las escalas de tiempo de este proyecto se volverán a calcular automáticamente</strong> </p> </td> 
   <td> <p>Determine cuándo se vuelve a calcular la escala de tiempo de un proyecto. Para obtener información sobre cómo volver a calcular la cronología del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Volver a calcular las líneas de tiempo del proyecto</a>.</p> <p>Las siguientes opciones están habilitadas de forma predeterminada. Puede seleccionar una o varias de las siguientes opciones:</p> 
    <ul> 
     <li> <p><strong>Cada noche</strong>: Seleccione esta opción para volver a calcular las líneas de tiempo del proyecto cada noche. Los cambios que realice en el proyecto que puedan afectar a la cronología no serán visibles inmediatamente. Workfront ​ ​ ​ vuelve a calcular las líneas de tiempo por la noche solo para los proyectos en los que se cumplen las dos condiciones siguientes:</p> <p> 
       <ul> 
        <li>Tener un estado de Actual</li> 
        <li>Han tenido una actualización en los últimos 3 meses</li> 
       </ul> </p> </li> 
     <li> <p><strong>Cuando cambia el ámbito de un proyecto</strong>: Seleccione esta opción para volver a calcular las líneas de tiempo del proyecto inmediatamente cuando se produzca un cambio en el ámbito del proyecto. Para obtener información sobre lo que constituye un cambio en el ámbito de un proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Volver a calcular las líneas de tiempo del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Cuando se asignen varios usuarios a una tarea, utilice la programación de la</strong> </p> </td> 
   <td> <p>Si un proyecto no tiene una programación asignada o si los usuarios asignados a sus tareas no tienen una programación asignada, Workfront utiliza la programación predeterminada del sistema para calcular la cronología de las tareas.</p> <p>Si asigna varios usuarios a la misma tarea en un proyecto tiene una programación asignada (y los usuarios asignados a las tareas también tienen una programación asignada), Workfront utiliza las siguientes programaciones:</p> 
    <ul> 
     <li><strong>Asignación principal</strong>: Workfront utiliza la programación de la Asignación principal en la tarea para calcular las líneas de tiempo.</li> 
     <li><strong>Proyecto</strong>: Workfront utiliza la programación del proyecto para calcular la cronología de cada tarea.</li> 
    </ul> <p>Para obtener más información sobre las programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Crear una programación</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Cálculos de escala de tiempo </p> </td> 
   <td> 
    <ul> 
     <li><strong>Horas habituales por día laborable</strong>: Establezca el número de horas en una jornada laboral normal para los usuarios que están trabajando en proyectos. El valor predeterminado es de 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>Días laborables típicos por semana</strong>: Establezca la semana laboral estándar para los usuarios que trabajarán en proyectos. El valor predeterminado es de 5 días.</li> 
    </ul> <p>Estas dos opciones convierten días en horas o semanas en días.</p> <p>Por ejemplo, si tiene una tarea con 8 horas planificadas y la duración se calcula en función de las horas planificadas, Workfront convierte esas horas en días para mostrar la duración como días.</p> <p>Desde el campo Días de trabajo típicos por semana, Workfront calcula el valor Equivalente de tiempo completo (FTE) para su sistema. Esto es lo que utiliza Workfront al calcular asignaciones para usuarios.</p> <p>Estos valores se utilizan cuando se planifica la cronología de los proyectos, se presupuestan los recursos o se registra el tiempo de los proyectos. </p> <p>No se utilizan cuando se establecen partes de horas para los usuarios del sistema, tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configuración de las preferencias de horas y horas</a>.</p> <p><b>NOTA</b>: Los administradores de Workfront no pueden desbloquear las preferencias de cálculos de línea de tiempo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Trimestres personalizados</strong> </p> </td> 
   <td> <p>Configure trimestres anuales personalizados para los usuarios que trabajarán en proyectos. Los trimestres personalizados suelen ser trimestres que no coinciden con el desglose tradicional de trimestres durante un año natural. Puede agregar varios trimestres personalizados. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados para proyectos</a>.</p> <p><b>NOTA</b>: Los administradores de Workfront no pueden desbloquear las preferencias de trimestres personalizados.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Casos comerciales {#business-cases}

Puede crear un caso empresarial para los proyectos recién creados asociados con el grupo para enviar solicitudes de proyecto. Puede definir preferencias para determinar qué áreas son visibles en la variable **Caso empresarial** formulario. Le recomendamos que habilite estas opciones para que otras herramientas, como el Optimizador de Portfolio, se actualicen correctamente. Para obtener más información sobre qué muestra cada campo, consulte [Definir un caso empresarial](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Una vez que el administrador de Workfront habilita las secciones en el caso empresarial, el propietario de un proyecto puede crear un caso empresarial a nivel de proyecto. Para obtener información sobre cómo crear un caso práctico, consulte [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Vida después de la muerte  {#life-after-death}

Configure cualquiera de las siguientes preferencias para los proyectos recién creados asociados al grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Una vez que un proyecto se ha marcado como Completo, las personas aún pueden</strong> </p> </td> 
   <td> <p>Determine las reglas para su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a si una tarea o un problema se pueden eliminar después de marcar el estado del proyecto como Completado.</p> 
    <ul> 
     <li><strong>Eliminar tareas</strong>: Permite a los usuarios eliminar tareas de un proyecto una vez que el proyecto se ha marcado como Completado.<br></li> 
     <li><strong>Eliminar problemas</strong>: Permite a los usuarios eliminar problemas de un proyecto una vez que el proyecto se ha marcado como Completado.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Una vez marcado un proyecto como Completado, Finalizado o Pendiente de Aprobación, las personas podrán seguir utilizándolo</strong> </p> </td> 
   <td> <p>Determine las reglas para la organización (o el grupo, si configura las preferencias de proyecto para un grupo) con respecto a lo que sucede con las tareas, los problemas, los documentos y otros objetos de un proyecto una vez que se ha marcado el estado del proyecto <strong>Completar</strong>, <strong>Muerto</strong>o es <strong>Pendiente de aprobación</strong>.</p> 
    <ul> 
     <li><strong>Agregar y editar tareas</strong> Permite a los usuarios: 
      <ul> 
       <li>Edite tareas dentro de un proyecto después de que el proyecto se haya marcado como Completado, Finalizado o Pendiente de aprobación. Esto incluye agregar horas y cambiar entradas de gastos en una tarea.</li> 
       <li>Agregue tareas a un proyecto.</li> 
      </ul></li> 
     <li><strong>Adición y edición de problemas</strong>: Permite a los usuarios: 
      <ul> 
       <li>Edite los problemas dentro de un proyecto después de que el proyecto se haya marcado como Completado, Finalizado o Pendiente de aprobación.</li> 
       <li>Agregue problemas a un proyecto después de que el proyecto esté marcado como Completado o Muerto. (No se pueden agregar problemas a un proyecto que esté pendiente de aprobación).</li> 
      </ul></li> 
     <li> <p><strong>Agregar documentos al proyecto y a sus tareas y problemas</strong>: Permite a los usuarios agregar documentos a un proyecto (o agregar documentos a tareas y problemas dentro del proyecto) después de que el proyecto haya sido marcado como Completado o Muerto.</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
     <li> <p><strong>Adjuntar plantillas</strong>: Permite a los usuarios adjuntar plantillas a un proyecto después de que el proyecto se haya marcado como Completado o Muerto.</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
