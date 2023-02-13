---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar las preferencias de proyecto de todo el sistema
description: Como [!DNL Adobe Workfront] administrador, puede configurar las preferencias predeterminadas para todos los proyectos creados en todo el sistema. Estas preferencias afectan al comportamiento del proyecto, la tarea y el problema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2475'
ht-degree: 1%

---

# Configurar las preferencias de proyecto de todo el sistema

Como [!DNL Adobe Workfront] administrador, puede configurar las preferencias predeterminadas para todos los proyectos creados en todo el sistema. Estas preferencias afectan al comportamiento del proyecto, la tarea y el problema.

>[!NOTE]
>
>De forma predeterminada, estas preferencias están bloqueadas y los administradores de grupos no pueden modificarlas a nivel de grupo a menos que las desbloquee para todos los grupos del sistema. Para obtener más información, consulte [Bloquear o desbloquear las preferencias del proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

## Configurar las preferencias del proyecto para toda la organización

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Proyectos]**.

1. En la página que aparece, continúe con una de las 4 secciones enumeradas a continuación para configurar las preferencias de [!UICONTROL Estado del proyecto], [!UICONTROL Líneas de tiempo], [!UICONTROL Casos de uso]y [!UICONTROL La vida después de la muerte].
1. Si desea que todos los grupos de la organización utilicen las mismas preferencias de proyecto, asegúrese de que cada preferencia esté bloqueada ![](assets/lock-toggle-button.png) (este es el valor predeterminado).

   >[!IMPORTANT]
   >
   >Cuando una preferencia de proyecto está bloqueada, todos los grupos del sistema heredan cualquier cambio que realice en esa preferencia. Es importante comunicarse con los usuarios y grupos de toda la organización para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura las preferencias del proyecto.

   Para obtener información sobre cómo desbloquear una preferencia para que todos los grupos puedan configurarla y administrarla por su cuenta, consulte [Bloquear o desbloquear las preferencias del proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Haga clic en **[!UICONTROL Guardar]**.

* [[!UICONTROL Estado del proyecto]](#project-status)
* [[!UICONTROL Escalas de tiempo]](#timelines)
* [[!UICONTROL Casos comerciales]](#business-cases)
* [[!UICONTROL Vida después de la muerte]](#life-after-death)

### Estado del proyecto {#project-status}

Configure cualquiera de las siguientes preferencias para los proyectos recién creados en todo el sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permitir que los usuarios creen proyectos sin usar una plantilla]</td> 
   <td>  <p>Esta preferencia permite a los usuarios crear proyectos sin usar una plantilla al crear un proyecto desde las siguientes áreas: </p>
      <ul>
        <li>
        <p>Utilizar la opción [!UICONTROL Nuevo proyecto] en una lista de proyectos</p>
        </li>
          <li>
          <p>Convertir un problema en un proyecto desde la página del problema</p>
          </li>
         </ul>
        <p>Esta preferencia está habilitada de forma predeterminada. </p> 
        <p><b>NOTA</b></p>
        <p> Un administrador de grupo puede cambiar esta preferencia por un grupo. Cuando un usuario pertenece a varios grupos con preferencias diferentes, se le permitirá crear un proyecto sin plantilla si su grupo de inicio tiene esta preferencia habilitada.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Definir estado del nuevo proyecto como]</td> 
   <td> <p>Determine el estado de los nuevos proyectos.</p>  <p><b>NOTA</b>  
     <ul> 
      <li>Si usted u otro [!DNL Workfront] oculta el estado seleccionado aquí, el estado predeterminado cambia al primer estado de la lista de estado.</li> 
     </ul> 
     <ul> 
      <li> <p>Si un sistema bloqueado o un estado de grupo se establece como estado predeterminado y más tarde alguien lo desbloquea, el sistema intenta reemplazarlo por un estado bloqueado del mismo tipo de estado.</p> <p>Si no encuentra una, busca un estado obligatorio:</p> 
       <ul> 
        <li>Si hay un estado requerido que equivale al estado predeterminado desbloqueado, el estado requerido se convierte en el estado predeterminado, aunque esté desbloqueado.</li> 
        <li>Si ninguno de los estados requeridos equivale al estado predeterminado desbloqueado, el primer estado requerido en la lista de estado se convierte en el estado predeterminado.</li> 
       </ul> <p>Para obtener información sobre los estados necesarios, consulte los artículos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de proyectos del sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceso a la lista de estados de tareas del sistema</a>y <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceda a la lista de estados de problemas del sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calcular porcentaje completado basado en]</td> 
   <td> <p>El porcentaje completado de un proyecto o tarea principal se basa en el progreso general de las tareas. Esta información se puede calcular en función de la duración o del horario planificado de las tareas de un proyecto.</p> <p>Si selecciona [!UICONTROL Duration], la duración de cada tarea de un proyecto determina el porcentaje total completado del proyecto y la duración de cada subtarea determina el porcentaje total completado de la tarea principal.</p> <p>Si selecciona [!UICONTROL Duración], asegúrese de especificar [!UICONTROL Horario típico por día laboral] y [!UICONTROL Días laborables típicos por semana] en la sección [!UICONTROL Cronologías]. [!DNL Workfront] utiliza esta información para calcular el porcentaje completado de una tarea en función de la duración. </p> <p>Si selecciona [!UICONTROL Horario planificado], asegúrese de que todas las tareas de cada proyecto tengan definida la cantidad de [!UICONTROL Horario planificado] y que la cantidad no sea cero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Establezca automáticamente la condición del proyecto en función del estado de progreso]</td> 
   <td> <p>Esta preferencia permite a los usuarios establecer manualmente la [!UICONTROL Condition] de un proyecto ([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble]) o que tengan [!DNL Workfront] establezca la [!UICONTROL Condition] (Progress Status) automáticamente en función de la progresión del proyecto en la cronología. Para obtener más información sobre la condición de los proyectos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Descripción general de la condición y el tipo de condición del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Crear líneas de base automáticamente]</p> </td> 
   <td> <p>Esta preferencia crea automáticamente una línea de base (instantánea) de los detalles de la tarea y del proyecto cuando el estado del proyecto cambia a [!UICONTROL Actual]. Para obtener información sobre la creación de líneas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Crear líneas de base del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>El método de índice de rendimiento (PIM) del proyecto controla el método [!DNL Workfront] utiliza para calcular métricas de valores ganados como [!UICONTROL Cost Performance Index] (CPI) y [!UICONTROL Estimate At Completion] (EAC). Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular [!UICONTROL Cost Performance Index] (CPI)</a> y <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calcular Estimación Al Finalizar] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL basado en horas]</strong>: [!DNL Workfront] utiliza [!UICONTROL Horario planificado] para calcular métricas de rendimiento como EAC y CPI. Cuando el PIM se calcula en función de las horas, el EAC se muestra como un número de horas. Asegúrese de que tiene un valor para [!UICONTROL Horario planificado] distinto de cero.</li> 
     <li> <p><strong>[!UICONTROL Basado en los costes]</strong>: [!DNL Workfront] utiliza [!UICONTROL Costo laboral planeado] para calcular métricas de rendimiento como EAC y CPI. Asegúrese de que las funciones de su trabajo o los usuarios estén asociados con las tasas de costo por hora. Cuando el PIM se calcula en función de los costes, el EAC se muestra como un valor de moneda.</p> <p>El administrador de proyectos puede modificar esta configuración a nivel de proyecto mediante el área [!UICONTROL Finance] en [!UICONTROL Detalles del proyecto]. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área [!UICONTROL Finance] del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimación al finalizar ]</p> </td> 
   <td> <p>Determinar qué datos [!DNL Workfront] utiliza para calcular la [!UICONTROL Estimate at Completion] (EAC) que representa el coste total proyectado de un proyecto.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcular a nivel de proyecto]</strong>:EAC para la tarea principal y el proyecto se determinan introduciendo [!UICONTROL Real Hours] o [!UICONTROL Real Labor Cost] en las Fórmulas EAC. Este cálculo incluye [!UICONTROL Real Hours] o [!UICONTROL Costs and Expenses] añadidos directamente a la tarea o proyecto principal.</li> 
     <li> <p><strong>[!UICONTROL Resumen de tareas/subtareas]</strong>: Las CAO para la tarea principal y el proyecto se determinan sumando la CAO para cada tarea secundaria. Este cálculo excluye [!UICONTROL Real Hours] o [!UICONTROL Real Costs and Expenses] añadidos directamente a la tarea o proyecto principal.</p> <p>El administrador de proyectos puede modificar esta configuración a nivel de proyecto mediante el área [!UICONTROL Finance] de [!UICONTROL Detalles del proyecto]. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área [!UICONTROL Finance] del proyecto</a>.</p> </li> 
    </ul> <p>Para obtener más información sobre cómo se calcula la CAO, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular [!UICONTROL Estimación Al Finalizar] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Escalas de tiempo {#timelines}

Configure cualquiera de las siguientes preferencias para los proyectos recién creados en todo el sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Programar desde]</td> 
   <td> <p>Determine si los nuevos proyectos están programados desde la fecha de inicio o desde la fecha de finalización cuando se crean.</p> 
    <ul> 
     <li><strong>[!UICONTROL Fecha de inicio]</strong>: Las nuevas tareas predeterminadas de la restricción de tareas [!UICONTROL lo antes posible] y los administradores de proyectos deben proporcionar un [!UICONTROL Fecha de inicio planeada] para el proyecto.</li> 
     <li><strong>[!UICONTROL Fecha de finalización]</strong>: Las nuevas tareas se configuran de forma predeterminada en [!UICONTROL As Late As Late possible] Task Constraint y se solicita a los administradores de proyectos que proporcionen un [!UICONTROL Planned Completion Date] para el proyecto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tiempo de espera del usuario desactivado]</td> 
   <td> <p>Determine si el tiempo de espera del Asignado principal de una tarea ajusta las fechas planificadas para esa tarea en un proyecto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Considere el tiempo de espera del usuario en las duraciones de las tareas]</strong>: Cualquier tiempo libre programado para el Asignado Principal de una tarea ajusta las fechas planificadas de la tarea si el tiempo de espera se produce durante la duración de la tarea. Esta es la configuración predeterminada. </p> <p>Por ejemplo, si una tarea con una restricción de [!UICONTROL lo antes posible] está programada para empezar el 1 de junio y para completarse el 3 de junio, y el usuario asignado principal tiene marcado el 2 de junio como Tiempo de espera, las fechas programadas para la tarea se ajustan al 1 de junio al 4 de junio.</p> <p><b>IMPORTANTE</b>: La duración de la tarea no cambia al seleccionar esta configuración. Solo cambian las fechas planificadas, dependiendo de la restricción de tareas.</p> </li> 
     <li><strong>[!UICONTROL Ignorar el tiempo de espera del usuario en duraciones de tareas]</strong>: Las fechas previstas de cada tarea en un proyecto permanecen como estaba planeado originalmente, incluso si el Asignado Principal de una tarea tiene tiempo libre durante su duración.</li> 
    </ul> <p>Tenga en cuenta lo siguiente al seleccionar opciones para esta configuración:</p> 
    <ul> 
     <li>Cuando cambia esta configuración, solo los proyectos y las plantillas creados después del cambio heredan la configuración actualizada. </li> 
     <li> <p>El valor Restricción de tareas de la tarea determina qué fechas de tareas planificadas se deben ajustar: </p> 
      <ul> 
       <li>Fecha planificada de inicio</li> 
       <li>Fecha planificada de finalización</li> 
       <li>Ambas fechas</li> 
       <li>Ninguna fecha. </li> 
      </ul> <p>Por ejemplo, si una tarea tiene una restricción de [!UICONTROL Fechas fijas], las fechas no se ajustan cuando el usuario asignado principal tiene tiempo de espera, aunque la opción [!UICONTROL Considere el tiempo de espera del usuario en la duración de la tarea] esté seleccionada. Para obtener información sobre las restricciones de tareas, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Información general sobre la restricción de tareas</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Los plazos del proyecto se vuelven a calcular automáticamente]</p> </td> 
   <td> <p>Determine cuándo se vuelve a calcular la escala de tiempo de un proyecto. Para obtener información sobre cómo volver a calcular la cronología del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Volver a calcular las líneas de tiempo del proyecto</a>.</p> <p>Las siguientes opciones están habilitadas de forma predeterminada. Puede seleccionar una o varias de las siguientes opciones:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Cada noche]</strong>: Seleccione esta opción para volver a calcular las líneas de tiempo del proyecto cada noche. Los cambios que realice en el proyecto que puedan afectar a la cronología no serán visibles inmediatamente. [!DNL Workfront​​​] vuelve a calcular las líneas de tiempo por la noche solo para proyectos en los que se cumplen las dos condiciones siguientes:</p> <p> 
       <ul> 
        <li>Tener un estado de [!UICONTROL Current]</li> 
        <li>Han tenido una actualización en los últimos 3 meses</li> 
       </ul> </p> </li> 
     <li> <p><strong>Cuando cambia el ámbito de un proyecto</strong>: Seleccione esta opción para volver a calcular las líneas de tiempo del proyecto inmediatamente cuando se produzca un cambio en el ámbito del proyecto. Para obtener información sobre lo que constituye un cambio en el ámbito de un proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Volver a calcular las líneas de tiempo del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cuando se asignan varios usuarios a una tarea, utilice la programación del]</p> </td> 
   <td> <p>Si un proyecto no tiene una programación asignada o si los usuarios asignados a sus tareas no tienen una programación asignada, [!DNL Workfront] utiliza la programación predeterminada del sistema para calcular la cronología de las tareas.</p> <p>Si asigna varios usuarios a la misma tarea en un proyecto tiene una programación asignada (y los usuarios asignados a las tareas también tienen una programación asignada),[!UICONTROL Workfront] utiliza las siguientes programaciones:</p> 
    <ul> 
     <li><strong>[!UICONTROL Asignación primaria]</strong>: [!DNL Workfront] utiliza la programación de la asignación principal en la tarea para calcular las líneas de tiempo.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] utiliza la programación del proyecto para calcular la cronología de cada tarea.</li> 
    </ul> <p>Para obtener más información sobre las programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Crear una programación</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Cálculos de línea de tiempo] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Horas habituales por día laboral]</strong>: Establezca el número de horas en una jornada laboral normal para los usuarios que están trabajando en proyectos. El valor predeterminado es de 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Días laborables típicos por semana]</strong>: Establezca la semana laboral estándar para los usuarios que trabajarán en proyectos. El valor predeterminado es de 5 días.</li> 
    </ul> <p>Estas dos opciones convierten días en horas o semanas en días.</p> <p>Por ejemplo, si tiene una tarea con 8 horas planificadas y la duración se calcula en función de las horas planificadas, [!DNL Workfront] convierte esas horas en días para mostrar la duración como días.</p> <p>Desde el campo Típico [!UICONTROL días laborables por semana], [!DNL Workfront] calcula el valor de Equivalente de tiempo completo (FTE) para su sistema. Esto es lo que [!DNL Workfront] utiliza para calcular asignaciones para usuarios.</p> <p>Estos valores se utilizan cuando se planifica la cronología de los proyectos, se presupuestan los recursos o se registra el tiempo de los proyectos. </p> <p>No se utilizan cuando se establecen partes de horas para los usuarios del sistema, tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Preferencias de horas y horas de [!UICONTROL Configurar]</a>.</p> <p><b>NOTA</b>: [!DNL Workfront] los administradores de no pueden desbloquear las preferencias de [!UICONTROL Cronología calculada].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestre personalizado]</p> </td> 
   <td> <p>Configure trimestres anuales personalizados para los usuarios que trabajarán en proyectos. Los trimestres personalizados suelen ser trimestres que no coinciden con el desglose tradicional de trimestres durante un año natural. Puede agregar varios trimestres personalizados. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados para proyectos</a>.</p>  <p><b>NOTA</b>: [!DNL Workfront] los administradores no pueden desbloquear las preferencias de [!UICONTROL Barrios personalizados].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Casos comerciales] {#business-cases}

Puede crear un caso empresarial para los proyectos recién creados en todo el sistema para enviar solicitudes de proyecto. Puede definir preferencias para determinar qué áreas son visibles en la variable **[!UICONTROL Caso empresarial]** formulario. Le recomendamos que habilite estas opciones para que otras herramientas, como el [!UICONTROL Optimizador de Portfolio], actualice correctamente. Para obtener más información sobre qué muestra cada campo, consulte [Definir un caso empresarial](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Después de la [!DNL Workfront] el administrador habilita las secciones en la variable [!UICONTROL Caso empresarial], un propietario de proyecto puede crear un caso empresarial a nivel de proyecto. Para obtener información sobre cómo crear un caso práctico, consulte [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Vida después de la muerte] {#life-after-death}

Configure cualquiera de las siguientes preferencias para proyectos recién creados en todo el sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Una vez que un proyecto se ha marcado como Completo, las personas aún pueden hacerlo] </p> </td> 
   <td> <p>Determine las reglas para su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a si una tarea o un problema se pueden eliminar después de marcar el estado del proyecto como [!UICONTROL Complete].</p> 
    <ul> 
     <li><strong>[!UICONTROL Eliminar tareas]</strong>: Permite a los usuarios eliminar tareas de un proyecto después de que el proyecto se haya marcado como [!UICONTROL Complete].<br></li> 
     <li><strong>[!UICONTROL Eliminar problemas]</strong>: Permite a los usuarios eliminar problemas de un proyecto después de que el proyecto se haya marcado como [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Una vez que un proyecto está marcado como Completado, Muerto o Pendiente de aprobación, las personas aún pueden hacerlo]</p> </td> 
   <td> <p>Determine las reglas para la organización (o el grupo, si configura las preferencias de proyecto para un grupo) con respecto a lo que sucede con las tareas, los problemas, los documentos y otros objetos de un proyecto una vez que se ha marcado el estado del proyecto <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL muerto]</strong>o es <strong>[!UICONTROL Pendiente de aprobación]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Agregar y editar tareas]</strong> Permite a los usuarios:
      <ul>
       <li>Edite tareas dentro de un proyecto después de que el proyecto haya sido marcado como [!UICONTROL Complete], [!UICONTROL Dead] o sea [!UICONTROL Pending Approval]. Esto incluye agregar horas y cambiar entradas de gastos en una tarea.</li>
       <li>Agregue tareas a un proyecto.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Agregar y editar problemas]</strong>: Permite a los usuarios:
      <ul>
       <li>Edite los problemas dentro de un proyecto después de que el proyecto haya sido marcado como [!UICONTROL Complete], [!UICONTROL Dead] o [!UICONTROL Pending Approval].</li>
       <li>Agregue problemas a un proyecto después de que el proyecto esté marcado como [!UICONTROL Complete] o [!UICONTROL Dead]. (No se pueden agregar problemas a un proyecto que sea [!UICONTROL Pendiente de aprobación]).</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Agregar documentos al proyecto y a sus tareas y problemas]</strong>: Permite a los usuarios agregar documentos a un proyecto (o agregar documentos a tareas y problemas dentro del proyecto) después de que el proyecto haya sido marcado como [!UICONTROL Complete] o [!UICONTROL Dead].</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
     <li> <p><strong>[!UICONTROL Adjuntar plantillas]</strong>: Permite a los usuarios adjuntar plantillas a un proyecto después de que el proyecto haya sido marcado como [!UICONTROL Complete] o [!UICONTROL Dead].</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
