---
product-area: projects
navigation-topic: create-tasks
title: Crear tareas en un proyecto
description: Solo puede crear tareas en un proyecto una vez creado el proyecto.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 59%

---

# Creación de tareas en un proyecto

<!-- Audited: 10/2024 -->

Puede crear tareas en Adobe Workfront de las siguientes maneras:

* Cree una tarea en un proyecto desde cero, una vez creado el proyecto.

  Después de crear un proyecto, puede agregar tareas y modificarlas para organizar el plan del proyecto. Para obtener más información sobre cómo crear un proyecto, vea [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

* Crear tareas agregando una plantilla a un proyecto.

  Para obtener información, consulte [Adjuntar una plantilla a un proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Cree tareas personales y muévalas a un proyecto.

  Puede crear tareas personales realizando una de las siguientes acciones:

   * Crear una solicitud de trabajo ad hoc y enviarla a un usuario
   * Crear un elemento pendiente en el área de Inicio

  Para obtener información acerca de cómo crear tareas personales que no están en un proyecto, vea [Crear tareas personales](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

  Puede mover tareas personales a un proyecto y convertirlas en tareas de trabajo.

Este artículo describe cómo crear tareas desde cero y cómo mover tareas personales a un proyecto.

También puede crear tareas de las siguientes maneras:

* Copiando o duplicando tareas existentes. Para obtener más información, vea [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Moviendo tareas de un proyecto a otro. Para obtener más información, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license</p> </td> 
   <td><p>Standard</p> 
   <p>Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects. </a></p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Creación de tareas en un proyecto

Crear tareas en un proyecto es similar a crear tareas en una plantilla. Puede seguir los pasos descritos a continuación al agregar tareas de plantilla a una plantilla.

Para crear tareas en un proyecto:

1. Vaya al proyecto donde desea crear una tarea.
1. Haga clic en **Tareas** en el panel izquierdo.
1. (Condicional) Si está viendo la lista de tareas en una vista Agile, haga clic en el icono **Vista de lista** ![](assets/list-view-in-agile-view-for-tasks.png) en la esquina superior derecha para mostrar la lista de tareas.
1. (Opcional) Haga clic en el icono **Modo de planificación** ![](assets/nwe-plan-mode-icon-task-list.png) y seleccione **Guardar de forma manual**; a continuación, seleccione **Estándar** o **Planificación de la cronología**. Esto deshabilita la opción **Guardar automáticamente**, que está habilitada de manera predeterminada.

   ![Seleccione Guardar de forma manual](assets/manual-save-option.png)

   >[!TIP]
   >
   >Puede invertir los cambios al seleccionar Guardar de forma manual.

1. Cree una nueva tarea mediante uno de los procedimientos siguientes:

   * Haga clic en **Nueva tarea** en la parte superior de la lista de tareas.
   * Haga clic en **Agregar más tareas** en la parte inferior de la lista de tareas.

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Condicional) Si hizo clic en **Nueva tarea**, haga lo siguiente:

   1. Especifique cualquiera de los campos de la lista limitada de campos dentro del cuadro **Nueva tarea** y, a continuación, haga clic en **Crear tarea** si desea crear rápidamente una tarea.

      O

      Para actualizar todos los campos de la tarea, haga clic en **Más opciones** para abrir el cuadro **Crear tarea**.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      Se abre el cuadro **Crear tarea**.

      ![](assets/create-task-larger-box-nwe-350x244.png)


      >[!NOTE]
      >
      >Según la forma en que el administrador de Workfront configure la plantilla de diseño, los campos del cuadro Crear tarea podrían mostrar diferentes campos en el entorno. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Especifique información para las siguientes áreas en el panel izquierdo del cuadro Crear tarea:

      * Nombre de la tarea
      * Información general
      * Asignaciones
      * Formularios personalizados
      * Finanzas
      * Configuración

        Para obtener información sobre cómo definir todos los campos relacionados con tareas en una tarea, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. (Condicional y opcional) Si desea que la tarea sea recurrente, actualice el campo **Frecuencia de periodicidad**. Para obtener más información sobre la creación de tareas recurrentes, consulte [Crear tareas recurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Opcional) Haga clic en **Documentos** en el panel izquierdo para adjuntar un documento a la nueva tarea y, a continuación, haga clic en **Agregar o vincular archivos** para agregar un documento a la tarea desde el equipo, otro servicio o para vincular documentos y carpetas desde el equipo u otro servicio.

1. (Condicional) Si ha hecho clic en **Agregar más tareas** en el paso 5, empiece a introducir la información de la tarea mediante la edición en línea y, a continuación, pulse Intro.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Se recomienda utilizar esta opción, especialmente cuando se agregan varias tareas a la lista.

   ![](assets/add-more-tasks-inline.png)

1. (Condicional) Realice una de las siguientes acciones:

   * Si ha hecho clic en **Nueva tarea** en el paso 5, haga clic en **Crear tarea** para guardar los cambios y agregar la nueva tarea al proyecto.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Si ha hecho clic en **Agregar más tareas** en el paso 5, haga lo siguiente:

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Haga clic en cualquier lugar del explorador para enviar los cambios o pulse Intro.
      1. (Opcional) En la lista de tareas, seleccione la tarea recién creada y, a continuación, haga clic en **Agregar sangría**.

         Esto hace que la nueva tarea sea secundaria o subtarea de la tarea anterior.

         Para obtener más información acerca de las tareas secundarias, vea la sección &quot;Crear subtareas a partir de la sección de subtareas de tareas&quot; en el artículo [Crear subtareas](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

      1. (Condicional) Si ha deshabilitado la opción **Autoguardar** después de pulsar **Agregar más tareas**, puede hacer lo siguiente:

         * Haga clic en **Deshacer** en cualquier momento para revertir el último cambio o en **Cancelar** para revertir todos los cambios que se hayan realizado en la lista de tareas.
         * Si anteriormente ha hecho clic en **Deshacer**, haga clic en **Rehacer** para volver a aplicar el último cambio cancelado.
         * Haga clic en **Guardar** para guardar los cambios en la lista de tareas.
   1. (Opcional) En una lista de tareas, haga clic en la sección **Predecesora** para agregarle predecesoras. Para obtener más información, vea [Crear una relación de predecesoras mediante el área de predecesoras](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
   1. (Opcional) En una lista de tareas, haga clic en la sección **Subtareas** para agregar tareas secundarias. Para obtener más información, consulte [Crear subtareas](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

## Crear tareas moviendo una tarea personal a un proyecto

1. (Condicional) Asegúrese de que usted y otros usuarios hayan creado tareas personales.

   Para obtener más información, consulte [Crear tareas personales](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).
1. Cree un filtro de tareas personales y aplíquelo a un informe o una lista de tareas.

   Para obtener más información, vea [Filtro: tareas personales](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).

   ![](assets/personal-tasks-report.png)
1. Haga clic en el nombre de una tarea en el informe de tareas personales para abrirla.

   Workfront guarda las tareas personales en un proyecto personal no enumerado al que siempre se le asigna un nombre según este patrón: Tareas de &quot;&lt; Nombre completo del usuario >. Por ejemplo, un proyecto personal podría llamarse &quot;Tareas de Rick&quot;.

1. En la página de tareas, haga clic en el **menú Más** ![](assets/more-icon.png) y, a continuación, haga clic en **Mover**. Para obtener más información sobre cómo mover tareas, vea [Mover tareas](/help/quicksilver/manage-work/tasks/manage-tasks/move-tasks.md).

   Cuando termine de mover la tarea, la tarea se mostrará en el proyecto seleccionado. La escala de tiempo del proyecto puede verse afectada por la escala de tiempo de la nueva tarea.
