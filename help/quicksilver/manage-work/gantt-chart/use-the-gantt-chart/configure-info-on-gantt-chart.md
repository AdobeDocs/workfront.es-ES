---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Configure cómo se muestra la información en la variable [!UICONTROL Gantt] Gráfico
description: Puede configurar la información que se muestra en el diagrama de Gantt de lista de tareas y en el diagrama de Gantt de lista de proyectos.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Configure cómo se muestra la información en la variable [!UICONTROL Diagrama de Gantt]

Puede configurar la información que aparece en la lista de tareas [!UICONTROL Diagrama de Gantt] y la lista de proyectos [!UICONTROL Diagrama de Gantt].

## Requisitos de acceso

Debe tener lo siguiente para seguir los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL View] o acceso superior al proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Comprender las opciones de visualización

La tabla siguiente detalla las opciones de visualización para la variable [!UICONTROL Diagrama de Gantt]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fechas reales]</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Fecha de inicio real] y [!UICONTROL Fecha de finalización real] se muestran con un icono de triángulo. Si la [!UICONTROL Fecha de finalización real] es nula, solo se muestra la [!UICONTROL Fecha de inicio real].</p> <p>Para obtener más información sobre las fechas de inicio y finalización, consulte <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Descripción general del proyecto [!UICONTROL Fecha real de finalización] </a> y <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Descripción general del proyecto [!UICONTROL Fecha de inicio real] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asignaciones]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="assign_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Muestra los asignadores de tareas. Pase el ratón sobre la <strong>[!UICONTROL Detalles]</strong> vínculo al lado del nombre de un usuario asignado para ver información más detallada sobre ellos, incluido el porcentaje de su asignación a la tarea.</p> <p>Los asignadores no se muestran en el [!UICONTROL Gantt chart] cuando el [!UICONTROL Gantt chart] se exporta al PDF. Cuando se exporta el [!UICONTROL Gantt chart] al PDF, los destinatarios asignados se muestran únicamente en la lista de tareas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Línea de base]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>Una instantánea de proyecto que representa fragmentos clave de datos sobre el proyecto incluidos en el plan de proyecto inicial. Las bases de referencia pueden tomarse durante toda la vida del proyecto. Cuando habilite para mostrar líneas de base en el [!UICONTROL Gantt chart], seleccione la línea de base que desea mostrar. Sólo se puede ver una línea de base en el [!UICONTROL Gantt chart] a la vez, y se mostrará en forma de barra gris.</p> <p>Para obtener más información sobre las líneas de base, consulte <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Crear líneas de base del proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de confirmación]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>La fecha que un usuario asignado da como compromiso de cuándo se completará la tarea se muestra con un marcador en el [!UICONTROL Diagrama de Gantt]. </p> <p>Para obtener más información sobre las fechas de confirmación, consulte <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Información general sobre [!UICONTROL Fecha de confirmación]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % completado]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  El porcentaje de la tarea que se completa se muestra en la línea de tareas.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ruta crítica]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>Las tareas que podrían afectar a la línea de tiempo del proyecto se consideran parte de la ruta crítica y están claramente marcadas en rojo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Diamantes [!UICONTROL Milestone]</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamante.png"> </td> 
   <td> <p>Aparece un icono de diamante después de la tarea asociada a un hito. Pase el cursor sobre un hito para ver el nombre y la fecha del hito. La variable [!DNL Workfront] el administrador determina el color de cada diamante de hito.</p> <p>Para obtener más información sobre hitos, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Crear una ruta de hitos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Líneas [!UICONTROL Milestone]</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Se muestra una línea después de la tarea asociada a un hito. Pase el cursor sobre un hito para ver el nombre y la fecha del hito. La variable [!DNL Workfront] el administrador determina el color de cada línea de hitos.</p> <p> Para obtener más información sobre hitos, consulte  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Crear una ruta de hitos</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecesores]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecesor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Línea de una tarea a otra que muestra la relación predecesora entre las dos tareas. Para resaltar una línea predecesora individual, pase el ratón sobre ella. Haga clic en él para mantenerlo resaltado. Solo se puede resaltar una línea predecesora a la vez.</p> <p>A <strong>[!UICONTROL Predecesor]</strong> se muestra junto a cualquier tarea que tenga una relación predecesora que abarque varias páginas en el diagrama de Gantt o en cualquier tarea que tenga un predecesor entre proyectos.</p> <p>Haga clic en el <strong>[!UICONTROL Predecesor]</strong> para ver todas las tareas predecesora y sucesora, así como detalles sobre cada tarea, como el nombre de la tarea, el tipo de relación predecesora y las fechas clave.</p> <p>Nota: El [!UICONTROL Gantt Chart] de una lista de proyectos muestra información sobre los predecesores entre proyectos. Para obtener más información sobre cómo crear relaciones predecesoras entre diferentes proyectos, consulte <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Crear predecesores entre proyectos</a></p> <p>Para obtener más información sobre las predecesoras, consulte <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Aplicar predecesores</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado de progreso]</td> 
   <td> <p>[!UICONTROL On Time] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__Oct._2017.png"></p> <p>[!UICONTROL Detrás]    <img src="assets/task-behind--oct.-2017.png" alt="task_back_Oct._2017.png"></p> <p>[!UICONTROL En Riesgo]    <img src="assets/task-at-risk.png" alt="task_at_Risk.png"></p> <p>Retrasado        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>Estado del progreso actual en una tarea determinada. </p> <p>Para obtener información más detallada sobre cada tipo de [!UICONTROL Progress Status], consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Información general sobre el [!UICONTROL Progress Status] de la tarea</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fechas proyectadas]</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_estimated_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>El cronograma previsto que señala las [!UICONTROL Projected Start] y [!UICONTROL Complpletion dates] en función del trabajo actual completado, más el trabajo restante. </p> <p>Para obtener más información sobre las fechas de finalización previstas, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Información general sobre [!UICONTROL Fecha de finalización prevista] para proyectos, tareas y problemas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar las opciones de visualización

1. Ir a la lista de tareas [!UICONTROL Diagrama de Gantt] o la lista de proyectos [!UICONTROL Diagrama de Gantt].\
   Para obtener más información sobre dónde puede [!UICONTROL Diagrama de Gantt] se encuentra, consulte [Introducción a [!UICONTROL Diagrama de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. (Opcional) Seleccione el **[!UICONTROL Cambiar a fechas proyectadas]** configuración para mostrar las tareas por su [!UICONTROL Fechas proyectadas]. De forma predeterminada, las tareas se muestran según su [!UICONTROL Fechas planificadas] en el [!UICONTROL Diagrama de Gantt].
1. Haga clic en el icono de opciones para mostrar el **[!UICONTROL Opciones]** para abrir el Navegador.\
   ![Options.png](assets/options-350x129.png)

1. Seleccione las opciones de configuración que desea mostrar en la [!UICONTROL Diagrama de Gantt].

   >[!NOTE]
   > No todas las opciones de configuración están disponibles en la lista de proyectos [!UICONTROL Diagrama de Gantt].

1. Haga clic en cualquier lugar del [!UICONTROL Diagrama de Gantt] para cerrar el **[!UICONTROL Opciones]** para abrir el Navegador.
