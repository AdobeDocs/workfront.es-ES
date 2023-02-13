---
product-area: reporting
navigation-topic: reporting-elements
title: Uso de la vista Milestone
description: Puede aplicar la vista Milestone a una lista de proyectos o a un informe.
author: Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: dcdcf21903d0fceb3c05039689bb87ae4c834d07
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 1%

---

# Uso de la vista Milestone

Puede aplicar la vista Milestone a una lista de proyectos o a un informe.

Para poder utilizar la vista de hitos, es necesario configurar los hitos, agregar las rutas de hitos a los proyectos y asociar los hitos a las tareas, tal como se describe en los artículos [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) y [Asociar hitos con tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

La vista Milestone está disponible cuando se visualiza una lista de proyectos o un informe de proyecto. En las secciones siguientes se describe cómo ver y utilizar la vista de hitos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Trabajo o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Ver o tener más acceso a Informes, Tableros y Calendarios</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver permisos de un informe de proyecto para aplicar la vista Milestone a un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Cambiar a la vista Milestone {#switch-to-the-milestone-view}

1. Vaya a la lista de proyectos o al informe de proyecto que contiene los hitos que desea ver.
1. Haga clic en el **Ver** menú desplegable y haga clic en **Milestone**.

   La lista o el informe se muestra en una vista Milestone.

   Para obtener información sobre la vista de hito, consulte la sección [Información general sobre la vista Milestone](#milestone-view-overview) en este artículo.

## Información general sobre la vista Milestone {#milestone-view-overview}

La vista Milestone está disponible en listas de proyectos e informes de proyectos. Esta vista le permite ver rápidamente todos los hitos asociados con tareas dentro de los proyectos que está viendo.


>[!NOTE]
>
>La vista Milestone no está disponible en las siguientes áreas:
>* Hojas de tiempo, en la lista de proyectos al agregar un proyecto.



Para obtener información sobre cómo cambiar a la vista Milestone, consulte la sección [Cambiar a la vista Milestone](#switch-to-the-milestone-view) en este artículo.

![Proyecto con vista de hito](assets/project-with-milestone-view-with-complete.png)

### Secciones de vista de Milestone

Al aplicar la vista Milestone a una lista de proyectos, los proyectos se muestran en las secciones siguientes:

* Los proyectos asociados a una ruta de hitos aparecen primero, enumerados con el nombre de sus rutas de hitos respectivas.

   Workfront ordena los proyectos de la primera sección según los criterios siguientes, en este orden:

   1. Identificador de la ruta de hitos. Puede ver el ID de ruta de Milestone en un informe de ruta de Milestone.

   2. El campo seleccionado como primer campo de clasificación para la lista de proyectos en la vista aplicada anteriormente a la lista de proyectos, antes de seleccionar la vista Milestone.

* A continuación, en la sección Sin asignar , se muestran los proyectos que no están asociados a una ruta de hitos. Workfront ordena los proyectos en la sección Sin asignar por el campo seleccionado como el primer campo de clasificación para la lista de proyectos en la vista previamente aplicada a la lista de proyectos, antes de seleccionar la vista Milestone.

### Información del proyecto en la vista Milestone

Cuando se visualiza una lista de proyectos o un informe de proyectos en la vista Milestone, está disponible la siguiente información:

* **Fechas planificadas o fechas proyectadas:** Especifique si desea mostrar Fechas planificadas o Fechas proyectadas en la vista Milestone.\
   Las fechas se muestran para el inicio y la finalización, así como para cada hito dentro de la ruta de Milestone.\
   Si está viendo Fechas planificadas y también tiene acceso de Administrar al proyecto, puede editar las siguientes fechas directamente desde la vista Milestone: (Si está viendo Fechas proyectadas, las fechas no se pueden editar porque las Fechas proyectadas se calculan y no se pueden cambiar manualmente).

   * **Fechas de inicio del proyecto:** Si un proyecto está programado desde la fecha de inicio, puede cambiar manualmente la fecha de inicio del proyecto y, a continuación, calcular la fecha de finalización.
   * **Fechas de finalización del proyecto:** Si un proyecto está programado desde la fecha de finalización, puede cambiar manualmente la fecha de finalización del proyecto y, a continuación, calcular la fecha de inicio.
   * **Fechas de finalización de la tarea:** Puede actualizar manualmente Finalización para tareas directamente desde la vista Milestone.

* **Porcentaje completado:** Muestra el porcentaje de finalización de cada tarea y proyecto.\
   Puede desactivar la visualización del porcentaje de finalización, tal como se describe en la sección [Configurar la información que se muestra en la vista Milestone](#configure-what-information-displays-in-the-milestone-view) en este artículo.\
   Puede ajustar el porcentaje de finalización directamente desde la vista Milestone, tal como se describe en la sección [Ajustar porcentaje completado para tareas en la vista Milestone](#adjust-percent-complete-for-tasks-in-the-milestone-view) en este artículo.

* **Iconos de estado de tarea:** Se muestra un icono de estado junto a cada proyecto y tarea en la vista Milestone.

   * A tiempo\
      ![](assets/gantt-ontime.png)

   * Rezagado\
      ![](assets/gantt-behind.png)

   * En riesgo\
      ![](assets/gantt-atrisk.png)

   * Retrasado\
      ![](assets/gantt-late.png)
   Puede desactivar la visualización de estos iconos de estado, tal como se describe en la sección [Configurar la información que se muestra en la vista Milestone](#configure-what-information-displays-in-the-milestone-view) en este artículo.\
   Para obtener información más detallada sobre cada tipo de estado, consulte el artículo [Información general sobre el estado de progreso de la tarea](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Sombreado de estado de tarea para tareas completadas**: Después de marcar una tarea como Completada, el fondo de la tarea aparece sombreado en la vista Milestone para indicar si la tarea se completó a tiempo o tarde:

   * **Sombreado rojo para la columna de tareas**: El fondo de una tarea aparece en rojo cuando el estado de progreso es **Late**.

   * **Sombreado verde para la columna de tarea**: El fondo de una tarea aparece en verde cuando el estado de progreso es **Tiempo de activación**.

* **Sombreado del estado del proyecto para las columnas Inicio y Finalización del proyecto**:

   * **Columna Inicio del proyecto**: El fondo de la columna Inicio del proyecto solo es rojo o verde cuando se rellena la fecha de inicio real:

      * **Sombreado rojo para la columna Inicio del proyecto**: El fondo de la columna Inicio del proyecto aparece en rojo cuando el estado de progreso del proyecto es **Late**.

      * **Sombreado verde para la columna Inicio del proyecto**: El fondo de la columna Inicio del proyecto aparece en verde cuando el estado de progreso del proyecto es **Tiempo de activación**.
   * **Columna Finalización del proyecto**: El fondo de la columna Finalización del proyecto solo está rojo o verde cuando se rellena la fecha de finalización real:

      * **Sombreado rojo para la columna Finalización del proyecto**: El fondo de la columna Finalización del proyecto aparece en rojo cuando el estado de progreso del proyecto es **Late**.

      * **Sombreado verde para la columna Finalización del proyecto**: El fondo de la columna Finalización del proyecto aparece en verde cuando el estado de progreso del proyecto es **Tiempo de activación**.
   * No se asigna ningún sombreado de color a las columnas Inicio y Finalización cuando las tareas tienen un estado de progreso de En riesgo o Detrás.

   ![Vista Milestone con sombreado](assets/milestone-view-with-shading.png)

* **Nombre del proyecto**: El nombre del proyecto se muestra con un vínculo al proyecto.
* **Icono de condición del proyecto**: Al lado del nombre del proyecto se muestra un icono que indica la condición del proyecto.

## Configurar la información que se muestra en la vista Milestone {#configure-what-information-displays-in-the-milestone-view}

Puede configurar si los siguientes elementos se muestran en la vista Milestone:

* Iconos de estado de progreso
* Porcentaje completado de proyectos y tareas

De forma predeterminada, se muestran los iconos de estado del proyecto y el porcentaje completado de los proyectos.

Los cambios que realice en estas opciones solo se aplicarán a usted; otros usuarios no se ven afectados. Los cambios que realice se mantendrán la próxima vez que inicie sesión en Adobe Workfront.

Para configurar si se muestran los iconos de estado del proyecto y el porcentaje de finalización de los proyectos:

1. Vaya a la lista de proyectos o al informe de proyecto que contiene los hitos que desea ver.
1. Haga clic en el **Ver** menú desplegable y haga clic en **Milestone**.\
   Si está viendo una lista de proyectos dentro de un Portfolio o un programa, seleccione la **Milestone** subpestaña .

1. Haga clic en **Opciones** en la esquina superior derecha de la vista Milestone.\
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Estado de progreso</td> 
      <td> <p>Seleccione esta opción para mostrar los iconos de estado del progreso junto a cada proyecto y tarea.</p> <p>Esta opción está activada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Porcentaje completado</td> 
      <td> <p>Seleccione esta opción para mostrar el porcentaje de finalización junto a cada proyecto y tarea.</p> <p>Esta opción está activada de forma predeterminada.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Ajustar porcentaje completado para tareas en la vista Milestone {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Puede ajustar el porcentaje completado para las tareas en la vista Milestone. No se puede ajustar el porcentaje completado para una tarea principal (una tarea que contiene subtareas).

Para ajustar el porcentaje completado de una tarea en la vista Milestone:

1. Vaya a la lista de proyectos o al informe de proyecto que contiene los hitos que desea ver.
1. Haga clic en el **Ver** menú desplegable y haga clic en **Milestone**.

1. (Condicional) Si los porcentajes de finalización no se muestran actualmente en la vista Milestone, haga clic en **Opciones** en la esquina superior derecha de la vista Milestone, asegúrese de que **Porcentaje completado** está activada.

1. Haga clic en el porcentaje de finalización debajo de una tarea, especifique un nuevo porcentaje y, a continuación, pulse Intro.
