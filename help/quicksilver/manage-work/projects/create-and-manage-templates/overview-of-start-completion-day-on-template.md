---
product-area: templates
navigation-topic: templates-navigation-topic
title: Información general sobre los días de inicio y finalización de una plantilla
description: Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados con los proyectos de su organización. Aunque los proyectos tienen fechas específicas de inicio y finalización, las plantillas tienen fechas genéricas de inicio y finalización que indican dónde caerán estas fechas en el proyecto, según la cronología general del proyecto.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 87%

---

# Información general sobre los días de inicio y finalización de una plantilla

Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados con los proyectos de su organización. Aunque los proyectos tienen fechas específicas de inicio y finalización, las plantillas tienen fechas genéricas de inicio y finalización que indican dónde caerán estas fechas en el proyecto, según la cronología general del proyecto.

**Ejemplo:** Si la fecha de inicio de un proyecto es el 1 de abril y desea que una tarea comience el 3 de abril (dos días después del inicio del proyecto), la tarea correspondiente de la plantilla que crea el proyecto debe comenzar el día 2 de la plantilla, donde el primer día de la plantilla se considera el día 0.

## Día de inicio

Tenga en cuenta lo siguiente al trabajar con plantillas y tareas de plantilla:

* De forma predeterminada, las plantillas tienen un día de inicio de 0, y las tareas de plantilla y la plantilla muestran un día de inicio de 0. El día de inicio de las tareas de plantilla puede cambiar, pero esto no cambia el día de inicio de la plantilla.
* El día de inicio de una tarea de plantilla representa el número de días laborables que Workfront añade a la fecha de inicio planificada de la tarea cuando se crea un proyecto a partir de la plantilla. Por ejemplo, puede tener una plantilla con una sola tarea cuyo día de inicio de la tarea de plantilla es 4. El día de inicio de la plantilla sigue siendo 0. Cuando crea un proyecto a partir de esta plantilla en el que el modo de programación del proyecto es Fecha de inicio y la fecha planificada de inicio del proyecto es el 1 de noviembre de 2019, la tarea recién creada añade 4 días a esta fecha y establece su valor de fecha de inicio planificada en el 5 de noviembre de 2019.

A continuación se indican algunas acciones que pueden cambiar el día de inicio de las tareas de plantilla:

* Actualizar la duración de las tareas de plantilla predecesoras
* Actualizar las restricciones de la tarea

  Al utilizar restricciones de tarea basadas en fechas, puede actualizar manualmente el día de inicio de las tareas de plantilla. Algunos ejemplos de restricciones de tareas basadas en fechas son Fechas fijas, No comenzar antes del, No comenzar después del, Debe comenzar el.

* Actualizar los predecesores de tareas de la plantilla

## Día de finalización

El día de finalización de la plantilla es el día en el que se completa la última tarea de plantilla. De forma predeterminada, todas las tareas de plantilla y la plantilla muestran un día de finalización de 1, ya que Workfront supone que cualquier tarea de plantilla tiene una duración de 1 día. El día de finalización de las tareas de plantilla puede cambiar, lo que también cambia el día de finalización de la plantilla. El día de finalización de la plantilla se convierte en la fecha planificada de finalización del futuro proyecto y los días de finalización de las tareas de plantilla se convierten en las fechas planificadas de finalización de las tareas futuras del proyecto.

A continuación se indican algunas acciones que pueden cambiar el día de finalización de las tareas de plantilla:

* Actualizar la duración de las tareas de plantilla
* Actualizar las restricciones de la tarea

  Al utilizar restricciones de tarea basadas en la fecha, puede actualizar manualmente el día de finalización de las tareas de plantilla. Algunos ejemplos de restricciones de tareas basadas en fechas son Fechas fijas, No finalizar antes del, No finalizar después del, Debe finalizar el.

* Actualizar los predecesores de tareas de la plantilla

## Trabajar con plantillas programadas desde la finalización

Puede programar una plantilla a partir del día de finalización. Para obtener más información, consulte [Edición de plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Tenga en cuenta lo siguiente al trabajar con plantillas programadas desde la fecha de finalización:

* Si se cambia el día de inicio, la restricción de tarea se establece en Debe comenzar el.
* Si se cambia el día de finalización, la restricción de tarea se establece en Debe finalizar el.
* Cuando la plantilla está programada desde el día de finalización, el día de restricción de la tarea se calcula a partir del día de finalización.

  **Ejemplo:** la duración de la plantilla es de 285 días y tiene una tarea de plantilla de 60 días. Si establece la restricción de tarea en Debe comenzar el y el día de restricción en 120, tendrá un día de inicio de 165 (285 - 120) y un día de finalización de 225 (165 + 60). Por lo tanto, cuando edita el Día de inicio, en realidad se interpreta como Día de restricción.
