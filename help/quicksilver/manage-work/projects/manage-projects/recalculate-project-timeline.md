---
product-area: projects
navigation-topic: manage-projects
title: Recalcular escalas de tiempo del proyecto
description: Volver a calcular las escalas de tiempo permite a los administradores ver cómo los diferentes factores relacionados con el proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: fe9d3cfbb50bfda672360b918d971cc77b0b8b0a
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 11%

---

# Recalcular escalas de tiempo del proyecto

<!--Audited: 06/2025-->

Volver a calcular las escalas de tiempo permite a los administradores ver cómo los diferentes factores relacionados con el proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas.

Realizar cambios en los horarios, el tiempo libre del personal y otros elementos fuera del ámbito de un proyecto no afecta inmediatamente a la cronología del proyecto. La escala de tiempo del proyecto se ve afectada cuando se recalcula la escala de tiempo. Las influencias externas no surten efecto en el proyecto hasta que se vuelve a calcular.

Este artículo describe las formas en que se produce el recálculo de escala de tiempo.

El cálculo automático de escala de tiempo se produce sin acceso especial para ninguno de los usuarios implicados en el trabajo en el proyecto. Además, puede recalcular manualmente la escala de tiempo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nueva licencia: estándar </p> 
   O
   <p>Licencia actual: plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> <p>El administrador del sistema debe recalcular la escala de tiempo de todos los proyectos del sistema</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en un proyecto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Recálculo automático

