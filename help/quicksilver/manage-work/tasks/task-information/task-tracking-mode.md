---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre el modo de seguimiento de tareas
description: Puede ajustar la configuración Modo de seguimiento de una tarea al crear o editar una tarea para controlar cómo y cuándo se muestran los indicadores de estado de progreso de una tarea. Adobe Workfront muestra los indicadores de estado de progreso al configurar determinadas opciones de configuración para realizar el seguimiento del progreso en las tareas.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 3%

---

# Información general sobre el modo de seguimiento de tareas

Puede ajustar la configuración Modo de seguimiento de una tarea al crear o editar una tarea para controlar cómo y cuándo se muestran los indicadores de estado de progreso de una tarea. Adobe Workfront muestra los indicadores de estado de progreso al configurar determinadas opciones de configuración para realizar el seguimiento del progreso en las tareas.

Para obtener más información sobre el estado de progreso de las tareas, consulte [Información general sobre el estado de progreso de la tarea](../../../manage-work/tasks/task-information/task-progress-status.md).

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

Como propietario de una tarea o administrador de proyectos, puede seleccionar cómo Workfront indica el estado del progreso en cada tarea. Para obtener información sobre cómo configurar el modo de seguimiento en las tareas, consulte [Configurar el modo de seguimiento para tareas](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Puede seleccionar entre las siguientes opciones:

* [El usuario debe actualizar](#user-must-update)
* [Asumir a tiempo](#assume-on-time)
* [Ignorar advertencias tardías](#ignore-late-warnings)
* [Completar automáticamente](#auto-complete)
* [Predecesora](#predecessor)

### El usuario debe actualizar {#user-must-update}

Cuando se selecciona esta opción, Workfront utiliza el porcentaje de horas completas y reales de la tarea registrado para determinar el estado de progreso de la tarea. Esta es la opción predeterminada.

### Asumir a tiempo {#assume-on-time}

Workfront supone que una tarea se completará a tiempo independientemente del estado de finalización actual. Si no es así, Workfront asume automáticamente una fecha de finalización prevista del siguiente día laborable. Debe indicar cuándo se completa la tarea. Utilice esta opción cuando los usuarios no actualicen regularmente sus tareas.

### Ignorar advertencias tardías {#ignore-late-warnings}

El estado de progreso de una tarea pasa a estar en tiempo de activación hasta que llegue a ser tarde. Por ejemplo, si programa una tarea para que dure 10 días y el día en que se va a completar, la tarea muestra un porcentaje de finalización del 60 %, Workfront actualiza la fecha de finalización prevista añadiendo cuatro días y el estado de progreso de la tarea pasa a ser tarde.

### Completar automáticamente {#auto-complete}

Workfront asume que las tareas se completarán como están programadas y las marca como completas en sus fechas de vencimiento o de finalización planificadas. Hasta entonces, Workfront utiliza el porcentaje completado y las horas reales registradas para determinar el estado de progreso. Sin embargo, independientemente del estado de progreso antes de la fecha de finalización programada, Workfront sigue marcando la tarea finalizada.

Existen las siguientes excepciones:

* Si la tarea tiene predecesores incompletos, no se completará automáticamente hasta que se hayan completado todos sus predecesores.
* Si la tarea tiene una restricción de Fecha fija, la tarea siempre se completa en la Fecha de finalización planeada, independientemente de si se han completado sus predecesores.

>[!IMPORTANT]
>
>Si selecciona que las tareas se completen automáticamente, la tarea se completará cuando se vuelva a calcular la hora del proyecto. Si el tipo de actualización del proyecto está definido como automático o automático y en cambio, la línea de tiempo del proyecto se calcula diariamente. Para obtener información sobre los nuevos cálculos de cronología en los proyectos, consulte [Volver a calcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>La hora de la fecha de finalización real es la medianoche del día en que la línea de tiempo se calcula automáticamente. La hora utilizada para generar esta marca de tiempo es la zona horaria del sistema, tal como la define el administrador de Workfront en la sección Información del cliente de Configuración. Para obtener información sobre la configuración de la zona horaria del sistema, consulte [Configurar información básica para el sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Predecesora {#predecessor}

Workfront calcula la fecha de finalización prevista de una tarea según su relación predecesora. El estado de progreso de una tarea se determina en función de esta estimación. Por ejemplo, la tarea B tiene una duración de 1 día y está programada para completarse dos días después de su predecesora, la tarea A, que debería tardar cinco días. A continuación, un usuario actualiza la tarea B al 50 % completado, pero el predecesor, la tarea A, aún no se ha iniciado. Workfront programa la tarea dependiente B para su finalización seis días después de la fecha de inicio de la tarea predecesora, lo que permite 5 días para la tarea A y 1 día para la tarea B.
