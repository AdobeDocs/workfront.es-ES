---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Descripción general de las predecesoras de tareas
description: Un predecesor es la tarea de la que depende otra tarea (denominada tarea sucesora o dependiente). Adobe Workfront admite cinco tipos de dependencias predecesoras.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---

# Descripción general de las predecesoras de tareas

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Un predecesor es la tarea de la que depende otra tarea (denominada tarea sucesora o dependiente). Adobe Workfront admite cinco tipos de dependencias predecesoras. Para comprender las dependencias predecesoras, consulte [Descripción general de los tipos de dependencia de tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Información general sobre los predecesores

Comprender la funcionalidad del predecesor es importante para comprender las cronologías de sus proyectos.

Existen relaciones de predecesor entre tareas tanto dentro de un único proyecto como entre varios proyectos.

En el caso de la dependencia de varios proyectos, puede establecer predecesores entre proyectos.

Tanto si las tareas predecesoras como las sucesoras pertenecen al mismo proyecto o a dos proyectos diferentes, las dependencias y las líneas de tiempo se calculan del mismo modo.

En cuanto a los predecesores, la cronología del proyecto se ve afectada por lo siguiente:

* Dependencia del predecesor
* Valor y tipo de registro\
   Para obtener más información sobre dependencia y etiquetas, consulte [Ejemplos de valores predecesores en una lista de tareas](#examples-of-predecessor-values-in-a-task-list).

Por ejemplo, si la tarea A es la predecesora de la tarea B en una relación de finalización-inicio y la tarea B tiene una restricción de tareas de Tan pronto como sea posible, Workfront asigna la tarea B a una fecha de inicio planificada inmediatamente después de la fecha de finalización planificada de la tarea A, independientemente de si la predecesora se aplica o no.

Para comprender las relaciones predecesoras, debe comprender:

* **Tipos de dependencia:** Los predecesores están vinculados por varios tipos de dependencia. Para obtener más información sobre los tipos de dependencia, consulte [Descripción general de los tipos de dependencia de tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Ejecución de un predecesor:** Al aplicar un predecesor, la tarea sucesora no puede comenzar hasta que se complete el predecesor. La tarea sucesora se muestra como comenzando inmediatamente después de que finalice el predecesor.

   Workfront no permite que se marque como In Progress o Complete hasta que se complete el predecesor. Sin embargo, Workfront permite que se informe de horas sobre la tarea.\
   Para obtener más información sobre cómo aplicar predecesores, consulte [Aplicar predecesores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Etiquetas:** Puede crear etiquetas en las dependencias que creen un retraso que debe producirse tras la finalización de una tarea predecesora y antes de que pueda comenzar la tarea sucesora. Los retrasos afectan a la cronología del proyecto.

   Para comprender los tipos de retraso, consulte [Descripción general de los tipos de retraso](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Crear relaciones predecesoras

Para crear predecesores, consulte cualquiera de los siguientes artículos:

* Para establecer predecesores con la ficha Predecesores de la tarea, consulte [Crear una relación predecesora con el área Predecesoras](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Para establecer predecesores en una lista de tareas, consulte [Crear una relación predecesora en la lista de tareas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Para establecer relaciones predecesoras encadenando tareas, consulte [Crear relaciones de predecesor encadenando tareas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Para establecer predecesores entre proyectos, consulte [Crear predecesores entre proyectos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Localización de los predecesores de una tarea {#locate-the-predecessors-of-a-task}

Para buscar los predecesores de una tarea, realice una de las siguientes acciones:

* Vaya al proyecto en el que está trabajando y haga lo siguiente:

   1. Busque la tarea para la que desea buscar los predecesores y haga clic en la tarea.
   1. Haga clic en **Predecesores** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más**, luego **Predecesores**.
   1. El nombre del proyecto en el que se encuentra el predecesor se muestra en la **Proyecto** para abrir el Navegador.

      El número de la variable **#** muestra el número de tarea predecesor. Por ejemplo, &quot;6&quot; significa la sexta tarea del proyecto.

      ![Sección Predecesoras de la tarea](assets/predecessors-area-with-task-header.png)

* Vaya al proyecto en el que está trabajando y haga lo siguiente:

   1. Haga clic en el **Tareas** pestaña .
   1. Elija la **Vista estándar** en la parte superior de la lista de tareas.
   1. La variable **Predecesores** muestra los números de la tarea predecesora.

      Para un predecesor de varios proyectos, la columna Predecesores muestra el número de referencia del proyecto al que pertenece el predecesor y el número de la tarea, separados por dos puntos.

      El icono predecesor se vuelve verde cuando la tarea predecesora se marca como completada. Esto indica que la tarea dependiente está lista para funcionar.

      Pase el ratón sobre este valor para obtener más información sobre el predecesor, el proyecto y las fechas.

      ![Detalles del predecesor](assets/predecessor-details-in-task-list.png)

## Ejemplos de valores predecesores en una lista de tareas {#examples-of-predecessor-values-in-a-task-list}

Cuando vea predecesores en una lista de tareas, es posible que vea cualquiera de los siguientes tipos de predecesores con sus respectivos tipos de dependencias e importes de retraso:

* **1fs -** El número de tarea predecesora es 1. El tipo de dependencia es Finish-Start. En la cronología del proyecto, esta tarea está programada para iniciarse inmediatamente después de que finalice la tarea 1. A pesar de esto, puede seguir siendo marcado como In Progress o Complete.
* **1 -** El número de tarea predecesora es 1. Esto es igual que **1fs**, porque **fs** es la relación predecesora predeterminada en Workfront.

* **1fse -** El número de tarea predecesora es 1. El tipo de dependencia es Finish-Start-Enforced. En la cronología del proyecto, esta tarea se muestra como comenzando inmediatamente después de finalizar la tarea 1. Workfront no permite que se marque como In Progress o Complete hasta que se complete la tarea 1. Sin embargo, Workfront permite que se informe de horas sobre la tarea.
* **1fs+3d -** El número de tarea predecesora es 1. El tipo de dependencia es Finish-Start con un tiempo de retraso de 3 días. En la línea de tiempo del proyecto, esta tarea se muestra como comenzando 3 días laborables después de que la tarea 1 haya finalizado.
* **1fs-3d -** El número de tarea predecesora es 1. El tipo de dependencia es Finish-Start con un tiempo de retraso de 3 días. En la cronología del proyecto, esta tarea se muestra como 3 días laborables antes de que finalice la tarea predecesora.
* **1fs+3de** -El número de tarea predecesora es 1. El tipo de dependencia es Finish-Start-Enforced con un tiempo de retraso de 3 días. En la línea de tiempo del proyecto, esta tarea se muestra como comenzando 3 días laborables después de que la tarea 1 haya finalizado. Workfront no permite que se marque como In Progress o Complete hasta que se complete la tarea 1. Sin embargo, Workfront permite que se informe de horas sobre la tarea.

   >[!NOTE]
   >
   >El valor forzado (**e**) debe agregarse al registro, no al predecesor.

* **4515:2** El número de tarea predecesora es 2. - Es una dependencia de tipo Fin a Inicio, no forzada, con el predecesor del proyecto con número de referencia **4515**; el número de tarea predecesora es **2**.

## Ver información de predecesor

Puede ver la información del predecesor en las siguientes áreas de Workfront. Esto incluye información sobre los predecesores entre proyectos:

* En el nivel de tarea, en la sección Predecesores .

   Para obtener información sobre la visualización de la información predecesora en la sección Predecesores , consulte la sección [Localización de los predecesores de una tarea](#locate-the-predecessors-of-a-task) en este artículo.

* En el diagrama de Gantt.

   Para obtener información sobre cómo mostrar los predecesores en el diagrama de Gantt, consulte [Configurar cómo se muestra la información en el diagrama de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* En una lista de tareas.

   Para ver información sobre los predecesores de las tareas en una lista de tareas, puede realizar una de las siguientes acciones:

   * Aplique la vista estándar integrada en una lista de tareas.

      Para obtener información sobre la visualización de la información predecesora en la vista Estándar, consulte la sección [Localización de los predecesores de una tarea](#locate-the-predecessors-of-a-task) en este artículo.

   * Cree una vista de tarea o un informe y añada la columna Predecesores a esa vista.

      Para obtener más información sobre la creación de una vista personalizada para las tareas con información de predecesor, consulte [Ver: detalles del predecesor](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* En el encabezado de la tarea al acceder a la tarea.

   ![](assets/qs-predecessor-info-in-task-header-350x141.png)
