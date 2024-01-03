---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Información general sobre predecesoras de tareas
description: Una predecesora es la tarea de la que depende otra tarea (denominada tarea sucesora o dependiente). Adobe Workfront admite cinco tipos de dependencias de predecesoras.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

# Información general sobre predecesoras de tareas

<!--Audited: 12/2023-->

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Una predecesora es la tarea de la que depende otra tarea (denominada tarea sucesora o dependiente). Adobe Workfront admite cinco tipos de dependencias de predecesoras. Para comprender las dependencias de predecesoras, consulte [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Información general sobre predecesoras

Es importante comprender la funcionalidad de predecesoras para comprender las escalas de tiempo de los proyectos.

Las relaciones de predecesoras de tareas existen tanto entre tareas de un mismo proyecto como entre tareas de distintos proyectos.

En el caso de dependencia entre proyectos, puede establecer predecesoras entre proyectos entre tareas de dos proyectos diferentes.

Tanto si las tareas predecesoras como sucesoras pertenecen al mismo proyecto o a dos proyectos diferentes, las dependencias y las escalas de tiempo de cada proyecto se calculan de la misma manera.

En el caso de las tareas predecesoras, la cronología del proyecto se ve afectada por lo siguiente:

* Dependencia de predecesora
* Valor de retardo y tipo\
  Para obtener más información sobre la dependencia y los retardos, consulte [Ejemplos de valores de predecesoras en una lista de tareas](#examples-of-predecessor-values-in-a-task-list).

  Por ejemplo, si la tarea A es la predecesora de la tarea B en una relación fin-comienzo y la tarea B tiene una delimitación de tarea de Lo antes posible, Workfront asigna a la tarea B una fecha de comienzo planificada inmediatamente después de la fecha de finalización planificada de la tarea A, independientemente de si la predecesora se aplica o no.

Para comprender las relaciones de predecesoras, debe comprender lo siguiente:

* **Tipos de dependencias:** Las predecesoras están vinculadas por varios tipos de dependencias. Para obtener más información sobre los tipos de dependencia, consulte [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Aplicar un predecesor:** Al aplicar una tarea predecesora, la tarea sucesora no se puede iniciar hasta que la predecesora finalice. La tarea sucesora se muestra como iniciándose inmediatamente después de que finalice la predecesora.

  Cuando la tarea predecesora no se completa (o inicia) y no se aplica, la tarea sucesora puede comenzar, pero la cronología del proyecto se ve afectada por las fechas de las tareas predecesoras y sucesoras.

  Con un predecesor forzado, Workfront no permite que la tarea sucesora se marque como En curso o Completada hasta que se complete el predecesor.

  Sin embargo, Workfront permite que se informe de las horas de la tarea.\
  Para obtener más información sobre cómo aplicar predecesoras, consulte [Forzar predecesoras](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Desfases:** Puede crear retardos en las dependencias que crean un retraso que debe producirse después de la finalización de una tarea predecesora y antes de que pueda comenzar la tarea sucesora. Los retrasos afectan a la cronología del proyecto.

  Para comprender los tipos de retardo, consulte [Resumen de tipos de retardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Crear relaciones de predecesoras

Para crear predecesoras, consulte cualquiera de los siguientes artículos:

* Para establecer predecesoras mediante la ficha Predecesoras de la tarea, consulte [Cree una relación de predecesoras mediante el área Predecesoras](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Para establecer predecesoras en una lista de tareas, consulte [Crear una relación de predecesoras en la lista de tareas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Para establecer relaciones de predecesoras encadenando tareas, consulte [Crear relaciones de predecesoras encadenando tareas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Para establecer predecesoras entre proyectos, consulte [Crear predecesoras entre proyectos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Busque las tareas predecesoras de una tarea {#locate-the-predecessors-of-a-task}

Para buscar las tareas predecesoras de una tarea, realice una de las siguientes acciones:

* Vaya al proyecto en el que está trabajando y haga lo siguiente:

   1. Busque la tarea para la que desea buscar las predecesoras y haga clic en la tarea.
   1. Clic **Predecesoras** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más**, entonces **Predecesoras**.
   1. El nombre del proyecto en el que se encuentra el predecesor se muestra en el **Proyecto** columna.

      El número del **#** muestra el número de tarea predecesora. Por ejemplo, &quot;6&quot; significa la sexta tarea del proyecto.

      ![Sección de predecesoras de la tarea](assets/predecessors-area-with-task-header.png)

* Vaya al proyecto en el que está trabajando y haga lo siguiente:

   1. Haga clic en **Tareas** pestaña.
   1. Elija la **Vista estándar** al principio de la lista de tareas.
   1. El **Predecesoras** muestra los números de las tareas predecesoras.

      Para una tarea predecesora entre proyectos, la columna Predecesoras muestra el número de referencia del proyecto al que pertenece la tarea predecesora y el número de la tarea, separados por dos puntos.

      El icono del predecesor se vuelve verde cuando la tarea del predecesor se marca como completada. Esto indica que la tarea dependiente está lista para trabajar.

      Pase el ratón sobre este valor para obtener más información sobre el predecesor, el proyecto y las fechas.

      ![Detalles de la predecesora](assets/predecessor-details-in-task-list.png)

## Ejemplos de valores de predecesoras en una lista de tareas {#examples-of-predecessor-values-in-a-task-list}

Cuando vea predecesoras en una lista de tareas, puede que vea cualquiera de los siguientes tipos de predecesoras con sus respectivos tipos de dependencia y cantidades de retardo:

* **1fs -** El número de tarea predecesora es 1. El tipo de dependencia es Fin-Inicio. En la escala de tiempo del proyecto, esta tarea está programada para iniciarse inmediatamente después de que finalice la tarea 1. A pesar de esto, aún puede marcarse como En curso o Completado.
* **1 -** El número de tarea predecesora es 1. Esto es lo mismo que **1fs**, porque **fs** es la relación de predecesora predeterminada en Workfront.

* **1fse -** El número de tarea predecesora es 1. El tipo de dependencia es Fin-Comienzo-Aplicado. En la escala de tiempo del proyecto, esta tarea se muestra como si comenzara inmediatamente después de que finalice la tarea 1. Workfront no permite que se marque como En curso o Completado hasta que se complete la tarea 1. Sin embargo, Workfront permite que se informe de las horas de la tarea.
* **1fs+3d -** El número de tarea predecesora es 1. El tipo de dependencia es Fin-Comienzo con un tiempo de retardo de 3 días. En la escala de tiempo del proyecto, esta tarea se muestra como el inicio de 3 días hábiles después de que finalice la tarea 1.
* **1fs-3d -** El número de tarea predecesora es 1. El tipo de dependencia es Fin-Comienzo con un tiempo de retardo de 3 días. En la escala de tiempo del proyecto, esta tarea se muestra como el comienzo de 3 días laborables antes de que finalice la tarea predecesora.
* **1fs+3de** -El número de tarea predecesora es 1. El tipo de dependencia es Fin-Comienzo-Aplicado con un tiempo de retardo de 3 días. En la escala de tiempo del proyecto, esta tarea se muestra como el inicio de 3 días hábiles después de que finalice la tarea 1. Workfront no permite que se marque como En curso o Completa hasta que se complete la Tarea 1. Sin embargo, Workfront permite que se informe de las horas de la tarea.

  >[!NOTE]
  >
  >Debe agregar el valor obligatorio (**e**) al modelo Lag, y no al predecesor.

* **4515:2** El número de tarea predecesora es 2. - Es una dependencia de tipo Fin a comienzo, no forzada, con el predecesor en el proyecto con número de referencia **4515**.

## Ver información de predecesoras

Puede ver la información de predecesoras en las siguientes áreas de Workfront. Esto incluye información sobre las tareas predecesoras entre proyectos:

* En el nivel de tarea, en la sección Predecesoras.

  Para obtener información acerca de cómo ver la información de predecesoras en la sección Predecesoras, vea la sección [Busque las tareas predecesoras de una tarea](#locate-the-predecessors-of-a-task) en este artículo.

* En el gráfico Gantt.

  Para obtener información acerca de cómo mostrar predecesoras en el gráfico Gantt, consulte [Configurar cómo se muestra la información en el gráfico Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* En una lista de tareas.

  Para ver información sobre las tareas predecesoras de las tareas en una lista de tareas, puede realizar una de las siguientes acciones:

   * Aplicar la vista estándar integrada en una lista de tareas.

     Para obtener información acerca de cómo ver la información de predecesoras en la vista Estándar, vea la sección [Busque las tareas predecesoras de una tarea](#locate-the-predecessors-of-a-task) en este artículo.

   * Cree una vista de tareas o un informe y agregue la columna Predecesoras a esa vista.

     Para obtener más información sobre la creación de una vista personalizada para tareas con información de predecesoras, consulte [Ver: detalles de predecesoras](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* En el encabezado de la tarea al acceder a la tarea.

  ![](assets/qs-predecessor-info-in-task-header-350x141.png)
