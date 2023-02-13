---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Crear asignaciones avanzadas
description: Puede administrar asignaciones de tareas o de problemas mediante Asignaciones avanzadas.
author: Alina
feature: Work Management
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Crear asignaciones avanzadas

Puede administrar asignaciones de tareas o de problemas mediante Asignaciones avanzadas.

Puede ajustar la siguiente información de asignación al realizar asignaciones avanzadas:

* Asignar usuarios a la tarea o problema (esto se puede llevar a cabo fuera de una asignación avanzada).
* Ajuste y redistribuya el número de horas que se asigna a cada usuario asignado.
* Determine qué usuario debe designarse como propietario o como asignado principal de la tarea o del problema.
* Especifique la función que cumple cada usuario al trabajar en la tarea o el problema.

>[!NOTE]
>
>Al asignar usuarios al trabajo, su disponibilidad según sus programaciones afecta a las Fechas planificadas y proyectadas de las tareas y los problemas. Para obtener información sobre las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Áreas de Adobe Workfront en las que puede realizar asignaciones avanzadas

Este artículo describe cómo acceder a Asignaciones anticipadas en el encabezado de la tarea o del problema.

Además, puede realizar asignaciones avanzadas en las siguientes áreas de Workfront:

* En listas e informes, cuando el campo Asignaciones aparece en la vista.
* En la sección Asignaciones al editar una tarea. Para obtener más información, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* En el encabezado de la tarea o del problema, en el área Asignaciones .
* En el equilibrador de carga de trabajo. Para obtener más información, consulte [Asignar trabajo manualmente mediante el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

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
   <td> <p>Editar acceso a Tareas y Problemas</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribute o permisos superiores para una tarea o problema</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Realizar asignaciones avanzadas

1. Vaya al proyecto en el que desea asignar una tarea o un problema.
1. Haga clic en **Tareas** o **Problemas** en el panel izquierdo, haga clic en el nombre de una tarea o problema de la lista.

   >[!TIP]
   >
   >Puede realizar asignaciones avanzadas directamente en la lista de tareas o problemas si hay dos o más personas asignadas. Haga clic dentro del **Asignaciones** en la misma línea que la tarea o el problema y, a continuación, haga clic en el botón **Icono de personas** para abrir la ventana Asignaciones avanzadas. Pase al paso 5 para seguir creando asignaciones avanzadas.\
   >![](assets/nwe-advanced-assignments-350x55.png)   >

1. Haga clic en **Asignar a** en el **Asignaciones** campo en el encabezado de la tarea o problema

   O

   Haga clic en el nombre de las asignaciones si la tarea o el problema ya están asignados.

1. Haga clic en **Avanzadas**.

   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. En el **Buscar personas, roles y equipos** , empiece a escribir el nombre de un usuario, función o equipo y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!NOTE]
   >
   >Si el nombre del usuario contiene un carácter especial, debe incluir el carácter especial en el campo de búsqueda.

1. (Opcional) Continúe agregando asignadores en la **Buscar personas, roles o equipos** para añadir varios recursos a la tarea o al problema.

   >[!TIP]
   >
   >* Puede asignar varios usuarios, funciones de trabajo o equipos. Solo puede asignar usuarios activos, funciones de trabajo y equipos.
   >
   >
   >* Al agregar una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función de trabajo para verla a medida que los agrega.
   >
   >
   >* Si se asignó un usuario, una función de trabajo o un equipo antes de desactivarlos, se asignarán al elemento de trabajo. En este caso, se recomienda lo siguiente:
      >   
      >   * Reasigne el elemento de trabajo a los recursos activos.
      >   * Asocie a los usuarios de un equipo desactivado con un equipo activo y reasigne el elemento de trabajo al equipo activo.


1. Para cada usuario de la variable **Usuario asignado** , especifique la siguiente información:


   * **Propietario**: Pase el ratón sobre el nombre del usuario asignado y haga clic en **Convertir en principal** en el campo Propietario si desea marcar al usuario asignado como el propietario de la tarea o del problema. Una casilla de verificación verde indica que el usuario especificado es el contacto principal de la tarea o problema. Adobe Workfront marca la primera función de usuario o trabajo que asigna a una tarea o problema como Propietario o Asignación Principal. Un equipo no puede ser designado como el propietario principal de una tarea o problema.

      >[!IMPORTANT]
      >
      >En función de cómo configure las preferencias del administrador de Workfront o del administrador de grupos de su proyecto, Workfront puede utilizar la programación del propietario de la tarea para calcular la cronología de la tarea cuando tenga varios usuarios asignados a la tarea. Para obtener información sobre los asignadores de tareas múltiples, consulte la sección &quot;Asignar varios usuarios a una tarea&quot; en el artículo [Asignación de tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Asignaciones** : Cuando el Tipo de duración de una tarea es Simple, especifique el número de horas que cada usuario o función de trabajo debe asignarse a la tarea. La suma de todas las horas asignadas a cada usuario es igual al número de la variable **Horas planificadas** en la parte inferior de la columna Asignaciones . En todos los demás casos, especifique el porcentaje de tiempo (o asignación) que desea que el usuario asignado invierta en resolver la tarea o el problema.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

      >[!TIP]
      >
      >
      >   
      >   
      >   * Después de modificar manualmente las asignaciones de asignación en las tareas, las horas planificadas de las tareas podrían actualizarse en consecuencia. Para obtener más información, consulte la sección &quot;Actualizar las horas planificadas de la tarea al administrar las asignaciones de usuarios&quot; en el artículo [Información general sobre las horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).
      >   * No puede modificar manualmente las asignaciones de asignación en problemas.
      >   * No puede modificar manualmente las asignaciones para los equipos asignados a tareas.


   * **Función del usuario asignado:** Seleccione la función que el usuario debe utilizar al realizar esta asignación.  La función principal del usuario se muestra de forma predeterminada. Haga clic en el cuadro Función del usuario asignado para seleccionar otra función.  Cuando asigna la tarea o el problema a una función primero y luego agrega un usuario que pueda cumplir esa función como segunda asignación, la lista de usuarios sugeridos se filtra para los usuarios que pueden cumplir las funciones ya asignadas a la tarea y el problema.

      ![](assets/advanced-assignments-box-select-a-role-350x243.png)

   * **Tipo de duración**: Esto solo está disponible para tareas. Haga clic en el nombre del Tipo de duración y seleccione un Tipo de duración en el menú desplegable. Para obtener información sobre los tipos de duración, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Duración:** Puede actualizar este campo para una tarea cuando tenga permisos de gestión para la tarea.

      Para obtener más información, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Cuando se edita la información de asignación de forma masiva, aparece un cuadro de diálogo similar para asignar usuarios, horas, asignación y propietario de tareas.

   * **Horas planificadas**: Cuando el tipo de duración es Asignación calculada o Simple, actualice el número de horas planificadas. Como resultado, los porcentajes de asignación o las horas de cada recurso se distribuyen de manera uniforme. Workfront calcula las horas planificadas cuando el tipo de duración es Trabajo calculado o Manejado de esfuerzo. Para obtener más información, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

      ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. Haga clic en **Guardar**.
