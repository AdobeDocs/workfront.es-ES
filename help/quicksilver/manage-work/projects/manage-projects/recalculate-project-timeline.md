---
product-area: projects
navigation-topic: manage-projects
title: Volver a calcular las líneas de tiempo del proyecto
description: El cálculo de las líneas de tiempo permite a los administradores ver cómo los distintos factores relacionados con el proyecto están afectando a la cronología del proyecto. La cronología de un proyecto se refiere a fechas planificadas y proyectadas.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Volver a calcular las líneas de tiempo del proyecto

El cálculo de las líneas de tiempo permite a los administradores ver cómo los distintos factores relacionados con el proyecto están afectando a la cronología del proyecto. La cronología de un proyecto se refiere a fechas planificadas y proyectadas.

Los cambios en los programas, el tiempo libre del personal y otros elementos fuera del alcance de un proyecto no afectan inmediatamente al calendario del proyecto. La cronología del proyecto se ve afectada cuando se vuelve a calcular la cronología. Las influencias externas no surten efecto en el proyecto hasta que no se vuelva a calcular.

Este artículo describe las formas en que se produce el cálculo de la cronología.

## Requisitos de acceso

<!--drafted for P&P: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
El cálculo automático de la cronología se produce sin acceso especial para cualquiera de los usuarios que participan en el proyecto.

Sin embargo, debe tener el siguiente acceso para volver a calcular manualmente la escala de tiempo de un proyecto:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Administrador del sistema para volver a calcular la cronología de todos los proyectos del sistema</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Nuevo cálculo automático

