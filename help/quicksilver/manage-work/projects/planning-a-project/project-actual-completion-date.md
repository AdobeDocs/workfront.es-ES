---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Descripción general de la fecha de finalización real del proyecto
description: Los proyectos, las tareas y los problemas tienen una Fecha de finalización real en Adobe Workfront. Esta es la fecha en la que el proyecto, la tarea o el problema se marcaron como completados.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: 3a3dc541219706e3f6a4700889db344c110838bb
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Descripción general de la fecha de finalización real del proyecto

Los proyectos, las tareas y los problemas tienen una Fecha de finalización real en Adobe Workfront. Esta es la fecha en la que el proyecto, la tarea o el problema se marcaron como completados.

## Fechas reales de finalización

La fecha de finalización real representa la fecha y hora reales en que se completa el trabajo. Cuando una tarea o un problema se marca como Listo o Completado, Workfront establece automáticamente la fecha del cambio en el estado del elemento como la fecha de finalización real de la tarea o el problema. Si esa fecha no refleja con precisión cuándo se completó la tarea o el problema, puede editar manualmente la fecha de finalización real.

Por ejemplo, puede marcar una tarea o un problema Listo el lunes, pero sabe que el trabajo se completó el viernes anterior. Después de marcar la tarea o el problema como Listo, puede actualizar manualmente la fecha de finalización real de la tarea o el problema a la fecha del viernes anterior para reflejar la finalización real.

No puede editar manualmente la fecha de finalización real de un proyecto, pero puede cambiar manualmente el estado de un proyecto, lo que puede almacenar un cambio en la fecha de finalización real.

La fecha de finalización real de un proyecto se establece de las siguientes maneras:

* Actualizando manualmente el estado del proyecto: si el modo de finalización del proyecto se establece en Manual y cambia manualmente el estado del proyecto a Completado, se déclencheur la fecha de finalización real del proyecto para que se actualice a la fecha y hora en que se cambie el estado.
* Automáticamente, cuando se completa la última tarea del proyecto: si el modo de finalización del proyecto se establece en Automático y marca la última tarea como Completada o actualiza la fecha de finalización real de la última tarea, la fecha de finalización real del proyecto también se actualiza con esa fecha.

   Para obtener información sobre cómo configurar el modo de finalización de un proyecto, consulte el artículo [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!NOTE]
   >
   >Workfront utiliza la fecha de finalización real de la tarea del proyecto que se completó por última vez como la fecha de finalización real de todo el proyecto.

Un administrador de Workfront o de grupo determina si Workfront utiliza la fecha actual o la fecha de finalización planeada de una tarea o un problema cuando se establecen como Completada o Cerrada. Para obtener información sobre la configuración de las preferencias de problemas y tareas, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Localizar fechas de finalización reales

La fecha de finalización real se encuentra en las siguientes áreas de Workfront:

* Áreas de detalles de problemas, tareas y proyectos
* Editar proyecto, tarea y cuadros de problema
* Área de actualizaciones de proyectos, tareas y problemas como actualización del sistema.
* Listas o informes de proyectos, tareas o problemas.

Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
