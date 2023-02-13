---
product-area: projects
navigation-topic: issue-information
title: Descripción general del problema Fecha de finalización prevista
description: La fecha de finalización prevista de una emisión es la fecha en la que se espera que se complete la emisión.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Descripción general del problema Fecha de finalización prevista

La fecha de finalización prevista de una emisión es la fecha en la que se espera que se complete la emisión.

Puede especificar la fecha de finalización planeada de un problema o dejar que Adobe Workfront lo calcule según ciertos criterios. 

Las fechas de finalización previstas de las emisiones no afectan a la fecha de finalización prevista del proyecto. Solo las fechas de finalización previstas de las tareas afectan a la fecha de finalización prevista del proyecto. Para obtener más información sobre la fecha de finalización prevista del proyecto, consulte [Establecer la fecha de finalización prevista del proyecto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La fecha de finalización prevista de una emisión difiere de la fecha de finalización de la emisión o de la fecha de finalización prevista de la emisión de las siguientes maneras:
>
>* La fecha de confirmación es la fecha en la que la persona asignada al problema calcula manualmente que habrá completado el problema. Para obtener más información, consulte los siguientes artículos:
   * [Resumen de la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [Interacciones entre la fecha de confirmación y la fecha de finalización prevista](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* La fecha de finalización prevista es una fecha calculada por Workfront que tiene en cuenta factores externos para determinar una fecha de vida real para la cual el problema se puede completar de forma realista. Para obtener más información, consulte [Información general sobre la fecha de finalización prevista para proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## Establecer manualmente la fecha de finalización planeada de un problema

Debe tener acceso de edición a problemas y permisos de administración del problema para poder actualizar la fecha de finalización planeada del problema.

Puede establecer manualmente la fecha de finalización planeada de un problema en las siguientes áreas de Workfront:

* En el cuadro Editar problema o en el área Detalles del problema al crear o editar un problema. Para obtener más información, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).
* En el área de inicio si se muestra la fecha de finalización planeada al ver un problema. Para obtener más información, consulte [Actualizar o editar un elemento de trabajo en el área principal](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* En el encabezado del problema. Para obtener más información, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* En una lista de problemas o informe cuando se muestra en la vista el campo Fecha de finalización planeada .

   Para obtener más información, consulte [Editar problemas en una lista](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Cómo calcula Workfront automáticamente la fecha de finalización prevista de un problema

Cuando Workfront calcula automáticamente la fecha de finalización planeada de un problema, lo siguiente puede influir en la fecha:

* Fecha de inicio planeada

   La fecha de entrada y la fecha de inicio planeada deben coincidir en un problema cuando se crea el problema por primera vez.

* La duración predeterminada tal como se configura en la sección Detalles de cola del proyecto. Para obtener más información, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Si la duración predeterminada es 0 días, la fecha de finalización planeada coincide con la fecha de inicio planeada del problema.

* Programación del proyecto

Cuando se configura automáticamente, la fecha de finalización planeada se determina según el siguiente cálculo: 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Ejemplo:** Por ejemplo, si la tarea tiene una fecha de inicio de viernes, 14 de enero y la duración predeterminada es de 5 días, la fecha de finalización planeada es viernes, 21 de enero, si la programación del proyecto es de lunes a viernes durante 8 horas al día.

Existen las siguientes situaciones:

* Si el proyecto no tiene una programación, se tiene en cuenta la programación predeterminada del sistema de Workfront. Para obtener más información, consulte [Información general sobre las programaciones](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Si el horario es de lunes a viernes de 9:00 a 1:00 (4 horas al día) y el horario habitual del sistema de Workfront es de 8 horas, la fecha de finalización prevista es el 27 de enero.

>[!TIP]
Workfront tiene en cuenta las excepciones de programación, como los días festivos y los fines de semana, al calcular las fechas de finalización planificadas.

 
