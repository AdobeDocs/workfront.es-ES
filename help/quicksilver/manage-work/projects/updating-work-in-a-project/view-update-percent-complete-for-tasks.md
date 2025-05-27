---
product-area: projects
navigation-topic: update-work-in-a-project
title: Ver y actualizar el porcentaje completado de las tareas
description: Puede actualizar el porcentaje completado de una tarea para indicar el progreso que ha realizado en la tarea hacia completarla. Actualizar el porcentaje completado por problemas es similar a actualizarlo para una tarea. Este artículo describe cómo actualizar el porcentaje completado de una tarea.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 66fc75ed9a7fca4b44ac776c314a6e08a6fbd450
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 42%

---

# Ver y actualizar el porcentaje completado de las tareas

<!--Audited: 05/2025-->

Puede actualizar el porcentaje completado de una tarea para indicar el progreso que ha realizado para completarla.

Actualizar el porcentaje completado por problemas es similar a actualizarlo para una tarea. Este artículo describe cómo actualizar el porcentaje completado de una tarea.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para actualizar las tareas manualmente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nueva licencia: estándar</p> 
   O
   <p>Licencia actual: Trabajo o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para la tarea</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Áreas en las que se puede actualizar el porcentaje completado de una tarea

Puede actualizar el porcentaje completado de una tarea en cualquiera de las siguientes áreas:

* **En una lista de tareas**: puede actualizar el porcentaje completado de una tarea cuando se muestre la columna Porcentaje completado.

  Para obtener más información acerca de la edición integrada, consulte [Editar elementos dentro de una lista de Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **En la vista Hito**: puede actualizar el porcentaje completado de una tarea al usar la vista Hito en una lista de proyectos o un informe de proyectos.

  >[!TIP]
  >
  >  No se puede actualizar el porcentaje completado de los problemas en la vista de Hito.


  Para obtener más información, consulte [Usar la vista de hito](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **En el encabezado de tarea**: puede actualizar el porcentaje completado de una tarea en el encabezado de tarea.

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **En el panel de resumen de una tarea**: puede actualizar el porcentaje completado de una tarea en la parte superior del panel Resumen al ver la tarea en las siguientes áreas:

   * Lista de tareas o informes
   * Plantilla de horas
   * Distribuidor de cargas de trabajo

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  Para obtener más información, consulte [Información general sobre el resumen](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Inicio**: puede actualizar el porcentaje completado de una tarea o problema desde el panel Resumen en el área Inicio o desde el widget Mi trabajo.

  Para obtener más información, consulte [Introducción a Inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

## Consideraciones acerca de la actualización del porcentaje completado de una tarea

* Cuando marca una tarea como 100% completada, el estado de la tarea se actualiza a Completada. El estado de un problema se actualiza a Cerrado.
* Al completar una tarea, también se actualiza el porcentaje completado del elemento principal y del proyecto.
* Los siguientes escenarios existen para tareas y proyectos principales:
   * No se puede actualizar el porcentaje completado de una tarea principal al 100 % cuando el modo de finalización de resumen del proyecto se haya establecido en Automático y las subtareas no se hayan completado.
   * Puede actualizar el porcentaje completado de una tarea principal o de un proyecto al 100% cuando el modo de finalización de resumen del proyecto esté establecido en Manual y las subtareas estén completadas o incompletas.

  Para obtener más información, consulte [Editar proyectos](../manage-projects/edit-projects.md).

## Actualizar el porcentaje completado de una tarea

1. Vaya a cualquiera de las áreas en las que desee actualizar el porcentaje completado de una tarea.

   Para obtener más información, consulte la sección [Áreas donde puede actualizar el porcentaje completado de una tarea](#areas-where-you-can-update-the-percent-complete-of-a-task) en este artículo.

1. Busque el campo **Porcentaje completado** de la tarea cuyo porcentaje completado desee actualizar.

   >[!TIP]
   >
   >El campo Porcentaje completado siempre se muestra en la parte superior del panel Resumen.

1. Haga clic dentro del campo **Porcentaje completado** y escriba un número entre 0 y 100

   O

   Haga clic y arrastre la burbuja azul **Porcentaje completado** al número necesario para indicar la cantidad de la tarea que ha completado, cuando esté disponible.

   >[!NOTE]
   >
   >    * No puede introducir un número decimal cuando hace clic dentro de la burbuja Porcentaje completado.
   >    * Cuando arrastra y suelta la burbuja azul en el panel Resumen, el porcentaje completado se actualiza en un punto en incrementos.
   >
   >    * Cuando arrastra y suelta la burbuja azul en el encabezado de la tarea, el porcentaje completado se actualiza en incrementos de 5 puntos.

1. Pulse Enter en el teclado para guardar el porcentaje completado.

   El Porcentaje completado del proyecto o cualquier tarea principal también se puede actualizar automáticamente.

   El estado de la tarea o del problema también se actualiza.

