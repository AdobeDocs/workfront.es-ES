---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre "Puede comenzar" para tareas
description: Cuando una tarea está lista para iniciarse, Adobe Workfront agrega un indicador Puede comenzar a la tarea para identificar fácilmente que es seguro comenzar a trabajar en la tarea. Puede ver este indicador en la vista de una lista de tareas o un informe.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Información general sobre &quot;Puede comenzar&quot; para las tareas

Cuando una tarea está lista para iniciarse, Adobe Workfront agrega un indicador Puede comenzar a la tarea para identificar fácilmente que es seguro comenzar a trabajar en la tarea. Puede ver este indicador en la vista de una lista de tareas o un informe.

Cuando la tarea está lista para trabajar, el campo Puede comenzar de la tarea está establecido en Verdadero.

## Cómo marca Workfront una tarea como &quot;Puede comenzar&quot;

Workfront comprueba lo siguiente antes de marcar una tarea como True en el campo Puede comenzar:

* Si la tarea tiene un elemento principal, comprueba si el valor de Puede comenzar para el elemento principal que estableció en Verdadero. Si el valor de la tarea principal es False, entonces todas las subtareas tendrán también el valor de Puede comenzar establecido en False. 
* También comprueba si las tareas predecesoras de la tarea, así como las predecesoras de sus elementos primarios, están completas. Si están completas, el valor Puede comenzar para la tarea se establece en Verdadero. Si alguno de los predecesores de la tarea o de sus predecesores principales no está completo o tiene el estado de Completo-Pendiente de aprobación, el valor de Puede comenzar para la tarea se establece en Falso. 

  Para obtener información acerca de las tareas predecesoras, vea [Descripción general de las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Consideraciones acerca de la identificación de tareas listas para iniciarse

* Si el tipo de dependencia entre una tarea y sus predecesoras es Start-Start, la predecesora debe iniciarse antes de que la relación de predecesoras se considere resuelta y se puedan iniciar las tareas sucesoras. Para obtener información acerca de los tipos de dependencia, vea [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Si una tarea tiene una predecesora entre proyectos, la finalización de la predecesora no almacena en déclencheur el indicador Puede comenzar para que se aplique a la sucesora automáticamente. Debe recalcular manualmente la escala de tiempo del proyecto de la sucesora o Workfront debe recalcularla automáticamente, antes de que la tarea sucesora se muestre como tarea de Puede comenzar. Para obtener más información sobre cómo recalcular las escalas de tiempo de un proyecto, vea [Recalcular escalas de tiempo de un proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Para obtener información acerca de las tareas predecesoras entre proyectos, vea [Crear tareas predecesoras entre proyectos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
