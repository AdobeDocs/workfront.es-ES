---
product-area: projects
navigation-topic: create-tasks
title: Crear tareas en un proyecto
description: Solo puede crear tareas en un proyecto una vez creado el proyecto.
author: Alina
feature: Work Management
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---

# Crear tareas en un proyecto

Solo puede crear tareas en un proyecto una vez creado el proyecto.

Por ejemplo, después de crear un proyecto, es posible que desee agregar tareas y modificarlas para organizar el plan del proyecto. Para obtener más información sobre cómo crear un proyecto, consulte [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

Para obtener información sobre la creación de tareas personales que no están en un proyecto, consulte la sección &quot;Crear una tarea personal&quot; en el artículo [Crear elementos de trabajo desde el área principal](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

En este artículo se describe cómo crear tareas desde cero. También puede crear tareas de las siguientes maneras:

* Copiar o duplicar tareas existentes. Para obtener más información, consulte [Copiar y duplicar tareas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Al mover tareas de un proyecto a otro. Para obtener más información, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Requisitos de acceso

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td><p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
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
   <td role="rowheader"> <p role="rowheader">Licencia de Adobe Workfront*</p> </td> 
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

## Crear tareas en un proyecto

1. Vaya al proyecto en el que desea crear una tarea.
1. Haga clic en **Tareas** en el panel izquierdo.
1. (Condicional) Si está viendo la lista de tareas en una vista ágil, haga clic en el botón **Vista de lista** icono ![](assets/list-view-in-agile-view-for-tasks.png) en la esquina superior derecha para mostrar la lista de tareas.
1. (Opcional) Haga clic en el **Modo de plan** icono ![](assets/nwe-plan-mode-icon-task-list.png) y seleccione **Guardar manualmente** y, a continuación, seleccione **Estándar** o **Planificación de la cronología**. Esto deshabilita la variable **Autoguardar** que está activada de forma predeterminada.

   ![](assets/nwe-autosave-off-manual-highlighted-350x58.png)

   >[!TIP]
   >
   >Puede invertir los cambios al seleccionar Guardar manualmente.

1. Cree una nueva tarea realizando una de las siguientes acciones:

   * Haga clic en **Nueva tarea** en la parte superior de la lista de tareas
   * Haga clic en **Agregar más tareas** en la parte inferior de la lista de tareas

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Condicional) Si ha hecho clic en **Nueva tarea** haga lo siguiente:

   1. Especifique cualquiera de los campos de la lista limitada de campos dentro de la variable **Nueva tarea** y haga clic en **Crear tarea** si desea crear rápidamente una tarea.

      O

      Para actualizar todos los campos de la tarea, haga clic en **Más opciones** para abrir el **Crear tarea** en la ventana

      ![](assets/nwe-create-task-small-screen-350x272.png)

      La variable **Crear tarea** se abre.

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >Según la configuración de la plantilla de diseño que configure el administrador de Workfront, los campos del cuadro Crear tarea podrían mostrar diferentes campos en el entorno. Para obtener más información, consulte [Personalización de la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Especifique información para las siguientes áreas en el panel izquierdo del cuadro Crear tarea:

      * Nombre de la tarea
      * Información general
      * Asignaciones
      * Forms personalizado
      * Finanzas
      * Configuración

         Para obtener información sobre la definición de todos los campos relacionados con tareas en una tarea, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
   1. (Condicional y opcional) Si desea que la tarea sea recurrente, actualice la variable **Frecuencia de periodicidad** campo . Para obtener más información sobre la creación de tareas recurrentes, consulte [Crear tareas recurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Opcional) Haga clic en **Documentos** en el panel izquierdo para adjuntar un documento a la nueva tarea y, a continuación, haga clic en **Agregar o vincular archivos** para agregar un documento a la tarea desde el equipo, otro servicio o para vincular documentos y carpetas desde el equipo u otro servicio.


1. (Condicional) Si ha hecho clic en **Agregar más tareas** en el paso 5, empiece a introducir la información de la tarea mediante la edición en línea y, a continuación, pulse Intro.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Se recomienda utilizar esta opción, especialmente al añadir varias tareas a la lista.

   ![](assets/ctp4-350x26.png)

1. (Condicional) Realice una de las siguientes acciones:

   * Si ha hecho clic **Nueva tarea** en el paso 5, haga clic en **Crear tarea** para guardar los cambios y agregar la nueva tarea al proyecto.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Si ha hecho clic **Agregar más tareas** en el paso 5, haga lo siguiente:

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Haga clic en cualquier lugar del explorador para enviar los cambios o pulse Intro.
      1. (Opcional) En la lista de tareas, seleccione la tarea recién creada y haga clic en **Sangría**.

         Esto hace que la nueva tarea sea secundaria o subtarea de la tarea anterior.

         Para obtener más información sobre las tareas secundarias, consulte [Información general sobre tareas](../../../manage-work/tasks/task-information/tasks-overview.md).

      1. (Condicional) Si deshabilitó el **Autoguardar** opción después de pulsar **Agregar más tareas**, puede hacer lo siguiente:

         * Haga clic en **Deshacer** en cualquier momento para revertir el último cambio, o **Cancelar** para invertir todos los cambios realizados en la lista de tareas.
         * Si ha hecho clic anteriormente **Deshacer**, haga clic en **Rehacer** para volver a aplicar el último cambio que ha cancelado.
         * Haga clic en **Guardar** para guardar los cambios en la lista de tareas.
