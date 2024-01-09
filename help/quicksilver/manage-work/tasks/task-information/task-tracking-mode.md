---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general del modo de seguimiento de tareas
description: Puede ajustar la configuración Modo de seguimiento de una tarea al crear o editar una tarea para controlar cómo y cuándo se muestran los indicadores de estado de progreso de una tarea. Adobe Workfront muestra indicadores de estado de progreso al configurar ciertas opciones para el seguimiento del progreso de las tareas.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: d2836549ee3c615201ce5f3454258e9af31efa42
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# Información general del modo de seguimiento de tareas

<!-- Audited: 01/2024 -->

Puede ajustar la configuración Modo de seguimiento de una tarea al crear o editar una tarea para controlar cómo y cuándo se muestran los indicadores de estado de progreso de una tarea. Adobe Workfront muestra indicadores de estado de progreso al configurar ciertas opciones para el seguimiento del progreso de las tareas.

Para obtener más información sobre el estado de progreso de las tareas, consulte [Resumen del estado de progreso de tareas](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## Opciones del modo de seguimiento {#tracking-mode-options}

Como propietario de una tarea o jefe de proyecto, puede seleccionar la forma en que Workfront indica el estado de progreso de cada tarea. Para obtener información sobre cómo establecer el modo de seguimiento en sus tareas, consulte [Establecer el modo de seguimiento para las tareas](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Puede seleccionar las siguientes opciones:

* [El usuario debe actualizar](#user-must-update)
* [Asumir a tiempo](#assume-on-time)
* [Ignorar advertencias tardías](#ignore-late-warnings)
* [Completar automáticamente](#auto-complete)
* [Predecesora](#predecessor)

### El usuario debe actualizar {#user-must-update}

Si se selecciona esta opción, Workfront utiliza el porcentaje completado y las horas reales registradas de la tarea para determinar el estado de progreso de la tarea. Esta es la opción predeterminada.

### Asumir a tiempo {#assume-on-time}

Workfront supone que una tarea se completará a tiempo independientemente del estado actual de finalización. Si la tarea no se completa a tiempo (en la fecha planificada de finalización), Workfront supone automáticamente una fecha planificada de finalización del siguiente día laborable. Aún debe indicar cuándo se completa la tarea. Utilice esta opción cuando los usuarios no actualicen con regularidad sus tareas.

### Ignorar advertencias tardías {#ignore-late-warnings}

El estado de progreso de una tarea será A tiempo hasta que se haga Tarde. Por ejemplo, si programa una tarea para que dure 10 días y en el día en que se debe completar la tarea muestra un porcentaje completado del 60 %, Workfront actualiza la fecha proyectada de finalización añadiendo cuatro días y el estado de progreso de la tarea pasa a ser Late.

### Completar automáticamente {#auto-complete}

Workfront supone que las tareas se completarán según lo programado y las marca como completadas en sus fechas de vencimiento o planificadas de finalización. Hasta entonces, Workfront utiliza el porcentaje completado y las horas reales registradas para determinar el estado del progreso. Sin embargo, independientemente del estado del progreso antes de la fecha programada de finalización, Workfront sigue marcando la tarea como completada.

Existen las siguientes excepciones:

* Si la tarea tiene predecesoras incompletas, no se completará automáticamente hasta que se completen todas sus predecesoras. Se deben aplicar las predecesoras.
* Si la tarea tiene una delimitación de Fecha fija, la tarea siempre se completa en la Fecha planificada de finalización, independientemente de si se han completado sus predecesoras.

>[!IMPORTANT]
>
>Si selecciona que las tareas se completen automáticamente, la tarea se completará cuando se recalcule la hora del proyecto. Si el Tipo de actualización del proyecto se establece en Automática o Automática y al cambiar, la cronología del proyecto se calcula diariamente. Para obtener información sobre los cálculos de escala de tiempo en proyectos, consulte [Recalcular escalas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>La hora de la fecha real de finalización es la medianoche del día en que se calcula automáticamente la escala de tiempo. La hora utilizada para generar esta marca de tiempo es la zona horaria del sistema definida por el administrador de Workfront en la sección Información del cliente de la Configuración. Para obtener información sobre cómo establecer la zona horaria del sistema, consulte [Configurar la información básica del sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Predecesora {#predecessor}

Workfront calcula la fecha proyectada de finalización de una tarea según su relación de predecesora. El estado de progreso de una tarea se determina según esta estimación. Por ejemplo, la Tarea B tiene una Duración de 1 Día y está programada para completarse dos días después de su predecesora, la Tarea A, que debería tardar cinco días. Un usuario actualiza la Tarea B al 50% completada, pero la predecesora, la Tarea A, aún no se ha iniciado. Workfront programa la tarea dependiente B para su finalización seis días después de la fecha de inicio de la tarea predecesora, lo que permite 5 días para la Tarea A y 1 día para la Tarea B.
