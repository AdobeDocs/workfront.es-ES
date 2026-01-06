---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Información general sobre la modificación de asignaciones de tareas
description: Puede asignar tareas a usuarios, equipos o funciones de trabajo, o anular su asignación. Puede asignar varios recursos al mismo tiempo o solo un recurso. Puede asignar una tarea a la vez o varias tareas de forma masiva.
author: Lisa
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 97%

---

# Información general sobre la modificación de asignaciones de tareas

Puede asignar tareas a usuarios, equipos o funciones de trabajo, o anular su asignación. Puede asignar varios recursos al mismo tiempo o solo un recurso. Puede asignar una tarea a la vez o varias tareas de forma masiva.

>[!TIP]
>
>Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos.
>
>Si se asignó un usuario, una función o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
>
>* Reasignar el elemento de trabajo a los recursos activos.
>* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.
>

Este artículo contiene información general sobre el impacto de la modificación de asignaciones de tareas. Para obtener información sobre cómo asignar tareas, consulte los siguientes artículos:

* Para obtener información sobre la asignación de tareas, consulte [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) y [Modificar varias asignaciones de usuario en una lista de tareas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Para obtener información sobre la modificación de asignaciones de varias tareas en el área Programación, consulte “Modificar varias asignaciones de usuario a tareas en las áreas de programación”.
* Para obtener información sobre la asignación de tareas mediante el Distribuidor de cargas de trabajo, consulte [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Parte de la información de este artículo también se aplica a las asignaciones a problemas. Para obtener más información sobre la asignación de problemas y otras consideraciones adicionales, consulte [Información general sobre la modificación de asignaciones de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Cuándo modificar asignaciones de usuarios a tareas

Es posible que desee modificar las asignaciones de usuario a tareas por distintos motivos, entre los que se incluyen los siguientes:

* Los usuarios se unen o abandonan el equipo
* La duración de las vacaciones de un usuario se extiende más allá de las fechas de vencimiento de la tarea

  >[!NOTE]
  >
  >Al asignar usuarios para trabajar, su disponibilidad según sus programaciones afecta a las fechas planificadas y proyectadas de las tareas. Para obtener información acerca de las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Una función o usuario específico se establecen como asignados para varias tareas y desea modificar rápidamente todos los elementos que necesita asignar a un usuario o función diferentes

## Consideraciones para varias asignaciones a funciones, equipos y usuarios

Tenga en cuenta lo siguiente al asignar varios recursos a un elemento de trabajo:

* Los usuarios pueden tener más de una función asociada a su perfil. Para obtener información sobre cómo asociar usuarios con roles de trabajo, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Las tareas o problemas suelen asignarse primero a uno o varios roles de trabajo o a un equipo. Cuando los proyectos están listos para iniciarse, es posible que también deban asignarse a usuarios.\
  Si se asigna una tarea o un problema a una o varias funciones y, a continuación, también se asigna un usuario, Adobe Workfront decide qué función se asocia al usuario adicional (si corresponde) según las siguientes reglas:

   * Si solo hay una función asignada y coincide con la función principal del usuario, la tarea o el problema se asignan únicamente al usuario que desempeña su función principal.
   * Si hay varias funciones asignadas y al menos una de las funciones coincide con las funciones secundarias del usuario, la tarea o el problema se asigna al usuario que desempeña una de sus otras funciones (que Workfront selecciona aleatoriamente si hay varias coincidencias), así como cualquier función adicional asignada.
   * Si hay una o más funciones asignadas y no hay coincidencias con las funciones del usuario, la tarea o el problema se asignan tanto a la función o funciones como al usuario.

* Si se asigna una tarea o un problema a un equipo y también se asigna un usuario, la tarea o el problema permanecen asignados tanto al equipo como al usuario.

## Cómo afecta la eliminación de usuarios asignados a las horas de la tarea y los porcentajes de asignación

La eliminación de usuarios puede afectar a las horas de las tareas y a los porcentajes de asignación. El efecto que tiene la eliminación de un usuario en la tarea depende del Tipo de duración seleccionado para esa tarea. Para obtener más información sobre los tipos de duración, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Cuando elimina un usuario de una tarea con los siguientes tipos de duración:

* **Sencilla:** las horas planificadas asignadas a ese usuario se restan del total de horas planificadas de la tarea.

  >[!IMPORTANT]
  >
  >Esto podría afectar negativamente al plan del proyecto porque cambia el total de horas planificadas para la tarea y el proyecto.

* **Condicionada por el esfuerzo:** el porcentaje de asignación no cambia para otros usuarios.
* **Asignación calculada:** los porcentajes de asignación de otros usuarios se ajustan para que el total sea igual al 100 %.
* **Trabajo calculado:** el porcentaje de asignación no cambia para otros usuarios.

## Consideraciones sobre la anulación de asignación de tareas

Puede quitar asignaciones de una tarea a la vez o puede quitar asignaciones de varias tareas en lotes.

Para obtener más información acerca de cómo quitar asignaciones de tareas en lotes, consulte [Modificar varias asignaciones de usuario en una lista de tareas](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Tenga en cuenta lo siguiente al eliminar asignaciones de tareas:

* Cuando quita la asignación de un usuario de una tarea, la tarea permanece asignada a la función que el usuario cumplió en la tarea.
* Cuando quita la asignación de una función o de un equipo de una tarea, esta permanece sin asignar si no está asignada a ningún otro recurso.
