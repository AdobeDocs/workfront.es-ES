---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar las preferencias de proyecto de todo el sistema
description: Como administrador de  [!DNL Adobe Workfront] , puede configurar las preferencias predeterminadas para todos los proyectos creados en el sistema. Estas preferencias afectan al comportamiento del proyecto, la tarea y el problema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '2670'
ht-degree: 93%

---

# Configurar las preferencias de proyecto de todo el sistema

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Como administrador de [!DNL Adobe Workfront], puede configurar las preferencias predeterminadas para todos los proyectos creados en el sistema. Estas preferencias afectan al comportamiento del proyecto, la tarea y el problema.

>[!NOTE]
>
>De forma predeterminada, estas preferencias están bloqueadas y los administradores de grupos no pueden modificarlas en el nivel de grupo a menos que las desbloquee para todos los grupos del sistema. Para obtener más información, consulte [Bloquear o desbloquear las preferencias de proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar las preferencias del proyecto para toda la organización

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Proyectos]**.

1. En la página **Preferencias del proyecto**, continúe con una de las cuatro secciones que se enumeran a continuación para configurar las preferencias de [!UICONTROL Estado del proyecto], [!UICONTROL Cronologías], [!UICONTROL Casos empresariales] y [!UICONTROL Vida después de la muerte].
1. Si desea que todos los grupos de la organización usen las mismas preferencias de proyecto, asegúrese de que cada preferencia esté bloqueada ![Bloquear alternancia](assets/lock-toggle-button.png) (este es el valor predeterminado).

   >[!IMPORTANT]
   >
   >Cuando una preferencia de proyecto está bloqueada, todos los grupos del sistema heredan los cambios que realice en dicha preferencia. Es importante comunicarse con los usuarios y grupos de toda la organización para asegurarse de que se tienen en cuenta todas las necesidades a la hora de configurar las preferencias del proyecto.

   Para obtener información sobre cómo desbloquear una preferencia para que todos los grupos puedan configurarla y administrarla por su cuenta, consulte [Bloquear o desbloquear las preferencias de proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Haga clic en **[!UICONTROL Guardar]**.

* [[!UICONTROL Project Status]](#project-status)
* [[!UICONTROL Timelines]](#timelines)
* [[!UICONTROL Business Cases]](#business-cases)
* [[!UICONTROL Life After Death]](#life-after-death)

### Estado del proyecto {#project-status}

Configure cualquiera de las siguientes preferencias para proyectos recién creados en todo el sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Allow users to create projects without using a template]</td> 
   <td>  <p>Esta preferencia permite a los usuarios crear proyectos sin usar plantillas al crear proyectos de las siguientes áreas: </p>
      <ul>
        <li>
        <p>Utilizar la opción [!UICONTROL New Project] en una lista de proyectos</p>
        </li>
          <li>
          <p>Convertir un problema en un proyecto desde la página del problema</p>
          </li>
         </ul>
        <p>Esta preferencia está habilitada de forma predeterminada. </p> 
        <p><b>NOTA</b></p>
        <p> Un administrador de grupos puede cambiar esta preferencia para un grupo. Cuando un usuario pertenece a varios grupos con diferentes preferencias, puede crear un proyecto sin plantilla si su grupo de inicio tiene esta preferencia habilitada.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Set new project's status to]</td> 
   <td> <p>Determinar el estado de los nuevos proyectos.</p>  <p><b>NOTA</b>  
     <ul> 
      <li>Si usted u otro administrador de [!DNL Workfront] oculta el estado seleccionado aquí, el estado predeterminado cambia al primer estado de la lista de estados.</li> 
     </ul> 
     <ul> 
      <li> <p>Si un sistema bloqueado o un estado de grupo está establecido como estado predeterminado y más tarde alguien lo desbloquea, el sistema intenta reemplazarlo por un estado bloqueado del mismo tipo de estado.</p> <p>Si no encuentra ninguno, busca un estado obligatorio:</p> 
       <ul> 
        <li>Si hay un estado obligatorio que equivale al estado predeterminado desbloqueado, el estado obligatorio se convierte en el estado predeterminado, incluso si está desbloqueado.</li> 
        <li>Si ninguno de los estados obligatorios equivale al estado predeterminado desbloqueado, el primer estado obligatorio de la lista de estados se convierte en el estado predeterminado.</li> 
       </ul> <p>Para obtener información acerca de los estados requeridos, consulte los artículos <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceder a la lista de estados de proyecto del sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceder a la lista de estados de tarea del sistema</a> y <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Acceder a la lista de estados de problema del sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calculate Percent Complete based on]</td> 
   <td> <p>Workfront calcula el porcentaje completado de un proyecto o una tarea principal utilizando el porcentaje completado de cada tarea del proyecto y la duración o las horas planificadas de cada tarea.</p><p>Los usuarios asignados a cada tarea establecen manualmente el porcentaje completado de esta.</p><p>Aquí puede seleccionar si Workfront utilizará la duración o las horas planificadas de las tareas para calcular el porcentaje completado de los proyectos.</p> <p>Si selecciona [!UICONTROL Duration], la duración de cada tarea de un proyecto determinará el porcentaje completado global del proyecto y la duración de cada subtarea determinará el porcentaje completado global de su tarea principal.</p> <p>Si selecciona [!UICONTROL Duration], asegúrese de especificar las [!UICONTROL Typical hours per work day] y los [!UICONTROL Typical work days per week] en la sección [!UICONTROL Timelines]. [!DNL Workfront] utiliza esta información al calcular el porcentaje completado de una tarea según la duración. </p> <p>Si selecciona [!UICONTROL Planned Hours], asegúrese de que todas las tareas de cada proyecto tengan definida la cantidad de [!UICONTROL Planned Hours] y de que la cantidad no sea cero.</p><p>Para obtener más información, consulte <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Información general de porcentaje completado del proyecto</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Automatically set the project's Condition based on the Progress Status]</td> 
   <td> <p>Esta preferencia permite a los usuarios establecer manualmente la [!UICONTROL Condition] de un proyecto en ([!UICONTROL On Target], [!UICONTROL At Risk] o [!UICONTROL In Trouble]) o hacer que [!DNL Workfront] establezca la [!UICONTROL Condition] (estado del progreso) automáticamente según la progresión del proyecto en la línea de tiempo. Para obtener más información acerca de la condición de los proyectos, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Información general sobre la condición y el tipo de condición del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Create baselines automatically]</p> </td> 
   <td> <p>Esta preferencia crea automáticamente una línea de base (instantánea) de los detalles de tareas y proyectos cuando el estado del proyecto cambia a [!UICONTROL Current]. Para obtener información sobre la creación de líneas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Crear líneas de base de proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>El método de índice de rendimiento (PIM) del proyecto controla el método que utiliza [!DNL Workfront] para calcular métricas de valor ganado como [!UICONTROL Cost Performance Index] (CPI) y [!UICONTROL Estimate At Completion] (EAC). Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcular [!UICONTROL Cost Performance Index] (CPI)</a> y <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculate Estimate At Completion] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Hour-based]</strong>: [!DNL Workfront] utiliza las [!UICONTROL Planned Hours] para calcular métricas de rendimiento como el EAC y el CPI. Cuando el PIM se calcula en función de las horas, la EAC se muestra como un número de horas. Asegúrese de tener un valor distinto de cero de [!UICONTROL Planned Hours].</li> 
     <li> <p><strong>[!UICONTROL Cost-based]</strong>: [!DNL Workfront] utiliza el [!UICONTROL Planned Labor Cost] para calcular métricas de rendimiento como el EAC y el CPI. Asegúrese de que las funciones o los usuarios estén asociados a las tarifas de coste por hora. Cuando el PIM se calcula en función de los costes, la EAC se muestra como un valor de moneda.</p> <p>El jefe de proyecto puede modificar esta opción en el nivel de proyecto mediante el área [!UICONTROL Finance] de [!UICONTROL Project Details]. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área [!UICONTROL Finance] del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimate at Completion ]</p> </td> 
   <td> <p>Determine los datos que utiliza [!DNL Workfront] para calcular el [!UICONTROL Estimate at Completion] (EAC), que representa el coste proyectado total de un proyecto.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calculate at project level]</strong>: el EAC de la tarea principal y el proyecto se determinan introduciendo las [!UICONTROL Actual Hours] o el [!UICONTROL Actual Labor Cost] en las fórmulas de EAC. El cálculo incluye las [!UICONTROL Actual Hours] o los [!UICONTROL Costs and Expenses] añadidos directamente a la tarea principal o el proyecto.</li> 
     <li> <p><strong>[!UICONTROL Roll up from tasks/subtasks]</strong>: el EAC de la tarea principal y el proyecto se determinan sumando el EAC de cada tarea secundaria. Este cálculo excluye las [!UICONTROL Actual Hours] o los [!UICONTROL Actual Costs and Expenses] que se hayan añadido directamente a la tarea principal o el proyecto.</p> <p>El jefe de proyecto puede modificar esta opción en el nivel de proyecto mediante el área [!UICONTROL Finance] de [!UICONTROL Project Details]. Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Administrar información en el área [!UICONTROL Finance] del proyecto</a>.</p> </li> 
    </ul> <p>Para obtener más información sobre el cálculo del EAC, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcular el [!UICONTROL Estimate At Completion] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Cronologías {#timelines}

Configure cualquiera de las siguientes preferencias para proyectos recién creados en todo el sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Schedule From]</td> 
   <td> <p>Determine si los nuevos proyectos se programan desde la fecha de inicio o desde la fecha de finalización cuando se crean.</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Date]</strong>: las nuevas tareas tienen como valor predeterminado la restricción de tarea [!UICONTROL As Soon As Possible] y se pide a los jefes de proyecto que proporcionen una [!UICONTROL Planned Start Date] para el proyecto.</li> 
     <li><strong>[!UICONTROL Completion Date]</strong>: las nuevas tareas tienen como valor predeterminado la restricción de tarea [!UICONTROL As Late As Possible] y se pide a los jefes de proyecto que proporcionen una [!UICONTROL Planned Completion Date] para el proyecto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Determine si el tiempo libre del usuario asignado principal de una tarea ajusta las fechas planificadas de esa tarea en un proyecto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consider user time off in task durations]</strong>: los días libres programados para el usuario asignado principal de una tarea ajustan las fechas planificadas de la tarea si los días libres tienen lugar en el período de duración de la tarea. Esta es la configuración predeterminada. </p> <p>Por ejemplo, si una tarea con una restricción [!UICONTROL As Soon As Possible] está programada para comenzar el 1 de junio y finalizar el 3 de junio, y el usuario asignado principal tiene marcado el 2 de junio como día libre, las fechas planificadas de la tarea se ajustarán del 1 de junio al 4 de junio.</p> <p><b>IMPORTANTE</b>:</p> <p>La duración de la tarea no cambia al seleccionar esta configuración. Solo cambian las fechas planificadas, dependiendo de la Restricción de tarea.</p> </li> 
     <li><strong>[!UICONTROL Ignore user time off in task durations]</strong>: las fechas planificadas de cada tarea en un proyecto permanecen como se planificó originalmente, aunque el usuario asignado principal de una tarea tenga días libres durante su duración.</li> 
    </ul> <p>Tenga en cuenta lo siguiente al seleccionar opciones para esta configuración:</p> 
    <ul> 
     <li>Al cambiar esta configuración, solo los proyectos y las plantillas creados después del cambio heredan la configuración actualizada. </li> 
     <li> <p>El valor Restricción de tarea de la tarea determina qué fechas de tareas planificadas se deben ajustar: </p> 
      <ul> 
       <li>Fecha de inicio planificada</li> 
       <li>Fecha planificada de finalización</li> 
       <li>Ambas fechas</li> 
       <li>Ninguna fecha. </li> 
      </ul> <p>Por ejemplo, si una tarea tiene una Restricción de [!UICONTROL Fixed Dates], las fechas no se ajustan cuando el usuario asignado principal tiene días libres, incluso si la opción [!UICONTROL Consider user time off in task duration] está seleccionada. Para obtener más información sobre las restricciones de tarea, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Información general de la restricción de tarea</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Project timelines are automatically re-calculated]</p> </td> 
   <td> <p>Determine cuándo se vuelve a calcular la línea de tiempo de un proyecto. Para obtener información sobre cómo recalcular la escala de tiempo del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular las escalas de tiempo del proyecto</a>.</p> <p>Las siguientes opciones están habilitadas de forma predeterminada. Puede seleccionar una o varias de las siguientes opciones de configuración:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every night]</strong>: seleccione esta opción para recalcular las escalas de tiempo del proyecto cada noche. Los cambios que realice en el proyecto y que puedan afectar a la línea de tiempo no serán visibles de inmediato. [!DNL Workfront​​​] recalcula las escalas de tiempo por la noche solamente para proyectos donde se cumplen las dos condiciones siguientes:</p> <p> 
       <ul> 
        <li>Tiene un estado de [!UICONTROL Current]</li> 
        <li>Ha tenido una actualización en los últimos 3 meses</li> 
        <li>Ha tenido un tipo de actualización de uno de los siguientes:</li>
        <ul>
        <li>Automático y al cambiar</li>
        <li>Solo al cambiar</li>
        <li>Solo automático</li> 
      </ul>       
    <b>SUGERENCIA:</b>
    <p>Los proyectos cuyo tipo de actualización es Solo manual no se ven afectados por esta configuración.</p>
    <li> <p><strong>Cuando cambia el ámbito de un proyecto</strong>: seleccione esta opción para recalcular las escalas de tiempo del proyecto inmediatamente cuando se produzca un cambio de ámbito del proyecto. Para obtener información sobre lo que constituye un cambio de ámbito del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalcular las escalas de tiempo del proyecto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL When multiple users are assigned to a task use the schedule of the]</p> </td> 
   <td> <p>Si un proyecto no tiene asignada ninguna programación o si los usuarios asignados a sus tareas no tienen asignada una programación, [!DNL Workfront] utiliza el horario predeterminada del sistema para calcular la escala de tiempo de las tareas.</p> <p>Si asigna varios usuarios a la misma tarea en un proyecto y el proyecto tiene una programación asignada y los usuarios asignados a las tareas también tienen una programación asignada, [!UICONTROL Workfront] utiliza las siguientes programaciones:</p> 
    <ul> 
     <li><strong>[!UICONTROL Primary Assignment]</strong>: [!DNL Workfront] usa la programación de la asignación principal de la tarea para calcular las escalas de tiempo.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] usa la programación del proyecto para calcular la escala de tiempo de cada tarea.</li> 
    </ul> <p>Para obtener más información acerca de las programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Crear una programación</a>.</p> </td> 
  </tr>

