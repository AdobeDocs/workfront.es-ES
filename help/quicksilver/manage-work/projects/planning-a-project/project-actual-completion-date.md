---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Descripción general del proyecto Fecha real de finalización
description: Los proyectos, las tareas y los problemas tienen una fecha real de finalización en Adobe Workfront. Es la fecha en la que se marcó la finalización del proyecto, la tarea o el problema.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Descripción general del proyecto Fecha real de finalización

Los proyectos, las tareas y los problemas tienen una fecha real de finalización en Adobe Workfront. Es la fecha en la que se marcó la finalización del proyecto, la tarea o el problema.

## Fechas reales de finalización

La Fecha real de finalización representa la fecha y hora reales en que se completó el trabajo. Cuando una tarea o un problema se marca como Listo o Completo, Workfront establece automáticamente la fecha del cambio de estado del elemento como la Fecha real de finalización de la tarea o el problema. Si esa fecha no indica con precisión cuándo se completó la tarea o el problema, puede editar manualmente la Fecha real de finalización.

Por ejemplo, puede marcar una tarea o un problema como Listo el lunes, pero sabe que el trabajo se completó el viernes anterior. Después de marcar la tarea o el problema como Listo, puede actualizar manualmente la Fecha real de finalización de la tarea o el problema a la fecha del viernes anterior para reflejar la finalización real.

No puede editar manualmente la fecha real de finalización de un proyecto, pero puede cambiar manualmente el estado de un proyecto, que puede almacenar en déclencheur un cambio en su fecha real de finalización.

La fecha real de finalización de un proyecto se establece de las siguientes maneras:

* Actualizando manualmente el estado del proyecto: si el modo de finalización del proyecto se establece en manual y cambia manualmente el estado del proyecto a completo, el déclencheur es que la fecha real de finalización del proyecto se actualice a la fecha y hora de la última tarea finalizada.
* Automáticamente, cuando se complete la última tarea del proyecto: si el modo de finalización del proyecto se establece en automático y marca la última tarea como completada o actualiza la fecha de finalización real de la última tarea, la fecha de finalización real del proyecto también se actualiza con esa fecha.

  Para obtener información acerca de cómo establecer el modo de finalización de un proyecto, vea el artículo [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront utiliza la fecha real de finalización de la última tarea del proyecto como fecha real de finalización de todo el proyecto.

Un administrador de Workfront o de grupo determina si Workfront utiliza la fecha actual o la fecha planificada de finalización de una tarea o un problema cuando se establecen como Completada o Cerrada. Para obtener información sobre cómo establecer las preferencias de tareas y problemas, consulte [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Buscar fechas de finalización reales

La fecha real de finalización se encuentra en las siguientes áreas de Workfront:

* Áreas de detalles de proyecto, tarea y problema
* Editar cuadros de proyecto, tarea y problema
* Actualizaciones de proyectos, tareas y problemas como una actualización del sistema.
* Listas o informes de proyectos, tareas o problemas.

Para obtener más información acerca de la creación de informes, vea el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
