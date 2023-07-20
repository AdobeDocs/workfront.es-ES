---
content-type: overview
product-area: projects
keywords: recurrente, recurrente, recurrente
navigation-topic: manage-tasks
title: Información general sobre tareas recurrentes
description: Información general sobre tareas recurrentes
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 3%

---

# Información general sobre tareas recurrentes

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

Puede crear tareas recurrentes para actividades que tenga que repetir como parte de un solo proyecto.

Este artículo describe información y consideraciones sobre la creación y edición de tareas recurrentes.

Para obtener información sobre cómo crear tareas recurrentes en Adobe Workfront, consulte [Creación de tareas recurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Información general y consideraciones sobre tareas recurrentes

Puede optar por crear tareas recurrentes para indicar el trabajo repetible durante la duración de un proyecto.

Por ejemplo, durante un proyecto de TI, es probable que deba realizarse un backup del software a intervalos regulares. La creación de una tarea recurrente para esta actividad reduce el tiempo necesario para configurar varias tareas individuales.

Tenga en cuenta lo siguiente al crear tareas recurrentes en Workfront:

* No puede agregar tareas recurrentes a una plantilla.
* No puede agregar una frecuencia de periodicidad a una tarea existente.
* Las tareas recurrentes aparecen como subtareas o tareas secundarias para la ocurrencia principal que aparece como la tarea principal.
* No puede adjuntar una aprobación a una tarea principal recurrente.
* Workfront transfiere la mayoría de los campos que se actualizan para la periodicidad principal al crearlos a las tareas secundarias. Los campos siguientes no transfieren a las tareas secundarias cuando se crean:

   * La restricción de tarea de las tareas secundarias cambia automáticamente a:

      * Debe comenzar el para los proyectos planificados desde la fecha de inicio.
      * Debe completarse el para los proyectos planificados desde la fecha de finalización.

   * Los documentos adjuntos al padre no se transfieren a los hijos.

* Los siguientes cambios se producen en la tarea principal después de indicar que la tarea es recurrente:

   * El nombre del campo Duración cambia a Duración por resolicitud para la tarea principal. Permanece Duración para las tareas secundarias.
   * El estado se desactiva en la tarea principal y se establece automáticamente en Nuevo en las tareas secundarias. La tarea principal se completa automáticamente y el estado se actualiza a Completo cuando se completan todos los elementos secundarios.
   * Los únicos tipos de duración disponibles para tareas recurrentes son:

      * Sencilla
      * Condicionada por el esfuerzo
* La Duración y las Horas planificadas indicadas para una nueva tarea recurrente son la Duración y las Horas planificadas de cada ocurrencia. La duración de la tarea principal es el tiempo entre la fecha planificada de inicio de la tarea más temprana y la fecha planificada de finalización de la tarea más reciente. Las horas planificadas de la tarea principal son el total de todas las horas planificadas de todas las ocurrencias.

## Consideraciones para editar tareas recurrentes

Es posible que algunos cambios que realice en una tarea principal recurrente no se actualicen en todas las repeticiones existentes. Las tareas secundarias que muestran progreso o que se han actualizado individualmente no se actualizarán cuando actualice el principal. Workfront considera que una tarea muestra el progreso en las siguientes situaciones:

* El estado se actualiza y la tarea deja de ser New
* El porcentaje completado de la tarea es mayor que cero
* La tarea tiene relaciones de predecesora

La siguiente tabla ilustra si los cambios realizados en el déclencheur principal se actualizan en los elementos secundarios que no se han editado individualmente o si muestran progreso:

| Campos actualizados en la tarea principal | Las actualizaciones se transfieren a elementos secundarios sin editar o elementos secundarios sin progreso registrado |
|---|---|
| Frecuencia de periodicidad* | ✔ |
| Asignaciones | ✔ |
| Nombre | ✔ |
| Descripción | ✔ |
| Prioridad | ✔ |
| Duración | ✔ |
| Horas planificadas | ✔ |
| Tipo de costo | ✔ |
| Tipo de ingresos | ✔ |
| Nivelación de recursos | ✔ |
| Retraso de nivelación | ✔ |
| Restricción de tarea | No actualiza los elementos secundarios |
| Adjuntar o quitar Forms personalizado | No actualiza los elementos secundarios |
| Tipo de duración | No actualiza los elementos secundarios |
| Información de formulario personalizado | No actualiza los elementos secundarios |

{style="table-layout:auto"}

&#42; Cuando se actualiza la frecuencia de periodicidad de una tarea principal, existen los siguientes escenarios:

* Si cambia la Frecuencia de periodicidad en una tarea principal existente, las subtareas existentes se eliminan y reemplazan por nuevas subtareas que siguen a la nueva frecuencia de periodicidad si no muestran ningún progreso y si no las ha actualizado manualmente.
* Si cambia la Frecuencia de periodicidad en una tarea principal existente, las subtareas que muestran progreso no se eliminan. Estas tareas se consideran separadas de la periodicidad en este punto.

&#42;&#42; Las asignaciones realizadas en la tarea principal se aplican a todas las subtareas de forma recurrente. Cualquier cambio realizado en la asignación de la tarea principal anula cualquier asignación individual de la subtarea. Si la tarea muestra progreso, la asignación no cambia.

 
