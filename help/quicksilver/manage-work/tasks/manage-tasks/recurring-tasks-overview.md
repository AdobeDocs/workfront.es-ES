---
content-type: overview
product-area: projects
keywords: recurrente,recurrente,recurrente,recurrente
navigation-topic: manage-tasks
title: Información general sobre las tareas recurrentes
description: Información general sobre las tareas recurrentes
author: Alina
feature: Work Management
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 2%

---

# Información general sobre las tareas recurrentes

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

Puede crear tareas recurrentes para las actividades que tiene que repetir como parte de un solo proyecto.

Este artículo describe información y consideraciones sobre la creación y edición de tareas recurrentes.

Para obtener información sobre cómo crear tareas recurrentes en Adobe Workfront, consulte [Crear tareas recurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Información general y consideraciones sobre las tareas recurrentes

Puede elegir crear tareas recurrentes para indicar el trabajo repetible durante la vida de un proyecto.

Por ejemplo, durante un proyecto de TI, es probable que se deba realizar un backup del software a intervalos regulares. La creación de una tarea recurrente para esta actividad reduce el tiempo necesario para configurar varias tareas individuales.

Tenga en cuenta lo siguiente al crear tareas recurrentes en Workfront:

* No se pueden agregar tareas recurrentes a una plantilla.
* No se puede agregar una frecuencia de periodicidad a una tarea existente.
* Las tareas recurrentes aparecen como subtareas o como elementos secundarios para la incidencia principal que aparece como la tarea principal.
* No se puede adjuntar una aprobación a una tarea recurrente principal.
* Workfront transfiere la mayoría de los campos que actualiza para la periodicidad principal al crearla en las tareas secundarias. Los campos siguientes no se transfieren a las tareas secundarias cuando se crean:

   * La restricción de tareas de las tareas secundarias cambia automáticamente a:

      * Debe comenzar en los proyectos que estén planificados desde la fecha de inicio.
      * Debe Completar el para los proyectos planificados desde la fecha de finalización.
   * Los documentos adjuntos al padre no se transfieren a los hijos.


* Los siguientes cambios se producen en la tarea principal después de indicar que la tarea es recurrente:

   * El campo Duración cambia a Duración por incidencia para la tarea principal. Sigue siendo Duración para las tareas secundarias.
   * El estado está deshabilitado en la tarea principal y se establece automáticamente como Nuevo en los elementos secundarios. La tarea principal se completa automáticamente y el estado se actualiza a Complete cuando se completan todos los elementos secundarios.
   * Los únicos tipos de duración disponibles para tareas recurrentes son:

      * Sencilla
      * Condicionada por el esfuerzo

## Consideraciones para editar tareas recurrentes

Es posible que algunos cambios que realice en un elemento principal de tarea recurrente no se actualicen en todas las recurrencias existentes. Las tareas secundarias que muestran progreso o se han actualizado individualmente no se actualizarán al actualizar el elemento principal. Workfront considera que una tarea muestra el progreso en las siguientes situaciones:

* El estado se actualiza y la tarea ya no es New
* El porcentaje completado de la tarea es mayor que cero
* La tarea tiene relaciones predecesoras

La siguiente tabla ilustra si los cambios realizados en las actualizaciones del déclencheur principal en los elementos secundarios que no se han editado de forma individual o muestran el progreso:

| Campos actualizados en la tarea principal | Actualizaciones de la transferencia a niños sin editar o a niños sin progreso registrado |
|---|---|
| Frecuencia de periodicidad* | š |
| Asignaciones&#42;&#42; | ✔ |
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

&#42; Los siguientes escenarios existen cuando actualiza la Frecuencia de periodicidad de una tarea principal:

* Si cambia la Frecuencia de periodicidad en una tarea principal existente, las subtareas existentes se eliminan y se sustituyen por nuevas subtareas que siguen la nueva frecuencia de periodicidad si no muestran ningún progreso y si no las ha actualizado manualmente.
* Si cambia la Frecuencia de periodicidad en una tarea principal existente, las subtareas que muestran progreso no se eliminan. Estas tareas se consideran independientes de la recurrencia en este punto.

&#42;&#42; Las asignaciones realizadas en la tarea principal se aplican a todas las subtareas de la recurrencia. Cualquier cambio realizado en la asignación en la tarea principal anula cualquier asignación individual en la subtarea. Si la tarea muestra progreso, la asignación no cambia.

 
