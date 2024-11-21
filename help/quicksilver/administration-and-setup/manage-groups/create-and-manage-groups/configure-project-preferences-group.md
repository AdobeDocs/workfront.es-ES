---
title: Configurar las preferencias de proyecto de un grupo
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Si es administrador de un grupo y un administrador de Adobe Workfront desbloquea una preferencia de proyecto para todos los grupos del sistema, puede configurar esa preferencia para que el grupo afecte a todos los proyectos subsiguientes que cree el grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '2825'
ht-degree: 1%

---

# Configurar las preferencias de proyecto de un grupo


<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Si es administrador de un grupo y un administrador de Adobe Workfront desbloquea una preferencia de proyecto para todos los grupos del sistema, puede configurar esa preferencia para que el grupo afecte a todos los proyectos subsiguientes que cree el grupo.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>* Normalmente, una preferencia desbloqueada permanece desbloqueada indefinidamente. Si el administrador de Workfront vuelve a bloquearlo, la configuración del sistema vuelve a tener efecto y se pierde la configuración de las preferencias realizadas por los administradores del grupo.
>* Las preferencias establecidas para el grupo asociado a un proyecto tienen prioridad sobre las preferencias establecidas para el grupo de inicio del usuario que crea el proyecto.
>* Algunas preferencias de nivel de grupo afectan a las plantillas de proyecto que crea para el grupo. Para obtener más información, consulte la sección [Ver, trabajar y crear plantillas para su grupo desde el área de grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) en el artículo [Crear y modificar plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Una vez que un administrador de Workfront desbloquea una preferencia en el sistema, puede configurarla y, a continuación, bloquearla para garantizar que todos los miembros del grupo y de sus subgrupos estén utilizando la misma configuración. Esto es paralelo a la capacidad que tiene un administrador de Workfront para configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, vea [Bloquear o desbloquear las preferencias de proyecto, tarea o problema de los subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

La configuración a nivel de grupo también es posible para las preferencias de tareas y problemas y para las preferencias de hojas de horas y horas. Para obtener más información, consulte [Configurar las preferencias de tareas y problemas para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) y [Configurar las preferencias de horas y hojas de horas para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Para obtener información acerca de cómo un administrador de Workfront desbloquea las preferencias de un proyecto, vea [Bloquear o desbloquear las preferencias de proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
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

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar una preferencia de proyecto desbloqueada para un grupo

>[!TIP]
>
>Si es administrador de Workfront, puede omitir los pasos del 1 al 4 si va a Configuración > Preferencias de proyecto > Proyectos y busca el nombre del grupo en el cuadro de la parte superior de la página.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo cuyas preferencias de proyecto desee configurar.
1. En el panel izquierdo, haga clic en **Preferencias de proyecto**.
1. En la página que aparece, continúe con una de las 4 secciones que se enumeran a continuación para configurar las preferencias de Estado del proyecto, Cronología, Casos comerciales y Vida después de la muerte.

   >[!TIP]
   >
   >Si pasa el ratón por encima de una preferencia y se muestra información del objeto para indicarle que está bloqueada, puede pedir al administrador de Workfront que la desbloquee para todos los grupos de la organización.

* [Estado del proyecto](#project-status)
* [Líneas de tiempo](#timelines)
* [Casos comerciales](#business-cases)
* [Vida después de la muerte](#life-after-death)

### Estado del proyecto {#project-status}

Configure cualquiera de las siguientes preferencias para proyectos recién creados y asociados con el grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Permitir a los usuarios crear proyectos sin usar una plantilla</td>
<td><p>Esta preferencia permite a los usuarios crear proyectos sin utilizar una plantilla al crear un proyecto desde las siguientes áreas:</p>
<ul>
<li><p>Utilizar la opción Nuevo proyecto en una lista de proyectos</p></li>

<li><p>Conversión de un problema en un proyecto desde la página del problema</p></li>
</ul>

<p>Esta preferencia está habilitada de forma predeterminada en el sistema.</p>
<p><b>NOTA</b></p>
<p>Cuando un usuario pertenece a varios grupos con diferentes preferencias, se le permitirá crear un proyecto sin plantilla si al menos uno de sus grupos tiene esta preferencia habilitada.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Definir el estado del nuevo proyecto como</td> 
   <td> <p>Determine el estado de los nuevos proyectos.</p> <p><b>NOTA</b>   
     <ul> 
      <li>Si usted u otro administrador de Workfront oculta el estado seleccionado aquí, el estado predeterminado cambia al primer estado de la lista de estados.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Para las preferencias de proyecto de grupo, solo puede seleccionar un estado bloqueado o un estado requerido como estado predeterminado.</li> 
      <li> <p>Si un sistema bloqueado o un estado de grupo está establecido como estado predeterminado y más tarde alguien lo desbloquea, el sistema intenta reemplazarlo con un estado bloqueado del mismo tipo de estado.</p> <p>Si no encuentra ninguna, busca un estado requerido:</p> 
       <ul> 
        <li>Si hay un estado obligatorio que equivale al estado predeterminado desbloqueado, el estado requerido se convierte en el estado predeterminado, incluso si está desbloqueado.</li> 
        <li>Si ninguno de los estados requeridos equivale al estado predeterminado desbloqueado, el primer estado requerido de la lista de estados se convierte en el estado predeterminado.</li> 
       </ul> <p>Para obtener información acerca de los estados requeridos, vea los artículos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Obtener acceso a la lista de estados de proyectos del sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Obtener acceso a la lista de estados de tareas del sistema</a> y <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Obtener acceso a la lista de estados de problemas del sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calcular porcentaje completado en función de</td> 
   <td> <p>El porcentaje completado de un proyecto o tarea principal se basa en el progreso general de las tareas. Esta información se puede calcular en función de la duración o las horas planificadas de las tareas de un proyecto.</p> <p>Si selecciona Duración, la Duración de cada tarea de un proyecto determina el porcentaje completado global del proyecto, y la Duración de cada subtarea determina el porcentaje completado global de su tarea principal.</p> <p>Si selecciona Duración, asegúrese de especificar las Horas típicas por día laborable y los Días laborables típicos por semana en la sección Escalas de tiempo. Workfront utiliza esta información al calcular el porcentaje completado de una tarea según la duración. </p> <p>Si selecciona Horas planificadas, asegúrese de que todas las tareas de cada proyecto tengan la cantidad de Horas planificadas definida y que la cantidad no sea cero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Establecer automáticamente Condición de proyecto según el estado de Progreso</td> 
   <td> <p>Esta preferencia permite a los usuarios establecer la condición de un proyecto manualmente (como destino, en riesgo o con problemas) o hacer que Workfront establezca la condición (estado de progreso) automáticamente en función de la progresión del proyecto en la cronología. Para obtener más información acerca de la condición de los proyectos, vea <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Información general sobre la condición del proyecto y el tipo de condición</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Crear automáticamente líneas base</p> </td> 
   <td> <p>Esta preferencia crea automáticamente una línea de base (instantánea) de los detalles de tareas y proyectos cuando el estado del proyecto cambia a Actual. Para obtener información acerca de cómo crear líneas de base, vea <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Crear líneas de base de proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Método de índice de rendimiento </p> </td> 
   <td> <p>El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza Workfront para calcular métricas de valor ganado como el índice de rendimiento de costes (CPI) y la estimación al finalizar (EAC). Para obtener más información, vea <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular el índice de rendimiento de costos (CPI)</a>y <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular la estimación al finalizar (EAC)</a></p> 
    <ul> 
     <li><strong>Basado en horas</strong>: Workfront usa las horas planificadas para calcular métricas de rendimiento como EAC y CPI. Cuando el PIM se calcula en función de las horas, el EAC se muestra como un número de horas. Asegúrese de que tiene un valor de Horas planificadas distinto de cero.</li> 
     <li> <p><strong>Basado en costos</strong>: Workfront usa Costo de mano de obra planificado para calcular métricas de rendimiento como EAC y CPI. Asegúrese de que los puestos de trabajo o los usuarios estén asociados a las tarifas de coste por hora. Cuando el PIM se calcula en función de los costes, el EAC se muestra como un valor de moneda.</p> <p>El jefe de proyecto puede modificar esta configuración en el nivel de proyecto mediante el área Finanzas de Detalles del proyecto. Para obtener más información, vea <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área Finanzas del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Estimar al finalizar </p> </td> 
   <td> <p>Determine qué datos utiliza Workfront para calcular el valor de Estimar al finalizar (EAC) que representa el coste total proyectado de un proyecto.</p> 
    <ul> 
     <li><strong>Calcular a nivel de proyecto</strong>:EAC para la tarea y el proyecto principales se determinan al introducir Horas reales o Costo de mano de obra real en las Fórmulas EAC. Este cálculo incluye las horas reales o los costos y gastos agregados directamente a la tarea o proyecto principal.</li> 
     <li> <p><strong>Resumir a partir de tareas/subtareas</strong>: el EAC de la tarea y el proyecto principales se determina resumiendo el EAC de cada tarea secundaria. Este cálculo excluye las horas reales o los costos y gastos reales agregados directamente a la tarea o proyecto principal.</p> <p>El jefe de proyecto puede modificar esta configuración en el nivel de proyecto mediante el área Finanzas de Detalles del proyecto. Para obtener más información, vea <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área Finanzas del proyecto</a>.</p> </li> 
    </ul> <p>Para obtener más información sobre cómo calcula el EAC, vea <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular estimación al finalizar (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Cronologías {#timelines}

Configure cualquiera de las siguientes preferencias para proyectos recién creados y asociados con el grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Programar desde</td> 
   <td> <p>Determine si los nuevos proyectos se programan desde la fecha de inicio o desde la fecha de finalización cuando se crean.</p> 
    <ul> 
     <li><strong>Fecha de inicio</strong>: las nuevas tareas tienen como valor predeterminado la restricción de tarea Lo antes posible y se pide a los jefes de proyecto que proporcionen una fecha planificada de inicio para el proyecto.</li> 
     <li><strong>Fecha de finalización</strong>: las nuevas tareas tienen el valor predeterminado de la restricción de tarea Lo más tarde posible y se pide a los jefes de proyecto que proporcionen una fecha planificada de finalización para el proyecto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tiempo libre del usuario</td> 
   <td> <p>Determine si el tiempo libre de la persona asignada principal de una tarea ajusta las fechas planificadas para esa tarea en un proyecto.</p> 
    <ul> 
     <li> <p><strong>Considere el tiempo libre del usuario en las duraciones de las tareas</strong>: cualquier tiempo libre programado para la persona asignada principal de una tarea ajusta las fechas planificadas de la tarea si el tiempo libre se produce durante la duración de la tarea. Esta es la configuración predeterminada. </p> <p>Por ejemplo, si una tarea con una delimitación de Lo antes posible está programada para comenzar el 1 de junio y finalizar el 3 de junio, y la persona asignada principal tiene marcado el 2 de junio como Tiempo de espera, las fechas planificadas de la tarea se ajustarán del 1 de junio al 4 de junio.</p> <p><b>IMPORTANTE</b>: La duración de la tarea no cambia al seleccionar esta configuración. Solo cambian las fechas planificadas, dependiendo de la Restricción de tarea.</p> </li> 
     <li><strong>Ignorar tiempo libre del usuario en las duraciones de tareas</strong>: las fechas planificadas de cada tarea en un proyecto permanecen tal y como se planeó originalmente, aunque la persona asignada principal de una tarea tenga tiempo libre durante su duración.</li> 
    </ul> <p>Tenga en cuenta lo siguiente al seleccionar opciones para esta configuración:</p> 
    <ul> 
     <li>Al cambiar esta configuración, solo los proyectos y las plantillas creados después del cambio heredan la configuración actualizada. </li> 
     <li> <p>El valor Restricción de tarea de la tarea determina qué fechas de tareas planificadas se deben ajustar: </p> 
      <ul> 
       <li>Fecha planificada de inicio</li> 
       <li>Fecha planificada de finalización</li> 
       <li>Ambas fechas</li> 
       <li>Ninguna cita. </li> 
      </ul> <p>Por ejemplo, si una tarea tiene una Restricción de fechas fijas, las fechas no se ajustan cuando el usuario asignado principal tiene tiempo libre, incluso si la opción Considerar el tiempo libre del usuario en la duración de la tarea está seleccionada. Para obtener información acerca de las restricciones de tareas, vea <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Introducción a la restricción de tareas</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Las escalas de tiempo del proyecto se volverán a calcular automáticamente</strong> </p> </td> 
   <td> <p>Determine cuándo se vuelve a calcular la escala de tiempo de un proyecto. Para obtener información sobre cómo recalcular la escala de tiempo del proyecto, vea <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular escalas de tiempo del proyecto</a>.</p> <p>Las siguientes opciones están habilitadas de forma predeterminada. Puede seleccionar una o varias de las siguientes opciones de configuración:</p> 
    <ul> 
     <li> <p><strong>Cada noche</strong>: seleccione esta opción para recalcular las escalas de tiempo del proyecto cada noche. Los cambios que realice en el proyecto y que puedan afectar a la escala de tiempo no serán visibles de inmediato. Workfront​​​ vuelve a calcular las escalas de tiempo por la noche solo para los proyectos en los que se cumplen las dos condiciones siguientes:</p> <p> 
       <ul> 
        <li>Tener un estado de Actual</li> 
        <li>Ha tenido una actualización en los últimos 3 meses</li> 
       </ul> </p> </li> 
     <li> <p><strong>Cuando cambie el ámbito de un proyecto</strong>: seleccione esta opción para recalcular las escalas de tiempo del proyecto inmediatamente cuando se produzca un cambio en el ámbito del proyecto. Para obtener información sobre lo que constituye un cambio en el ámbito del proyecto, vea <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Volver a calcular las escalas de tiempo del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Cuando se asignan varios usuarios a una tarea, utilice la programación de ...</strong> </p> </td> 
   <td> <p>Si un proyecto no tiene una programación asignada o si los usuarios asignados a sus tareas no tienen una programación asignada, Workfront utiliza la programación predeterminada del sistema para calcular la escala de tiempo de las tareas.</p> <p>Si asigna varios usuarios a la misma tarea en un proyecto que tiene una programación asignada (y los usuarios asignados a las tareas también tienen una programación asignada), Workfront utiliza las siguientes programaciones:</p> 
    <ul> 
     <li><strong>Asignación principal</strong>: Workfront usa la programación de la asignación principal de la tarea para calcular las escalas de tiempo.</li> 
     <li><strong>Proyecto</strong>: Workfront usa la programación del proyecto para calcular la escala de tiempo de cada tarea.</li> 
    </ul> <p>Para obtener más información acerca de las programaciones, vea <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Crear una programación</a>.</p> </td> 
  </tr> 
 <tr> 
   <td role="rowheader"> <p><span class="preview"><strong>Cuando se asigne un usuario a una tarea, utilice la programación de...</strong></span> </p> </td> 
   <td> <div class="preview"><p>Si un proyecto no tiene asignada una programación o si los usuarios asignados a sus tareas no tienen asignada una programación, [!DNL Workfront] utiliza la programación predeterminada del sistema para calcular la escala de tiempo de las tareas.</p>

<p>Si asigna un usuario a una tarea de un proyecto y tanto el proyecto como el usuario tienen asociada una programación, [!UICONTROL Workfront] utilizará las siguientes programaciones:</p> 
    <ul> 
     <li><strong>[!UICONTROL Usuario]</strong>: La programación del usuario asignado en la tarea para calcular las escalas de tiempo.</li> 
     <li><strong>[!UICONTROL Project]</strong>: La programación del proyecto para calcular la escala de tiempo de la tarea.</li> 
    </ul> <p>Para obtener más información acerca de las programaciones, vea <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Crear una programación</a>.</p></div></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Cálculos de cronología </p> </td> 
   <td> 
    <ul> 
     <li><strong>Horas típicas por día laborable</strong>: establezca la cantidad de horas en un día laborable típico para los usuarios que trabajarán en proyectos. El valor predeterminado es de 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>Días laborables habituales por semana</strong>: establezca la semana laboral estándar para los usuarios que trabajarán en proyectos. El valor predeterminado es 5 días.</li> 
    </ul> <p>Estas dos opciones convierten los días en horas o las semanas en días.</p> <p>Por ejemplo, si tiene una tarea con 8 horas planificadas y la duración se calcula según las horas planificadas, Workfront convierte esas horas en días para mostrar la duración como días.</p> <p>En el campo Días laborables típicos por semana, Workfront calcula el valor de Tiempo equivalente completo (FTE) para su sistema. Esto es lo que utiliza Workfront al calcular las asignaciones para los usuarios.</p> <p>Estos valores se utilizan cuando se planifican las escalas de tiempo de los proyectos, se presupuestan los recursos o se registra el tiempo en los proyectos. </p> <p>No se usan al establecer hojas de horas para los usuarios del sistema, como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configurar las preferencias de horas y hojas de horas</a>.</p> <p><b>NOTA</b>: Los administradores de Workfront no pueden desbloquear las preferencias de cálculos de escala de tiempo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Trimestres personalizados</strong> </p> </td> 
   <td> <p>Configure trimestres anuales personalizados para los usuarios que trabajarán en proyectos. Los trimestres personalizados suelen ser trimestres que no coinciden con el desglose tradicional de trimestres durante un año natural. Puede agregar varios trimestres personalizados. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados para proyectos</a>.</p> <p><b>NOTA</b>: Los administradores de Workfront no pueden desbloquear las preferencias de trimestres personalizados.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Casos comerciales {#business-cases}

Puede crear un caso empresarial para los proyectos recién creados asociados al grupo para enviar solicitudes de proyecto. Puede definir las preferencias para determinar qué áreas están visibles en el formulario **Caso comercial**. Se recomienda habilitar estas opciones para que otras herramientas, como Portfolio Optimizer, se actualicen correctamente. Para obtener más información acerca de lo que muestra cada campo, vea [Definir un caso comercial: índice de artículo](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Una vez que el administrador de Workfront habilita las secciones del caso empresarial, un propietario del proyecto puede crear un caso empresarial en el nivel de proyecto. Para obtener información sobre cómo crear un caso empresarial, vea [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Vida después de la muerte  {#life-after-death}

Configure cualquiera de las siguientes preferencias para proyectos recién creados y asociados con el grupo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Después de que un proyecto se haya marcado como Completo, los usuarios aún pueden</strong> </p> </td> 
   <td> <p>Determine las reglas para su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a si una tarea o un problema se puede eliminar después de que el estado del proyecto se haya marcado como Completado.</p> 
    <ul> 
     <li><strong>Eliminar tareas</strong>: permite a los usuarios eliminar tareas de un proyecto después de que el proyecto se haya marcado como Completado.<br></li> 
     <li><strong>Eliminar problemas</strong>: permite a los usuarios eliminar problemas de un proyecto después de que el proyecto se haya marcado como Completado.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Después de que un proyecto se marque como Completo, como Inactivo o tiene Aprobación pendiente, los usuarios aún pueden</strong> </p> </td> 
   <td> <p>Determine las reglas para su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a lo que sucede con las tareas, problemas, documentos y otros objetos de un proyecto después de que el estado del proyecto se haya marcado como <strong>Completo</strong>, <strong>Inactivo</strong> o tiene <strong>Aprobación pendiente</strong>.</p> 
    <ul> 
     <li><strong>Agregar y editar tareas</strong> Permite a los usuarios: 
      <ul> 
       <li>Editar tareas dentro de un proyecto después de que el proyecto se haya marcado como Completo, Inactivo o tiene Aprobación pendiente. Esto incluye agregar horas y cambiar entradas de gastos en una tarea.</li> 
       <li>Agregar tareas a un proyecto.</li> 
      </ul></li> 
     <li><strong>Agregar y editar problemas</strong>: permite a los usuarios: 
      <ul> 
       <li>Editar problemas dentro de un proyecto después de que el proyecto se haya marcado como Completo, Inactivo o Pendiente de aprobación.</li> 
       <li>Agregar problemas a un proyecto después de que el proyecto se haya marcado como Completo o Inactivo. (No puede agregar problemas a un proyecto que tenga Aprobación pendiente).</li> 
      </ul></li> 
     <li> <p><strong>Agregar documentos al proyecto y a sus tareas y problemas</strong>: permite a los usuarios agregar documentos a un proyecto (o agregar documentos a tareas y problemas dentro del proyecto) después de que el proyecto se haya marcado como Completo o Inactivo.</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
     <li> <p><strong>Adjuntar plantillas</strong>: permite a los usuarios adjuntar plantillas a un proyecto después de que el proyecto se haya marcado como Completado o Inactivo.</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
