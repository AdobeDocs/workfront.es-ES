---
product-area: projects
navigation-topic: manage-tasks
title: Mover tareas
description: Puede mover tareas a diferentes proyectos o a diferentes tareas principales en Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1360'
ht-degree: 2%

---

# Mover tareas

Puede mover tareas en Adobe Workfront entre los siguientes objetos:

* Tarea ad hoc de un proyecto.
* Una tarea de un proyecto a otro.
* Una tarea de un proyecto en un proyecto principal diferente de otro proyecto.
* Una tarea dentro del mismo proyecto en un elemento principal diferente.

Puede mover una tarea a nivel de tarea o puede moverla de una lista de tareas.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar las acciones de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas</p> <p>Contribute o permisos superiores para el proyecto con capacidad para agregar tareas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mover una tarea a una lista

Para mover una tarea mostrada en una lista de tareas:

1. Vaya al proyecto que contiene la tarea o tareas que desea mover.
1. Haga clic en **Tareas** en el panel izquierdo para mostrar la lista de tareas.
1. Asegúrese de que la variable **Autoguardar** esté activada y, a continuación, seleccione la tarea o tareas que desee mover.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >No se pueden mover tareas cuando la variable **Autoguardar** está desactivado.

1. (Opcional y condicional) Si desea mover las tareas seleccionadas dentro del mismo proyecto, haga clic en las tareas seleccionadas, arrástrelas y suéltelas donde desee que se muevan en el proyecto.

   Después de colocar las tareas en el lugar correcto del proyecto, los cambios realizados en la jerarquía de tareas se guardan inmediatamente. Toda la información asociada a cada tarea se mueve con las tareas.

1. (Condicional) Seleccione la tarea o tareas que desee mover y realice una de las siguientes acciones:

   * Haga clic en el **Más** menú ![](assets/qs-more-menu.png) en la parte superior de la lista de tareas, haga clic en **Mover a**.
   * Haga clic con el botón derecho en las tareas seleccionadas y, a continuación, haga clic en **Mover a**.
   * Al seleccionar una tarea, haga clic en el botón **Más** menú ![](assets/more-icon-task-list.png) junto al nombre de la tarea en la lista y, a continuación, haga clic en **Mover a**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   Aparece el cuadro Mover tarea

1. Continúe moviendo la tarea, tal como se describe en la sección [Mover una tarea al nivel de tarea](#move-a-task-at-the-task-level) en este artículo, empezando por el paso 4.

   <!--
   is this still accurate?!
   -->

## Mover una tarea al nivel de tarea {#move-a-task-at-the-task-level}

Además de mover tareas de una lista de tareas, también puede mover una tarea al nivel de tarea, después de haberla abierto. 

1. Busque una tarea en el sistema de Workfront.
1. Haga clic en el nombre de la tarea para abrirla.
1. Haga clic en el **Más** menú desplegable ![](assets/qs-more-menu.png) junto al nombre de la tarea y, a continuación, haga clic en **Mover a**. Aparece el cuadro Mover tarea .

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Opcional) Actualice el **Nombre de la tarea**. La tarea se mueve con el nuevo nombre en la nueva ubicación. Workfront no registra el nombre original de la tarea.

   >[!TIP]
   >
   >Este campo está atenuado y no se puede editar al seleccionar mover varias tareas en una lista. Puede situarse sobre el campo Nombre de la tarea y se mostrará una lista de todas las tareas seleccionadas.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Escriba el nombre del **Proyecto de destino** donde desea que la tarea se mueva en la **Seleccionar proyecto de destino** campo .

   Si desea mover la tarea dentro del mismo proyecto, escriba el nombre del proyecto actual.

   >[!TIP]
   >
   >* El nombre del proyecto distingue entre mayúsculas y minúsculas.
   >* También puede empezar a escribir el número de referencia o introducir el ID del proyecto. Esto puede ayudarle a distinguir entre proyectos con nombres idénticos.
   >* En la lista solo se muestran 100 proyectos.


