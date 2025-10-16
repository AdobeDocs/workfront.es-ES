---
product-area: projects
navigation-topic: issue-information
title: Resumen de la fecha planificada de finalización del problema
description: La fecha planificada de finalización de un problema es la fecha en la que se espera que se resuelva el problema.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 11%

---

# Resumen de la fecha planificada de finalización del problema

<!--Audited: 08/2025-->

La fecha planificada de finalización de un problema es la fecha en la que se espera que se resuelva el problema.

Puede especificar la fecha planificada de finalización de un problema o dejar que Adobe Workfront lo calcule en función de determinados criterios.

Las Fechas planificadas de finalización de los problemas no afectan a la fecha planificada de finalización del proyecto. Solo las fechas planificadas de finalización de las tareas afectan a la fecha planificada de finalización del proyecto. Para obtener más información sobre la fecha planificada de finalización del proyecto, consulte [Establecer la fecha planificada de finalización del proyecto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La fecha planificada de finalización de una incidencia difiere de la fecha de confirmación de la incidencia o de la fecha proyectada de finalización de la incidencia de las siguientes maneras:
>
>* La fecha de confirmación es la fecha en la que la persona asignada a la incidencia calcula manualmente que habrá finalizado la incidencia. Para obtener más información, consulte los siguientes artículos:
>
>   * [Información general sobre la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interacciones entre la fecha de confirmación y la fecha planificada de finalización](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* La fecha proyectada de finalización es una fecha calculada por Workfront que tiene en cuenta factores externos para determinar una fecha real en la que se puede completar el problema de forma realista. Para obtener más información, consulte [Información general sobre la fecha proyectada de finalización para proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Establecer manualmente la fecha planificada de finalización de un problema

Debe tener acceso de edición a Problemas y permisos de administración sobre el problema para poder actualizar la Fecha planificada de finalización del problema.

Puede establecer manualmente la fecha planificada de finalización de un problema en las siguientes áreas de Workfront:

* En el cuadro Editar problema o en el área Detalles del problema al crear o editar un problema. Para obtener más información, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).
* En el área de Inicio si la fecha planificada de finalización se muestra en el panel de resumen de un problema. Para obtener más información, consulte [Actualizar o editar un elemento de trabajo en el área de inicio](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* En el encabezado del problema. Para obtener más información, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* En una lista de problemas o un informe cuando el campo Fecha planificada de finalización se muestra en la vista.

  Para obtener más información, consulte [Editar problemas en una lista](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Cómo Workfront calcula automáticamente la fecha planificada de finalización de un problema

Cuando Workfront calcula la fecha planificada de finalización de un problema automáticamente, la fecha puede verse afectada por lo siguiente:

* Fecha de inicio planificada

  La fecha de entrada y la fecha planificada de inicio deben coincidir en un problema la primera vez que lo cree.

* Duración predeterminada según se ha configurado en la sección Detalles de cola del proyecto. Para obtener más información, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

  Si la duración predeterminada es 0 días, la fecha planificada de finalización coincide con la fecha planificada de inicio del problema.

* Programación del proyecto

Cuando se establece automáticamente, la fecha planificada de finalización se determina según el siguiente cálculo:

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Ejemplo:** Por ejemplo, si la tarea tiene una fecha de inicio del viernes 14 de enero y la duración predeterminada es 5 días, la fecha planificada de finalización será el viernes 21 de enero si la programación del proyecto es de lunes a viernes durante 8 horas al día.

Se dan las siguientes situaciones:

* Si el proyecto no tiene un Horario, se tiene en cuenta el Horario predeterminado del sistema Workfront. Para obtener más información, consulte [Resumen de horarios](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Si el Horario es de lunes a viernes de 9 a. m. a 1 p. m. (4 horas al día) y las horas típicas por día laboral de su sistema Workfront son 8 horas, la fecha planificada de finalización es el 27 de enero.

>[!TIP]
>
>Workfront tiene en cuenta las excepciones de horario como los días festivos y los fines de semana al calcular las fechas planificadas de finalización.


