---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Información general sobre la modificación de asignaciones de tareas
description: Puede asignar o anular la asignación de tareas de usuarios, equipos o funciones de trabajo. Puede asignar varios recursos al mismo tiempo o solo un recurso. Puede asignar una tarea a la vez o varias tareas de forma masiva.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Información general sobre la modificación de asignaciones de tareas

Puede asignar o anular la asignación de tareas de usuarios, equipos o funciones de trabajo. Puede asignar varios recursos al mismo tiempo o solo un recurso. Puede asignar una tarea a la vez o varias tareas de forma masiva.

>[!TIP]
>
>Puede asignar varios usuarios, funciones de trabajo o equipos. Solo puede asignar usuarios activos, funciones de trabajo y equipos.
>
>Si se asignó un usuario, una función de trabajo o un equipo antes de desactivarlos, se asignarán al elemento de trabajo. En este caso, se recomienda lo siguiente:
>
>* Reasigne el elemento de trabajo a los recursos activos.
>* Asocie a los usuarios de un equipo desactivado con un equipo activo y reasigne el elemento de trabajo al equipo activo.
>


Este artículo contiene información general sobre el impacto de la modificación de asignaciones de tareas. Para obtener información sobre cómo asignar tareas, consulte los siguientes artículos:

* Para obtener información sobre la asignación de tareas, consulte [Asignación de tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) y [Modificar varias asignaciones de usuario en una lista de tareas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Para obtener información sobre la modificación de asignaciones en varias tareas del área Programación, consulte [Modificar asignaciones de varios usuarios a tareas en las áreas de programación](../../../resource-mgmt/resource-scheduling/modify-multipl-assignments-scheduling-areas.md).
* Para obtener información sobre la asignación de tareas mediante el equilibrador de carga de trabajo, consulte [Información general sobre la asignación de trabajo en el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Parte de la información de este artículo también se aplica a las asignaciones a problemas. Para obtener más información sobre la asignación de problemas y consideraciones adicionales, consulte [Información general sobre la modificación de asignaciones de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Cuándo modificar las asignaciones de usuario en las tareas

Puede que desee modificar las asignaciones de usuario para las tareas por varios motivos, entre los que se incluyen:

* Los usuarios se unen o abandonan el equipo
* Un usuario toma vacaciones que se extienden más allá de las fechas de vencimiento de la tarea

   >[!NOTE]
   >
   >Al asignar usuarios al trabajo, su disponibilidad según sus programaciones afecta a las Fechas planificadas y proyectadas de las tareas. Para obtener información sobre las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Un usuario o función específica se establece como usuario asignado para varias tareas y desea modificar rápidamente todos los elementos que se asignarán a un usuario o función diferente

## Consideraciones para varias asignaciones a funciones de trabajo, equipos y usuarios

Tenga en cuenta lo siguiente al asignar varios recursos a un elemento de trabajo:

* Los usuarios pueden tener más de una función de trabajo asociada a su perfil. Para obtener información sobre cómo asociar usuarios con funciones de trabajo, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Normalmente, las tareas o los problemas se asignan primero a una o varias funciones de trabajo o a un equipo. Cuando los proyectos están listos para iniciarse, es posible que también deban asignarse a usuarios.\
   Si se asigna una tarea o un problema a una o varias funciones y, a continuación, también se asigna un usuario, Adobe Workfront decide qué rol de trabajo se asociará al usuario adicional (si lo hay) de acuerdo con las siguientes reglas:

   * Si solo hay una función de trabajo asignada y coincide con la función principal del usuario, la tarea o el problema se asignan solo al usuario que cumple su función principal.
   * Si hay varias funciones asignadas y al menos una de ellas coincide con las funciones secundarias del usuario, la tarea o el problema se asigna al usuario que cumple una de sus Otras funciones (que Workfront selecciona al azar si hay varias coincidencias), así como a cualquier función adicional asignada.
   * Si hay una o más funciones de trabajo asignadas y no hay coincidencias con las funciones del usuario, la tarea o el problema se asignan tanto a la función o a las funciones como al usuario.

* Si se asigna una tarea o un problema a un equipo y también se asigna un usuario, la tarea o el problema permanece asignado tanto al equipo como al usuario.

## Cómo afecta la eliminación de asignadores a las horas de tarea y a los porcentajes de asignación

La eliminación de usuarios puede afectar a las horas de la tarea y a los porcentajes de asignación. El efecto que tiene al quitar un usuario en la tarea depende del tipo de duración seleccionado para la tarea. Para obtener información sobre el tipo de duración, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Al eliminar un usuario de una tarea con los siguientes tipos de duración:

* **Simple:** Las horas programadas asignadas a ese usuario se restan del total de horas planificadas de la tarea.

   >[!IMPORTANT]
   >
   >Esto podría afectar negativamente al plan del proyecto porque cambia el total de horas planificadas para la tarea y el proyecto.

* **Esfuerzo impulsado:** El porcentaje de asignación no cambia para otros usuarios.
* **Asignación calculada:** Los porcentajes de asignación de otros usuarios se ajustan para que el total sea igual al 100 %.
* **Trabajo calculado:** El porcentaje de asignación no cambia para otros usuarios.

## Consideraciones sobre la desasignación de tareas

Puede quitar asignaciones de una tarea a la vez o quitar asignaciones de varias tareas de forma masiva.

Para obtener más información sobre cómo quitar asignaciones de tareas en masa, consulte [Modificar varias asignaciones de usuario en una lista de tareas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Tenga en cuenta lo siguiente al quitar asignaciones de tareas:

* Cuando anula la asignación de un usuario de una tarea, la tarea permanece asignada a la función de trabajo que el usuario cumplió en la tarea.
* Cuando anula la asignación de una función de trabajo o de un equipo de una tarea, la tarea permanece sin asignar si no está asignada a ningún otro recurso.
