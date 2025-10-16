---
product-area: projects
navigation-topic: manage-tasks
title: Copiar y duplicar tareas
description: Puede copiar una tarea de un proyecto a otro o duplicar una tarea dentro del mismo proyecto.
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '1679'
ht-degree: 99%

---

# Copiar y duplicar tareas

Puede copiar una tarea de un proyecto a otro o duplicar una tarea dentro del mismo proyecto.

Puede copiar o duplicar una o varias tareas o tareas principales a la vez.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración de una tarea</p> <p>Permisos de aportación o superiores para el proyecto</p> 
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
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Consideraciones para copiar tareas

Al copiar una tarea, tenga en cuenta lo siguiente:

* Al copiar una tarea de un proyecto a otro, es posible que se recalculen las fechas de las tareas. Para realizar un nuevo cálculo se tendrá en consideración la programación que utiliza el nuevo proyecto y la información de Programación desde del proyecto.
* Los formularios personalizados se copian con la tarea. La información de los campos personalizados se transfiere a las tareas copiadas únicamente cuando selecciona copiar Datos personalizados al copiar la tarea.
* Tiene la oportunidad de seleccionar copiar algunos elementos asociados con la tarea a la tarea copiada durante el proceso de copia. Sin embargo, de forma predeterminada, los siguientes objetos no se transfieren a la tarea copiada:
   * Problemas
   * Horas registradas
   * Comentarios de usuarios <!--not sure about this, enable only if requested by users and verified by Product: System activity comments transfer to the new task if they relate to information that you specifically select to be copied. For example, if you select to copy Expenses to the new task, system comments that identify adding expenses to the task will transfer to the copied task. -->
* Los siguientes elementos se mueven a la tarea copiada de forma predeterminada:

   * Los hitos se transfieren a la tarea copiada y se eliminan de la tarea original.
   * Las subtareas se transfieren a la nueva tarea.

* Puede copiar una tarea a la vez, o puede copiar varias tareas a la vez cuando edita tareas en una lista.

## Copiar tareas en una lista {#copy-tasks-in-a-list}

1. Vaya al proyecto que contiene las tareas que desea copiar.

   O

   Ir a un informe de tareas.

