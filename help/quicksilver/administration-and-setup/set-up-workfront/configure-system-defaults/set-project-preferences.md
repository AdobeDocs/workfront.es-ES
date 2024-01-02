---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar las preferencias de proyecto de todo el sistema
description: Como un [!DNL Adobe Workfront] administrador, puede configurar las preferencias predeterminadas para todos los proyectos creados en el sistema. Estas preferencias afectan al comportamiento del proyecto, la tarea y el problema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: cf044c8cff6b1172ec460ae232cd07c9b7c808b7
workflow-type: tm+mt
source-wordcount: '2513'
ht-degree: 0%

---

# Configurar las preferencias de proyecto de todo el sistema

<!--Audited: 12/2023-->

Como un [!DNL Adobe Workfront] administrador, puede configurar las preferencias predeterminadas para todos los proyectos creados en el sistema. Estas preferencias afectan al comportamiento del proyecto, la tarea y el problema.

>[!NOTE]
>
>De forma predeterminada, estas preferencias están bloqueadas y los administradores de grupos no pueden modificarlas en el nivel de grupo a menos que las desbloquee para todos los grupos del sistema. Para obtener más información, consulte [Bloquear o desbloquear las preferencias de proyecto de todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan</p></td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   O
   <p>Actual: [!UICONTROL plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>[!UICONTROL Administrador del sistema]</p> <p><b>NOTA</b>:</p><p>Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar las preferencias del proyecto para toda la organización

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Proyectos]**.

1. En el **Preferencias de proyecto** , continúe con una de las 4 secciones enumeradas a continuación para configurar las preferencias de [!UICONTROL Estado del proyecto], [!UICONTROL Cronología], [!UICONTROL Casos comerciales], y [!UICONTROL Vida después de la muerte].
1. Si desea que todos los grupos de la organización utilicen las mismas preferencias de proyecto, asegúrese de que todas las preferencias estén bloqueadas ![](assets/lock-toggle-button.png) (esta es la opción predeterminada).

   >[!IMPORTANT]
   >
   >Cuando una preferencia de proyecto está bloqueada, todos los grupos del sistema heredan los cambios que realice en dicha preferencia. Es importante comunicarse con los usuarios y grupos de toda la organización para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que se configuran las preferencias del proyecto.

   Para obtener información sobre cómo desbloquear una preferencia para que todos los grupos puedan configurarla y administrarla por su cuenta, consulte [Bloquear o desbloquear las preferencias de proyecto de todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Haga clic en **[!UICONTROL Guardar]**.

* [[!UICONTROL Estado del proyecto]](#project-status)
* [[!UICONTROL Cronología]](#timelines)
* [[!UICONTROL Casos comerciales]](#business-cases)
* [[!UICONTROL Vida después de la muerte]](#life-after-death)

### Estado del proyecto {#project-status}

Configure cualquiera de las siguientes preferencias para proyectos recién creados en todo el sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permitir que los usuarios creen proyectos sin usar una plantilla]</td> 
   <td>  <p>Esta preferencia permite a los usuarios crear proyectos sin utilizar una plantilla al crear un proyecto desde las siguientes áreas: </p>
      <ul>
        <li>
        <p>Utilizar la opción [!UICONTROL Nuevo proyecto] en una lista de proyectos</p>
        </li>
          <li>
          <p>Conversión de un problema en un proyecto desde la página del problema</p>
          </li>
         </ul>
        <p>Esta preferencia está habilitada de forma predeterminada. </p> 
        <p><b>NOTA</b></p>
        <p> Un administrador de grupo puede cambiar esta preferencia para un grupo. Cuando un usuario pertenece a varios grupos con diferentes preferencias, puede crear un proyecto sin plantilla si su grupo de inicio tiene esta preferencia habilitada.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Establecer estado de nuevo proyecto en]</td> 
   <td> <p>Determine el estado de los nuevos proyectos.</p>  <p><b>NOTA</b>  
     <ul> 
      <li>Si usted u otro [!DNL Workfront] El administrador oculta el estado seleccionado aquí. El estado predeterminado cambia al primer estado de la lista de estados.</li> 
     </ul> 
     <ul> 
      <li> <p>Si un sistema bloqueado o un estado de grupo está establecido como estado predeterminado y más tarde alguien lo desbloquea, el sistema intenta reemplazarlo con un estado bloqueado del mismo tipo de estado.</p> <p>Si no encuentra ninguna, busca un estado requerido:</p> 
       <ul> 
        <li>Si hay un estado obligatorio que equivale al estado predeterminado desbloqueado, el estado requerido se convierte en el estado predeterminado, incluso si está desbloqueado.</li> 
        <li>Si ninguno de los estados requeridos equivale al estado predeterminado desbloqueado, el primer estado requerido de la lista de estados se convierte en el estado predeterminado.</li> 
       </ul> <p>Para obtener información sobre los estados obligatorios, consulte los artículos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de proyectos del sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de tareas del sistema</a>, y <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de problemas del sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calcular porcentaje completado en función de]</td> 
   <td> <p>El porcentaje completado de un proyecto o tarea principal se basa en el progreso general de las tareas. Esta información se puede calcular en función de la duración o las horas planificadas de las tareas de un proyecto.</p> <p>Si selecciona [!UICONTROL Duración], la Duración de cada tarea de un proyecto determina el porcentaje completado global del proyecto y la Duración de cada subtarea determina el porcentaje completado global de su tarea principal.</p> <p>Si selecciona [!UICONTROL Duración], asegúrese de especificar las [!UICONTROL Horas habituales por día laborable] y [!UICONTROL Días laborables habituales por semana] en la sección [!UICONTROL Líneas de tiempo]. [!DNL Workfront] utiliza esta información al calcular el porcentaje completado de una tarea según la duración. </p> <p>Si selecciona [!UICONTROL Horas planificadas], asegúrese de que todas las tareas de cada proyecto tengan definida la cantidad de [!UICONTROL Horas planificadas] y de que la cantidad no sea cero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Establecer automáticamente la condición del proyecto según el estado de progreso]</td> 
   <td> <p>Esta preferencia permite a los usuarios establecer manualmente la [!UICONTROL Condición] de un proyecto en ([!UICONTROL En el destino], [!UICONTROL En riesgo], [!UICONTROL En problemas]) o tener [!DNL Workfront] establezca la condición [!UICONTROL] (estado de progreso) automáticamente según la progresión del proyecto en la cronología. Para obtener más información sobre la condición de los proyectos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Descripción general de la condición y el tipo de condición del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Crear líneas base automáticamente]</p> </td> 
   <td> <p>Esta preferencia crea automáticamente una línea de base (instantánea) de los detalles de tareas y proyectos cuando el estado del proyecto cambia a [!UICONTROL Actual]. Para obtener información sobre la creación de líneas base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Crear líneas base del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método de índice de rendimiento] </p> </td> 
   <td> <p>El Método del índice de rendimiento (PIM) para el proyecto controla el método [!DNL Workfront] utiliza para calcular métricas de valor ganado como [!UICONTROL Índice de rendimiento de costos] (CPI) y [!UICONTROL Estimar al finalizar] (EAC). Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular [!UICONTROL Índice de rendimiento de costos] (CPI)</a> y <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calcular estimación al finalizar] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Basado en horas]</strong>: [!DNL Workfront] utiliza [!UICONTROL Horas planificadas] para calcular métricas de rendimiento como EAC y CPI. Cuando el PIM se calcula en función de las horas, el EAC se muestra como un número de horas. Asegúrese de que tiene un valor distinto de cero para [!UICONTROL Horas planificadas].</li> 
     <li> <p><strong>[!UICONTROL Basado en costos]</strong>: [!DNL Workfront] utiliza [!UICONTROL Costo de mano de obra planificado] para calcular métricas de rendimiento como EAC y CPI. Asegúrese de que los puestos de trabajo o los usuarios estén asociados a las tarifas de coste por hora. Cuando el PIM se calcula en función de los costes, el EAC se muestra como un valor de moneda.</p> <p>El jefe de proyecto puede modificar esta configuración en el nivel de proyecto mediante el área de [!UICONTROL Finance] en Detalles del proyecto de [!UICONTROL]. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área de [!UICONTROL Finance] del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimar al finalizar ]</p> </td> 
   <td> <p>Determinar qué datos [!DNL Workfront] utiliza para calcular el [!UICONTROL Estimar al finalizar] (EAC) que representa el costo total proyectado de un proyecto.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcular en el nivel de proyecto]</strong>: EAC para la tarea y el proyecto principales se determinan introduciendo [!UICONTROL Horas reales] o [!UICONTROL Coste laboral real] en las fórmulas EAC. Este cálculo incluye [!UICONTROL Horas reales] o [!UICONTROL Costos y gastos] agregados directamente a la tarea o proyecto principal.</li> 
     <li> <p><strong>[!UICONTROL Resumir a partir de tareas/subtareas]</strong>: EAC para la tarea principal y el proyecto se determinan sumando el EAC para cada tarea secundaria. Este cálculo excluye las [!UICONTROL Horas reales] o los [!UICONTROL Costos y gastos reales] que se hayan agregado directamente a la tarea o proyecto principal.</p> <p>El jefe de proyecto puede modificar esta configuración en el nivel de proyecto mediante el área de [!UICONTROL Finance] en Detalles del proyecto de [!UICONTROL].Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área de [!UICONTROL Finance] del proyecto</a>.</p> </li> 
    </ul> <p>Para obtener más información sobre cómo calcula el EAC, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular [!UICONTROL Estimación al finalizar] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Escalas de tiempo {#timelines}

Configure cualquiera de las siguientes preferencias para proyectos recién creados en todo el sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Programación de [!UICONTROL desde]</td> 
   <td> <p>Determine si los nuevos proyectos se programan desde la fecha de inicio o desde la fecha de finalización cuando se crean.</p> 
    <ul> 
     <li><strong>[!UICONTROL Fecha de inicio]</strong>: las nuevas tareas tienen como valor predeterminado la restricción de tarea de [!UICONTROL Lo antes posible] y se pide a los jefes de proyecto que proporcionen una fecha planificada de inicio de [!UICONTROL] para el proyecto.</li> 
     <li><strong>[!UICONTROL Fecha de finalización]</strong>: las nuevas tareas tienen como valor predeterminado la restricción de tarea de [!UICONTROL Lo más tarde posible] y se pide a los jefes de proyecto que proporcionen una fecha planificada de finalización de [!UICONTROL] para el proyecto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tiempo libre del usuario]</td> 
   <td> <p>Determine si el tiempo libre de la persona asignada principal de una tarea ajusta las fechas planificadas para esa tarea en un proyecto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Considere el tiempo libre del usuario en las duraciones de las tareas]</strong>: Cualquier tiempo libre programado para la persona asignada principal de una tarea ajusta las fechas planificadas de la tarea si el tiempo libre se produce durante la duración de la tarea. Esta es la configuración predeterminada. </p> <p>Por ejemplo, si una tarea con una restricción de [!UICONTROL As Soon As Possible] está programada para comenzar el 1 de junio y finalizar el 3 de junio, y la persona asignada principal tiene marcado el 2 de junio como Tiempo de espera, las fechas planificadas de la tarea se ajustarán del 1 de junio al 4 de junio.</p> <p><b>IMPORTANTE</b>:</p> <p>La duración de la tarea no cambia al seleccionar esta configuración. Solo cambian las fechas planificadas, dependiendo de la Restricción de tarea.</p> </li> 
     <li><strong>[!UICONTROL Omitir tiempo libre del usuario en duraciones de tareas]</strong>: las fechas planificadas de cada tarea en un proyecto permanecen tal como se planificó originalmente, incluso si la persona asignada principal de una tarea tiene tiempo libre durante su duración.</li> 
    </ul> <p>Tenga en cuenta lo siguiente al seleccionar opciones para esta configuración:</p> 
    <ul> 
     <li>Al cambiar esta configuración, solo los proyectos y las plantillas creados después del cambio heredan la configuración actualizada. </li> 
     <li> <p>El valor Restricción de tarea de la tarea determina qué fechas de tareas planificadas se deben ajustar: </p> 
      <ul> 
       <li>Fecha planificada de inicio</li> 
       <li>Fecha planificada de finalización</li> 
       <li>Ambas fechas</li> 
       <li>Ninguna cita. </li> 
      </ul> <p>Por ejemplo, si una tarea tiene una restricción de [!UICONTROL Fechas fijas], las fechas no se ajustan cuando el usuario asignado principal tiene tiempo libre, aunque la opción [!UICONTROL Considerar el tiempo libre del usuario en la duración de la tarea] esté seleccionada. Para obtener información sobre las delimitaciones de tareas, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Información general sobre restricciones de tarea</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Las escalas de tiempo del proyecto se vuelven a calcular automáticamente]</p> </td> 
   <td> <p>Determine cuándo se vuelve a calcular la escala de tiempo de un proyecto. Para obtener información sobre cómo recalcular la escala de tiempo del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular escalas de tiempo del proyecto</a>.</p> <p>Las siguientes opciones están habilitadas de forma predeterminada. Puede seleccionar una o varias de las siguientes opciones de configuración:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Todas las noches]</strong>: seleccione esta opción para recalcular las escalas de tiempo de los proyectos cada noche. Los cambios que realice en el proyecto y que puedan afectar a la escala de tiempo no serán visibles de inmediato. [!DNL Workfront​​​] recalcula las escalas de tiempo por la noche solo para proyectos donde se cumplen las dos condiciones siguientes:</p> <p> 
       <ul> 
        <li>Tener un estado de [!UICONTROL Actual]</li> 
        <li>Ha tenido una actualización en los últimos 3 meses</li> 
        <li>Ha tenido un tipo de actualización de uno de los siguientes:</li>
        <ul>
        <li>Automático y al cambiar</li>
        <li>Solo al cambiar</li>
        <li>Solo automático</li> 
      </ul>       
    <b>SUGERENCIA:</b>
    <p>Los proyectos que tienen un tipo de actualización de solo manual no se ven afectados por esta configuración.</p>
    <li> <p><strong>Cuando cambie el ámbito de un proyecto</strong>: seleccione esta opción para recalcular las escalas de tiempo del proyecto inmediatamente cuando se produzca un cambio en el ámbito del proyecto. Para obtener información sobre lo que constituye un cambio en el ámbito del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular escalas de tiempo del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cuando se asignan varios usuarios a una tarea, utilice la programación de]</p> </td> 
   <td> <p>Si un proyecto no tiene asignada una programación o si los usuarios asignados a sus tareas no tienen asignada una programación, [!DNL Workfront] utiliza la programación predeterminada del sistema para calcular la escala de tiempo de las tareas.</p> <p>Si asigna varios usuarios a la misma tarea en un proyecto y el proyecto tiene una programación asignada y los usuarios asignados a las tareas también tienen una programación asignada, [!UICONTROL Workfront] utiliza las siguientes programaciones:</p> 
    <ul> 
     <li><strong>[!UICONTROL Asignación principal]</strong>: [!DNL Workfront] utiliza la programación de la asignación principal de la tarea para calcular las escalas de tiempo.</li> 
     <li><strong>[!UICONTROL Proyecto]</strong>: [!DNL Workfront] utiliza la programación del proyecto para calcular la escala de tiempo de cada tarea.</li> 
    </ul> <p>Para obtener más información sobre las programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Creación de una programación</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Cálculos de escala de tiempo] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Horas habituales por día laborable]</strong>: establezca el número de horas en un día de trabajo típico para los usuarios que trabajarán en proyectos. El valor predeterminado es de 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Días laborables habituales por semana]</strong>: establezca la semana laboral estándar para los usuarios que trabajan en proyectos. El valor predeterminado es 5 días.</li> 
    </ul> <p>Estas dos opciones convierten los días en horas o las semanas en días.</p> <p>Por ejemplo, si tiene una tarea con 8 horas planificadas y la duración se calcula según las horas planificadas, [!DNL Workfront] convierte esas horas en días para mostrar la Duración como días.</p> <p>En el campo Típico de [!UICONTROL días laborables por semana], [!DNL Workfront] calcula el valor de Equivalente a tiempo completo (FTE) para su sistema. Esto es lo que [!DNL Workfront] se utiliza al calcular las asignaciones para los usuarios.</p> <p>Estos valores se utilizan cuando se planifican las escalas de tiempo de los proyectos, se presupuestan los recursos o se registra el tiempo en los proyectos. </p> <p>No se utilizan para establecer plantillas de horas para los usuarios del sistema, como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Hoja de horas y preferencias de horas de [!UICONTROL Configure]</a>.</p> <p><b>NOTA</b>:</p> <p>[!DNL Workfront] los administradores no pueden desbloquear las preferencias de [!UICONTROL Cálculos de escala de tiempo].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestres personalizados]</p> </td> 
   <td> <p>Configure trimestres anuales personalizados para los usuarios que trabajarán en proyectos. Los trimestres personalizados suelen ser trimestres que no coinciden con el desglose tradicional de trimestres durante un año natural. Puede agregar varios trimestres personalizados. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados para proyectos</a>.</p>  <p><b>NOTA</b>: </p><p>[!DNL Workfront] los administradores no pueden desbloquear las preferencias de [!UICONTROL Trimestres personalizados].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Casos comerciales] {#business-cases}

Puede crear un caso empresarial para los proyectos recién creados en todo el sistema para enviar solicitudes de proyectos. Puede definir las preferencias para determinar qué áreas son visibles en la **[!UICONTROL Caso comercial]** formulario. Le recomendamos que habilite estas opciones para que otras herramientas, como [!UICONTROL Portfolio Optimizer], actualice correctamente. Para obtener más información sobre lo que muestra cada campo, consulte [Definir un caso comercial: índice de artículos](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Después del [!DNL Workfront] El administrador de habilita las secciones de [!UICONTROL Caso comercial], un Propietario del proyecto puede crear un caso empresarial en el nivel de proyecto. Para obtener información sobre la creación de un caso empresarial, consulte [Crear un caso comercial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Vida después de la muerte] {#life-after-death}

Configure cualquiera de las siguientes preferencias para proyectos recién creados en todo el sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Después de que un proyecto se haya marcado como Completo, los usuarios aún pueden] </p> </td> 
   <td> <p>Determine las reglas de su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a si una tarea o un problema se puede eliminar después de que el estado del proyecto se haya marcado como [!UICONTROL Completado].</p> 
    <ul> 
     <li><strong>[!UICONTROL Eliminar tareas]</strong>: permite a los usuarios eliminar tareas de un proyecto después de que el proyecto se haya marcado como [!UICONTROL completado].<br></li> 
     <li><strong>[!UICONTROL Eliminar problemas]</strong>: permite a los usuarios eliminar problemas de un proyecto después de que el proyecto se haya marcado como [!UICONTROL completado].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Después de que un proyecto se marque como Completo, como Inactivo o tiene Aprobación pendiente, los usuarios aún pueden]</p> </td> 
   <td> <p>Determine las reglas de su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a lo que sucede con las tareas, problemas, documentos y otros objetos de un proyecto una vez marcado su estado <strong>[!UICONTROL Completo]</strong>, <strong>[!UICONTROL Inactivo]</strong>, o es <strong>[!UICONTROL Pendiente de aprobación]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Agregar y editar tareas]</strong> Permite a los usuarios:
      <ul>
       <li>Editar tareas dentro de un proyecto después de que el proyecto se haya marcado como [!UICONTROL completo], [!UICONTROL muerto] o tenga [!UICONTROL pendiente de aprobación]. Esto incluye agregar horas y cambiar entradas de gastos en una tarea.</li>
       <li>Agregar tareas a un proyecto.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Agregar y editar problemas]</strong>: permite a los usuarios:
      <ul>
       <li>Editar problemas dentro de un proyecto después de que el proyecto se haya marcado como [!UICONTROL completo], [!UICONTROL inactivo] o [!UICONTROL pendiente de aprobación].</li>
       <li>Agregue problemas a un proyecto después de que el proyecto se haya marcado como [!UICONTROL completo] o [!UICONTROL muerto]. (No se pueden agregar problemas a un proyecto que tenga [!UICONTROL Pendiente de aprobación].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Agregar documentos al proyecto y a sus tareas y problemas]</strong>: permite a los usuarios agregar documentos a un proyecto (o agregar documentos a tareas y problemas del proyecto) después de que el proyecto se haya marcado como [!UICONTROL completado] o [!UICONTROL muerto].</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
     <li> <p><strong>[!UICONTROL Adjuntar plantillas]</strong>: permite a los usuarios adjuntar plantillas a un proyecto después de que el proyecto se haya marcado como [!UICONTROL completo] o [!UICONTROL muerto].</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
