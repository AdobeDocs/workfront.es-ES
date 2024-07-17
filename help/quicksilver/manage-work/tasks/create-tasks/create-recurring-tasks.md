---
product-area: projects
navigation-topic: create-tasks
title: Creación de tareas recurrentes
description: Puede crear tareas recurrentes para las tareas que tenga que repetir como parte de un solo proyecto.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# Creación de tareas recurrentes

<!--Audited: 01/2024-->

Puede crear tareas recurrentes para las tareas que tenga que repetir como parte de un solo proyecto.

Para obtener información general acerca de tareas recurrentes, incluido el impacto de la edición de una tarea recurrente existente, vea [Información general sobre tareas recurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>Nuevo: estándar</p> 
   <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute para el proyecto con capacidad para Agregar tareas o superior</p> 
   <p>Al crear una tarea, recibe automáticamente permisos de administración para la tarea</p> 
   <p> Para obtener información acerca de los permisos de tareas, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartir una tarea </a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront. Para obtener más información acerca de los requisitos de acceso, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una tarea recurrente

>[!NOTE]
>
>No puede crear una tarea recurrente modificando una tarea existente. Debe crear una tarea desde cero.

1. Vaya al proyecto en el que desea crear una tarea recurrente y, a continuación, haga clic en la sección **Tareas** del panel izquierdo.
1. Haga clic en **Nueva tarea**.

   Aparece el cuadro de diálogo Nueva tarea.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Haga clic en **Más opciones** y, a continuación, escriba un nombre para la tarea en el campo **Nombre de tarea**.
1. Continúe actualizando la tarea del mismo modo que lo haría si agregara una tarea nueva. Para obtener más información sobre cómo agregar una tarea nueva, vea [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   La Duración y las Horas planificadas indicadas para una nueva tarea recurrente son la Duración y las Horas planificadas de cada ocurrencia. La duración de la tarea principal es el tiempo entre la fecha planificada de inicio de la tarea más temprana y la fecha planificada de finalización de la tarea más reciente. Las horas planificadas de la tarea principal son el total de todas las horas planificadas de todas las ocurrencias.

1. Haga clic en **Información general** en el panel izquierdo.
1. Desplácese hacia abajo hasta la sección **Programación de periodicidad** y, a continuación, seleccione la opción **Convertir en tarea recurrente**.

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

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
      <td> <p>La tarea se repite cada día, cada 2 días, cada 3 días, etc., según la cadencia seleccionada. Puede configurar las tareas para que se repitan hasta cada sexto día. El valor predeterminado es 1 día. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Día laborable</strong> </td> 
      <td> <p> La tarea se repite cada día laborable, cada 2 días laborables, cada 3 días laborables, etc., según la cadencia seleccionada. Puede configurar las tareas para que se repitan hasta cada sexto día laborable.</p> <p>Esta opción usa la programación predeterminada definida por el administrador del sistema, tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Semana</strong> </td> 
      <td> <p> La tarea se repite cada semana, cada 2 semanas, cada 3 semanas, etc., según la cadencia seleccionada.</p> <p>En el campo <strong>Repeticiones</strong>, seleccione el día de la semana en el que desea que se realice cada tarea. Puede seleccionar varios días. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mes</strong> </td> 
      <td> <p>La tarea se repite cada mes, cada 2 meses, cada 3 meses, etc., según la cadencia seleccionada. Puede seleccionar entre 1 y 12 meses. </p> <p>En el campo <strong>Repeticiones</strong>, seleccione entre las siguientes opciones cuando desee que se realice la tarea:</p> 
       <ul> 
        <li> <p><strong>cada mes en el día &lt;fecha del mes&gt;</strong> </p> <p>Puede seleccionar días del 1 al 30 o bien <strong>últimos</strong>. Por ejemplo, puede seleccionar "cada mes el día 30". </p> </li> 
        <li> <p><strong>todos los meses el &lt;number&gt; &lt;day of the week&gt;</strong> </p> <p>En el primer menú desplegable, puede seleccionar un número entre 1 y 4 para el número de la semana del mes o puede seleccionar "último". </p> <p>En el segundo menú desplegable, puede seleccionar cualquier día de la semana. </p> <p>Por ejemplo, puede seleccionar "cada mes el segundo martes". </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Si tiene una excepción de programación asociada a la programación del proyecto, las tareas recurrentes no pueden iniciarse durante la excepción. Las tareas recurrentes que se producen durante la excepción de programación están programadas para iniciarse el primer día hábil que sigue a la excepción. Para obtener más información sobre las excepciones de horario, consulte el artículo [Crear un horario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. En el campo **Comienza**, seleccione la fecha y la hora en que desea que comiencen las tareas recurrentes.
1. En el campo **Finaliza**, seleccione la fecha y la hora en que desea que se completen las tareas periódicas

   O

   Seleccione **después de `<number>` repeticiones** para indicar cuántas veces debe ocurrir la tarea recurrente. Workfront crea el mismo número de repeticiones para las tareas que el número indicado en este campo.

1. Haga clic en **Crear tarea.**

   Se muestra la lista de tareas. La tarea recurrente se crea como una tarea principal y todas las recurrencias son sus tareas secundarias. Workfront generó automáticamente los nombres de las tareas secundarias, utilizando el nombre introducido para el principal seguido de un número. Las tareas recurrentes se colocan al final de la lista de tareas.

   Para obtener más información sobre los campos que se rellenan automáticamente a partir de la tarea principal recurrente, consulte [Información general sobre tareas recurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Opcional) Modifique cada tarea recurrente como lo haría con cualquier otra tarea del proyecto.

   Por ejemplo, puede agregar asignaciones, predecesoras y duraciones, así como modificar cualquier otra información sobre la tarea, incluidos los campos personalizados.

   >[!IMPORTANT]
   >
   >Modificar la periodicidad principal después de que los hijos se hayan modificado individualmente puede causar información diferente entre los hijos o entre los hijos y el padre. Para obtener más información, vea [Información general sobre tareas recurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
