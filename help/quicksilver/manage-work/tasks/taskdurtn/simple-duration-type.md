---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: "Resumen del tipo de duración: Simple"
description: El tipo de duración simple es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte Información general sobre la duración de la tarea y el tipo de duración.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 1efd7c0270fe1396345cfa6e5499e8f998297d61
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Información general del tipo de duración: Simple

El tipo de duración simple es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general acerca de los tipos de duración en Workfront, vea [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Descripción general del tipo de duración simple

Su Workfront o un administrador de grupo pueden establecer el tipo de duración predeterminado de su sistema o grupo como Simple. En este caso, todas las tareas nuevas se crearán con este tipo de duración. Para obtener información sobre cómo cambiar las preferencias de tareas y problemas como parte de las preferencias de proyectos de nivel de sistema o de grupo, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Cuando una tarea tiene un tipo de duración sencillo, ocurre lo siguiente:

* Los jefes de proyecto pueden modificar tanto la duración como las horas planificadas de una tarea al modificar cómo deben distribuirse esas horas entre las personas asignadas.

  Para obtener más información, vea [Actualizar las horas y la duración planificadas de una tarea con un tipo de duración simple](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >Cuando crea una tarea por primera vez, le asigna el Tipo de duración simple y no especifica una Duración, Workfront calcula la Duración de la tarea en función de la cantidad de Horas planificadas que especifique para la tarea. Si modifica manualmente la Duración de una tarea de Duración simple, Workfront deja de hacer coincidir las Horas planificadas con la Duración porque supone que desea definirlas manualmente.
  >
  >Workfront calcula la duración de las tareas cuya duración no se ha modificado manualmente mediante la fórmula siguiente:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >El administrador de Workfront define `Typical hours per work day` en el área de Preferencias de proyecto de la Configuración de la instancia.

* El porcentaje de asignación está oculto y las horas de asignación pueden editarse en su lugar.
* Todos los clientes nuevos tienen el Tipo de duración de nivel de sistema establecido en Simple.

## Cambiar el tipo de duración de una tarea a Simple

Para obtener información acerca de cómo cambiar el tipo de duración de una tarea, vea [Actualizar el tipo de duración de una tarea](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
