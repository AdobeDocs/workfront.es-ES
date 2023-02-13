---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Administrar horas de asignación de usuarios y funciones en tareas
description: Al asignar usuarios o funciones a una tarea, se les asigna trabajar un determinado número de horas para completar la tarea. Puede modificar manualmente la cantidad de horas que cada usuario o función de trabajo está asignado cuando se asigna a una tarea, cuando el tipo de duración de la tarea es simple.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Administrar horas de asignación de usuarios y funciones en tareas

Al asignar usuarios o funciones a una tarea, se les asigna trabajar un determinado número de horas para completar la tarea. Puede modificar manualmente la cantidad de horas que cada usuario o función de trabajo está asignado cuando se asigna a una tarea, cuando el tipo de duración de la tarea es simple.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribute o permisos superiores para la tarea</p> <p>Editar permisos para actualizar las horas de asignación en el cuadro Editar tarea</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones para modificar las horas de asignación de una tarea

>[!IMPORTANT]
>
>Después de modificar manualmente las asignaciones para cada asignación en las tareas, las horas planificadas de las tareas podrían actualizarse en consecuencia. Para obtener más información, consulte la sección [Actualizar las horas planificadas de la tarea al administrar las asignaciones de usuario](../../../manage-work/tasks/task-information/planned-hours.md#update) en el artículo [Información general sobre las horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

* El total de horas asignadas a recursos individuales asignados a la tarea representa las horas planificadas de la tarea.
* Si hay un usuario o una asignación de función a una tarea, la cantidad de horas asignadas al usuario o a la función coincide con las horas planificadas de la tarea.
* En el caso de varias asignaciones, a cada usuario o función de trabajo se le asigna una cantidad igual de horas para trabajar en la tarea, de forma predeterminada, si el tipo de duración de la tarea es simple. Para obtener más información, consulte los siguientes artículos:

   * [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Información general del tipo de duración: Sencilla](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Cuando la tarea tiene un tipo de duración simple, puede cambiar manualmente la cantidad de horas asignadas para cada usuario o función de trabajo para indicar que algunos de los asignadores de tareas pueden tener más tiempo para trabajar en una tarea que otros.
* No puede modificar la cantidad de horas asignadas a equipos asignados a tareas.
* No puede modificar manualmente la asignación de funciones de usuario o trabajo para problemas.
* También puede administrar las asignaciones diarias, semanales o mensuales de usuarios a tareas o problemas mediante el equilibrador de carga de trabajo. Para obtener más información, consulte [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modificación de las horas de asignación de funciones o usuarios para una tarea

1. Vaya a una tarea para cuyas asignaciones desee cambiar las horas de asignación.
1. Haga clic en el **Más** menú ![](assets/qs-more-icon-on-an-object.png) junto al nombre de la tarea y, a continuación, haga clic en **Editar**, luego **Asignaciones**.

   O

   Haga clic en el **Asignaciones** en el encabezado de la tarea y haga clic en **Avanzadas**.

1. Asegúrese de que la variable **Tipo de duración** de la tarea es **Sencilla**.
1. Modifique el **Asignaciones** para cada tarea asignada. Son asignaciones generales para cada asignación a esta tarea, durante toda la duración de la tarea. Esto también podría actualizar el horario planificado general de la tarea.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Haga clic en **Guardar**.
