---
product-area: projects
navigation-topic: create-tasks
title: Crear tareas recurrentes
description: Puede crear tareas recurrentes para las tareas que debe repetir como parte de un solo proyecto.
author: Alina
feature: Work Management
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Crear tareas recurrentes

Puede crear tareas recurrentes para las tareas que debe repetir como parte de un solo proyecto.

Para obtener información general sobre las tareas recurrentes, incluido el impacto de editar una tarea recurrente existente, consulte [Información general sobre las tareas recurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

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
   <td> <p>Editar acceso a Tareas y proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a las tareas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Concesión de acceso a tareas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute para el proyecto con capacidad para agregar tareas o superior</p> <p>Cuando crea una tarea, automáticamente recibe permisos de gestión para la tarea</p> <p> Para obtener información sobre los permisos de tareas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartir una tarea </a>. </p> <p>Para obtener información sobre la solicitud de permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear una tarea recurrente

>[!NOTE]
>
>No se puede crear una tarea recurrente modificando una tarea existente. Debe crear una tarea desde cero.

1. Vaya al proyecto en el que desea crear una tarea recurrente y, a continuación, haga clic en el botón **Tareas** en el panel izquierdo.
1. Haga clic en **Nueva tarea**.

   Aparece el cuadro de diálogo Nueva tarea .

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Haga clic en **Más opciones** a continuación, introduzca un nombre para la tarea en la **Nombre de la tarea** campo .
1. Continúe actualizando la tarea del mismo modo que lo haría si agregara una tarea nueva. Para obtener más información sobre cómo agregar una tarea nueva, consulte [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)
1. Haga clic en **Información general** en el panel izquierdo.
1. Desplácese hacia abajo hasta el **Programación de periodicidad** y, a continuación, seleccione **Convertir en una tarea recurrente** .

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. En el **Frecuencia** lista desplegable, seleccione el número de unidades de tiempo en las que desea que se realice la tarea y el tipo de unidades de tiempo. Seleccione entre las siguientes opciones:

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
      <td role="rowheader"><strong>días</strong> </td> 
      <td> <p>La tarea se repite todos los días, cada 2 días, cada 3 días, etc., según la cadencia que seleccione. Puede configurar tareas para que se repitan hasta cada 6 días. El valor predeterminado es 1 día. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Día de trabajo</strong> </td> 
      <td> <p> La tarea se repite cada día laborable, cada 2 días hábiles, cada 3 días hábiles, etc., según la cadencia seleccionada. Puede configurar las tareas para que se repitan hasta cada sexto día hábil.</p> <p>Esta opción utiliza la programación predeterminada definida por el administrador del sistema, tal como se describe en <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Semana</strong> </td> 
      <td> <p> La tarea se repite cada semana, cada 2 semanas, cada 3 semanas, etc., según la cadencia que seleccione.</p> <p>En el <strong>Repetidas</strong> , seleccione el día de la semana en el que desea que se produzca cada tarea. Puede seleccionar varios días. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mes</strong> </td> 
      <td> <p>La tarea se repite cada mes, cada 2 meses, cada 3 meses, etc., según la cadencia que seleccione. Puede seleccionar entre 1 y 12 meses. </p> <p>En el <strong>Repetidas</strong> , seleccione entre las siguientes opciones cuando desee que se produzca la tarea:</p> 
       <ul> 
        <li> <p><strong>todos los meses &lt;month date=""&gt;</strong> </p> <p>Puede seleccionar días del 1 al 30 o seleccionar <strong>last</strong>. Por ejemplo, puede seleccionar "cada mes del día 30". </p> </li> 
        <li> <p><strong>todos los meses &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>En el primer menú desplegable, puede seleccionar un número entre 1 y 4 para el número de la semana del mes, o bien seleccionar "último". </p> <p>En el segundo menú desplegable, puede seleccionar cualquier día de la semana. </p> <p>Por ejemplo, puede seleccionar "cada mes del segundo martes". </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Si tiene una excepción de programación asociada con la programación del proyecto, las tareas recurrentes no se pueden iniciar durante la excepción. Las tareas recurrentes que se producen durante la excepción de programación están programadas para iniciarse en el primer día hábil siguiente a la excepción. Para obtener más información sobre las excepciones de programación, consulte el artículo [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. En el **Inicios** , seleccione la fecha y la hora en que desea que comiencen las tareas recurrentes.
1. En el **Finaliza** , seleccione la fecha y la hora en que desea que se completen las tareas recurrentes

   O

   Select **after `<number>` ocurrencias** para indicar cuántas veces debe ocurrir la tarea recurrente. Workfront crea el mismo número de recurrencias para las tareas que el número indicado en este campo.

1. Haga clic en **Crear tarea.**

   Se muestra la lista de tareas. La tarea recurrente se crea como principal y todas las recurrencias son secundarias. Workfront generó automáticamente los nombres de las tareas secundarias utilizando el nombre introducido para el elemento principal seguido de un número. Para obtener más información sobre los campos que se rellenan automáticamente desde la tarea recurrente principal, consulte [Información general sobre las tareas recurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Opcional) Modifique cada tarea recurrente como lo haría con cualquier otra tarea del proyecto.

   Por ejemplo, puede agregar asignaciones, predecesores, duraciones y modificar cualquier otra información sobre la tarea, incluidos los campos personalizados.

   >[!IMPORTANT]
   >
   >Modificar la recurrencia del padre después de que se hayan modificado individualmente los hijos puede causar información diferente entre el hijo o entre el hijo y el padre. Para obtener más información, consulte [Información general sobre las tareas recurrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
