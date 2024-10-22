---
product-area: projects
navigation-topic: create-tasks
title: Creación de tareas en un proyecto
description: Sólo puede crear tareas en un proyecto una vez creado el proyecto.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 1%

---

# Creación de tareas en un proyecto

<!-- Audited: 1/2024 -->

Sólo puede crear tareas en un proyecto una vez creado el proyecto.

Por ejemplo, después de crear un proyecto, puede que desee agregar tareas y modificarlas para organizar el plan del proyecto. Para obtener más información sobre cómo crear un proyecto, vea [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

<!--Not possible anymore, after new Home: For information about creating personal tasks that are not in a project, see the [Create a personal task](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task) section in the article [Create work items and projects from the Home area](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).-->

Este artículo describe cómo crear tareas desde cero. También puede crear tareas de las siguientes maneras:

* Copiando o duplicando tareas existentes. Para obtener más información, vea [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Al mover tareas de un proyecto a otro. Para obtener más información, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licencia de Adobe Workfront</p> </td> 
   <td><p>Actual: Trabajo o superior</p> 
   O
   <p>Nuevo: estándar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Proyectos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute para el proyecto con capacidad para Agregar tareas o superior</p> <p>Al crear una tarea, recibe automáticamente permisos de administración para la tarea</p> <p> Para obtener información acerca de los permisos de tareas, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartir una tarea </a>. </p> <p>Para obtener información sobre cómo solicitar permisos adicionales, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de tareas en un proyecto

1. Vaya al proyecto donde desea crear una tarea.
1. Haga clic en **Tareas** en el panel izquierdo.
1. (Condicional) Si está viendo la lista de tareas en una vista Agile, haga clic en el icono **Vista de lista** ![](assets/list-view-in-agile-view-for-tasks.png) en la esquina superior derecha para mostrar la lista de tareas.
1. (Opcional) Haga clic en el icono **Modo de planificación** ![](assets/nwe-plan-mode-icon-task-list.png) y seleccione **Guardar de forma manual**; a continuación, seleccione **Estándar** o **Planificación de la cronología**. Esto deshabilita la opción **Guardar automáticamente**, que está habilitada de manera predeterminada.

   ![Seleccionar Guardar de forma manual](assets/manual-save-option.png)

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

   1. (Condicional y opcional) Si desea que la tarea sea periódica, actualice el campo **Frecuencia de periodicidad**. Para obtener más información acerca de la creación de tareas recurrentes, vea [Crear tareas recurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Opcional) Haga clic en **Documentos** en el panel izquierdo para adjuntar un documento a la nueva tarea y, a continuación, haga clic en **Agregar o vincular archivos** para agregar un documento a la tarea desde el equipo, otro servicio o para vincular documentos y carpetas desde el equipo u otro servicio.

1. (Condicional) Si hizo clic en **Agregar más tareas** en el paso 5, empiece a escribir la información de la tarea mediante la edición en línea y, a continuación, presione Entrar.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Se recomienda utilizar esta opción, especialmente cuando se añaden varias tareas a la lista.

   ![](assets/add-more-tasks-inline.png)

1. (Condicional) Realice una de las siguientes acciones:

   * Si hizo clic en **Nueva tarea** en el paso 5, haga clic en **Crear tarea** para guardar los cambios y agregar la nueva tarea al proyecto.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Si hizo clic en **Agregar más tareas** en el paso 5, haga lo siguiente:

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Haga clic en cualquier lugar del explorador para enviar los cambios o pulse Intro.
      1. (Opcional) En la lista de tareas, seleccione la tarea recién creada y luego haga clic en **Sangría**.

         Esto hace que la nueva tarea sea secundaria o subtarea de la tarea anterior.

         Para obtener más información acerca de tareas secundarias, vea [Crear subtareas](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

      1. (Condicional) Si deshabilitó la opción **Guardar automáticamente** después de presionar **Agregar más tareas**, puede hacer lo siguiente:

         * Haz clic en **Deshacer** en cualquier momento para revertir el último cambio o en **Cancelar** para revertir todos los cambios que hiciste en la lista de tareas.
         * Si anteriormente hizo clic en **Deshacer**, haga clic en **Rehacer** para volver a aplicar el último cambio que canceló.
         * Haga clic en **Guardar** para guardar los cambios en la lista de tareas.
