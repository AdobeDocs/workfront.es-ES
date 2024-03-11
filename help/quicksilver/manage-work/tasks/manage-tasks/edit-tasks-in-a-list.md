---
product-area: projects
navigation-topic: manage-tasks
title: Edición de tareas en una lista
description: Puede editar la información de las tareas en una lista de tareas editando los campos mostrados en la lista. Para obtener información sobre otras formas de editar tareas, consulte Editar tareas.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '2848'
ht-degree: 2%

---

# Edición de tareas en una lista {#edit-tasks-in-a-list}

Puede editar la información de las tareas en una lista de tareas editando los campos mostrados en la lista. Para obtener información sobre otras formas de editar tareas, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Editar acceso a Tareas y Proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Aportar o permisos superiores a la tarea y al proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Consideraciones sobre la edición de tareas en una lista {#considerations-about-editing-tasks-in-a-list}

Editar tareas en una lista es una forma rápida de realizar cambios en varias tareas simultáneamente, con una visión clara de cómo los cambios podrían afectar a la cronología del proyecto.

Tenga en cuenta lo siguiente al editar tareas en una lista:

* A diferencia de la necesidad de permisos de administración para la tarea al editarla en el cuadro de edición, puede editar una tarea en una lista sólo con permisos de contribución para la tarea. Esto le permite editar la siguiente información limitada para la tarea:

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
   * Agregar gastos, tareas o problemas

* Puede editar una tarea en las siguientes listas:

   * La sección Tareas del proyecto
   * La sección Subtareas del proyecto
   * Un informe de tareas

     >[!NOTE]
     >
     >De forma predeterminada, Workfront guarda automáticamente los cambios realizados en las tareas en la sección Subtareas o en un informe de tareas.

* Puede controlar cuándo Workfront guarda los cambios realizados en las tareas de una lista. Los cambios se pueden guardar automáticamente o puede guardarlos manualmente.

  Para obtener información sobre cómo configurar cuándo Workfront guarda los cambios realizados en las tareas de una lista, consulte la [Seleccione una opción de guardado al editar tareas en una lista](#select-a-save-option-when-editing-tasks-in-a-list) de este artículo.

* Otros usuarios deben actualizar sus páginas para poder ver las actualizaciones que realice en una tarea.

## Seleccione una opción de guardado al editar tareas en una lista {#select-a-save-option-when-editing-tasks-in-a-list}

Puede decidir dónde se guardan automáticamente los cambios realizados en las tareas de una lista, a medida que se producen o si desea guardar manualmente cada cambio.

>[!IMPORTANT]
>
>Dependiendo de si guarda las tareas automática o manualmente, puede sobrescribir la información de otra persona mientras está editando tareas en una lista. Para obtener información sobre cómo Workfront guarda los cambios en las tareas que realiza simultáneamente con otros usuarios, consulte [Información general sobre cómo guardar cambios simultáneos en una lista de tareas](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Al guardar los cambios en una lista para un proyecto que tiene seleccionada la opción Automático o Automático y Al cambiar como Tipo de actualización, Workfront actualiza la cronología del proyecto, junto con todas las dependencias dentro del proyecto y entre proyectos. Los cálculos de escala de tiempo pueden llevar mucho tiempo si el proyecto es grande o si hay muchas dependencias. Algunos métodos de edición de una lista de tareas pueden ser más rápidos que otros, según el método que seleccione para guardar los cambios.

Puede controlar cuándo Workfront guarda los cambios realizados en las tareas de una lista. Existen los siguientes escenarios: 

* Puede hacer que Workfront guarde automáticamente los cambios después de cada actualización.

  Para obtener más información, consulte la sección [Editar tareas en una lista y guardar automáticamente los cambios](#edit-tasks-in-a-list-and-automatically-save-changes) en este artículo.

* Puede controlar cuándo se aplican varios cambios a la vez manualmente con un botón Guardar.

  Para obtener más información, consulte la sección [Editar tareas en una lista y guardar cambios manualmente](#edit-tasks-in-a-list-and-manually-save-changes) en este artículo.

### Editar tareas en una lista y guardar automáticamente los cambios {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>Guardar los cambios y todas las dependencias del proyecto puede ser más lento si el proyecto tiene más de 2000 tareas o si tiene muchas dependencias.

Tenga en cuenta lo siguiente al guardar los cambios de la lista de tareas automáticamente:

* Puede aplicar una vista personalizada a la lista de tareas y editar cualquier campo relacionado con la tarea al que tenga acceso para actualizar.
* No puede revertir los cambios guardados automáticamente. Esta es la configuración predeterminada.
* Workfront vuelve a calcular la escala de tiempo del proyecto y todas las dependencias entre proyectos y en proyectos automáticamente después de cada cambio, cuando el tipo de actualización del proyecto es Automatic o Automatic and On Change. Para obtener información sobre el tipo de actualización del proyecto, consulte [Seleccione el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tareas en una lista y guardar cambios automáticamente:

1. Vaya al proyecto y haga clic en **Tareas** sección.
1. Haga clic en **Menú del modo de planificación** ![](assets/qs-list-mode-or-save-mode-icon-small.png) en la parte superior de la lista y asegúrese de que la variable **Autoguardar** La opción está seleccionada.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Edite cualquier campo para el que tenga permisos para actualizar manualmente.

   ![](assets/inline-editing-a-task-350x26.png)

1. (Opcional) Pulse **Escape** para cancelar los cambios.
1. Pulse Entrar para guardar los cambios realizados en las tareas y en la cronología del proyecto.
1. (Opcional) Haga clic con el botón derecho en una tarea que desee modificar.

   O

   Haga clic en **Más** menú ![](assets/more-icon-task-list.png) a la derecha del nombre de la tarea.

1. (Opcional) Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Abrir en una pestaña nueva</strong></td> 
      <td>Abre la tarea en una nueva pestaña del explorador. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Editar</strong></td> 
      <td><p>Abre el <strong>Editar tarea</strong> , donde puede editar la tarea.</p><p>Para obtener información sobre cómo editar una tarea, consulte <a href="#edit-tasks-in-a-list" class="MCXref xref">Edición de tareas en una lista</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar</td> 
      <td><p>Elimina la tarea.</p><p>Para obtener información sobre la eliminación de tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Eliminar tareas</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sangría</td> 
      <td><p>Aplica sangría a la tarea en un nivel. </p><p>Esta opción solo se muestra en tareas independientes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anulación de sangría</td> 
      <td><p>Anula la sangría de la tarea en un nivel. </p><p>Esta opción solo se muestra en tareas secundarias. </p></td> 
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
      <td role="rowheader">Duplicar</td> 
      <td><p>Crea una versión duplicada de la tarea dentro del mismo proyecto. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar en</td> 
      <td><p>Copia la tarea en otro proyecto.</p><p>Para obtener información sobre cómo copiar y duplicar tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar y duplicar tareas</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mover a</td> 
      <td><p>Mueve la tarea a otro proyecto.</p><p>Para obtener información sobre cómo mover tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Mover tareas</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   Los cambios se guardan automáticamente y no se pueden invertir.

### Editar tareas en una lista y guardar cambios manualmente {#edit-tasks-in-a-list-and-manually-save-changes}

Puede guardar manualmente los cambios realizados en las tareas de una lista. Al guardar los cambios de esta forma, tiene la flexibilidad de revertirlos antes de guardarlos.

>[!TIP]
>
>* No se pueden invertir los cambios realizados en las tareas de una lista cuando se están editando en la sección Subtareas o en un informe de tareas.
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
* Workfront déclencheur las notificaciones sobre los cambios realizados en las tareas solo después de guardar los cambios.

Existen dos maneras de guardar manualmente los cambios realizados en las tareas de una lista. A continuación se describen estas dos formas.

* [Guardar cambios en una lista de tareas manualmente al seleccionar la opción Guardar estándar de forma manual](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Guardar cambios en una lista de tareas manualmente al seleccionar la opción Guardar planificación de cronología de forma manual](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Guardar cambios en una lista de tareas manualmente al seleccionar la opción Guardar estándar de forma manual {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Si el proyecto tiene más de 2000 tareas, o si tiene muchas dependencias, podría tardar un tiempo en identificar visualmente los cambios realizados en las tareas y cómo estos cambios afectan a todas las dependencias del proyecto. En este caso, guardar los cambios puede llevar más tiempo si el proyecto tiene más de 2000 tareas o si tiene muchas dependencias.

Tenga en cuenta lo siguiente al actualizar tareas en una lista después de seleccionar la opción Guardar estándar de forma manual:

* Puede aplicar una vista personalizada a la lista de tareas y editar cualquier campo relacionado con tareas para el que tenga permisos de Administrar en esa vista.
* Workfront calcula la cronología del proyecto y todas las dependencias entre proyectos y entre proyectos después de hacer clic en Guardar, cuando el tipo de actualización del proyecto es Automática o Automática y Al cambiar. Para obtener información sobre el tipo de actualización del proyecto, consulte [Seleccione el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tareas de una lista al seleccionar la opción Guardar de forma manual como estándar:

1. Vaya a un proyecto y haga clic en **Tareas** sección .
1. Haga clic en **Modo de planificación** menú ![](assets/qs-list-mode-or-save-mode-icon-small.png) en la parte superior de la lista y seleccione **Guardado manual**, luego haga clic en **Standard** > **Aplicar**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   Se muestra una configuración de la barra de herramientas con opciones para deshacer, rehacer y guardar los cambios.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Haga clic dentro de cualquier campo para el que tenga permisos para actualizar manualmente. El campo se vuelve editable y puede realizar los cambios.

   ![](assets/inline-editing-a-task-350x26.png)

1. Pulse Intro para guardar temporalmente los cambios realizados.
1. (Opcional) Haga clic en **Icono Deshacer** ![](assets/undo-icon-on-task-list.png) para revertir un cambio y devolver un campo a su estado original.
1. (Opcional y condicional) Haga clic en **Icono Rehacer** ![](assets/redo-icon-on-task-list.png) para restaurar el cambio revertido.

1. (Opcional) Haga clic con el botón derecho en una tarea que desee modificar.

   O

   Haga clic en **Más** menú ![](assets/more-icon-task-list.png).

1. (Opcional) Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Abrir en una pestaña nueva</strong> </td> 
      <td>Abre la tarea en una nueva pestaña del explorador. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar</td> 
      <td>Para obtener información sobre la eliminación de tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Eliminar tareas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sangría</td> 
      <td> <p>Aplica sangría a la tarea en un nivel. </p> <p>Esta opción solo se muestra en tareas independientes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anulación de sangría</td> 
      <td> <p>Anula la sangría de la tarea en un nivel. </p> <p>Esta opción solo se muestra en tareas secundarias. </p> </td> 
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
      <td role="rowheader">Duplicar</td> 
      <td> <p>Crea una versión duplicada de la tarea dentro del mismo proyecto. </p> <p>Para obtener información sobre cómo copiar y duplicar tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar y duplicar tareas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront actualiza todas las dependencias dentro del proyecto y entre proyectos cuando realiza cambios en la cronología de las tareas.
1. Clic **Guardar** cuando desee mantener los cambios de la tarea de forma permanente y guardar la cronología del proyecto.

#### Guardar cambios en una lista de tareas manualmente al seleccionar la opción Guardar planificación de cronología de forma manual {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Guardar los cambios y todas las dependencias del proyecto es más rápido. No está disponible para proyectos con más de 2000 tareas.

>[!IMPORTANT]
>
>Se recomienda utilizar esta opción al editar una lista grande de tareas de más de unos cientos que tienen muchas dependencias. El uso de esta opción permite identificar visualmente los cambios mucho más rápido que con la opción de guardado manual.

Tenga en cuenta lo siguiente al utilizar la opción Guardar planificación de la cronología de forma manual en una lista de tareas:

* No se puede aplicar la opción de planificación Guardar escala de tiempo de forma manual a proyectos que tengan más de 2000 tareas.
* No se puede aplicar una vista personalizada, un filtro o una agrupación a la lista de tareas. Los menús desplegables Ver, Filtro y Agrupación, así como el icono de vista Agile, están desactivados. La vista aplicada de forma predeterminada contiene un número limitado de campos.
* La cronología del proyecto y todas las dependencias del proyecto se calculan automáticamente después de cada cambio cuando el tipo de actualización del proyecto es Automática o Automática y Al cambiar.
* Las dependencias entre proyectos se calculan después de hacer clic en Guardar, cuando el tipo de actualización del proyecto es Automática o Automática y Al cambiar. Para obtener información sobre el tipo de actualización del proyecto, consulte [Seleccione el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Para editar tareas en una lista al utilizar la opción Guardar planificación de cronología de forma manual:

1. Vaya a un proyecto y haga clic en **Tareas** sección.
1. Haga clic en **Modo de planificación** menú ![](assets/qs-list-mode-or-save-mode-icon-small.png) en la parte superior de la lista y seleccione **Guardado manual**, luego haga clic en **Planificación de calendario**> **Aplicar**.

   Esta opción aparece atenuada para los proyectos con más de 2000 tareas.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Cuando se aleja de esta página, Workfront vuelve a habilitar la opción de guardado automático.

   Observe los siguientes cambios en la lista:

   * Los menús desplegables Ver, Agrupar y Filtrar se eliminan y la vista se reemplaza por los campos siguientes:

      * Número de tarea
      * Nombre de la tarea
      * Tipo de restricción
      * Duración
      * Fecha planificada de inicio
      * Fecha planificada de finalización
      * Predecesoras
      * Asignaciones
      * Estado
      * Porcentaje completado

   * Se eliminará el icono de vista de Agile.
   * Se muestra una configuración de la barra de herramientas con opciones para deshacer, rehacer y guardar los cambios.

     ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Edite cualquier campo para el que tenga permisos para actualizar manualmente.

   ![](assets/inline-editing-a-task-350x26.png)

1. Pulse Intro para guardar temporalmente los cambios realizados.
1. (Opcional) Haga clic en **Icono Deshacer** ![](assets/undo-icon-on-task-list.png) para revertir un cambio y devolver un campo a su estado original.
1. (Opcional y condicional) Haga clic en **Icono Rehacer** ![](assets/redo-icon-on-task-list.png) para restablecer el cambio revertido.

1. (Opcional) Haga clic con el botón derecho en una tarea que desee modificar

   O

   Haga clic en **Más** menú ![](assets/more-icon-task-list.png).

1. Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Abrir en una pestaña nueva</strong> </td> 
      <td>Abre la tarea en una nueva pestaña del explorador. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminar</td> 
      <td>Para obtener información sobre la eliminación de tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Eliminar tareas</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sangría</td> 
      <td> <p>Aplica sangría a la tarea en un nivel. </p> <p>Esta opción solo se muestra en tareas independientes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anulación de sangría</td> 
      <td> <p>Anula la sangría de la tarea en un nivel. </p> <p>Esta opción solo se muestra en tareas secundarias. </p> </td> 
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
      <td role="rowheader">Duplicar</td> 
      <td> <p>Crea una versión duplicada de la tarea dentro del mismo proyecto. </p> <p>Para obtener información sobre cómo copiar y duplicar tareas, consulte <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiar y duplicar tareas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront actualiza todas las dependencias entre proyectos y proyectos al cambiar la cronología de una tarea.
1. Clic **Guardar** cuando desee mantener los cambios de la tarea de forma permanente y guardar la cronología del proyecto.

## Edición de una tarea en una lista mediante el Resumen

1. Vaya al proyecto que contiene las tareas que desea editar.
1. Clic **Tareas** en el panel izquierdo.

   Se muestra la lista de tareas del proyecto.

1. Haga clic en el menú Más ![](assets/more-icon-task-list.png) después del nombre de la tarea, haga clic en **Abrir resumen**. Seleccione la tarea que desee editar y haga clic en el icono **Icono Abrir resumen** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) en la esquina superior derecha de la lista.

   El **Resumen** abre.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (Opcional) Haga clic en **Icono X** en la parte superior derecha del Resumen para cerrar el panel y editar las tareas en línea.

   Siga los pasos para editar una tarea en una lista y editarla en línea.

   Para obtener información sobre cómo editar la tarea en una lista, consulte [Consideraciones sobre la edición de tareas en una lista](#considerations-about-editing-tasks-in-a-list) en este artículo.

1. (Opcional) Escriba una actualización para la tarea en la **Actualizaciones** área.
1. Haga clic en cualquiera de los siguientes iconos o áreas para ir a la tarea y editar la información en el nivel de tarea:

   | Documentos | Clic **Haga clic aquí para agregar** para agregar documentos a la tarea. |
   |---|---|
   | Detalles | Haga clic en para actualizar la información sobre la tarea. |
   | Formularios personalizados | Haga clic en para añadir o quitar Forms personalizado o actualizar la información de los formularios. |
   | Horas | Haga clic en para registrar horas. |
   | Rutas de aprobación | Haga clic en para añadir aprobaciones de tarea. |

   {style="table-layout:auto"}

1. Haga clic en el botón Atrás del explorador para volver a la lista de tareas cuando termine de actualizar la tarea.

## Editar tareas de forma masiva

Puede editar varias tareas a la vez. Asegúrese de tener permisos de administración en las tareas para poder editarlas.

1. Vaya a un proyecto que contenga las tareas que desee editar por lotes.
1. Clic **Tareas** en el panel izquierdo.
1. Asegúrese de que la variable **Autoguardar** La opción está seleccionada.

   >[!IMPORTANT]
   >
   >No puede editar tareas de forma masiva al guardar tareas manualmente.

   Para obtener más información sobre cómo guardar los cambios realizados en las tareas de una lista, consulte la sección [Consideraciones sobre la edición de tareas en una lista](#considerations-about-editing-tasks-in-a-list) en este artículo.

1. Seleccione varias tareas en la lista de tareas.
1. Haga clic en **Icono Editar** ![](assets/qs-edit-icon.png).

   El **Editar tareas** se abre el cuadro de diálogo.

1. Especifique la información que desea cambiar para todas las tareas seleccionadas.

   Editar la información de todas las tareas es idéntico a editar la información de una tarea. Si desea editar la duración de la tarea, las tareas seleccionadas deben tener la misma restricción de tarea; de lo contrario, la variable **Duración** el campo no se rellena.

   Para obtener más información sobre cómo editar una tarea, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >La información que está cambiando en todas las tareas seleccionadas anulará la información existente en las tareas individuales, excepto en el caso de **Asignaciones** field. Si se añade un nuevo usuario asignado en una edición masiva, se añadirá ese usuario asignado a todas las tareas seleccionadas. Si otras personas asignadas están asignadas a las tareas seleccionadas, permanecerán asignadas además de la añadida mediante la edición masiva.

1. Clic **Forms personalizado** para editar los formularios personalizados adjuntos a todas las tareas seleccionadas. En la lista solo se muestran los formularios personalizados activos.

   Si las tareas seleccionadas no tienen ningún formulario personalizado en común, no se mostrará ningún formulario en esta sección.

   Solo puede editar los campos de los formularios que están adjuntos a todas las tareas seleccionadas y para los que tiene permisos de edición.

1. (Opcional) En la sección Forms personalizado, seleccione **Volver a calcular expresiones personalizadas** para garantizar que todos los campos personalizados calculados que se encuentran en los formularios personalizados adjuntos a las tareas seleccionadas estén actualizados.
1. Haga clic en **Guardar cambios**.

   Todos los cambios realizados ahora están visibles en todas las tareas seleccionadas.

Para obtener información sobre la edición masiva de formularios personalizados, consulte la sección &quot;Editar varios Forms personalizados al editar objetos por lotes&quot; en [Administrar formularios personalizados adjuntos a objetos](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
