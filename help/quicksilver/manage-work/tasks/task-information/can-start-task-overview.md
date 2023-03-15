---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Descripción general de '`Can Start` para las tareas'
description: Cuando una tarea está lista para iniciarse, Adobe Workfront agrega un indicador de "Puede comenzar" a la tarea para identificar fácilmente que es seguro comenzar a trabajar en ella. Puede ver este indicador en la vista de una lista de tareas o de un informe.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Información general sobre &quot;Can Start&quot; para tareas

Cuando una tarea está lista para iniciarse, Adobe Workfront agrega un indicador de &quot;Puede comenzar&quot; a la tarea para identificar fácilmente que es seguro comenzar a trabajar en ella. Puede ver este indicador en la vista de una lista de tareas o de un informe.

Cuando la tarea está lista para su trabajo, el campo Puede comenzar de la tarea se establece en True.

## Cómo marca Workfront una tarea como &quot;Puede comenzar&quot;

Workfront comprueba los siguientes elementos antes de marcar una tarea como True en el campo Can Start :

* Si la tarea tiene un elemento principal, comprueba si el valor de Can Start para el elemento principal que estableció es True. Si el valor del elemento principal es False, todas las subtareas tendrán también el valor Puede comenzar establecido en False. 
* También comprueba si los predecesores de la tarea y los predecesores de sus padres están completos. Si se han completado, el valor Puede comenzar para la tarea se establece en Verdadero. Si alguno de los predecesores de tareas o los predecesores de sus padres no están completos o tienen un estado de Aprobación Completa Pendiente, el valor Puede Iniciar para la tarea se establece en False. 

   Para obtener información sobre las predecesoras de tareas, consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Consideraciones sobre la identificación de tareas listas para iniciarse

* Si el Tipo de dependencia entre una tarea y sus predecesores es Start-Start, el predecesor debe comenzar antes de que se considere que la relación predecesora se ha resuelto y que las tareas sucesoras puedan iniciarse. Para obtener información sobre los tipos de dependencia, consulte [Descripción general de los tipos de dependencia de tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Si una tarea tiene un predecesor entre proyectos, la finalización del predecesor no déclencheur que el indicador Puede comenzar se aplique automáticamente al sucesor. Debe volver a calcular manualmente la escala de tiempo del proyecto del sucesor o Workfront debe recalcularlo automáticamente antes de que la tarea sucesora se muestre como una tarea Puede comenzar. Para obtener más información sobre cómo recalcular las líneas de tiempo del proyecto, consulte [Volver a calcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   Para obtener información sobre los predecesores entre proyectos, consulte [Crear predecesores entre proyectos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
