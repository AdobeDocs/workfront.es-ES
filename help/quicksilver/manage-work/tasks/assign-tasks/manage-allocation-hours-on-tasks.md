---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Administrar horas de asignación de usuarios y funciones en las tareas
description: Al asignar usuarios o funciones a una tarea, se les asigna trabajar un determinado número de horas para completar la tarea. Puede modificar manualmente la cantidad de horas que se asigna a cada usuario o rol cuando se le asigna una tarea, cuando el tipo de duración de la tarea es Simple.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 830ad0411084844ace1e1e543c3ebefcb558af80
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Administrar horas de asignación de usuarios y funciones en las tareas

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar </p>
   <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribute o permisos superiores para la tarea</p> <p>Editar permisos para actualizar las horas de asignación en el cuadro Editar tarea</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones para modificar las horas de asignación de una tarea

>[!IMPORTANT]
>
>Después de modificar manualmente las asignaciones de cada asignación en las tareas, las horas planificadas de las tareas podrían actualizarse en consecuencia. Para obtener más información, vea la sección [Actualizar horas planificadas de tareas al administrar asignaciones de usuarios](../../../manage-work/tasks/task-information/planned-hours.md#update) en el artículo [Resumen de horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

* El total de horas asignadas a recursos individuales asignados a la tarea representa las horas planificadas de la tarea.
* Si hay una asignación de usuario o rol a una tarea, la cantidad de horas asignadas al usuario o rol coincide con las horas planificadas de la tarea.
* En el caso de varias asignaciones, a cada usuario o rol se le asigna la misma cantidad de horas para trabajar en la tarea, de forma predeterminada, si el tipo de duración de la tarea es Simple. Para obtener más información, consulte los siguientes artículos:

   * [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Información general del tipo de duración: Simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Cuando la tarea tiene un Tipo de duración simple, puede cambiar manualmente la cantidad de horas asignadas para cada usuario o rol para indicar que algunos de los usuarios asignados pueden tener más tiempo para trabajar en una tarea que otros.
* No se puede modificar la cantidad de horas asignadas a los equipos asignados a las tareas.
* No puede modificar manualmente la asignación de usuarios o funciones para los problemas.
* También puede administrar las asignaciones diarias, semanales o mensuales de usuarios a tareas o problemas mediante el Distribuidor de cargas de trabajo. Para obtener más información, consulte [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modificar las horas de asignación de usuarios o funciones de una tarea

1. Vaya a una tarea cuyas asignaciones desee cambiar las horas de asignación.
1. Haga clic en el menú **Más** ![](assets/qs-more-icon-on-an-object.png) junto al nombre de la tarea, luego haga clic en **Editar** y luego en **Asignaciones**.

   O

   Haga clic en el área **Asignaciones** del encabezado de la tarea y, a continuación, haga clic en **Avanzadas**.

1. Asegúrese de que el **Tipo de duración** de la tarea sea **Simple**.
1. Modifique las **Asignaciones** para cada usuario asignado a la tarea. Son asignaciones generales para cada asignación a esta tarea, para toda la duración de la tarea. Esto también puede actualizar las horas planificadas generales de la tarea.

   ![Modificar asignaciones](assets/advanced-assignments-duration-type-allocations.png)

1. Haga clic en **Guardar**.
