---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Configurar el modo en que se muestra la información en el gráfico [!UICONTROL Gantt]
description: Puede configurar la información que se muestra en el gráfico Gantt de lista de tareas y en el gráfico Gantt de lista de proyectos.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 8%

---

# Configurar cómo se muestra la información en el [!UICONTROL gráfico Gantt]

<!-- Audited: 5/2025 -->

Puede configurar la información que se muestra en el Diagrama de Gantt de lista de tareas y en el Diagrama de Gantt de lista de proyectos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquete</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> 
   <p>[!UICONTROL Light] o superior<p>
   <p>[!UICONTROL Review] o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos y tareas</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL View] o acceso superior al proyecto y las tareas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Light<p>
   <p>Or</p>
   <p>Current: Review</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Comprender las opciones de visualización

En la tabla siguiente se detallan las opciones de presentación del [!UICONTROL gráfico Gantt]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Fechas reales</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Fecha real de inicio] y [!UICONTROL Fecha real de finalización] se muestran con un icono en forma de triángulo. Si la [!UICONTROL Fecha real de finalización] es nula, solo se muestra la [!UICONTROL Fecha real de inicio].</p> <p>Para obtener más información, vea <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Información general del proyecto [!UICONTROL Fecha real de finalización] </a> y <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Información general del proyecto [!UICONTROL Fecha real de inicio] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="assignments_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Muestra las personas asignadas a tareas. Pase el ratón sobre el enlace Detalles junto al nombre del usuario asignado para ver información más detallada sobre él, incluido el porcentaje de su asignación a la tarea.</p> <p>Las personas asignadas no aparecen en el [!UICONTROL Gantt chart] cuando el [!UICONTROL Gantt chart] se exporta a PDF. Cuando se exporta el diagrama de Gantt de [!UICONTROL] a PDF, las personas asignadas sólo aparecen en la lista de tareas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baseline]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>Instantánea del proyecto que representa datos clave sobre el proyecto incluido en el plan inicial del proyecto. Las líneas de base se pueden tomar en toda la cronología del proyecto. Cuando habilite la visualización de líneas de base en el gráfico Gantt de [!UICONTROL], seleccione la línea de base que desee mostrar. Sólo se puede ver una línea de base en el gráfico Gantt [!UICONTROL] a la vez, y se mostrará en forma de barra gris.</p> <p>Para obtener más información acerca de las líneas de base, vea <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Crear líneas de base de proyecto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commit Date]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>La fecha que un usuario asignado indica como su compromiso de cuándo se completará la tarea se muestra con un marcador en el gráfico Gantt [!UICONTROL]. </p> <p>Para obtener más información acerca de las fechas de confirmación, vea <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Fecha de confirmación] información general</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % completado]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  El porcentaje de la tarea que se completa se muestra en la línea de tareas.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ruta crítica]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>Las tareas que podrían afectar a la cronología del proyecto se consideran parte de la Ruta crítica y están claramente marcadas en rojo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hito] diamantes</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamantes.png"> </td> 
   <td> <p>Después de la tarea asociada a un hito aparece un icono de diamante. Pase el ratón sobre un hito para ver su nombre y fecha. El administrador [!DNL Workfront] determina el color de cada diamante de hito.</p> <p>Para obtener más información acerca de los hitos, vea <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Crear una ruta de hitos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Líneas de [!UICONTROL Milestone]</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Después de la tarea asociada a un hito aparece una línea. Pase el ratón sobre un hito para ver su nombre y fecha. El administrador [!DNL Workfront] determina el color de cada línea de hito.</p> <p> Para obtener más información sobre los hitos, consulte  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Crear una ruta de hitos</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecesoras]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Línea de una tarea a otra que muestra la relación de predecesoras entre las dos tareas. Para resaltar una línea de predecesora individual, pase el ratón sobre ella. Haga clic en él para mantenerlo resaltado. Sólo se puede resaltar una línea predecesora cada vez.</p> <p>Se muestra un icono de [!UICONTROL Predecesora] junto a cualquier tarea que tenga una relación de predecesora que abarque varias páginas en el diagrama de Gantt o en cualquier tarea que tenga una predecesora entre proyectos.</p> <p>Haga clic en el icono [!UICONTROL Predecesora] para ver todas las tareas predecesoras y sucesoras y sus detalles, como el nombre de la tarea, el tipo de relación predecesora y las fechas clave.</p> <p>Nota: El gráfico Gantt [!UICONTROL] de una lista de proyectos muestra información sobre las tareas predecesoras entre proyectos. Para obtener más información acerca de cómo crear relaciones de predecesoras entre diferentes proyectos, vea <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Crear predecesoras entre proyectos</a></p> <p>Para obtener más información sobre las predecesoras, vea <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Aplicar predecesoras</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Progress Status]</td> 
   <td> <p>[!UICONTROL On Time] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__oct._2017.png"></p> <p>[!UICONTROL Detrás]    <img src="assets/task-behind--oct.-2017.png" alt="task_hind__Oct._2017.png"></p> <p>[!UICONTROL En Riesgo]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>Retrasado        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>El estado del progreso actual en una tarea determinada. </p> <p>Para obtener más información, vea <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Información general sobre el estado del progreso de [!UICONTROL] de la tarea</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fechas proyectadas</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="Gantt_proyectado_fechas.png" style="width: 272;height: 152;"> </td> 
   <td> <p>Cronología prevista que marca las fechas proyectadas de inicio y finalización en función del trabajo actual completado, más el trabajo restante. </p> <p>Para obtener más información sobre las fechas de finalización proyectadas, vea <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Información general sobre la fecha de finalización proyectada para proyectos, tareas y problemas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar opciones de visualización

1. Vaya al **Gráfico Gantt de lista de tareas** o al **Gráfico Gantt de lista de proyectos**.\
   Para obtener más información sobre dónde se encuentra el gráfico Gantt, vea [Introducción al gráfico Gantt [!UICONTROL 2}.]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)

1. (Opcional) Seleccione la configuración **Cambiar a fechas proyectadas** para mostrar las tareas según sus fechas proyectadas. De forma predeterminada, las tareas se muestran según sus fechas planificadas.
1. Haga clic en el icono **Opciones**. Se abre el cuadro de diálogo **Opciones**.\
   ![Opciones.png](assets/options-350x129.png)

1. Seleccione las opciones de configuración que desee mostrar en el [!UICONTROL gráfico Gantt].

   >[!NOTE]
   >
   > No todas las opciones de configuración están disponibles en la lista de proyectos [!UICONTROL Diagrama de Gantt].

1. Haga clic en cualquier lugar del gráfico Gantt para cerrar el cuadro de diálogo **Opciones**.
