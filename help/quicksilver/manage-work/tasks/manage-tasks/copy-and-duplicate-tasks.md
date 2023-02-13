---
product-area: projects
navigation-topic: manage-tasks
title: Copiar y duplicar tareas
description: Puede copiar una tarea de un proyecto en otro o duplicarla dentro del mismo proyecto.
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1670'
ht-degree: 1%

---

# Copiar y duplicar tareas

Puede copiar una tarea de un proyecto en otro o duplicarla dentro del mismo proyecto.

Puede copiar o duplicar una o varias tareas o tareas principales a la vez.

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
   <td> <p>Trabajo o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en una tarea </p> <p>Contribute o permisos superiores para el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones para copiar tareas

Tenga en cuenta lo siguiente al copiar una tarea:

* Los problemas no se copian con la tarea.
* Los hitos se transfieren a la tarea copiada y se eliminan de la tarea original.

Puede copiar una tarea en las siguientes áreas de la aplicación web de Adobe Workfront:

* En el nivel de tarea, desde el **Más icono** ![](assets/qs-more-menu-19x7.png) a la derecha del nombre de la tarea.

   Para obtener más información, consulte la [Copiar una tarea en el nivel de tarea](#copy-a-task-at-the-task-level) en este artículo.

* En una lista de tareas, realizando una de las siguientes acciones:

   * Haga clic con el botón derecho en el nombre de una tarea.
   * Seleccione la tarea (o tareas) y expanda el **Más** icono ![](assets/more-icon-task-list.png) en la parte superior de la lista de tareas.
   * Seleccione una tarea y expanda el **Más** icono ![](assets/more-icon-task-list.png) junto al nombre de la tarea.

      Esta opción no está disponible al seleccionar varias tareas.
   Para obtener más información, consulte la [Copiar tareas en una lista](#copy-tasks-in-a-list) en este artículo.

## Copiar tareas en una lista {#copy-tasks-in-a-list}

1. Vaya al proyecto que contiene la tarea o tareas que desea copiar.

   O

   Vaya a un informe de tareas.

1. Haga clic en **Tareas** en el panel izquierdo.
1. Haga clic en el **Menú del modo Plan** ![](assets/qs-list-mode-or-save-mode-icon-small.png) , luego **Autoguardar**.

   >[!IMPORTANT]
   >
   >Puede copiar tareas en una lista solo cuando guarde automáticamente los cambios. Para obtener información sobre cómo guardar opciones al editar tareas, consulte [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Seleccione la tarea o tareas que desee copiar y realice una de las siguientes acciones:

   * Haga clic en el **Más menú** en la parte superior de la lista de tareas, haga clic en **Copiar en**.
   * Haga clic con el botón derecho en las tareas seleccionadas y, a continuación, haga clic en **Copiar en**.
   * Al seleccionar una tarea, haga clic en el botón **Más** menú ![](assets/more-icon-task-list.png) junto al nombre de la tarea en la lista y, a continuación, haga clic en **Copiar en**.
   ![](assets/copy-task-in-list-nwe-350x131.png)

1. Continúe copiando la tarea, tal como se describe en la sección [Copiar una tarea en el nivel de tarea](#copy-a-task-at-the-task-level) a partir del paso 4.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this still accurate?!)
   </MadCap:conditionalText>
   -->

## Copiar una tarea en el nivel de tarea {#copy-a-task-at-the-task-level}

Además de copiar tareas en una lista de tareas, también puede copiar una tarea después de abrirla. 

1. Busque una tarea en el sistema de Workfront.
1. Haga clic en el nombre de la tarea para abrirla. 
1. Haga clic en el **Más** menú desplegable ![](assets/qs-more-menu.png) junto al nombre de la tarea y, a continuación, haga clic en **Copiar** **a**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   Aparece el cuadro Copiar tarea .

1. (Opcional) Actualice el **Nombre de la tarea**.

   >[!TIP]
   >
   >Este campo está atenuado y no se puede editar al seleccionar para copiar varias tareas en una lista. Puede situarse sobre el campo Nombre de la tarea y se mostrará una lista de todas las tareas seleccionadas.
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. Escriba el nombre del **Proyecto de destino** donde desea copiar la tarea en la **Seleccionar proyecto de destino** campo . 

   >[!TIP]
   >
   >* El nombre del proyecto distingue entre mayúsculas y minúsculas.
   >* También puede empezar a escribir el número de referencia o introducir el ID del proyecto. Esto puede ayudarle a distinguir entre proyectos con nombres idénticos.
   >* En la lista solo se muestran 100 proyectos.


   El nombre del proyecto actual se muestra de forma predeterminada. Si desea copiar la tarea dentro del mismo proyecto, deje este campo sin cambios.

1. (Condicional) Haga clic en **acceso de solicitud** para solicitar acceso al proyecto, si no tiene acceso al proyecto seleccionado.
1. (Condicional) Continúe copiando la tarea en el proyecto de destino seleccionado sin solicitar acceso si tiene acceso para agregar tareas a una de las tareas del proyecto de destino.

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Se muestran mensajes similares si el proyecto seleccionado está pendiente de aprobación, completado o muerto, cuando el administrador de Workfront evita agregar tareas a estos proyectos. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Haga clic en **Opciones** en el panel izquierdo, anule la selección de los atributos de tarea que no desea copiar con la tarea. Todas las opciones están seleccionadas de forma predeterminada.

   >[!TIP]
   Seleccionar y anular la selección **Seleccionar todo** anula la selección de todas las opciones.

   Anule la selección de las siguientes opciones para no transferirlas a la tarea copiada. La tabla siguiente describe lo que sucede cuando se anula la selección de las opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Restricción</td> 
      <td> <p>La restricción de tareas se establece en Lo antes posible o lo más tarde posible, según la configuración del modo de programación del proyecto.</p> <p> Cuando se selecciona, la restricción actual de la tarea se transfiere a la tarea copiada. </p> <p>Nota: Cuando se mueve o copia una tarea con restricciones de fecha específica a otro proyecto y las fechas de restricción de la tarea están fuera de las fechas del nuevo proyecto, se ajusta la restricción de tareas a Tan pronto como sea posible o tan tarde como sea posible o a las fechas de inicio o finalización planificadas de los proyectos. Algunos ejemplos de restricciones de fechas específicas son Debe comenzar el, Debe finalizar el, Iniciar antes del, Iniciar antes del, Iniciar antes del, etc. Para obtener información sobre las restricciones de tareas y cómo pueden verse afectadas las restricciones de tareas o las fechas del proyecto, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre la restricción de tareas</a> y busque una restricción específica.</p> </td> 
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
      <td>El estado de la tarea es New. De lo contrario, la tarea copiada mantiene el estado de la tarea existente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Información financiera</td> 
      <td>Se elimina la información financiera de la tarea.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todos los predecesores</td> 
      <td> <p>Esto significa que las dependencias no se transfieren a las tareas copiadas. </p> <p>Cuando se selecciona, se conservan los predecesores dentro del grupo de tareas copiadas, mientras que otros se eliminan.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Los documentos adjuntos a la tarea no se transfieren a la tarea copiada. Esto incluye versiones, pruebas y documentos vinculados.</p> <p>Esto no incluye aprobaciones de documentos. Las aprobaciones de documento nunca se pueden copiar cuando se copia una tarea.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Los recordatorios de tareas no se transfieren a la tarea copiada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Los gastos registrados en la tarea no se transfieren a la tarea copiada. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permisos</td> 
      <td>Workfront elimina los nombres de todas las entidades que aparecen en la lista Compartir de la tarea. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td> <p>Los valores de los campos personalizados se borran y los formularios personalizados se transfieren a la tarea copiada. </p> <p>Cuando se selecciona, tanto los formularios como los valores de los campos personalizados se transfieren a la tarea copiada. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1.  (Opcional) Haga clic en **Seleccionar principal** en el panel izquierdo, seleccione la tarea en el proyecto de destino que desea que sea la principal de la tarea copiada.

   >[!TIP]
   Al seleccionar para copiar varias tareas de una lista, todas las tareas seleccionadas se convierten en las secundarias del elemento principal seleccionado.

   Seleccione un elemento principal realizando una de las siguientes acciones:

   * En la lista de tareas, seleccione uno de los elementos principales del plan de proyecto.
   * Haga clic en el icono de búsqueda ![Icono de búsqueda](assets/search-icon.png) y busque una tarea principal por su nombre.
   La tarea debe aparecer en la lista.

   ![Seleccionar tarea principal al mover una tarea con funcionalidad de búsqueda ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Seleccione el botón de opción para el elemento principal, una vez lo haya encontrado. 

   Si no selecciona una tarea principal, las tareas se copian como tareas principales en lugar de como subtareas y se colocan al final de la lista de tareas en el proyecto de destino. 

1. Haga clic en **Copiar tarea**

   O

   Haga clic en **Copiar tareas** cuando seleccione varias tareas en una lista.
Las tareas copiadas están ahora en el proyecto especificado y son subtareas de la tarea principal seleccionada o las últimas tareas del proyecto.

## Duplicar tareas

Puede duplicar rápidamente una tarea en una lista de tareas si necesita una tarea idéntica en el mismo proyecto.

* [Consideraciones sobre la duplicación de tareas](#considerations-for-duplicating-tasks)
* [Duplicar tareas](#duplicate-tasks)

### Consideraciones sobre la duplicación de tareas {#considerations-for-duplicating-tasks}

* Puede duplicar una tarea en una lista de tareas solo cuando la lista se ordena por número de tarea.

* La nueva tarea tendrá el mismo nombre que la tarea original.
* No se puede seleccionar qué información está duplicada en la nueva tarea. De forma predeterminada, casi toda la información de la tarea original se transfiere a la tarea duplicada, incluida la relación principal.
* Los siguientes elementos no se transfieren a la nueva tarea:

   * Horas registradas
   * Notas
   * Problemas
   * Solo los predecesores que están en el mismo grupo de tareas copiadas se copian también con las tareas sucesoras.

      **Ejemplo:** Por ejemplo, si copia la Tarea 2 y su predecesor, Tarea 1, al mismo tiempo, tendrá una copia de la Tarea 2 y una copia de la Tarea 1. La copia de la tarea 1 será la predecesora de la copia de la tarea 2. Pero si copia solo la Tarea 2 sin copiar su predecesor, entonces su copia no tendrá predecesor.

* Cuando se duplica una tarea principal, todas las tareas secundarias también se duplican, incluso cuando las tareas secundarias no están seleccionadas.
* Puede duplicar varias tareas al mismo tiempo.

   Sin embargo, no puede duplicar varias tareas que no sean secuenciales al mismo tiempo.

* Los hitos se mueven a la nueva tarea y se eliminan de la tarea original.

### Duplicar tareas

1. Vaya al proyecto que contiene la tarea o tareas que desea duplicar.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Realice una de las siguientes acciones:

   * (Condicional) Haga clic en el **Menú del modo Plan** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Autoguardar**, seleccione las tareas que desee duplicar y, a continuación, haga clic en el botón **Más menú** ![](assets/qs-more-menu-29x11.png) > **Duplicar**.

      ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * (Condicional) Haga clic en el **Menú del modo Plan** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Guardar manualmente** > **Estándar** o **Planificación de la cronología** y, a continuación, haga lo siguiente:

      1. Seleccione la tarea o tareas que desee duplicar y haga clic en **Duplicar**.
      1. (Opcional) Haga clic en **Deshacer** para invertir los cambios y no duplicar las tareas.
      1. (Opcional y condicional) Haga clic en **Rehacer** si ha hecho clic anteriormente **Deshacer**, para conservar los cambios y duplicar las tareas.

      1. Haga clic en **Guardar** para guardar los cambios.
   1. Editar tareas en una lista
