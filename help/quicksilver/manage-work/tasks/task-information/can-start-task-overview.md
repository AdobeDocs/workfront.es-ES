---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre "Puede comenzar" para tareas
description: Cuando una tarea está lista para empezar, Adobe Workfront añade el indicador “puede empezar” a la tarea para identificar fácilmente que es seguro que empiece a trabajar en ella. Puede ver este indicador en la vista de una lista de tareas o informes.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
TQID: https://experienceleague.adobe.com/jb8Vj9wMNCQj31cgjHMIm6M0RH3VusK5jBdNx233yjw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 440
ht-degree: 70%

---

# Información general sobre “Puede comenzar” para las tareas

Cuando una tarea está lista para empezar, Adobe Workfront añade el indicador “puede empezar” a la tarea para identificar fácilmente que es seguro que empiece a trabajar en ella. Puede ver este indicador en la vista de una lista de tareas o informes.

Cuando la tarea está lista para trabajar, el campo Puede comenzar de la tarea está establecido en verdadero.

## Cómo marca Workfront una tarea como &quot;Puede comenzar&quot;

Workfront comprueba lo siguiente antes de marcar una tarea como verdadero en el campo puede comenzar:

* Indica si el valor de Puede comenzar para el elemento principal se establece en Verdadero, si la tarea tiene un elemento principal. Si el valor de la tarea principal es falso, entonces todas las subtareas tendrán también el valor de puede comenzar establecido en falso.
* Si se han completado las tareas predecesoras de la tarea, así como las tareas predecesoras de sus padres. Si están completas, el valor puede comenzar para la tarea se establece en verdadero. Si alguno de los predecesores de la tarea o de sus predecesores principales no está completo o tiene el estado de completo-pendiente de aprobación, el valor de “puede comenzar” para la tarea se establece en falso.
* Si el tipo de dependencia de la tarea es Comienzo-Comienzo o Comienzo-Fin. Si el tipo de dependencia es Comienzo-Comienzo o Comienzo-Fin, la tarea dependiente tendrá el indicador &quot;Puede comenzar&quot; establecido en Verdadero después de que la tarea predecesora esté en curso (o después de que el porcentaje completado de la tarea predecesora sea mayor que 1%).

  Para obtener información acerca de las tareas predecesoras, consulte [Información general de las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Consideraciones acerca de la identificación de tareas listas para iniciarse

* Si el tipo de dependencia entre una tarea y sus predecesoras es de inicio a inicio, la predecesora debe comenzar antes de que se considere resuelta la relación y las tareas sucesoras puedan comenzar. Para obtener información acerca de los tipos de dependencia, consulte [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Si una tarea tiene una predecesora entre proyectos, la finalización de esta no activa automáticamente el indicador “puede comenzar” en la tarea sucesora. Debe recalcular manualmente la escala de tiempo del proyecto de la sucesora o Workfront debe recalcularla automáticamente, antes de que la tarea sucesora se muestre como tarea de Puede comenzar. Para obtener más información sobre cómo recalcular las escalas de tiempo de un proyecto, consulte [Recalcular escalas de tiempo de un proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Para obtener información sobre predecesores de proyectos cruzados, consulte [Crear predecesoras entre proyectos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