1. (Condicional) Haga clic en **Tareas** en el panel izquierdo si ha abierto el proyecto que contiene las tareas.
1. Haga clic en el icono **Modo de plan** ![](assets/qs-list-mode-or-save-mode-icon-small.png) y asegúrese de que la opción **Guardar automáticamente** esté habilitada.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Solo puede copiar tareas en una lista cuando guarda automáticamente los cambios. Para obtener información acerca de cómo guardar opciones al editar tareas, vea [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Seleccione la tarea o tareas que desee copiar y realice una de las siguientes acciones:

   * Haga clic en el **menú Más** en la parte superior de la lista de tareas y luego haga clic en **Copiar en**.
   * Haga clic con el botón derecho en las tareas seleccionadas y luego haga clic en **Copiar en**.
   * Al seleccionar una tarea, haga clic en el menú **Más** ![](assets/more-icon-task-list.png) junto al nombre de la tarea en la lista y, a continuación, haga clic en **Copiar en**.

   ![](assets/copy-task-in-list-nwe-350x131.png)

1. Continúe copiando la tarea, tal como se describe en la sección [Copie una tarea en el nivel de tarea](#copy-a-task-at-the-task-level) a partir del paso 4.

   <!--
      (NOTE: is this still accurate?!)
   -->

## Copiar una tarea en el nivel de tarea {#copy-a-task-at-the-task-level}

Además de copiar tareas en una lista de tareas, también puede copiar una tarea después de haberla abierto.

1. Encuentre una tarea en el sistema de Workfront buscándola.
1. Haga clic en el nombre de la tarea para abrirla.
1. Haga clic en el menú desplegable **Más** ![](assets/qs-more-menu.png) junto al nombre de la tarea y, a continuación, haga clic en **Copiar en**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   Se muestra el cuadro Copiar tarea.

1. (Opcional) Actualice el **Nombre de tarea**.

   >[!TIP]
   >
   >Este campo aparece atenuado y no se puede editar al seleccionar copiar varias tareas en una lista. Puede pasar el puntero por encima del campo Nombre de la tarea y se mostrará una lista de todas las tareas seleccionadas.
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. Escriba el nombre del **Proyecto de destino** donde desea copiar la tarea en el campo **Seleccionar proyecto de destino**.

   >[!TIP]
   >
   >* El nombre del proyecto distingue entre mayúsculas y minúsculas.
   >* También puede empezar a escribir el número de referencia o introducir el ID del proyecto. Esto puede ayudarle a distinguir entre proyectos con nombres idénticos.
   >* En la lista solo se muestran 100 proyectos.

   El nombre del proyecto actual se muestra de forma predeterminada. Si desea copiar la tarea dentro del mismo proyecto, deje este campo sin cambiar.

1. (Condicional) Haga clic en **solicitar acceso** para solicitar acceso al proyecto si no tiene acceso al proyecto seleccionado.
1. (Condicional) Continúe copiando la tarea en el proyecto de destino seleccionado sin solicitar acceso si tiene acceso para añadir tareas a una de las tareas del proyecto de destino.

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Se muestran mensajes similares si el proyecto seleccionado está pendiente de aprobación, completado o inactivo, cuando el administrador de Workfront impide añadir tareas a estos proyectos. Para obtener más información, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Haga clic en **Opciones** en el panel izquierdo y, a continuación, anule la selección de los atributos de la tarea que no desee copiar con la tarea. Todas las opciones están seleccionadas de forma predeterminada.

   >[!TIP]
   >
   >Si selecciona y luego anula la selección de **Seleccionar todo**, se anula la selección de todas las opciones.

   Anule la selección de las siguientes opciones para no transferirlas a la tarea copiada. En la tabla siguiente se describe lo que sucede cuando se anula la selección de las opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Restricción</td> 
      <td> <p>La restricción de tarea se establece en Lo antes posible o Lo más tarde posible según la configuración del modo de programación del proyecto.</p> <p> Cuando se selecciona esta opción, la restricción actual de la tarea se transfiere a la tarea copiada. </p> <p>Nota: Al mover o copiar una tarea con restricciones específicas de fecha a otro proyecto y las fechas de restricción de la tarea están fuera de las fechas del nuevo proyecto, la restricción de tarea cambia a Lo antes posible o Lo más tarde posible, o se ajustan las fechas de inicio o de finalización planificadas de los proyectos. Algunos ejemplos de restricciones de tareas específicas de fecha son Debe iniciarse el, Debe finalizarse el, No iniciar no antes del, No iniciar después del, etc. Para obtener información sobre las restricciones de tarea y cómo pueden verse afectadas las restricciones de tareas o las fechas de proyectos, vea <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre las restricciones de tarea</a> y busque una restricción específica.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Asignaciones</td> 
      <td> <p>Todas las asignaciones se eliminan de la tarea. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proceso de aprobación</td> 
      <td>Todos los procesos de aprobación se eliminan de la tarea.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progreso</td> 
      <td>El estado de la tarea es Nuevo. De lo contrario, la tarea copiada mantiene el estado de la tarea existente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Información financiera</td> 
      <td>Se elimina la información financiera de la tarea.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todas las predecesoras</td> 
      <td> <p>Esto significa que las dependencias no se transferirán a las tareas copiadas. </p> <p>Si se selecciona esta opción, se conservan las tareas predecesoras dentro del grupo de tareas copiadas y se eliminan otras.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Los documentos adjuntos a la tarea no se transfieren a la tarea copiada. Esto incluye versiones, pruebas y documentos vinculados.</p> <p>Esto no incluye las aprobaciones de documentos. Las aprobaciones de documentos nunca se pueden copiar cuando se copia una tarea.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Los recordatorios de una tarea no se transfieren a la tarea copiada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Los gastos registrados en la tarea no se transfieren a la tarea copiada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permisos</td> 
      <td>Workfront elimina los nombres de todas las entidades que se muestran en la lista de uso compartido de la tarea. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td> <p>Los valores de los campos personalizados se borran y los formularios personalizados se transfieren a la tarea copiada. </p> <p>Cuando se seleccionan, tanto los formularios como los valores de los campos personalizados se transfieren a la tarea copiada. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Haga clic en **Seleccionar principal** en el panel izquierdo y, a continuación, seleccione la tarea en el proyecto de destino que desea que sea la principal de la tarea copiada.

   >[!TIP]
   >
   >Al seleccionar copiar varias tareas en una lista, todas las tareas seleccionadas se convierten en las tareas secundarias de la principal seleccionada.

   Seleccione un elemento principal mediante una de las siguientes acciones:

   * En la lista de tareas, seleccione uno de los elementos principales del plan del proyecto.
   * Haga clic en el icono de búsqueda ![icono de Búsqueda](assets/search-icon.png) y busque una tarea principal por su nombre.

   La tarea se muestra en la lista.

   ![Seleccione la tarea principal al mover una tarea con la funcionalidad de búsqueda ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Seleccione el botón de opción del elemento principal, una vez encontrado.

   Si no selecciona una tarea principal, las tareas se copian como tareas principales en lugar de como subtareas y se colocan al final de la lista de tareas en el proyecto de destino.

1. Haga clic en **Copiar tarea**

   O

   Haga clic en **Copiar tareas** cuando seleccione varias tareas en una lista.
Las tareas copiadas ahora se encuentran en el proyecto especificado y son subtareas de la tarea principal seleccionada o de las últimas tareas del proyecto.

## Duplicar tareas

Puede duplicar rápidamente una tarea en una lista de tareas si necesita una tarea idéntica en el mismo proyecto.

* [Consideraciones para duplicar tareas](#considerations-for-duplicating-tasks)
* [Duplicar tareas](#duplicate-tasks)

### Consideraciones para duplicar tareas {#considerations-for-duplicating-tasks}

* Puede duplicar una tarea en una lista de tareas solo cuando la lista está ordenada por número de tarea.
* La nueva tarea tendrá el mismo nombre que la tarea original.
* No puede seleccionar qué información está duplicada en la nueva tarea. Casi toda la información de la tarea original se transferirá a la tarea duplicada, incluida la relación con la tarea principal, de forma predeterminada.
* Los elementos siguientes no se transfieren a la nueva tarea:

   * Horas registradas
   * Notas
   * Problemas
   * Solo las tareas predecesoras que están en el mismo grupo de tareas copiadas también se copian con sus tareas sucesoras.

     **EJEMPLO**

     Por ejemplo, si copia la Tarea 2 y su predecesora, la Tarea 1, al mismo tiempo, tendrá una copia de la Tarea 2 y una copia de la Tarea 1. La copia de la Tarea 1 será la predecesora de la copia de la Tarea 2. Pero si copia solo la Tarea 2 sin copiar su predecesora, su copia no tendrá predecesora.

* Al duplicar una tarea principal, también se duplican todas las tareas secundarias, incluso cuando estas últimas no están seleccionadas.
* Puede duplicar una o varias tareas al mismo tiempo.

  Sin embargo, no puede duplicar varias tareas que no sean secuenciales al mismo tiempo.

* Los hitos se mueven a la nueva tarea y se eliminan de la tarea original.

### Duplicar tareas

1. Vaya al proyecto que contiene la tarea o tareas que desea duplicar.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Realice una de las siguientes acciones:

   * (Condicional) Haga clic en el icono **Modo de plan** ![](assets/qs-list-mode-or-save-mode-icon-small.png) y asegúrese de que la opción **Guardar automáticamente** esté habilitada, seleccione las tareas que desee duplicar y, a continuación, haga clic en el **menú Más** ![](assets/qs-more-menu-29x11.png) > **Duplicar**.

     ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * (Condicional) Haga clic en el icono **Modo de plan** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Guardar de forma manual** > **Estándar** o **Planificación de escala de tiempo**, y después haga lo siguiente:

      1. Seleccione la tarea o tareas que desee duplicar y haga clic en **Duplicar**.
      1. (Opcional) Haga clic en **Deshacer** para revertir los cambios y no duplicar las tareas.
      1. (Opcional y condicional) Haga clic en **Rehacer** si anteriormente había hecho clic en **Deshacer** para conservar los cambios y duplicar las tareas.

      1. Haga clic en **Guardar** para guardar los cambios.

         Las tareas se duplican y se añaden al mismo proyecto que las tareas originales.
