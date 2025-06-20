---
title: Configurar las preferencias de proyecto de un grupo
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Si fuese administrador de un grupo y un administrador de Adobe Workfront desbloquease una preferencia de proyecto para todos los grupos del sistema, configure esa preferencia para el grupo para que afecte a todos los proyectos posteriores que cree el grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '2765'
ht-degree: 95%

---

# Configurar las preferencias del proyecto de un grupo


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Si fuese administrador de un grupo y un administrador de Adobe Workfront desbloquease una preferencia de proyecto para todos los grupos del sistema, configure esa preferencia para el grupo para que afecte a todos los proyectos posteriores que cree el grupo.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>* Normalmente, una preferencia desbloqueada permanecerá desbloqueada indefinidamente. Si el administrador de Workfront volviese a bloquearla, la configuración del sistema volverá a tener efecto y se perderá la configuración de las preferencias realizadas por los administradores del grupo.
>* Las preferencias establecidas para el grupo asociado a un proyecto tendrán prioridad sobre las preferencias establecidas para el grupo de inicio del usuario que cree el proyecto.
>* Algunas preferencias de nivel de grupo afectarán a las plantillas de proyecto que cree para el grupo. Para obtener más información, consulte la sección [Ver, trabajar y crear plantillas para grupos desde el área Grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) en el artículo [Crear y modificar plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Una vez que un administrador de Workfront desbloquee una preferencia en el sistema, podrá configurarla y, a continuación, bloquearla para garantizar que todos los miembros del grupo y los subgrupos usen la misma configuración. Esto es similar a la capacidad que tiene un administrador de Workfront para configurar y bloquear preferencias para todos los miembros del sistema. Para obtener más información, consulte [Bloquear o desbloquear las preferencias de un proyecto, tarea o problema para los subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

La configuración a nivel de grupo también es posible para las preferencias de tareas y problemas, así como para las preferencias de plantillas de horas y horas. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) y [Configurar las preferencias de plantillas de horas y horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Para obtener información acerca de cómo un administrador de Workfront desbloquea las preferencias de un proyecto, consulte [Bloquear o desbloquear las preferencias de proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

## Configurar una preferencia de proyecto desbloqueada para un grupo

>[!TIP]
>
>Si es administrador de Workfront, omita los pasos del 1 al 4 yendo a Configuración > Preferencias de proyecto > Proyectos y buscando el nombre del grupo en el cuadro de la parte superior de la página.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Icono de grupos](assets/groups-icon.png).

1. Haga clic en el nombre del grupo cuyas preferencias de proyecto quiera configurar.
1. En el panel izquierdo, haga clic en **Preferencias de proyecto**.
1. En la página que aparece, continúe con una de las 4 secciones que se enumeran a continuación para configurar las preferencias de Estado del proyecto, Cronologías, Casos empresariales y Vida después de la muerte.

   >[!TIP]
   >
   >Si al pasar el puntero por encima de una preferencia se mostrase ayuda contextual indicando que está bloqueada, pida al administrador de Workfront que la desbloquee para todos los grupos de la organización.

* [Estado del proyecto](#project-status)
* [Timelines](#timelines)
* [Casos empresariales](#business-cases)
* [Vida después de la muerte](#life-after-death)

### Estado del proyecto {#project-status}

Configure cualquiera de las siguientes preferencias para los proyectos recién creados y asociados al grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Permitir a los usuarios crear proyectos sin usar una plantilla</td>
<td><p>Esta preferencia permite a los usuarios crear proyectos sin usar plantillas al crear proyectos de las siguientes áreas:</p>
<ul>
<li><p>Usar la opción Nuevo proyecto en una lista de proyectos</p></li>

<li><p>Convertir un problema en un proyecto desde la página del problema</p></li>
</ul>

<p>Esta preferencia está habilitada de forma predeterminada en el sistema.</p>
<p><b>NOTA</b></p>
<p>Cuando un usuario pertenezca a varios grupos con diferentes preferencias, se le permitirá crear un proyecto sin plantilla si al menos uno de sus grupos tuviera esta preferencia habilitada.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Establecer el estado del proyecto nuevo en</td> 
   <td> <p>Determinar el estado de los nuevos proyectos.</p> <p><b>NOTA</b>   
     <ul> 
      <li>Si usted u otro administrador de Workfront oculta el estado seleccionado aquí, el estado predeterminado cambia al primer estado de la lista de estados.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">En el caso de las preferencias de proyecto de grupo, solo puede seleccionar un estado bloqueado o un estado obligatorio como estado predeterminado.</li> 
      <li> <p>Si un sistema bloqueado o un estado de grupo está establecido como estado predeterminado y más tarde alguien lo desbloquea, el sistema intenta reemplazarlo por un estado bloqueado del mismo tipo de estado.</p> <p>Si no encuentra ninguno, busca un estado obligatorio:</p> 
       <ul> 
        <li>Si hay un estado obligatorio que equivale al estado predeterminado desbloqueado, el estado obligatorio se convierte en el estado predeterminado, incluso si está desbloqueado.</li> 
        <li>Si ninguno de los estados obligatorios equivale al estado predeterminado desbloqueado, el primer estado obligatorio de la lista de estados se convierte en el estado predeterminado.</li> 
       </ul> <p>Para obtener información sobre los estados obligatorios, consulte los artículos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de proyectos del sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de tareas del sistema</a> y <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de problemas del sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calcular el porcentaje completado en función de</td> 
   <td> <p>El porcentaje completado de un proyecto o tarea principal se basa en el progreso general de las tareas. Esta información se puede calcular en función de la duración o las horas planificadas de las tareas de un proyecto.</p> <p>Si selecciona Duración, la duración de cada tarea de un proyecto determina el porcentaje completado global del proyecto, y la duración de cada subtarea determina el porcentaje completado global de su tarea principal.</p> <p>Si selecciona Duración, asegúrese de especificar las Horas típicas por día laborable y los Días laborables típicos por semana en la sección Líneas de tiempo. Workfront utiliza esta información para calcular el porcentaje completado de una tarea según la duración. </p> <p>Si selecciona Horas planificadas, asegúrese de que todas las tareas de cada proyecto tengan la cantidad de Horas planificadas definida y que la cantidad no sea cero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Establecer automáticamente Condición de proyecto según el estado de Progreso</td> 
   <td> <p>Esta preferencia permite a los usuarios establecer manualmente la condición de un proyecto (según el objetivo, en riesgo o con problemas) o hacer que Workfront establezca la condición (estado de progreso) automáticamente en función de la progresión del proyecto en la línea de tiempo. Para obtener más información sobre la condición de los proyectos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Información general sobre la condición del proyecto y el tipo de condición</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Crear automáticamente líneas base</p> </td> 
   <td> <p>Esta preferencia crea automáticamente una línea base (instantánea) de los detalles de tareas y proyectos cuando el estado del proyecto cambia a Actual. Para obtener información sobre cómo crear líneas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Crear líneas de base del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Método de índice de rendimiento </p> </td> 
   <td> <p>El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Workfront para calcular métricas de valor ganado como el índice de rendimiento de costes (CPI) y la estimación al finalizar (EAC). Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular el índice de rendimiento de costes (CPI)</a> y <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular la estimación al finalizar (EAC)</a></p> 
    <ul> 
     <li><strong>Basado en horas</strong>: Workfront usa las horas planificadas para calcular métricas de rendimiento como EAC y CPI. Cuando el PIM se calcula en función de las horas, la EAC se muestra como un número de horas. Asegúrese de que tiene un valor de Horas planificadas distinto de cero.</li> 
     <li> <p><strong>Basado en costes</strong>: Workfront usa Coste planificado de mano de obra para calcular métricas de rendimiento como EAC y CPI. Asegúrese de que las funciones o los usuarios estén asociados a las tarifas de coste por hora. Cuando el PIM se calcula en función de los costes, la EAC se muestra como un valor de moneda.</p> <p>El gerente del proyecto puede modificar esta configuración a nivel de proyecto mediante el área Finanzas en Detalles del proyecto. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área Finanzas del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Estimar al finalizar </p> </td> 
   <td> <p>Determine qué datos utiliza Workfront para calcular el valor del Coste estimado al finalizar (EAC) que representa el coste total proyectado de un proyecto.</p> 
    <ul> 
     <li><strong>Calcular a nivel de proyecto</strong>: el valor de EAC de la tarea principal y el proyecto se determinan introduciendo las horas reales o el coste real de la mano de obra en las fórmulas de EAC. El cálculo incluye las horas reales o costes y gastos añadidos directamente a la tarea o proyecto principal.</li> 
     <li> <p><strong>Resumen de tareas/subtareas:</strong> la estimación EAC de la tarea principal y el proyecto se determinan añadiendo la estimación EAC de cada tarea secundaria. El cálculo incluye las horas reales o los costes y gastos reales añadidos directamente a la tarea o proyecto principal.</p> <p>El gerente del proyecto puede modificar esta configuración a nivel de proyecto mediante el área Finanzas en Detalles del proyecto. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área Finanzas del proyecto</a>.</p> </li> 
    </ul> <p>Para obtener más información sobre cómo se calcula la EAC, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular estimación al finalizar (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Cronologías {#timelines}

Configure cualquiera de las siguientes preferencias para los proyectos recién creados y asociados al grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Programar desde</td> 
   <td> <p>Determine si los nuevos proyectos se programan desde la fecha de inicio o desde la fecha de finalización cuando se crean.</p> 
    <ul> 
     <li><strong>Fecha de inicio</strong>: las nuevas tareas tienen como valor predeterminado la restricción de tarea Lo antes posible y se pide a los gerentes del proyecto que proporcionen una fecha planificada de inicio para el proyecto.</li> 
     <li><strong>Fecha de finalización</strong>: las nuevas tareas tienen como valor predeterminado la restricción de tarea Lo más tarde posible y se pide a los gerentes del proyecto que proporcionen una fecha planificada de finalización para el proyecto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Días libres del usuario</td> 
   <td> <p>Determine si el tiempo libre del usuario asignado principal de una tarea ajusta las fechas planificadas de esa tarea en un proyecto.</p> 
    <ul> 
     <li> <p><strong>Considere el tiempo libre del usuario en las duraciones de las tareas</strong>: cualquier tiempo libre programado para la persona asignada principal de una tarea ajusta las fechas planificadas de la tarea si el tiempo libre se produce durante la duración de la tarea. Esta es la configuración predeterminada. </p> <p>Por ejemplo, si una tarea con una restricción de Lo antes posible está programada para comenzar el 1 de junio y finalizar el 3 de junio, y la persona asignada principal tiene marcado el 2 de junio como tiempo libre, las fechas planificadas de la tarea se ajustarán del 1 de junio al 4 de junio.</p> <p><b>IMPORTANTE</b>: la duración de la tarea no cambia al seleccionar esta configuración. Solo cambian las fechas planificadas, dependiendo de la Restricción de tarea.</p> </li> 
     <li><strong>Ignore el tiempo libre del usuario en las duraciones de la tarea</strong>: las fechas planificadas de cada tarea en un proyecto permanecen tal y como se planificó originalmente, aunque el usuario asignado principal de una tarea tenga tiempo libre durante su duración.</li> 
    </ul> <p>Tenga en cuenta lo siguiente al seleccionar opciones para esta configuración:</p> 
    <ul> 
     <li>Al cambiar esta configuración, solo los proyectos y las plantillas creados después del cambio heredan la configuración actualizada. </li> 
     <li> <p>El valor Restricción de tarea de la tarea determina qué fechas de tareas planificadas se deben ajustar: </p> 
      <ul> 
       <li>Fecha planificada de inicio</li> 
       <li>Fecha planificada de finalización</li> 
       <li>Ambas fechas</li> 
       <li>Ninguna fecha. </li> 
      </ul> <p>Por ejemplo, si una tarea tiene una Restricción de fechas fijas, las fechas no se ajustan cuando el usuario asignado principal tiene días libres, incluso si la opción Tenga en cuenta los días libres del usuario en las duraciones de la tarea está seleccionada. Para obtener más información sobre las restricciones de tarea, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Información general de la restricción de tarea</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Las líneas de tiempo del proyecto se recalculan automáticamente</strong> </p> </td> 
   <td> <p>Determine cuándo se vuelve a calcular la línea de tiempo de un proyecto. Para obtener información sobre cómo recalcular la escala de tiempo del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular las escalas de tiempo del proyecto</a>.</p> <p>Las siguientes opciones están habilitadas de forma predeterminada. Puede seleccionar una o varias de las siguientes opciones de configuración:</p> 
    <ul> 
     <li> <p><strong>Cada noche</strong>: seleccione esta opción para recalcular las líneas de tiempo del proyecto cada noche. Los cambios que realice en el proyecto y que puedan afectar a la línea de tiempo no serán visibles de inmediato. Workfront recalcula las líneas de tiempo por la noche solo para los proyectos en los que se cumplen las dos condiciones siguientes:</p> <p> 
       <ul> 
        <li>Tiene un estado Actual</li> 
        <li>Ha tenido una actualización en los últimos 3 meses</li> 
       </ul> </p> </li> 
     <li> <p><strong>Cuando cambia el ámbito de un proyecto</strong>: seleccione esta opción para recalcular las líneas de tiempo del proyecto inmediatamente cuando se produzca un cambio en el ámbito del proyecto. Para obtener información sobre lo que constituye un cambio de ámbito del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular las escalas de tiempo del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Cuando se asignan varios usuarios a una tarea, utilice la programación de ...</strong> </p> </td> 
   <td> <p>Si un proyecto no tiene una programación asignada o si los usuarios asignados a sus tareas no tienen una programación asignada, Workfront utiliza el horario predeterminado del sistema para calcular la línea de tiempo de las tareas.</p> <p>Si asigna varios usuarios a la misma tarea en un proyecto que tiene una programación asignada (y los usuarios asignados a las tareas también tienen una programación asignada), Workfront utiliza las siguientes programaciones:</p> 
    <ul> 
     <li><strong>Asignación principal</strong>: Workfront usa la programación de la asignación principal de la tarea para calcular las líneas de tiempo.</li> 
     <li><strong>Proyecto</strong>: Workfront usa la programación del proyecto para calcular la línea de tiempo de cada tarea.</li> 
    </ul> <p>Para obtener más información acerca de las programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Crear una programación</a>.</p> </td> 
  </tr> 
 <tr> 
   <td role="rowheader"> <p><strong>Cuando se asigne un usuario a una tarea, utilice la programación de...</strong> </p> </td> 
   <td> <p>Si un proyecto no tiene asignada ninguna programación o si los usuarios asignados a sus tareas no tienen asignada una programación, [!DNL Workfront] utiliza el horario predeterminada del sistema para calcular la escala de tiempo de las tareas.</p>

<p>Si asigna un usuario a una tarea de un proyecto y tanto el proyecto como el usuario tienen asociada una programación, [!UICONTROL Workfront] utilizará las siguientes programaciones:</p> 
    <ul> 
     <li><strong>[!UICONTROL Usuario]</strong>: La programación del usuario asignado en la tarea para calcular las escalas de tiempo.</li> 
     <li><strong>[!UICONTROL Project]</strong>: La programación del proyecto para calcular la escala de tiempo de la tarea.</li> 
    </ul> <p>Para obtener más información acerca de las programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Crear una programación</a>.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Cálculos de escala de tiempo </p> </td> 
   <td> 
    <ul> 
     <li><strong>Horas habituales por día laborable</strong>: establezca la cantidad de horas en un día laborable habitual para los usuarios que trabajarán en proyectos. El valor predeterminado es de 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>Días laborables habituales por semana</strong>: establezca la semana laboral estándar para los usuarios que trabajarán en proyectos. El valor predeterminado es de 5 días.</li> 
    </ul> <p>Estas dos opciones convierten los días en horas o las semanas en días.</p> <p>Por ejemplo, si tiene una tarea con 8 horas planificadas y la duración se calcula según las horas planificadas, Workfront convierte esas horas en días para mostrar la duración como días.</p> <p>En el campo Días laborables habituales por semana, Workfront calcula el valor de Equivalente a jornada completa (EJC) para su sistema. Esto es lo que utiliza Workfront al calcular las asignaciones para los usuarios.</p> <p>Estos valores se utilizan cuando se planifican las líneas de tiempo de los proyectos, se presupuestan los recursos o se registra el tiempo en los proyectos. </p> <p>No se usan cuando se establecen las plantillas de horas para los usuarios del sistema, tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configurar preferencias de plantilla de horas y horas</a>.</p> <p><b>NOTA</b>: Los administradores de Workfront no pueden desbloquear las preferencias de cálculos de línea de tiempo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Trimestres personalizados</strong> </p> </td> 
   <td> <p>Configure trimestres anuales personalizados para los usuarios que trabajarán en proyectos. Los trimestres personalizados suelen ser trimestres que no coinciden con el desglose tradicional de trimestres durante un año natural. Puede añadir varios trimestres personalizados. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados</a>.</p> <p><b>NOTA</b>: Los administradores de Workfront no pueden desbloquear las preferencias de trimestres personalizados.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Casos comerciales {#business-cases}

Puede crear un caso empresarial para los proyectos recién creados asociados al grupo para enviar solicitudes de proyecto. Puede definir las preferencias para determinar qué áreas están visibles en el formulario **Caso empresarial**. Se recomienda habilitar estas opciones para que otras herramientas, como el optimizador de portafolios, se actualicen correctamente. Para obtener más información acerca de lo que muestra cada campo, consulte [Definir un caso empresarial: índice de artículos](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Una vez que el administrador de Workfront habilita las secciones del caso empresarial, un propietario del proyecto puede crear un caso empresarial a nivel del proyecto. Para obtener información sobre cómo crear un caso empresarial, consulte [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Vida después de la muerte  {#life-after-death}

Configure cualquiera de las siguientes preferencias para los proyectos recién creados y asociados al grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Después de que un proyecto se haya marcado como Completado, los usuarios aún pueden</strong> </p> </td> 
   <td> <p>Determinar las reglas para su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a si una tarea o un problema se puede eliminar después de que el estado del proyecto se haya marcado como Completado.</p> 
    <ul> 
     <li><strong>Eliminar tareas</strong>: permite a los usuarios eliminar tareas de un proyecto después de que el proyecto se haya marcado como Completado.<br></li> 
     <li><strong>Eliminar problemas</strong>: permite a los usuarios eliminar problemas de un proyecto después de que el proyecto se haya marcado como Completado.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Después de que un proyecto se haya marcado como completado o inactivo, o si se encuentra pendiente de aprobación, los usuarios aún pueden</strong> </p> </td> 
   <td> <p>Determinar las reglas para su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a lo que sucede con las tareas, los problemas, los documentos y otros objetos de un proyecto después de que el estado del proyecto se haya marcado como <strong>Completado</strong>, <strong>Inactivo</strong> o esté <strong>Pendiente de aprobación</strong>.</p> 
    <ul> 
     <li><strong>Añadir y editar tareas</strong> Permite a los usuarios: 
      <ul> 
       <li>Editar tareas dentro de un proyecto después de que el proyecto se haya marcado como Completado, Inactivo o esté Pendiente de aprobación. Esto incluye añadir horas y cambiar entradas de gastos en una tarea.</li> 
       <li>Añadir tareas a un proyecto.</li> 
      </ul></li> 
     <li><strong>Añadir y editar problemas</strong>: permite a los usuarios: 
      <ul> 
       <li>Editar problemas dentro de un proyecto después de que el proyecto se haya marcado como Completado, Inactivo o esté Pendiente de aprobación.</li> 
       <li>Añadir problemas a un proyecto después de que el proyecto se haya marcado como Completado o Inactivo. (No puede añadir problemas a un proyecto que esté Pendiente de aprobación).</li> 
      </ul></li> 
     <li> <p><strong>Añadir documentos al proyecto y a sus tareas y problemas</strong>: permite a los usuarios añadir documentos a un proyecto (o añadir documentos a tareas y problemas dentro del proyecto) después de que el proyecto se haya marcado como Completado o Inactivo.</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
     <li> <p><strong>Adjuntar plantillas</strong>: permite a los usuarios adjuntar plantillas a un proyecto después de que el proyecto se haya marcado como Completado o Inactivo.</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
