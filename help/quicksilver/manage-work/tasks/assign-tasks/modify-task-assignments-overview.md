---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Información general sobre la modificación de asignaciones de tareas
description: Puede asignar tareas a usuarios, equipos o roles o anular su asignación. Puede asignar varios recursos al mismo tiempo o solo un recurso. Puede asignar una tarea a la vez o varias tareas de forma masiva.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# Información general sobre la modificación de asignaciones de tareas

Puede asignar tareas a usuarios, equipos o roles o anular su asignación. Puede asignar varios recursos al mismo tiempo o solo un recurso. Puede asignar una tarea a la vez o varias tareas de forma masiva.

>[!TIP]
>
>Puede asignar varios usuarios, roles o equipos. Solo puede asignar usuarios activos, roles y equipos.
>
>Si se asignó un usuario, un rol o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
>
>* Reasignar el elemento de trabajo a los recursos activos.
>* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.
>

Este artículo contiene información general sobre el impacto de la modificación de asignaciones de tareas. Para obtener información sobre cómo asignar tareas, consulte los siguientes artículos:

* Para obtener información acerca de la asignación de tareas, vea [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) y [Modificar asignaciones de varios usuarios en una lista de tareas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Para obtener información sobre la modificación de asignaciones de varias tareas en el área Programación, consulte &quot;Modificación de asignaciones de varios usuarios a tareas en las áreas Programación&quot;.
* Para obtener información acerca de cómo asignar tareas mediante el Distribuidor de cargas de trabajo, vea [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Parte de la información de este artículo también se aplica a las asignaciones a problemas. Para obtener más información sobre la asignación de problemas y otras consideraciones adicionales, consulte [Información general sobre la modificación de asignaciones de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Cuándo modificar asignaciones de usuarios en tareas

Es posible que desee modificar las asignaciones de usuario para tareas por varios motivos, entre los que se incluyen los siguientes:

* Los usuarios se unen o abandonan el equipo
* Un usuario se toma unas vacaciones que se extienden más allá de las fechas de vencimiento de la tarea

  >[!NOTE]
  >
  >Al asignar usuarios para que trabajen, su disponibilidad según sus programaciones afecta a las Fechas planificadas y proyectadas de las tareas. Para obtener información acerca de las programaciones, vea [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Un rol o usuario específico se establece como el usuario asignado para varias tareas y desea modificar rápidamente todos los elementos para asignarlos a un usuario o rol diferente

## Consideraciones para varias asignaciones a roles de trabajo, equipos y usuarios

Tenga en cuenta lo siguiente al asignar varios recursos a un elemento de trabajo:

* Los usuarios pueden tener más de una función de trabajo asociada a su perfil. Para obtener información sobre cómo asociar usuarios con roles de trabajo, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Las tareas o los problemas suelen asignarse primero a una o varias funciones del puesto o a un equipo. Cuando los proyectos están listos para iniciarse, es posible que también deban asignarse a usuarios.\
  Si se asigna una tarea o un problema a una o varias funciones y, a continuación, también se asigna un usuario, Adobe Workfront decide qué función de trabajo se asocia al usuario adicional (si corresponde) según las siguientes reglas:

   * Si solo hay una función de trabajo asignada y coincide con la función principal del usuario, la tarea o el problema se asignan únicamente al usuario que cumple su función principal.
   * Si hay varias funciones asignadas y al menos una de las funciones coincide con las funciones secundarias del usuario, la tarea o el problema se asigna al usuario que cumple una de sus otras funciones (que Workfront selecciona aleatoriamente si hay varias coincidencias), así como cualquier función adicional asignada.
   * Si hay uno o más roles asignados y no hay coincidencias con los roles del usuario, la tarea o el problema se asignan tanto al rol o los roles como al usuario.

* Si se asigna una tarea o un problema a un equipo y también se asigna un usuario, la tarea o el problema permanecen asignados tanto al equipo como al usuario.

## Cómo afecta la eliminación de usuarios asignados a las horas de tarea y los porcentajes de asignación

La eliminación de usuarios puede afectar a las horas de tareas y a los porcentajes de asignación. El efecto que tiene la eliminación de un usuario en la tarea depende del Tipo de duración seleccionado para la tarea. Para obtener información acerca del tipo de duración, vea [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Cuando elimina un usuario de una tarea con los siguientes tipos de duración:

* **Sencilla:** Las horas planificadas asignadas a ese usuario se restan del total de horas planificadas de la tarea.

  >[!IMPORTANT]
  >
  >Esto podría afectar negativamente al plan del proyecto porque cambia el total de horas planificadas para la tarea y el proyecto.

* **Condicionada por el esfuerzo:** El porcentaje de asignación no cambia para otros usuarios.
* **Asignación calculada:** Los porcentajes de asignación de otros usuarios se ajustan para que el total sea igual al 100%.
* **Trabajo calculado:** El porcentaje de asignación no cambia para otros usuarios.

## Consideraciones sobre la cancelación de asignación de tareas

Puede quitar asignaciones de una tarea a la vez o puede quitar asignaciones de varias tareas de forma masiva.

Para obtener más información acerca de cómo quitar asignaciones de tareas de forma masiva, vea [Modificar asignaciones de varios usuarios en una lista de tareas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Tenga en cuenta lo siguiente al eliminar asignaciones de tareas:

* Cuando anula la asignación de un usuario de una tarea, la tarea permanece asignada a la función de trabajo que el usuario cumplió en la tarea.
* Cuando anula la asignación de un rol o de un equipo a una tarea, esta permanece sin asignar si no está asignada a ningún otro recurso.