De forma predeterminada, las líneas de tiempo del proyecto se vuelven a calcular automáticamente cada día cuando cambia el ámbito del proyecto o cada noche. El administrador de Workfront determina si se calcularán automáticamente las cronologías cada noche o con cada cambio de ámbito administrando la configuración de las cronologías en el área Preferencias del proyecto de configuración. Para obtener más información, consulte [Configurar nuevos cálculos de cronología para proyectos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>Si la duración de un proyecto supera los 15 años, el cálculo automático se desactivará para ese proyecto. Solo puede seleccionar un tipo de actualización manual para un proyecto que dure más de 15 años. Si cambia las fechas del proyecto a menos de 15 años, debe volver a calcular manualmente la cronología una vez antes de que se calcule automáticamente.

* [Nuevo cálculo automático de los plazos del proyecto](#automatic-recalculation-of-project-timelines)
* [Acciones que tienen como déclencheur un nuevo cálculo automático de los plazos del proyecto](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)

### Nuevo cálculo automático de los plazos del proyecto {#automatic-recalculation-of-project-timelines}

Adobe Workfront vuelve a calcular las líneas de tiempo diariamente solo para los proyectos en los que se cumplen todas las condiciones siguientes:

* Tener un estado de Actual
* El tipo de actualización del proyecto está definido como automático o automático y en cambio

   Para obtener información sobre el tipo de actualización del proyecto, consulte [Información general sobre el tipo de actualización del proyecto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Tener una fecha de última actualización en los últimos tres meses\
   El administrador de Workfront puede cambiar esta funcionalidad predeterminada, tal como se describe en [Configurar nuevos cálculos de cronología para proyectos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* La última fecha de cálculo de la cronología del proyecto no está dentro del día del calendario actual. Esto significa que la última fecha de cálculo de la cronología del proyecto es anterior a las 00:00 del día actual.

Puede configurar la frecuencia con la que se actualiza la cronología del proyecto. Cuando se actualiza la línea de tiempo del proyecto, se vuelve a calcular en función de los cambios realizados en el proyecto.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Para obtener más información, consulte [Seleccione el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

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

### Acciones que tienen como déclencheur un nuevo cálculo automático de los plazos del proyecto {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Varios cambios de ámbito en la vida de un proyecto vuelven a calcular automáticamente la cronología del proyecto, incluidas las siguientes acciones:

* Actualizando el estado de la tarea.
* Mover una tarea a otro proyecto.
* Actualización de la Fecha Planificada o Fechas de Finalización Planificada de las Tareas.
* Actualizar el tipo de duración, la restricción de tareas o el número de personas asignadas a las tareas.
* Actualizando las relaciones predecesoras de la tarea.
* Adición de una aprobación a una tarea que también agrega una hora a la Fecha de Finalización Planificada de la tarea.\
   Para obtener más información sobre la configuración de aprobación, consulte [Configuración de la aprobación global](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Cálculo manual {#manual-recalculation}

Como propietario de un proyecto, puede volver a calcular manualmente las líneas de tiempo de proyectos individuales. El administrador de Workfront puede volver a calcular manualmente todas las líneas de tiempo en Workfront.

* [Volver a calcular los plazos para proyectos individuales o en bloque](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [Volver a calcular manualmente las líneas de tiempo de forma masiva en el cuadro Editar proyectos](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Volver a calcular las cronologías de todos los proyectos del sistema (solo administradores de Workfront)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Volver a calcular los plazos para proyectos individuales o en bloque {#recalculate-timelines-for-individual-projects-or-in-bulk}

Puede volver a calcular la cronología de un proyecto en Workfront desde la página del proyecto o desde una lista o informe de proyecto.

1. Vaya al proyecto para el que desea volver a calcular la cronología y haga clic en el **Más** icono ![](assets/qs-more-menu.png) a la izquierda del nombre del proyecto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   O

   Vaya a una lista de proyectos o a un informe y seleccione uno o varios proyectos. A continuación, haga clic en el **Más** icono ![](assets/qs-more-menu.png) en la parte superior de la lista.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >En función de la complejidad de sus proyectos, se recomienda no seleccionar un gran número de proyectos al volver a calcular sus plazos de forma masiva para garantizar un rendimiento óptimo. Algunas cosas que podrían hacer que un proyecto sea demasiado complejo pueden ser varias dependencias o asignaciones, o un gran número de campos personalizados.

1. Haga clic en **Volver a calcular línea de tiempo**.

   Una vez recalculada la cronología, verá un mensaje que indica que el cálculo se realizó correctamente.

   >[!TIP]
   >
   >Antes de que finalice el cálculo de la cronología, algunas fechas planificadas o proyectadas podrían mostrarse atenuadas. Esto significa que el nuevo cálculo aún no ha finalizado y las fechas están sujetas a cambios.

### Volver a calcular manualmente las líneas de tiempo de forma masiva en el cuadro Editar proyectos {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Puede volver a calcular manualmente las líneas de tiempo de varios proyectos editándolas de forma masiva.

>[!TIP]
>
>En función de la complejidad de sus proyectos, se recomienda no seleccionar un gran número de proyectos al editarlos de forma masiva para garantizar un rendimiento óptimo. Algunas cosas que podrían hacer que un proyecto sea demasiado complejo pueden ser varias dependencias o asignaciones o un gran número de campos personalizados.

1. Vaya a una lista de proyectos.
1. Seleccione varios proyectos de la lista y haga clic en **Editar**.
1. Haga clic en **Configuración** y, a continuación, seleccione **Volver a calcular las líneas de tiempo**.

1. Haga clic en **Guardar cambios**.

### Volver a calcular las cronologías de todos los proyectos del sistema (solo administradores de Workfront) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Los administradores de Workfront pueden ejecutar el diagnóstico Recalcular línea de tiempo para volver a calcular inmediatamente todas las líneas de tiempo del sistema Workfront. Esto permite a todos los administradores de proyectos ver la influencia de los cambios externos inmediatamente en las fechas planificadas y proyectadas.

Para obtener más información sobre cómo recalcular las líneas de tiempo para todo el sitio de Workfront, consulte la sección &quot;Recalcular las líneas de tiempo para toda la instancia de Workfront&quot; en [Configurar nuevos cálculos de cronología para proyectos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

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