</tr> 
  <tr> 
   <td role="rowheader"> <p>Cuando se asigna un usuario a una tarea, utilice la programación de...</p> </td> 
   <td> 
<p>Si un proyecto no tiene asignada ninguna programación o si los usuarios asignados a sus tareas no tienen asignada una programación, [!DNL Workfront] utiliza el horario predeterminada del sistema para calcular la escala de tiempo de las tareas.</p>

<p>Si asigna un usuario a una tarea de un proyecto y tanto el proyecto como el usuario asignado a las tareas tienen programaciones asociadas, [!UICONTROL Workfront] utilizará las siguientes programaciones:</p> 
    <ul> 
     <li><strong>[!UICONTROL Usuario]</strong>: [!DNL Workfront] utiliza la programación del usuario asignado en la tarea para calcular las escalas de tiempo.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] utiliza la programación del proyecto para calcular la escala de tiempo de la tarea.</li> 
    </ul> <p>Para obtener más información acerca de las programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Crear una programación</a>.</p>
</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Timeline Calculations] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typical hours per work day]</strong>: establezca el número de horas de un día de trabajo típico para los usuarios que trabajarán en los proyectos. El valor predeterminado es de 8 horas.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Typical work days per week]</strong>: establezca la semana laboral estándar para los usuarios que trabajan en proyectos. El valor predeterminado es de 5 días.</li> 
    </ul> <p>Estas dos opciones convierten los días en horas o las semanas en días.</p> <p>Por ejemplo, si tiene una tarea con 8 horas planificadas y la duración se calcula según las horas planificadas, [!DNL Workfront] convierte esas horas en días para mostrar la duración como días.</p> <p>En el campo [!UICONTROL Typical work days per week], [!DNL Workfront] calcula el valor de Equivalente a jornada completa (FTE) para su sistema. Esto es lo que [!DNL Workfront] usa al calcular asignaciones para los usuarios.</p> <p>Estos valores se utilizan cuando se planifican las líneas de tiempo de los proyectos, se presupuestan los recursos o se registra el tiempo en los proyectos. </p> <p>No se usan al establecer plantillas de horas para los usuarios del sistema, tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configure] preferencias de hoja de horas y de horas</a>.</p> <p><b>NOTA</b>:</p> <p>[!DNL Workfront] Los administradores no pueden desbloquear las preferencias de [!UICONTROL Timeline Calculations].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Custom Quarters]</p> </td> 
   <td> <p>Configure trimestres anuales personalizados para los usuarios que trabajarán en proyectos. Los trimestres personalizados suelen ser trimestres que no coinciden con el desglose tradicional de trimestres durante un año natural. Puede añadir varios trimestres personalizados. Para obtener más información, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Habilitar trimestres personalizados</a>.</p>  <p><b>NOTA</b>: </p><p>[!DNL Workfront] Los administradores no pueden desbloquear las preferencias de [!UICONTROL Custom Quarters].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Business Cases] {#business-cases}

Puede crear un caso empresarial para los proyectos recién creados en todo el sistema para enviar solicitudes de proyectos. Puede definir las preferencias para determinar qué áreas están visibles en el formulario **[!UICONTROL Business Case]**. Le recomendamos que habilite estas opciones para que otras herramientas, como [!UICONTROL Optimizador de portafolios], se actualicen correctamente. Para obtener más información acerca de lo que muestra cada campo, consulte [Definir un caso comercial: índice de artículos](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Una vez que el administrador de [!DNL Workfront] habilite las secciones del [!UICONTROL Business Case], un propietario del proyecto podrá crear un caso empresarial en el nivel de proyecto. Para obtener información sobre cómo crear un caso empresarial, consulte [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Life After Death]  {#life-after-death}

Configure cualquiera de las siguientes preferencias para proyectos recién creados en todo el sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a project has been marked as Complete, people can still] </p> </td> 
   <td> <p>Determine las reglas de su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a si una tarea o un problema se puede eliminar después de que el estado del proyecto se haya marcado como [!UICONTROL Complete].</p> 
    <ul> 
     <li><strong>[!UICONTROL Delete Tasks]</strong>: permite a los usuarios eliminar tareas de un proyecto después de que el proyecto se haya marcado como [!UICONTROL Complete].<br></li> 
     <li><strong>[!UICONTROL Delete Issues]</strong>: permite a los usuarios eliminar problemas de un proyecto después de que el proyecto se haya marcado como [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a Project is marked Complete, Dead, or it is Pending Approval, people can still]</p> </td> 
   <td> <p>Determine las reglas para su organización (o grupo, si está configurando las preferencias de proyecto para un grupo) con respecto a lo que sucede con las tareas, problemas, documentos y otros objetos de un proyecto después de que el estado del proyecto se haya marcado como <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Dead]</strong>, o bien <strong>[!UICONTROL Pending Approval]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Agregar y editar tareas:]</strong> Permite a los usuarios:
      <ul>
       <li><p>Editar tareas dentro de un proyecto después de que el proyecto se haya marcado como [!UICONTROL completo], [!UICONTROL muerto] o tenga [!UICONTROL pendiente de aprobación].</p>
           <p>Nota: Incluso cuando esta opción no está seleccionada, los usuarios pueden añadir y editar entradas de gastos. El registro de horas tiene una configuración independiente. Para permitir o evitar que los usuarios registren tiempo en proyectos con estado completo o muerto, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurar preferencias de horas y hojas de horas</a>.</p></li>
       <li>Añadir tareas a un proyecto.</li>
      </ul></li>
     <li><strong>[!UICONTROL Add and edit issues]</strong>: permite a los usuarios:
      <ul>
       <li>Editar problemas dentro de un proyecto después de que el proyecto se haya marcado como [!UICONTROL Complete], [!UICONTROL Dead] o [!UICONTROL Pending Approval].</li>
       <li>Añada problemas a un proyecto después de que el proyecto se haya marcado como [!UICONTROL Complete] o [!UICONTROL Dead]. (No se pueden añadir problemas a un proyecto que tenga [!UICONTROL Pending Approval].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Add documents to the project and to its tasks and issues]</strong>: permite a los usuarios añadir documentos a un proyecto (o añadir documentos a tareas y problemas dentro del proyecto) después de que el proyecto se haya marcado como [!UICONTROL Complete] o [!UICONTROL Dead].</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
     <li> <p><strong>[!UICONTROL Attach templates]</strong>: permite a los usuarios adjuntar plantillas a un proyecto después de que el proyecto se haya marcado como [!UICONTROL Complete] o [!UICONTROL Dead].</p> <p>Esta opción no se aplica a los proyectos que están pendientes de aprobación.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