1. (Condicional) Haga clic en **Solicitud de acceso** para solicitar acceso al proyecto, si no tiene acceso al proyecto seleccionado.
1. (Condicional) Continúe moviendo la tarea al proyecto de destino seleccionado sin solicitar acceso si tiene acceso para agregar tareas a una de las tareas del proyecto de destino.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Se muestran mensajes similares si el proyecto seleccionado está pendiente de aprobación, completado o muerto, cuando el administrador de Workfront evita agregar tareas a estos proyectos. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Opcional) Haga clic en **Opciones** en el panel izquierdo

   O

   Desplácese hacia abajo hasta el **Opciones** en el cuadro Mover tarea y, a continuación, anule la selección de cualquiera de los elementos enumerados en la tabla siguiente para eliminarlos de las tareas movidas . Todas las opciones están seleccionadas de forma predeterminada.

   >[!IMPORTANT]
   Al anular la selección de elementos en la lista Opciones, se pierden datos. La información de la tarea existente se eliminará y no se podrá recuperar.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleccionar todo</td> 
      <td>Anule la selección de esta opción para eliminar toda la información de la tarea al moverla a su nueva ubicación. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Restricción</td> 
      <td> <p>La restricción de tareas se establece en Lo antes posible o lo más tarde posible, según la configuración del modo de programación del proyecto.</p> <p> Cuando se selecciona, la restricción actual de la tarea se transfiere con la tarea. </p> 
      <p><b>NOTA</b>

   Cuando se mueve o copia una tarea con restricciones de fecha específica a otro proyecto y las fechas de restricción de la tarea están fuera de las fechas del nuevo proyecto, se ajusta la restricción de tareas a Tan pronto como sea posible o tan tarde como sea posible o a las fechas de inicio o finalización planificadas de los proyectos.

   Los siguientes son ejemplos de restricciones de fechas específicas:
   <ul>
      <li> Comenzar el</li>
      <li> Debe finalizarse el</li>
      <li> No iniciar antes del</li>
      <li> No iniciar después del</li>
      </ul>

   Para obtener información sobre las restricciones de tareas y cómo pueden verse afectadas las restricciones de tareas o las fechas del proyecto, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre la restricción de tareas</a> y busque una restricción específica.</p> </td>
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
      <td>El estado de la tarea es New. De lo contrario, se conserva el estado de la tarea existente. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Información financiera</td> 
      <td>La información financiera de la tarea se elimina y Workfront actualiza el Tipo de Coste de la tarea a Sin Coste y el Tipo de Ingresos de la tarea a No Facturable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Todos los predecesores</td> 
      <td> <p>Cuando se selecciona, la dependencia se convierte en un predecesor entre proyectos cuando se mueve la tarea a otro proyecto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td> <p>Los documentos adjuntos a la tarea no se transfieren a la tarea movida. Esto incluye versiones, pruebas y documentos vinculados.</p> <p>Esto no incluye aprobaciones de documentos. Las aprobaciones de documento nunca se pueden mover cuando se mueve una tarea.</p> 
      <b>NOTA</b>

   Si opta por no mover los documentos con la tarea, los documentos se eliminarán y se colocarán en la Papelera de reciclaje durante 30 días. Un administrador puede restaurarlos y restaurarlos en la tarea movida.

   Si la tarea se elimina una vez que se haya movido, los documentos restaurados se colocarán en el área Documentos de la página de usuario del administrador que los restaura.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td>Los recordatorios de tareas no se transfieren a la tarea movida. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td>Los gastos registrados en la tarea no se transfieren a la tarea movida. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permisos</td> 
      <td> <p>Workfront elimina los nombres de todas las entidades que aparecen en la lista Compartir de la tarea. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Opcional) Haga clic en **Seleccionar principal** en el panel izquierdo

   O

   Desplácese hasta el **Seleccionar principal** y, a continuación, seleccione la tarea en el proyecto de destino que desea que sea la principal de la tarea movida.

   >[!TIP]
   Al seleccionar mover varias tareas de una lista, todas las tareas seleccionadas se convierten en las secundarias del elemento principal seleccionado.

   Seleccione un elemento principal realizando una de las siguientes acciones:

   * En la lista de tareas, seleccione uno de los elementos principales del plan de proyecto.
   * Haga clic en el icono de búsqueda ![Icono de búsqueda](assets/search-icon.png) y busque una tarea principal por su nombre.

   La tarea debe aparecer en la lista.

   ![Seleccionar tarea principal al mover una tarea con funcionalidad de búsqueda ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Seleccione el botón de opción para el elemento principal, una vez lo haya encontrado.

   Si no selecciona una tarea principal, las tareas se mueven como tareas principales en lugar de como subtareas y se colocan al final de la lista de tareas en el proyecto de destino.

1. Haga clic en **Mover tarea**

   O

   Haga clic en **Mover tareas** cuando seleccione varias tareas en una lista.
Las tareas movidas están ahora en el proyecto especificado y son subtareas a una tarea principal o las últimas tareas del proyecto.
