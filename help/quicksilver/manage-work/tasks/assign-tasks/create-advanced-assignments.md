---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Crear asignaciones avanzadas
description: Puede administrar asignaciones de tareas o problemas mediante Asignaciones avanzadas.
author: Alina
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: ad5d6bfda24119076df8336ed291c0ba63e2c88a
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 0%

---

# Crear asignaciones avanzadas

{{highlighted-preview}}

Puede administrar asignaciones de tareas o problemas mediante Asignaciones avanzadas.

Puede ajustar la siguiente información de asignación al realizar asignaciones avanzadas:

* Asignar usuarios a la tarea o al problema (esto puede realizarse fuera de una asignación avanzada).
* Ajuste y redistribuya el número de horas que se asignan a cada usuario asignado.
* Determine qué usuario debe designarse como propietario o principal asignado a la tarea o al problema.
* Especifique la función que cumple cada usuario al trabajar en la tarea o el problema.
  <!--* <span class="preview">Override the billing rate for a job role.</span>-->

>[!NOTE]
>
>Al asignar usuarios para trabajar, su disponibilidad según sus programaciones afecta a las Fechas planificadas y proyectadas de las tareas y problemas. Para obtener información sobre las programaciones, consulte [Creación de una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Áreas de Adobe Workfront donde puede realizar asignaciones avanzadas

Este artículo describe cómo acceder a las asignaciones avanzadas en el encabezado de la tarea o del problema.

Además, puede realizar asignaciones avanzadas en las siguientes áreas de Workfront:

* En listas e informes cuando el campo Asignaciones aparece en la vista.
* En la sección Asignaciones al editar una tarea. Para obtener más información, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* En el encabezado de la tarea o del problema, en el área Asignaciones.
* En el Distribuidor de cargas de trabajo. Para obtener más información, consulte [Asignar trabajo manualmente mediante el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Problemas</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Aportar o permisos superiores a una tarea o problema</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Realizar asignaciones avanzadas

1. Vaya al proyecto donde desea asignar una tarea o un problema.
1. Clic **Tareas** o **Problemas** en el panel izquierdo, haga clic en el nombre de una tarea o problema en la lista.

   >[!TIP]
   >
   >Puede realizar asignaciones avanzadas directamente en la lista de tareas o problemas si hay dos o más personas asignadas. Haga clic dentro de **Asignaciones** en la misma línea que la tarea o el problema y, a continuación, haga clic en **Icono Personas** para abrir la ventana Asignaciones avanzadas. Pase al paso 5 para continuar creando asignaciones avanzadas.\
   >![](assets/nwe-advanced-assignments-350x55.png)
   >

1. Clic **Asignar a** en el **Asignaciones** en el encabezado de la tarea o problema

   O

   Haga clic en el nombre de las asignaciones si la tarea o el problema ya está asignado.

1. Clic **Avanzadas**.

   Imagen de muestra en el entorno de producción:
   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

   <span class="preview">Imagen de muestra en el entorno de vista previa:</span>
   ![Haga clic en Avanzadas](assets/assignments-box-in-task-header.png)

1. En el **Buscar personas, funciones y equipos** , empiece a escribir el nombre de un usuario, función o equipo y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!NOTE]
   >
   >Si el nombre del usuario contiene un carácter especial, debe incluirlo en el campo de búsqueda.

1. (Opcional) Continúe añadiendo usuarios asignados en la **Buscar personas, funciones o equipos** para agregar varios recursos a la tarea o al problema.

   >[!TIP]
   >
   >* Puede asignar varios usuarios, roles o equipos. Solo puede asignar usuarios activos, roles y equipos.
   >
   >
   >* Al agregar una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos.
   >Los usuarios deben estar asociados con al menos un rol para verlo a medida que los agregue.
   >Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Concesión de acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Si se asignó un usuario, un rol o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >   
   >   * Reasignar el elemento de trabajo a los recursos activos.
   >   * Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.
   >

   <!-- SHOULD BE THIRD BULLET POINT IN TIP TABLE WHEN THIS FEATURE IS RELEASED 
    * <span class="preview">When adding a job role assignment, you can search for the job role or location. Select the System/Default Job Role to use the default billing rate for the assignment, or select a Rate Card Job Role to override the rate at the assignment level. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
    -->

1. Para cada usuario en la **Asignado** , especifique la siguiente información:


   * **Propietario**: Pase el ratón sobre el nombre del usuario asignado y haga clic en **Convertir en principal** en el campo Propietario si desea marcar al usuario asignado como propietario de la tarea o del problema. La casilla de verificación verde indica que el usuario especificado es el contacto principal de la tarea o el problema. Adobe Workfront marca el primer usuario o rol que asigna a una tarea o problema como Asignación principal o Propietario. No se puede designar a un equipo como propietario principal de una tarea o un problema.

     >[!IMPORTANT]
     >
     >Según la forma en que el administrador de Workfront o el administrador del grupo hayan configurado las preferencias del proyecto, Workfront podría utilizar la programación del propietario de la tarea para calcular la cronología de la tarea cuando tenga varios usuarios asignados a la tarea. Para obtener información sobre los usuarios asignados a varias tareas, consulte la sección &quot;Asignar varios usuarios a una tarea&quot; en el artículo [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Asignaciones** : Cuando el tipo de duración de una tarea es Simple, especifique el número de horas que cada usuario o rol debe asignarse a la tarea. La suma de todas las horas asignadas a cada usuario es igual al número de la **Horas planificadas** en la parte inferior de la columna Asignaciones. En todos los demás casos, especifique el porcentaje de tiempo (o asignación) que desea que el usuario asignado dedique a resolver la tarea o el problema.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

     >[!TIP]
     >
     >
     >   
     >   
     >   * Después de modificar manualmente las asignaciones de las tareas, las horas planificadas de las tareas podrían actualizarse en consecuencia. Para obtener más información, consulte la sección &quot;Actualizar las horas planificadas de la tarea al administrar las asignaciones de usuario&quot; en el artículo [Resumen de horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).
     >   * No se pueden modificar manualmente las asignaciones de los problemas.
     >   * No se pueden modificar manualmente las asignaciones de los equipos asignados a tareas.
     >   
     >

   * **Rol de asignado:** Seleccione la función que el usuario debe utilizar al cumplir esta asignación.  La Función principal del usuario se muestra de forma predeterminada. Haga clic en el cuadro Función de asignado para seleccionar otra función.  Al asignar primero la tarea o el problema a un rol y, a continuación, agregar un usuario que pueda cumplir ese rol como segunda asignación, la lista de usuarios sugeridos se filtra para los usuarios que pueden cumplir los roles ya asignados a la tarea y al problema.

     Imagen de muestra en el entorno de producción:
     ![](assets/advanced-assignments-box-select-a-role-350x243.png)

     <span class="preview">Imagen de muestra en el entorno de vista previa:</span>
     ![Rol de asignado](assets/advanced-assignments-select-role.png)

   <!--<div class="preview">

   * **Location**: The location comes from the rate card, if a rate card attached to the project uses locations with the job roles. The location can't be changed. 

   * **Billing Rates**: The billing rate for a user comes from the system rate for the user or their associated job role. The billing rate for a job role comes from the system rate or from the rate card, if a rate card is attached to the project. Existing billing rates are not displayed in this field. Click in the field to change the billing rate for this specific task assignment.

   </div>-->

   * **Tipo de duración**: Esto solo está disponible para tareas. Haga clic en el nombre del tipo de duración y seleccione un tipo de duración en el menú desplegable. Para obtener información sobre los tipos de duración, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Duración:** Puede actualizar este campo para una tarea cuando tenga permisos de administración para la tarea.

     Para obtener más información, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Al editar por lotes la información de la asignación, aparece un cuadro de diálogo similar para asignar usuarios, horas, asignación y propietario de la tarea.

   * **Horas planificadas**: cuando el tipo de duración es Asignación calculada o Simple, actualice el número de horas planificadas. Como resultado, los porcentajes de asignación o las horas de cada recurso se distribuyen de forma uniforme. Workfront calcula las horas planificadas cuando el tipo de duración es Trabajo calculado o Condicionado por el esfuerzo. Para obtener más información, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

     Imagen de muestra en el entorno de producción:
     ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

     <div class="preview">

     Imagen de muestra en el entorno de vista previa:
     ![Asignaciones avanzadas](assets/advanced-assignments-duration-type-allocations.png)

     </div>

1. Haga clic en **Guardar**.
