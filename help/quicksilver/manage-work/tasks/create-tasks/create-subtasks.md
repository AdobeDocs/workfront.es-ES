---
product-area: projects
navigation-topic: create-tasks
title: Crear subtareas
description: En Adobe Workfront, las tareas pueden tener relaciones principal-secundario. Las tareas secundarias se denominan subtareas. Puede crear subtareas en la lista de tareas convirtiendo una tarea principal en una subtarea. También se puede convertir una subtarea en una tarea principal.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 73%

---

# Creación de subtareas

<!-- Audited: 01/2025 -->

En Adobe Workfront, las tareas pueden tener relaciones principal-secundario. Las tareas secundarias se denominan subtareas. Puede crear subtareas en la lista de tareas convirtiendo una tarea principal en una subtarea de otra tarea. También se puede convertir una subtarea en una tarea principal.

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project and the parent task with ability to Add Tasks or higher</p> <p>You automatically receive Manage permissions to the task after you create it.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Creación de subtareas

Puede crear subtareas desde la lista de tareas o desde la sección de subtareas de tareas.

>[!TIP]
>
>Crear subtareas para un proyecto es similar a crear subtareas de plantilla para crear tareas de plantilla en una plantilla.


### Crear subtareas desde la lista de tareas {#create-subtasks-from-the-task-list}

1. Vaya al proyecto donde desea crear subtareas.
1. Haga clic en **Tareas** en el panel izquierdo.
1. (Condicional) Si la tarea que desea convertir en la tarea secundaria no se encuentra ya directamente debajo de la tarea que desea convertir en la principal, arrástrela y suéltela en la ubicación adecuada en la lista de tareas.
1. Seleccione la tarea que desea convertir en subtarea y realice una de las siguientes acciones:

   * Haga clic en el icono **Sangría** ![](assets/indent-icon-nwe-33x29.png) para que la tarea seleccionada sea una subtarea de la tarea que hay directamente encima de ella.
   * Cuando utilice un teclado estándar inglés QWERTY, pulse Option + > (Mac) o Alt + > (Windows) en el teclado. Otros idiomas pueden utilizar los comandos Opción + , (Mac) o Alt + , (Windows) para aplicar sangría.

     >[!TIP]
     >
     >Los métodos abreviados del teclado no funcionan cuando se editan tareas en la edición en línea. En este caso, utilice el icono Sangría ![](assets/indent-icon-nwe-33x29.png) para crear subtareas.

   * Arrastre y suelte la tarea sobre la tarea que desea designar como la tarea principal.

     >[!NOTE]
     >
     >Solo puede aplicar sangría a las tareas cuando la lista de tareas está ordenada por Número de tarea y cuando no hay agrupaciones aplicadas a la lista de tareas.

### Crear subtareas desde la sección Subtareas de la tarea {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>Es posible que el administrador de su Workfront o de su grupo elimine la sección Subtareas de su entorno mediante una plantilla de diseño.

1. Vaya al proyecto donde desea crear subtareas.
1. Haga clic en la sección **Tareas** en el panel izquierdo.
1. Haga clic en el nombre de la tarea donde desea crear una subtarea.
1. Haga clic en la sección **Subtareas** del panel izquierdo, si está disponible.
1. Haga clic en **Nueva tarea**

   Para obtener información sobre cómo crear tareas, vea [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Haga clic en **Crear tarea.**

   La nueva tarea se crea como una subtarea de la tarea seleccionada en el paso 3. <!--ensure this is accurate-->

## Hacer de una subtarea una tarea principal

1. Vaya al proyecto donde desea convertir una subtarea en una tarea principal.
1. Haga clic en la sección **Tareas** en el panel izquierdo.
1. Seleccione la subtarea que desea convertir en tarea principal.
1. Haga clic en el icono **Anular sangría** ![](assets/outdent-icon-nwe-31x29.png) para que la subtarea sea una tarea principal.

   O

   En un teclado estándar inglés QWERTY, presione Opción + &lt; (Mac) o Alt + &lt; (Windows). Otros idiomas pueden utilizar los comandos Opción + . (Mac) o Alt + . (Windows) para anular la sangría.

   >[!NOTE]
   >
   >Solo puede anular la sangría de tareas cuando la lista de tareas esté ordenada por Número de tarea y cuando no haya agrupaciones aplicadas a la lista de tareas.
