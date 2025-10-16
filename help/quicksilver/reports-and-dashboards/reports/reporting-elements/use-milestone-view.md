---
product-area: reporting
navigation-topic: reporting-elements
title: Uso de la vista de hito
description: Puede aplicar la vista de Hito a una lista de proyectos o a un informe. Puede utilizar la vista de Hito para ver todos los hitos asociados con las tareas de los proyectos que está viendo.
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 56%

---

# Uso de la vista de hito

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<div class="preview">

La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Las mismas funciones también estarán disponibles en el entorno de producción para todos los clientes a partir de una semana desde la versión de vista previa.

Para obtener más información, vea [Modernización de la interfaz](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Puede aplicar la vista de Hito a una lista de proyectos o a un informe. Puede utilizar la vista de Hito para ver todos los hitos asociados con las tareas de los proyectos que está viendo.

Para poder utilizar la vista de hito, deben existir los siguientes elementos:

* Se configuran las rutas de los hitos. Para obtener más información, vea [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* Las rutas de hitos necesarias se añaden a los proyectos. Para obtener más información, consulte [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).
* Los hitos están asociados a tareas. Para obtener más información, consulte [Asociar hitos con tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

La vista Hito está disponible cuando se visualiza una lista de proyectos o un informe de proyectos. En las secciones siguientes se describe cómo ver y utilizar la vista de hito.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</strong></td> 
   <td> 
    <p>Estándar</p>
    <p>Trabajo o superior</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a informes, paneles de control, calendarios</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
    <td> <p>Ver permisos de un informe de proyecto para aplicar la vista de hito a un informe</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cambiar a la vista de hito {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Haga clic en el menú desplegable **Ver** y luego haga clic en **Hito**.

   La lista o el informe se muestra en una vista de hito.

   Para obtener información acerca de la vista de hito, consulte la sección [Información general de la vista de hito](#milestone-view-overview) en este artículo.

## Información general de vista de hito {#milestone-view-overview}

<div class="preview">

La vista de hito está disponible en listas de proyectos e informes de proyectos. Puede ver rápidamente todos los hitos asociados con las tareas de los proyectos que está viendo.

![Proyecto con vista de hito](assets/project-with-milestone-view-with-complete.png)

</div>

>[!NOTE]
>
>La vista de hito no está disponible en las áreas siguientes:
>
>* Plantillas de horas, en la lista de proyectos al añadir un proyecto.

Para obtener información acerca de cómo cambiar a la vista de hito, consulte la sección [Cambiar a la vista de hito](#switch-to-the-milestone-view) en este artículo.


### Secciones de vista de hito

Al aplicar la vista de hito a una lista de proyectos, estos se muestran en las secciones siguientes:

* Los proyectos asociados a una ruta de hitos se muestran primero, enumerados con el nombre de sus respectivas rutas de hitos.

  Workfront ordena los proyectos de la primera sección según los siguientes criterios, en este orden:

   1. Identificador de la ruta de hitos. Puede ver el ID de ruta de hitos en un informe de ruta de hitos.

   2. El campo seleccionado como el primer campo de ordenación para la lista de proyectos de la vista aplicada anteriormente a la lista de proyectos, antes de seleccionar la vista de hito.

* Los proyectos no asociados a una ruta de hitos se muestran a continuación, en la sección Sin asignar. Workfront ordena los proyectos de la sección Sin asignar por el campo seleccionado como primer campo de ordenación para la lista de proyectos de la vista aplicada anteriormente a la lista de proyectos, antes de seleccionar la vista de hito.

### Información del proyecto en la vista de hito

Cuando se visualiza una lista de proyectos o un informe de proyectos en la vista de hito, está disponible la siguiente información:

* **Fechas planificadas o fechas proyectadas:** especifique si desea mostrar las fechas planificadas o proyectadas en la vista de hito.\
  Se muestran las fechas para las fechas de inicio y finalización del proyecto, así como para la finalización de cada tarea de Hito en la Ruta de hitos.

  Si está viendo Fechas proyectadas, las fechas no se pueden editar. Workfront calcula las fechas proyectadas, que no se pueden cambiar de forma manual.

  Si está viendo Fechas planificadas y también tiene acceso de Administración al proyecto, puede editar las siguientes fechas directamente desde la vista de Hito:

   * **Fechas de inicio del proyecto:** Si un proyecto está programado a partir de la fecha de inicio, puede cambiar manualmente la fecha planificada de inicio del proyecto y, a continuación, se calcula la fecha planificada de finalización.
   * **Fechas de finalización del proyecto:** Si un proyecto está programado a partir de la fecha planificada de finalización, puede cambiar manualmente la fecha planificada de finalización del proyecto y, a continuación, se calcula la fecha planificada de inicio.
   * **Fechas de finalización de la tarea:** Puede actualizar manualmente la fecha planificada de finalización de las tareas directamente desde la vista Hito.

* **Porcentaje completado:** muestra el porcentaje de finalización de cada tarea y proyecto.

  Puede deshabilitar que se muestre el porcentaje de finalización, tal como se describe en la sección [Configurar la información que se muestra en la vista de hito](#configure-what-information-displays-in-the-milestone-view) de este artículo.

  Puede ajustar el porcentaje de finalización directamente desde la vista de hito, tal como se describe en la sección [Ajustar porcentaje completado para las tareas de la vista de hito](#adjust-percent-complete-for-tasks-in-the-milestone-view) de este artículo.

* **Iconos de estado de progreso de la tarea:** Según el entorno que utilice para ver la vista de hito, los siguientes son iconos que indican el estado de progreso de la tarea:

   * En el entorno Producción, los siguientes iconos de estado se muestran junto a cada proyecto y tarea en la vista Hito:

      * A tiempo\
        ![Icono de Tiempo de activación](assets/gantt-ontime.png)

      * Rezagado\
        ![Icono detrás](assets/gantt-behind.png)

      * En riesgo\
        ![Icono de riesgo](assets/gantt-atrisk.png)

      * Retrasado\
        ![Icono de retraso](assets/gantt-late.png)

     <!--get new screen shots or hide them for preview or production - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

  <div class="preview">

   * En el entorno de vista previa, junto a cada proyecto y tarea en la vista Hito se muestran los siguientes círculos de colores:

      * Tiempo de activación: verde
      * Detrás - amarillo
      * En riesgo: azul
      * Retrasado: rojo

  </div>

  Puede deshabilitar la visualización de estos iconos de estado, tal como se describe en la sección [Configurar la información que se muestra en la vista de hito](#configure-what-information-displays-in-the-milestone-view) de este artículo.

  Para obtener información más detallada sobre cada tipo de estado, consulte el artículo [Información general del estado del progreso de la tarea](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Sombreado de estado de tarea para tareas completadas**: después de marcar una tarea como Completada, el fondo de la tarea se sombrea en la vista de hito para indicar si la tarea se completó a tiempo o con retraso:

   * **Sombreado rojo para la columna de tarea**: el fondo de una tarea es rojo cuando el estado de progreso es **Retrasado**.

   * **Sombreado verde para la columna de tarea**: el fondo de una tarea es verde cuando el estado de progreso es **A tiempo**.

* **Sombreado de estado del proyecto para las columnas de inicio y finalización del proyecto**:

   * **Columna de inicio del proyecto**: el fondo de la columna de inicio del proyecto aparece en rojo o en verde sólo cuando se rellena la fecha de inicio real:

      * **Sombreado rojo para la columna Inicio del proyecto**: el fondo de la columna de inicio del proyecto es rojo cuando el estado del progreso del proyecto es **Retrasado**.

      * **Sombreado verde para la columna Inicio del proyecto**: el fondo de la columna Inicio del proyecto es verde cuando el estado del progreso del proyecto es **A tiempo**.

     >[!TIP]
     >
     >Debe ir a la página Detalles del proyecto para ver la fecha de inicio real del proyecto.

   * **Columna de finalización del proyecto**: el fondo de la columna Finalización del proyecto aparece en rojo o en verde cuando se rellena la fecha real de finalización:

      * **Sombreado rojo para la columna de finalización del proyecto**: el fondo de la columna Finalización del proyecto aparece en rojo cuando el estado del progreso del proyecto es **Retrasado**.

      * **Sombreado verde para la columna de finalización del proyecto**: el fondo de la columna Finalización del proyecto es verde cuando el estado de progreso del proyecto es **A tiempo**.

     >[!TIP]
     >
     >Debe ir a la página Detalles del proyecto para ver la fecha real de finalización del proyecto.

   * No se asigna ningún sombreado de color a las columnas Inicio y Finalización cuando las tareas tienen un estado de progreso de En riesgo o Retrasado.

  <!--add new screen shot for preview or production release; logged a bug as this is not happening in the new view - if at prod this is still missing, hide this screen shot-->

  ![Vista de hito con sombreado](assets/milestone-view-with-shading.png)

* **Nombre del proyecto**: el nombre del proyecto se muestra con un vínculo al proyecto.
* **Icono de condición del proyecto**: según el entorno en el que esté accediendo a la vista de Hito desde los siguientes indicadores se muestra la condición del proyecto:

   * En el entorno Producción, aparece un icono junto al nombre del proyecto que indica la condición del proyecto. La condición del proyecto puede ser una de las siguientes:

      * Bien encaminado
      * En riesgo
      * Con problemas

  <div class="preview">

   * En el entorno de vista previa, junto a cada proyecto se muestra un icono de condición en forma de círculo de color. Las condiciones posibles del proyecto y los colores del círculo son:

      * En Target: verde
      * En riesgo - amarillo
      * En problemas: rojo

     </div>


## Configurar la información que se muestra en la vista de hito {#configure-what-information-displays-in-the-milestone-view}

Puede configurar si se muestran los siguientes elementos en la vista de hito:

* Iconos de estado de progreso
* Porcentaje completado de proyectos y tareas

De forma predeterminada, se muestran los iconos de estado de progreso y el porcentaje completado de los proyectos y las tareas.

Los cambios que realice en estas opciones sólo se aplicarán a usted; los demás usuarios no se verán afectados. Los cambios que realice se conservarán la próxima vez que inicie sesión en Workfront.

Para configurar si se muestran los iconos de estado del proyecto y el porcentaje de finalización de los proyectos:

{{step1-to-projects}}

1. Haga clic en el menú desplegable **Vista** y luego haga clic en **Hito**.

1. En el entorno Producción, haga clic en **Opciones** en la esquina superior derecha de la vista Hito y, a continuación, seleccione una de las opciones en el paso siguiente.

   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

   <div class="preview">En el entorno de vista previa, seleccione una de las opciones del paso siguiente, en la esquina superior derecha de la vista de Hito.</div>

   <!--at Production release, replace this screen shot and adjust the Production/ Preview text above-->


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

## Ajustar el porcentaje completado de las tareas de la vista de hito {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Puede ajustar el porcentaje completado para las tareas en la vista de hito. No se puede ajustar el porcentaje completado de una tarea principal (una tarea que contiene subtareas) o de un proyecto.

Para ajustar el porcentaje completado de una tarea en la vista de hito:

{{step1-to-projects}}

1. Haga clic en el menú desplegable **Vista** y luego haga clic en **Hito**.

1. (Condicional) Si los porcentajes de finalización no se muestran actualmente en la vista Hito, habilite la vista Porcentaje completado de tareas y proyectos, tal como se describe en la sección [Configurar la información que se muestra en la vista Hito](#configure-what-information-displays-in-the-milestone-view) de este artículo.

1. En el entorno Producción, haga clic en el porcentaje de finalización debajo de una tarea, especifique un nuevo porcentaje y, a continuación, presione Entrar.

   <div class="preview">En el entorno Vista previa, mueva la diapositiva Porcentaje completado al nuevo porcentaje completado para actualizarlo. </div>