De manera predeterminada, las escalas de tiempo de los proyectos se recalculan automáticamente a diario cuando el ámbito del proyecto cambia o cada noche. El administrador de Workfront determina si se deben calcular automáticamente las escalas de tiempo cada noche o con cada cambio de ámbito administrando la configuración Escalas de tiempo en el área Preferencias de proyecto de Configuración. Para obtener más información, vea [Configurar cálculos de escala de tiempo para proyectos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>Si la escala de tiempo de un proyecto supera los 15 años, se deshabilita el cálculo automático para ese proyecto. Solo puede seleccionar un Tipo de actualización de manual para un proyecto de más de 15 años. Si cambia las fechas del proyecto a menos de 15 años, debe recalcular manualmente la escala de tiempo una vez antes de que se calcule automáticamente.

* [Recálculo automático de escalas de tiempo de proyectos](#automatic-recalculation-of-project-timelines)
* [Acciones que almacenan en déclencheur un nuevo cálculo automático de las escalas de tiempo del proyecto](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)


>[!IMPORTANT]
>
>Para los entornos de vista previa y espacio aislado de actualización personalizado, el recálculo por la noche está deshabilitado y las escalas de tiempo del proyecto no se recalculan automáticamente. Debe recalcular manualmente la cronología del proyecto para los entornos de Vista previa y de la Zona protegida de actualización personalizada.

### Recálculo automático de escalas de tiempo de proyectos {#automatic-recalculation-of-project-timelines}

Adobe Workfront vuelve a calcular las escalas de tiempo a diario solo para los proyectos en los que se cumplen todas las condiciones siguientes:

* Tiene un estado Actual
* El tipo de actualización del proyecto se establece en Automático o Automático y Al cambiar

  Para obtener información acerca del tipo de actualización del proyecto, vea [Descripción general del tipo de actualización del proyecto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Tener una fecha de última actualización en los últimos tres meses\
  El administrador de Workfront puede cambiar esta funcionalidad predeterminada, tal como se describe en [Configurar los cálculos de escala de tiempo para los proyectos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* La fecha del último cálculo de la escala de tiempo del proyecto no está dentro del día del calendario actual. Esto significa que la última fecha de cálculo de la escala de tiempo del proyecto es anterior a las 00:00 del día actual.

Puede configurar la frecuencia con la que se actualiza la cronología del proyecto. Cuando se actualiza la escala de tiempo del proyecto, se vuelve a calcular en función de los cambios realizados en el proyecto.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Para obtener más información, vea [Seleccionar el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### Acciones que almacenan en déclencheur un nuevo cálculo automático de las escalas de tiempo del proyecto {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Varios cambios de ámbito en la duración de un proyecto recalculan automáticamente la cronología del proyecto, incluidas las siguientes acciones:

* Actualizando estado de tarea.
* Mover una tarea a un proyecto diferente.
* Actualizando la fecha planificada o las fechas planificadas de finalización de las tareas.
* Actualizar el tipo de duración, la restricción de tarea o el número de personas asignadas en las tareas.
* Actualizando relaciones de predecesoras de tareas.
* Agregar una aprobación a una tarea que también agregue tiempo a la Fecha planificada de finalización de la tarea.\
  Para obtener más información acerca de la configuración de aprobación, vea [Configurar la configuración de aprobación global](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Recálculo manual {#manual-recalculation}

Como propietario de un proyecto, puede recalcular manualmente las escalas de tiempo de proyectos individuales. El administrador de Workfront puede recalcular manualmente todas las cronologías en Workfront.

* [Recalcular escalas de tiempo para proyectos individuales o en lotes](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [Recalcule las escalas de tiempo manualmente de forma masiva en el cuadro Editar proyectos](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Volver a calcular las escalas de tiempo de todos los proyectos del sistema (solo administradores de Workfront)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Volver a calcular escalas de tiempo para proyectos individuales o en bloque {#recalculate-timelines-for-individual-projects-or-in-bulk}

Puede recalcular la cronología de un proyecto en Workfront desde la página del proyecto o desde una lista de proyectos o un informe.

1. Vaya al proyecto para el que desea volver a calcular la escala de tiempo y haga clic en el icono **Más** ![Menú Más](assets/qs-more-menu.png) que aparece a la izquierda del nombre del proyecto

   ![Más lista desplegable](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   O

   Vaya a una lista de proyectos o a un informe, seleccione uno o varios proyectos y, a continuación, haga clic en el icono **Más** ![Menú Más](assets/qs-more-menu.png) que se encuentra en la parte superior de la lista.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Según la complejidad de sus proyectos, recomendamos no seleccionar un gran número de proyectos al volver a calcular sus escalas de tiempo de forma masiva para garantizar un rendimiento óptimo. Algunas cosas que pueden hacer que un proyecto sea demasiado complejo pueden ser varias dependencias o asignaciones o un gran número de campos personalizados.

1. Haga clic en **Volver a calcular escala de tiempo**.

   Una vez recalculada la escala de tiempo, verá un mensaje que indica que la actualización se realizó correctamente.

   >[!TIP]
   >
   >Antes de que finalice el recálculo de escala de tiempo, es posible que algunas fechas planificadas o proyectadas aparezcan atenuadas. Esto significa que el cálculo aún no ha finalizado y que las fechas están sujetas a cambios.

### Recalcule manualmente las escalas de tiempo de forma masiva en la casilla Editar proyectos {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Puede recalcular manualmente las escalas de tiempo de varios proyectos editándolas de forma masiva.

>[!TIP]
>
>Según la complejidad de sus proyectos, recomendamos no seleccionar un gran número de proyectos al editarlos de forma masiva para garantizar un rendimiento óptimo. Algunas cosas que podrían hacer que un proyecto sea demasiado complejo podrían ser varias dependencias o asignaciones o un gran número de campos personalizados.

1. Ir a una lista de proyectos.
1. Seleccione varios proyectos en la lista y luego haga clic en **Editar**.
1. Haga clic en **Configuración** y, a continuación, seleccione **Volver a calcular escalas de tiempo**.

1. Haga clic en **Guardar cambios**.

### Volver a calcular las escalas de tiempo de todos los proyectos del sistema (solo administradores de Workfront) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Los administradores de Workfront pueden ejecutar el diagnóstico Recalcular escala de tiempo para volver a calcular inmediatamente todas las escalas de tiempo en el sistema de Workfront. Esto permite a todos los gestores de proyectos ver la influencia de los cambios externos inmediatamente, tanto en las fechas planificadas como en las proyectadas.

Para obtener más información acerca de cómo recalcular las escalas de tiempo para todo el sitio de Workfront, vea la sección &quot;Recalcular escalas de tiempo para toda la instancia de Workfront&quot; en [Configurar cálculos de escala de tiempo para proyectos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
