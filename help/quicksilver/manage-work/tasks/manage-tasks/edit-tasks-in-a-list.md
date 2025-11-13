---
product-area: projects
navigation-topic: manage-tasks
title: Edición de tareas en una lista
description: Puede editar la información de las tareas en una lista de tareas editando los campos mostrados en la lista. Debe definir el modo de planificación en una lista de tareas para indicar cómo desea que se guarden los cambios en Workfront. Puede guardar los cambios de forma manual o automática.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '2851'
ht-degree: 63%

---

# Edición de tareas en una lista {#edit-tasks-in-a-list}

<!-- Audited: 10/2025 -->

<!--

<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Puede editar la información de las tareas en una lista de tareas editando los campos mostrados en la lista. Para obtener información acerca de otras formas de editar tareas, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Estándar<p>
   <p>Trabajo o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribuir o permisos superiores para la tarea y el proyecto</p></td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard<p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Consideraciones sobre la edición de tareas en una lista {#considerations-about-editing-tasks-in-a-list}

Editar tareas en una lista es una forma rápida de realizar cambios en varias tareas simultáneamente con una visión clara de cómo los cambios podrían afectar a la cronología del proyecto.

Tenga en cuenta lo siguiente al editar tareas en una lista:

* A diferencia de la necesidad de Administrar permisos para la tarea al editarla en el Cuadro de edición, puede editar una tarea en una lista solo con permisos de Contribuir para la tarea. Esto le permite editar la siguiente información limitada para la tarea:

   * Descripción
   * Estado
   * Porcentaje completado
   * Información de formulario personalizado

     >[!NOTE]
     >
     >Solo puede editar un campo personalizado de tarea en una lista si tiene permisos para actualizar el campo.

   * Registrar horas
   * Modificar asignaciones
   * Ver información financiera
   * Añadir gastos, tareas o problemas

* Puede editar una tarea en las siguientes listas:

   * La sección de tareas del proyecto
   * La sección de subtareas del proyecto
   * Un informe de tareas

     >[!NOTE]
     >
     >De forma predeterminada, Workfront guarda automáticamente los cambios realizados en las tareas en la sección Subtareas o en un informe de tareas.

* Puede controlar cuándo Workfront guarda los cambios realizados en las tareas de una lista definiendo el modo de planificación antes de empezar a editar las tareas.

  Puede decidir si Workfront guarda los cambios que realiza de la siguiente manera:

      * Automáticamente, después de cada cambio
     * Manualmente, solo después de hacer clic en Guardar.
  
  Para obtener información acerca de cómo configurar cuándo Workfront guarda los cambios realizados en las tareas de una lista, consulte la sección [Modificar modo de plan antes de editar las tareas de una lista](#modify-plan-mode-before-editing-tasks-in-a-list) en este artículo.

* Otros usuarios deben actualizar sus páginas para poder ver las actualizaciones que realice en una tarea.

## Modificar el modo de planificación antes de editar tareas en una lista

Puede decidir si los cambios realizados en las tareas de una lista se guardan automáticamente a medida que se producen o si desea guardar manualmente cada cambio. Para ello, debe modificar el modo de planificación en una lista de tareas antes de editar las tareas.

>[!IMPORTANT]
>
>Dependiendo de si guarda las tareas automática o manualmente, puede sobrescribir la información de otra persona mientras está editando tareas en una lista. Para obtener más información, vea [Información general sobre cómo guardar cambios simultáneos en una lista de tareas](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Al guardar los cambios en una lista para un proyecto que tiene seleccionada la opción Automático o Automático y al cambiar como Tipo de actualización, Workfront actualiza la cronología del proyecto, junto con todas las dependencias dentro del proyecto y entre proyectos. Los cálculos de cronología pueden llevar mucho tiempo si el proyecto es grande o si hay muchas dependencias. Algunos métodos de edición de una lista de tareas pueden ser más rápidos que otros, según el método que seleccione para guardar los cambios.

Puede controlar cuándo Workfront guarda los cambios realizados en las tareas de una lista. Se dan los siguientes escenarios:

* Puede hacer que Workfront guarde automáticamente los cambios después de cada actualización.

  Para obtener más información, consulte la sección [Definir el modo de planificación para guardar automáticamente los cambios](#set-the-plan-mode-to-automatically-save-changes) en este artículo.

* Puede controlar cuándo se aplican varios cambios a la vez manualmente con un botón Guardar.

  Para obtener más información, consulte la sección [Configurar el modo de planificación para guardar manualmente los cambios](#set-the-plan-mode-to-manually-save-changes) en este artículo.

### Configure el modo de planificación para guardar automáticamente los cambios

>[!TIP]
>
>Guardar los cambios y todas las dependencias del proyecto puede ser más lento si el proyecto tiene más de 2000 tareas o si tiene muchas dependencias.

Tenga en cuenta lo siguiente al guardar los cambios de la lista de tareas automáticamente:

* Puede aplicar una vista personalizada a la lista de tareas y editar cualquier campo relacionado con la tarea al que tenga acceso para actualizar.
* No puede revertir los cambios guardados automáticamente. Esta es la configuración predeterminada.
* Cuando el tipo de actualización del proyecto es Automática o Automática y Al cambiar, Workfront vuelve a calcular la cronología del proyecto y todas las dependencias entre proyectos automáticamente después de cada cambio. Para obtener información sobre el tipo de actualización del proyecto, consulte [Seleccionar el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tareas en una lista y guardar cambios automáticamente:

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.
1. En el panel izquierdo, haga clic en la sección **Tareas**.

1. Haga clic en el icono **Modo de plan** ![Icono de modo de plan](assets/plan-mode-icon.png) en la parte superior de la lista y asegúrese de que la opción **Guardar automáticamente** esté seleccionada.

   ![Habilitar la configuración de guardado automático](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Edite cualquier campo para el que tenga permisos para actualizar manualmente.

1. (Opcional) Pulse **Escape** para cancelar los cambios.
1. Presione **Enter** (Windows) o **Return** (Mac) en el teclado para guardar los cambios en las tareas y en la cronología del proyecto.
1. (Opcional) Haga clic con el botón derecho en una tarea que desee modificar.

   O

   Haga clic en el menú **Más** ![](assets/more-icon-task-list.png) a la derecha del nombre de la tarea.

1. (Opcional) Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Abrir en nueva ficha</td> 
      <td>Abre la tarea en una nueva pestaña del explorador. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Insertar la tarea arriba</td> 
      <td>Inserta una tarea encima de la tarea seleccionada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insertar tarea debajo</td> 
      <td>Inserta una tarea debajo de la tarea seleccionada</td> 
     </tr>
     <tr> 
      <td role="rowheader">Editar</td> 
      <td><p>Abre el cuadro Editar tarea, donde puede editar la tarea.</p><p>Para obtener información sobre cómo editar una tarea, consulte <a href="#edit-tasks-in-a-list" class="MCXref xref">Editar tareas en una lista</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar</td> 
      <td><p>Elimina la tarea.</p><p>Para obtener información sobre cómo eliminar tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Eliminar tareas</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sangría</td> 
      <td><p>Aplica un nivel de sangría a la tarea. </p><p>Esta opción solo se muestra en tareas independientes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anulación de sangría</td> 
      <td><p>Anula un nivel de sangría en la tarea. </p><p>Esta opción solo se muestra en tareas secundarias. </p></td> 
     </tr>  
     <tr> 
      <td role="rowheader">Duplicar</td> 
      <td><p>Crea una versión duplicada de la tarea dentro del mismo proyecto. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar en...</td> 
      <td><p>Copia la tarea en otro proyecto.</p><p>Para obtener información sobre cómo copiar y duplicar tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar y duplicar tareas</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mover a...</td> 
      <td><p>Mueve la tarea a otro proyecto.</p><p>Para obtener información sobre cómo mover tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Mover tareas</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

### Configure el modo de planificación para guardar los cambios manualmente {#edit-tasks-in-a-list-and-manually-save-changes}

Puede guardar manualmente los cambios realizados en las tareas de una lista. Al guardar los cambios de esta forma, tiene la flexibilidad de revertirlos antes de guardarlos.

>[!TIP]
>
>* No se pueden revertir los cambios realizados en las tareas de una lista cuando se están editando en la sección Subtareas o en un informe de tareas.
>* No existen limitaciones en cuanto a la cantidad de cambios que se pueden revertir. Puede invertir todas ellas una por una hasta que alcance el estado original de las tareas.
>

Tenga en cuenta lo siguiente al guardar los cambios en una lista de tareas manualmente:

* Para guardar los cambios de la lista de tareas manualmente, necesita permisos para administrar las tareas y el proyecto.
* No puede editar el proyecto. La opción para editar el proyecto está desactivada.
* No se puede actualizar la información en el encabezado del proyecto. Solo puede hacer lo siguiente al guardar manualmente los cambios en la lista de tareas:

   * Suscríbase al proyecto.
   * Añada el proyecto a su lista de favoritos.
   * Abra una tarea haciendo clic en su nombre en la lista.

* Edite las tareas de forma masiva. El icono Editar se desactiva al seleccionar varias tareas.
* Workfront activa las notificaciones sobre los cambios realizados en las tareas solo después de guardar los cambios.

Existen dos formas de guardar manualmente los cambios en las tareas de una lista:

* [Guardar cambios en una lista de tareas manualmente al seleccionar la opción estándar Guardar de forma manual](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Guardar cambios en una lista de tareas manualmente al seleccionar la opción Guardar planificación de cronología de forma manual](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Guardar cambios en una lista de tareas manualmente al seleccionar la opción estándar Guardar de forma manual {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Si el proyecto tiene más de 2000 tareas, o si tiene muchas dependencias, podría tardar un tiempo en identificar visualmente los cambios realizados en las tareas y cómo estos cambios afectan a todas las dependencias del proyecto. En este caso, guardar los cambios puede tardar más de lo previsto.

Tenga en cuenta lo siguiente al actualizar tareas en una lista después de seleccionar la opción estándar Guardar de forma manual:

* Puede aplicar una vista personalizada a la lista de tareas y editar cualquier campo relacionado con tareas para el que tenga permisos de Administrar en esa vista.
* Cuando el tipo de actualización del proyecto es Automática o Automática y Al cambiar, Workfront calcula la cronología del proyecto y todas las dependencias entre proyectos y entre proyectos después de hacer clic en Guardar. Para obtener información acerca del tipo de actualización del proyecto, consulte [Seleccionar el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tareas de una lista al seleccionar la opción estándar Guardar de forma manual:

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.

1. En el panel izquierdo, haga clic en la sección **Tareas**.

1. Haga clic en el icono **Modo de plan** ![Modo de plan](assets/plan-mode-icon.png) en la parte superior de la lista.

1. En el cuadro de diálogo **Modo de plan**, seleccione **Guardar de forma manual** y, a continuación, haga clic en **Estándar**.

   ![Habilitar la configuración de guardado manual](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Haga clic en **Aplicar**. Se muestra una configuración de la barra de herramientas con opciones para deshacer, rehacer y guardar los cambios.

   ![Barra de herramientas para guardar manualmente](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Haga clic dentro de cualquier campo para el que tenga permisos para actualizar manualmente. El campo se vuelve editable y puede realizar los cambios.

1. Presione **Enter** (Windows) o **Return** (Mac) en el teclado para guardar temporalmente los cambios que realizó.

1. (Opcional) Haga clic en el icono **Deshacer** ![Deshacer icono](assets/undo-icon-on-task-list.png) para revertir un cambio y devolver un campo a su estado original.

1. (Opcional y condicional) Haga clic en el icono **Rehacer** ![Rehacer](assets/redo-icon-on-task-list.png) para restaurar el cambio que ha revertido.

1. (Opcional) Haga clic con el botón derecho en una tarea que desee modificar.

   O

   Haga clic en el menú **Más**![](assets/more-icon-task-list.png).

1. (Opcional) Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Abrir en nueva ficha</td> 
      <td>Abre la tarea en una nueva pestaña del explorador. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Insertar la tarea arriba</td> 
      <td>Inserta una tarea encima de la tarea seleccionada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insertar tarea debajo</td> 
      <td>Inserta una tarea debajo de la tarea seleccionada</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar</td> 
      <td>Para obtener información acerca de cómo eliminar tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Eliminar tareas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sangría</td> 
      <td> <p>Aplica un nivel de sangría a la tarea. </p> <p>Esta opción solo se muestra en tareas independientes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anulación de sangría</td> 
      <td> <p>Anula un nivel de sangría en la tarea. </p> <p>Esta opción solo se muestra en tareas secundarias. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplicar</td> 
      <td> <p>Crea una versión duplicada de la tarea dentro del mismo proyecto. </p> <p>Para obtener información sobre cómo copiar y duplicar tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar y duplicar tareas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront actualiza todas las dependencias dentro del proyecto y entre proyectos cuando realiza cambios en la cronología de las tareas.
1. Haga clic en **Guardar** cuando quiera mantener los cambios de la tarea de forma permanente y guardar la cronología del proyecto.

#### Guardar cambios en una lista de tareas manualmente al seleccionar la opción Guardar planificación de cronología de forma manual {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Guardar los cambios y todas las dependencias del proyecto es más rápido. Esto no está disponible para proyectos con más de 2000 tareas.

>[!IMPORTANT]
>
>Se recomienda utilizar esta opción al editar una lista grande de tareas de más de unos cientos que tienen muchas dependencias. El uso de esta opción permite identificar visualmente los cambios mucho más rápido que con la opción de guardado manual.

Tenga en cuenta lo siguiente al utilizar la opción Guardar planificación de la cronología de forma manual en una lista de tareas:

* No se puede aplicar la opción Guardar planificación de la cronología de forma manual a proyectos que tengan más de 2000 tareas.
* No se puede aplicar una vista personalizada, un filtro o una agrupación a la lista de tareas. Los menús desplegables Ver, Filtro y Agrupación, así como el icono de vista Agile, están desactivados. La vista aplicada de forma predeterminada contiene un número limitado de campos.
* La cronología del proyecto y todas las dependencias del proyecto se calculan automáticamente después de cada cambio, cuando el Tipo de actualización del proyecto es Automática o Automática y al cambiar.
* Cuando el tipo de actualización del proyecto es Automática o Automática y Al cambiar, las dependencias entre proyectos se calculan después de hacer clic en Guardar. Para obtener información acerca del tipo de actualización del proyecto, consulte [Seleccionar el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tareas en una lista al utilizar la opción Guardar planificación de cronología de forma manual:


{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.

1. En el panel izquierdo, haga clic en la sección **Tareas**.

1. Haga clic en el icono **Modo de plan** ![Modo de plan](assets/plan-mode-icon.png) en la parte superior de la lista.

1. En el cuadro de diálogo **Modo de planificación**, seleccione **Guardar de forma manual** y, a continuación, haga clic en **Planificación de la cronología**.

   ![Aplicar configuración de planificación de la cronología](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >La opción **Planificación de tiempo** está atenuada para los proyectos con más de 2000 tareas.

1. Haga clic en **Aplicar**.

   Los siguientes cambios se producen en la lista:

   * Los menús desplegables Ver, Agrupar y Filtrar se eliminan y la vista se reemplaza por los campos siguientes:

      * Número de tarea
      * Nombre de la tarea
      * Tipo de restricción
      * Duración
      * Fecha de inicio planificada
      * Fecha planificada de finalización
      * Predecesoras
      * Asignaciones
      * Estado
      * Porcentaje completado

   * Se eliminará el icono de vista de Agile.
   * Se muestra una configuración de la barra de herramientas con opciones para deshacer, rehacer y guardar los cambios.

     ![Barra de herramientas para guardar manualmente](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Edite cualquier campo para el que tenga permisos para actualizar manualmente.

1. Presione **Enter** (Windows) o **Return** (Mac) en el teclado para guardar temporalmente los cambios que realizó.
1. (Opcional) Haga clic en el icono **Deshacer** ![Deshacer icono](assets/undo-icon-on-task-list.png) para revertir un cambio y devolver un campo a su estado original.
1. (Opcional y condicional) Haga clic en el icono **Rehacer** ![Rehacer](assets/redo-icon-on-task-list.png) para restablecer el cambio que ha revertido.

1. (Opcional) Haga clic con el botón derecho en una tarea que desee modificar.

   O

   Haga clic en el menú **Más** ![](assets/more-icon-task-list.png).

1. Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Abrir en nueva ficha</td> 
      <td>Abre la tarea en una nueva pestaña del explorador. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Insertar la tarea arriba</td> 
      <td>Inserta una tarea encima de la tarea seleccionada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insertar tarea debajo</td> 
      <td>Inserta una tarea debajo de la tarea seleccionada</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar</td> 
      <td>Para obtener información acerca de cómo eliminar tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Eliminar tareas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sangría</td> 
      <td> <p>Aplica un nivel de sangría a la tarea. </p> <p>Esta opción solo se muestra en tareas independientes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anulación de sangría</td> 
      <td> <p>Anula un nivel de sangría en la tarea. </p> <p>Esta opción solo se muestra en tareas secundarias. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplicar</td> 
      <td> <p>Crea una versión duplicada de la tarea dentro del mismo proyecto. </p> <p>Para obtener información sobre cómo copiar y duplicar tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar y duplicar tareas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront actualiza todas las dependencias dentro del proyecto y entre proyectos cuando realiza cambios en la cronología de una tarea.
1. Haga clic en **Guardar** cuando quiera mantener los cambios de la tarea de forma permanente y guardar la cronología del proyecto.

## Edición de una tarea en una lista mediante el Resumen

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.

1. En el panel izquierdo, haga clic en la sección **Tareas**. Se muestra la lista de tareas del proyecto.

1. Seleccione la tarea que desee editar y, a continuación, haga clic en el icono **Abrir resumen** ![Abrir icono de resumen](assets/task-summary-icon.png) en la esquina superior derecha de la lista. Se abre el panel **Resumen de tareas**.

1. (Opcional) Escriba una actualización para la tarea en el área **Actualizaciones**.
1. Haga clic en cualquiera de los siguientes iconos o áreas para ir a la tarea y editar la información en el nivel de tarea:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td>Agregar documentos a la tarea. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td>Agregue o quite formularios personalizados o actualice la información de los formularios.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Horas</td> 
      <td>Registrar horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rutas de aprobación</td> 
      <td>Agregar aprobaciones de tarea.</td> 
     </tr> 
     <tr> 
    </tbody> 
   </table>

1. Haga clic en **X** en la esquina superior derecha del panel para cerrarlo.

## Editar tareas de forma masiva

Puede editar varias tareas a la vez. Asegúrese de tener permisos de administración en las tareas para poder editarlas.

{{step1-to-projects}}

1. En la página **Proyectos**, seleccione un proyecto.
1. En el panel izquierdo, haga clic en la sección **Tareas**.

1. Haga clic en el icono **Modo de plan** ![Icono de modo de plan](assets/plan-mode-icon.png) en la parte superior de la lista y asegúrese de que la opción **Guardar automáticamente** esté seleccionada.

   ![Habilitar la configuración de guardado automático](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

   >[!IMPORTANT]
   >
   >No puede editar tareas de forma masiva al guardar tareas manualmente.

1. Seleccione más de una tarea en la lista de tareas.
1. (Opcional) Haga clic en el menú **Más** ![Menú más](assets/more-icon.png) en la parte superior de la lista de tareas y, a continuación, en **Volver a calcular expresiones** para actualizar toda la información en los campos personalizados calculados.
1. Haga clic en el icono **Editar** ![Editar icono](assets/qs-edit-icon.png). El cuadro de diálogo **Editar tareas** se abre en la nueva experiencia.

   Editar la información de todas las tareas es idéntico a editar la información de una tarea.

   Para obtener más información sobre cómo editar una tarea, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Condicional) En la nueva experiencia, haga lo siguiente:

   1. Especifique la información que desea cambiar para todas las tareas seleccionadas en cualquiera de las siguientes áreas:

      * Información general
      * Asignaciones
      * Formularios personalizados
      * Finanzas
      * Configuración
      * Configuración
      * Comentario

      >[!NOTE]
      >
      >* La información que está cambiando en todas las tareas seleccionadas anulará la información existente en las tareas individuales, excepto la del campo **Asignaciones**. Si se añade un nuevo usuario asignado en una edición masiva, se añadirá ese usuario asignado a todas las tareas seleccionadas. Si hay otras personas asignadas a las tareas seleccionadas, permanecerán asignadas además de las que se añadan mediante la edición masiva.
      >* Si desea editar la duración de la tarea, las tareas seleccionadas deben tener la misma restricción de tarea. De lo contrario, el campo **Duration** no se rellena.
      >
      >* En la lista solo se muestran los formularios personalizados activos. Si las tareas seleccionadas no tienen ningún formulario personalizado en común, no se mostrará ningún formulario en esta sección.
      >* Solo puede editar los campos de los formularios que están adjuntos a todas las tareas seleccionadas y para los que tiene permisos de edición.  Para obtener información sobre la edición en lotes de formularios personalizados, consulte [Administrar formularios personalizados adjuntos a objetos](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).

   1. Haga clic en **Guardar**.
   1. (Opcional) Haga clic en **Volver a la experiencia anterior** en la parte inferior del cuadro **Editar tareas**.

1. (Condicional) En la experiencia anterior, haga lo siguiente:

   1. Especifique la información que desea cambiar para todas las tareas seleccionadas en cualquiera de las siguientes áreas:

      * Información general
      * Configuración
      * Asignaciones
      * Formularios personalizados
      * Comentario

   1. (Opcional) En la sección **Forms personalizado**, seleccione la opción **Volver a calcular expresiones personalizadas** para asegurarse de que todos los campos personalizados calculados que están en los formularios personalizados adjuntos a las tareas seleccionadas estén actualizados.
   1. Haga clic en **Guardar cambios**. Todos los cambios que haya realizado estarán ahora visibles en todas las tareas seleccionadas.

