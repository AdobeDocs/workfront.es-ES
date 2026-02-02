---
product-area: projects
navigation-topic: create-tasks
title: Crear tareas recurrentes
description: Puede crear tareas recurrentes para las tareas que deba repetir como parte de un solo proyecto.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '890'
ht-degree: 97%

---

# Crear tareas recurrentes

<!--Audited: 01/2024-->

Puede crear tareas recurrentes para las tareas que deba repetir como parte de un solo proyecto.

Para obtener información general acerca de tareas recurrentes, incluido el impacto de la edición de una tarea recurrente existente, consulte [Información general sobre tareas recurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de aportación para el proyecto con capacidad para Añadir tareas o superior</p> 
   <p>Al crear una tarea, recibe automáticamente permisos de administración para dicha tarea</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p> 
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> 
   <p>When you create a task you automatically receive Manage permissions to the task</p> 
   <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator. For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Crear una tarea recurrente

>[!NOTE]
>
>No puede crear una tarea recurrente modificando una tarea existente. Debe crear una tarea desde cero.

1. Vaya al proyecto en el que desea crear una tarea recurrente y, a continuación, haga clic en la sección **Tareas** del panel izquierdo.
1. Haga clic en **Nueva tarea**.

   Aparece el cuadro de diálogo Nueva tarea.

   ![Crear pantalla pequeña de tarea](assets/nwe-create-task-small-screen-350x272.png)

1. Haga clic en **Más opciones** y, a continuación, escriba un nombre para la tarea en el campo **Nombre de la tarea**.
1. Continúe actualizando la tarea del mismo modo que lo haría si añadiera una tarea nueva. Para obtener más información sobre cómo añadir una tarea nueva, consulte [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   La duración y las horas planificadas indicadas para una nueva tarea recurrente son la duración y las horas planificadas de cada ocurrencia. La duración de la tarea principal es el tiempo entre la fecha de inicio planificada de la tarea más temprana y la fecha planificada de finalización de la tarea más reciente. Las horas planificadas de la tarea principal son el total de horas planificadas de todas las ocurrencias.

1. Haga clic en **Información general** en el panel izquierdo.
1. Desplácese hacia abajo hasta la sección **Programación de periodicidad** y, a continuación, seleccione la opción **Convertir en tarea recurrente**.

   ![Tareas recurrentes nuevas de la selección de programación de periodicidad](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. En la lista desplegable **Frecuencia**, seleccione el número de unidades de tiempo en que desea que se realice la tarea y el tipo de unidades de tiempo. Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo de periodicidad</th> 
      <th>Descripción</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Día</strong> </td> 
      <td> <p>La tarea se repite todos los días, cada dos o tres días, etc., según la cadencia seleccionada. Puede configurar las tareas para que se repitan hasta cada seis días. El valor predeterminado es un día. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Día laborable</strong> </td> 
      <td> <p> La tarea se repite todos los días, cada dos o tres días laborables, etc., según la cadencia seleccionada. Puede configurar las tareas para que se repitan hasta seis días laborables.</p> <p>Esta opción usa la programación predeterminada definida por el administrador del sistema, tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Semana</strong> </td> 
      <td> <p> La tarea se repite todas las semanas, cada dos o tres semanas, etc., según la cadencia seleccionada.</p> <p>En el campo <strong>Repeticiones</strong>, seleccione el día de la semana en el que desea que se realice cada tarea. Puede seleccionar varios días. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mes</strong> </td> 
      <td> <p>La tarea se repite cada mes, cada dos o tres meses, etc., según la cadencia seleccionada. Puede seleccionar entre 1 y 12 meses. </p> <p>En el campo <strong>Repeticiones</strong>, seleccione entre las siguientes opciones cuando desee que se realice la tarea:</p> 
       <ul> 
        <li> <p><strong>cada mes el día &lt;fecha del mes&gt;</strong> </p> <p>Puede seleccionar días del 1 al 30 o bien los <strong>últimos</strong>. Por ejemplo, puede seleccionar “cada mes el día 30”. </p> </li> 
        <li> <p><strong>todos los meses el &lt;number&gt; &lt;day of the week&gt;</strong> </p> <p>En el primer menú desplegable, puede seleccionar un número entre 1 y 4 para el número de la semana del mes o puede seleccionar “último”. </p> <p>En el segundo menú desplegable, puede seleccionar cualquier día de la semana. </p> <p>Por ejemplo, puede seleccionar “el segundo martes de cada mes”. </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Si tiene una excepción de programación asociada a la programación del proyecto, las tareas recurrentes no pueden iniciarse durante la excepción. Las tareas recurrentes que se producen durante la excepción de programación están programadas para iniciarse el primer día hábil posterior a la excepción. Para obtener más información sobre las excepciones de programación, consulte el artículo [Crear programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. En el campo **Comienza**, seleccione la fecha y la hora en que desea que comiencen las tareas recurrentes.
1. En el campo **Finaliza**, seleccione la fecha y la hora en que desea que se completen las tareas recurrentes

   O

   Seleccione **después de `<number>` repeticiones** para indicar cuántas veces debe producirse la tarea recurrente. Workfront crea la misma periodicidad para las tareas que el número indicado en este campo.

1. Haga clic en **Crear tarea.**

   Se muestra la lista de tareas. La tarea recurrente se crea como una tarea principal y todas las recurrencias son sus tareas secundarias. Workfront generó automáticamente los nombres de las tareas secundarias, utilizando el nombre introducido para la principal seguido de un número. Las tareas recurrentes se colocan al final de la lista de tareas.

   Para obtener más información sobre los campos que se rellenan automáticamente a partir de la tarea principal recurrente, consulte [Información general sobre las tareas recurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![Tareas recurrentes en la lista de tareas](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Opcional) Modifique cada tarea recurrente como lo haría con cualquier otra tarea del proyecto.

   Por ejemplo, puede añadir asignaciones, predecesoras y duraciones, así como modificar cualquier otra información sobre la tarea, incluidos los campos personalizados.

   >[!IMPORTANT]
   >
   >Modificar la periodicidad principal después de que las tareas secundarias se hayan modificado individualmente puede causar información diferente entre las tareas secundarias y la principal. Para obtener más información, consulte [Información general sobre las tareas recurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
