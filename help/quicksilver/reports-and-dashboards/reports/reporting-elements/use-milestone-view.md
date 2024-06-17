---
product-area: reporting
navigation-topic: reporting-elements
title: Uso de la vista de Hito
description: Puede aplicar la vista de Hito a una lista de proyectos o a un informe.
author: Nolan
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1302'
ht-degree: 0%

---

# Uso de la vista de Hito

<!-- Audited: 1/2024 -->

Puede aplicar la vista de Hito a una lista de proyectos o a un informe.

Antes de poder utilizar la vista de hito, es necesario configurar los hitos, añadir las rutas de hitos a los proyectos y asociar los hitos a las tareas, tal como se describe en los artículos [Creación de una trayectoria del hito](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) y [Asociar hitos a tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

La vista Hito está disponible cuando se visualiza una lista de proyectos o un informe de proyectos. En las secciones siguientes se describe cómo ver y utilizar la vista de hito.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront</strong></td> 
   <td> 
   <p>Nuevo: estándar</p>
   <p>Actual: Trabajo o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de visualización o superior a informes, tableros, calendarios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver permisos de un informe de proyecto para aplicar la vista de Hito a un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cambiar a la vista de Hito {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Haga clic en **Ver** y, a continuación, haga clic en **Hito**.

   La lista o el informe se muestra en una vista de Hito.

   Para obtener información sobre la vista de hito, consulte la sección [Información general de vista de Milestone](#milestone-view-overview) en este artículo.

## Información general de vista de Milestone {#milestone-view-overview}

La vista Hito está disponible en listas de proyectos e informes de proyectos. Esta vista permite ver rápidamente todos los hitos asociados con las tareas de los proyectos que está viendo.


>[!NOTE]
>
>La vista Hito no está disponible en las áreas siguientes:
>
>* Plantillas de horas, en la lista de proyectos al añadir un proyecto.


Para obtener información sobre cómo cambiar a la vista de Hito, vea la sección [Cambiar a la vista de Hito](#switch-to-the-milestone-view) en este artículo.

![Proyecto con vista de hito](assets/project-with-milestone-view-with-complete.png)

### Secciones de vista de hito

Al aplicar la vista de Hito a una lista de proyectos, estos se muestran en las secciones siguientes:

* Los proyectos asociados a una ruta de hitos se muestran primero, enumerados con el nombre de sus respectivas rutas de hitos.

  Workfront ordena los proyectos de la primera sección según los siguientes criterios, en este orden:

   1. ID de ruta de hitos. Puede ver el ID de ruta de hitos en un informe de ruta de hitos.

   2. Campo seleccionado como el primer campo de ordenación para la lista de proyectos de la vista aplicada anteriormente a la lista de proyectos, antes de seleccionar la vista de Hito.

* Los proyectos no asociados a una ruta de hitos se muestran a continuación, en la sección Sin asignar. Workfront ordena los proyectos de la sección Sin asignar por el campo seleccionado como primer campo de ordenación para la lista de proyectos de la vista aplicada anteriormente a la lista de proyectos, antes de seleccionar la vista de Hito.

### Información del proyecto en la vista de Hito

Cuando se visualiza una lista de proyectos o un informe de proyectos en la vista de Hito, está disponible la siguiente información:

* **Fechas planificadas o proyectadas:** Especifique si desea mostrar Fechas planificadas o Fechas proyectadas en la vista de Hito.\
  Se muestran las fechas de inicio y finalización, así como de cada hito dentro de la ruta de hitos.\
  Si está viendo Fechas planificadas y también tiene acceso de Gestión al proyecto, puede editar las siguientes fechas directamente desde la vista de Hito: (Si está viendo Fechas proyectadas, las fechas no se pueden editar porque las Fechas proyectadas se calculan y no se pueden cambiar manualmente).

   * **Fechas de inicio del proyecto:** Si un proyecto está programado a partir de la fecha de inicio, puede cambiar manualmente la fecha de inicio del proyecto y, a continuación, se calcula la fecha de finalización.
   * **Fechas de finalización del proyecto:** Si un proyecto está programado a partir de la fecha de finalización, puede cambiar manualmente la fecha de finalización del proyecto y, a continuación, se calcula la fecha de inicio.
   * **Fechas de finalización de tarea:** Puede actualizar manualmente la finalización de tareas directamente desde la vista Hito.

* **Porcentaje completado:** Muestra el porcentaje de finalización de cada tarea y proyecto.\
  Puede deshabilitar la visualización del porcentaje de finalización, tal como se describe en la sección [Configurar la información que se muestra en la vista de Hito](#configure-what-information-displays-in-the-milestone-view) en este artículo.\
  Puede ajustar el porcentaje de finalización directamente desde la vista Hito, tal como se describe en la sección [Ajustar el porcentaje completado de las tareas de la vista Hito](#adjust-percent-complete-for-tasks-in-the-milestone-view) en este artículo.

* **Iconos de estado de tarea:** Se muestra un icono de estado junto a cada proyecto y tarea en la vista de Hito.

   * A tiempo\
     ![](assets/gantt-ontime.png)

   * Rezagado\
     ![](assets/gantt-behind.png)

   * En riesgo\
     ![](assets/gantt-atrisk.png)

   * Retrasado\
     ![](assets/gantt-late.png)

  Puede deshabilitar la visualización de estos iconos de estado, tal como se describe en la sección [Configurar la información que se muestra en la vista de Hito](#configure-what-information-displays-in-the-milestone-view) en este artículo.\
  Para obtener información más detallada sobre cada tipo de estado, consulte el artículo [Resumen del estado de progreso de tareas](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Sombreado de estado de tarea para tareas completadas**: Después de que una tarea se marque como Completada, el fondo de la tarea se sombrea en la vista de Hito para indicar si la tarea se completó a tiempo o con retraso:

   * **Sombreado rojo para la columna de tareas**: el fondo de una tarea es rojo cuando el estado del progreso es **Retrasado**.

   * **Sombreado verde de la columna de tareas**: el fondo de una tarea es verde cuando el estado del progreso es **Tiempo de activación**.

* **Sombreado del estado del proyecto para las columnas Inicio del proyecto y Finalización**:

   * **Columna de inicio del proyecto**: el fondo de la columna Inicio del proyecto es rojo o verde solo cuando se rellena la Fecha de inicio real:

      * **Sombreado rojo para la columna Inicio del proyecto**: el fondo de la columna Inicio del proyecto aparece en rojo cuando el estado del progreso del proyecto es **Retrasado**.

      * **Sombreado verde de la columna Inicio del proyecto**: el fondo de la columna Inicio del proyecto es verde cuando el estado del progreso del proyecto es **Tiempo de activación**.

   * **Columna de finalización del proyecto**: el fondo de la columna Finalización del proyecto es rojo o verde solo cuando se rellena la Fecha real de finalización:

      * **Sombreado rojo para la columna de finalización del proyecto**: el fondo de la columna Finalización del proyecto aparece en rojo cuando se muestra el estado de progreso del proyecto **Retrasado**.

      * **Sombreado verde de la columna Finalización del proyecto**: el fondo de la columna Finalización del proyecto es verde cuando el estado del progreso del proyecto es **Tiempo de activación**.

   * No se asigna ningún sombreado de color a las columnas Inicio y Finalización cuando las tareas tienen un estado de progreso de En riesgo o Retrasado.

  ![Vista de Hito con sombreado](assets/milestone-view-with-shading.png)

* **Nombre del proyecto**: el nombre del proyecto se muestra con un vínculo al proyecto.
* **Icono de condición del proyecto**: Se muestra un icono junto al nombre del proyecto que indica la condición del proyecto.

## Configurar la información que se muestra en la vista de Hito {#configure-what-information-displays-in-the-milestone-view}

Puede configurar si se muestran los siguientes elementos en la vista de Hito:

* Iconos de estado de progreso
* Porcentaje completado de proyectos y tareas

De forma predeterminada, se muestran los iconos de estado del proyecto y el porcentaje completado de los proyectos.

Los cambios que realice en estas opciones sólo se aplicarán a usted; los demás usuarios no se verán afectados. Los cambios que realice se conservarán la próxima vez que inicie sesión en Adobe Workfront.

Para configurar si se muestran los iconos de estado del proyecto y el porcentaje de finalización de los proyectos:

{{step1-to-projects}}

1. Haga clic en **Ver** y, a continuación, haga clic en **Hito**.\
   Si está viendo una lista de proyectos dentro de un Portfolio o un programa, seleccione el **Hito** subpestaña.

1. Clic **Opciones** en la esquina superior derecha de la vista Hito.\
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Estado de progreso</td> 
      <td> <p>Seleccione esta opción para mostrar los iconos de estado de progreso junto a cada proyecto y tarea.</p> <p>Esta opción está habilitada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Porcentaje completado</td> 
      <td> <p>Seleccione esta opción para mostrar el porcentaje de finalización junto a cada proyecto y tarea.</p> <p>Esta opción está habilitada de forma predeterminada.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Ajustar el porcentaje completado de las tareas de la vista Hito {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Puede ajustar el Porcentaje completado para las tareas en la vista Hito. No se puede ajustar el Porcentaje completado para una tarea principal (una tarea que contiene subtareas).

Para ajustar el porcentaje completado de una tarea en la vista Hito:

{{step1-to-projects}}

1. Haga clic en **Ver** y, a continuación, haga clic en **Hito**.

1. (Condicional) Si los porcentajes de finalización no se muestran actualmente en la vista Hito, haga clic en **Opciones** en la esquina superior derecha de la vista Hito, asegúrese de que **Porcentaje completado** está activada.

1. Haga clic en el porcentaje de finalización debajo de una tarea, especifique un nuevo porcentaje y pulse Entrar.
