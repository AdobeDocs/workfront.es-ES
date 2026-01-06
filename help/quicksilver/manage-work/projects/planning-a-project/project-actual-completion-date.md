---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre la fecha de finalización real del proyecto
description: Los proyectos, las tareas y los problemas tienen una fecha de finalización real en Adobe Workfront. Es la fecha en la que el proyecto, la tarea o el problema se marcó como finalizado.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 99%

---

# Información general sobre la fecha de finalización real del proyecto

Los proyectos, las tareas y los problemas tienen una fecha de finalización real en Adobe Workfront. Es la fecha en la que el proyecto, la tarea o el problema se marcó como finalizado.

## Fecha de finalización real

La fecha de finalización real representa la fecha y hora reales en que se completó el trabajo. Cuando una tarea o un problema se marcan como Listo o Completa/Resuelto, Workfront establece automáticamente la fecha del cambio de estado del elemento como la Fecha de finalización real de la tarea o el problema. Si esa fecha no indica con precisión cuándo se completó la tarea o se resolvió el problema, puede editar manualmente la Fecha de finalización real.

Por ejemplo, puede marcar una tarea o un problema como Listo el lunes, pero sabe que el trabajo se completó el viernes anterior. Después de marcar la tarea o el problema como Listo, puede actualizar manualmente la Fecha de finalización real de la tarea o del problema a la fecha del viernes anterior para reflejar la finalización real.

No puede editar manualmente la fecha de finalización real de un proyecto, pero sí puede cambiar manualmente el estado de un proyecto, lo que puede activar un cambio en su fecha de finalización real.

La fecha de finalización real de un proyecto se establece de las siguientes maneras:

* Actualizando manualmente el estado del proyecto: si el modo de finalización del proyecto se establece en Manual y cambia manualmente el estado del proyecto a finalizado, esto hace que la fecha de finalización real del proyecto se actualice a la fecha y hora de la última tarea finalizada.
* Automáticamente, cuando se complete la última tarea del proyecto: si el modo de finalización del proyecto se establece en Automático y marca la última tarea como finalizada o actualiza la fecha de finalización real de la última tarea, la fecha de finalización real del proyecto también se actualiza con esa fecha.

  Para obtener información sobre cómo establecer el modo de finalización de un proyecto, consulte el artículo [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront utiliza la fecha de finalización real de la tarea del proyecto que se finalizó en último lugar como la fecha de finalización real de todo el proyecto.

Un administrador de Workfront o de grupos determina si Workfront utiliza la fecha actual o la fecha planificada de finalización de una tarea o un problema cuando su estado se establece como Completa/Resuelto o Cerrado. Para obtener información sobre cómo establecer las preferencias de tareas y problemas, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Buscar fechas de finalización reales

La fecha de finalización real se encuentra en las siguientes áreas de Workfront:

* Áreas de detalles de proyecto, tarea y problema
* Cuadros de edición de proyecto, tarea y problemas
* Área de actualizaciones de proyectos, tareas y problemas como actualización del sistema.
* Listas o informes de proyectos, tareas o problemas.

Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
