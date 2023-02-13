---
product-area: templates
navigation-topic: templates-navigation-topic
title: Información general sobre los días de inicio y finalización en una plantilla
description: Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados a los proyectos de su organización. Aunque los proyectos tienen fechas de inicio y finalización específicas, las plantillas tienen días genéricos de inicio y finalización como indicación de dónde corresponderán esas fechas al proyecto, según el calendario general del proyecto.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Información general sobre los días de inicio y finalización en una plantilla

Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados a los proyectos de su organización. Aunque los proyectos tienen fechas de inicio y finalización específicas, las plantillas tienen días genéricos de inicio y finalización como indicación de dónde corresponderán esas fechas al proyecto, según el calendario general del proyecto.

**Ejemplo:** Si la fecha de inicio de un proyecto es el 1 de abril y desea que una tarea comience el 3 de abril (dos días después del inicio del proyecto), la tarea correspondiente de la plantilla que crea el proyecto debe comenzar el día 2 de la plantilla, donde el primer día de la plantilla se considera día 0.

## Día de inicio

Tenga en cuenta lo siguiente al trabajar con plantillas y tareas de plantilla:

* De forma predeterminada, las plantillas tienen un Día de inicio de 0 y las tareas de plantilla y la plantilla muestran un Día de inicio de 0. El día de inicio de las tareas de plantilla puede cambiar, pero esto no cambia el día de inicio de la plantilla.
* El día de inicio de una tarea de plantilla representa el número de días laborables que Workfront agrega a la fecha de inicio prevista de la tarea cuando se crea un proyecto a partir de la plantilla. Por ejemplo, puede tener una plantilla con una sola tarea y el día de inicio de la tarea de plantilla es 4. El día de inicio de la plantilla sigue siendo 0. Cuando crea un proyecto a partir de esta plantilla en la que el modo de programación del proyecto es la fecha de inicio y la fecha de inicio planeada del proyecto es el 1 de noviembre de 2019, la tarea recién creada agrega 4 días a esta fecha y establece su valor Fecha de inicio planeada en el 5 de noviembre de 2019.

A continuación se indican algunas acciones que pueden cambiar el Día de inicio de las tareas de plantilla:

* Actualizar la duración de las tareas de la plantilla predecesora
* Actualizar las restricciones de la tarea

   Al utilizar Restricciones de tarea basadas en datos, puede actualizar manualmente el Día de inicio de las tareas de plantilla. Algunos ejemplos de restricciones de tareas basadas en datos son Fechas fijas, No iniciar antes de, Iniciar antes de, No más tarde de, Debe comenzar el.

* Actualizar los predecesores de tareas de plantilla

## Día de finalización

El día de finalización de la plantilla es el día en que se completa la última tarea de plantilla. De forma predeterminada, todas las tareas de plantilla y la plantilla muestran un día de finalización de 1, ya que Workfront supone que cualquier tarea de plantilla tiene una duración de 1 día. El día de finalización de las tareas de plantilla puede cambiar y esto también cambia el día de finalización de la plantilla. El día de finalización de la plantilla se convierte en la fecha de finalización prevista del proyecto futuro y los días de finalización de las tareas de plantilla se convierten en las fechas de finalización previstas de las futuras tareas del proyecto.

A continuación se indican algunas acciones que podrían cambiar el día de finalización de las tareas de plantilla:

* Actualizar la duración de las tareas de plantilla
* Actualizar las restricciones de la tarea

   Al utilizar Restricciones de tarea basadas en datos, puede actualizar manualmente el día de finalización de las tareas de plantilla. Algunos ejemplos de restricciones de tareas basadas en datos son Fechas fijas, No finalizar antes de, No finalizar después de, Debe finalizar el.

* Actualizar los predecesores de tareas de plantilla

## Trabajar con plantillas programadas desde Finalización

Puede programar una plantilla desde el día de finalización. Para obtener más información, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Tenga en cuenta lo siguiente al trabajar con plantillas programadas desde la fecha de finalización:

* Si se cambia el día de inicio, la restricción de tareas se establece en Debe comenzar el.
* Si se cambia el día de finalización, la restricción de tareas se establece en Debe finalizar el.
* Cuando la plantilla está programada desde el día de finalización, el día de restricción de la tarea se calcula desde el día de finalización.

   **Ejemplo:** La duración de la plantilla es de 285 días y tiene una tarea de plantilla con una duración de 60 días. Si establece la Restricción de tarea en Debe comenzar en y Día de restricción en 120, tendrá un Día de inicio de 165 (285 - 120) y un Día de finalización de 225 (165 + 60). Así que cuando edita el Día de inicio, se interpreta como Día de restricción.
