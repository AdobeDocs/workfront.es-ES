---
product-area: projects
navigation-topic: create-tasks
title: Creación de subtareas
description: En Workfront, las tareas pueden tener relaciones principal-secundario. Las tareas secundarias se denominan subtareas. Puede crear subtareas en la lista de tareas convirtiendo una tarea principal en una subtarea. También puede convertir una subtarea en una tarea principal.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Creación de subtareas

<!-- Audited: 1/2024 -->

En Workfront, las tareas pueden tener relaciones principal-secundario. Las tareas secundarias se denominan subtareas. Puede crear subtareas en la lista de tareas convirtiendo una tarea principal en una subtarea. También puede convertir una subtarea en una tarea principal.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Nuevo: estándar</p>
   <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Proyectos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de contribución para el proyecto y la tarea principal con capacidad para Agregar tareas o superior</p> <p>Una vez creada la tarea, recibirá automáticamente permisos de administración.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de subtareas

Puede crear subtareas desde la lista de tareas o desde la sección de subtareas de tareas.

### Crear subtareas de la lista de tareas {#create-subtasks-from-the-task-list}

1. Vaya al proyecto donde desea crear subtareas.
1. Haga clic en **Tareas** en el panel izquierdo.
1. (Condicional) Si la tarea que desea convertir en la tarea secundaria no se encuentra ya directamente debajo de la tarea que desea convertir en la principal, arrástrela a la ubicación adecuada en la lista de tareas.
1. Seleccione la tarea que desea convertir en subtarea y realice una de las siguientes acciones:

   * Haga clic en **Sangría** icono ![](assets/indent-icon-nwe-33x29.png) para hacer que la tarea seleccionada sea una subtarea a la tarea directamente encima de ella.
   * Cuando utilice un teclado estándar inglés QWERTY, pulse Option + > (Mac) o Alt + > (Windows) en el teclado. Otros idiomas pueden utilizar los comandos Opción + , (Mac) o Alt + , (Windows) para aplicar sangría.

     >[!TIP]
     >
     >Los métodos abreviados del teclado no funcionan cuando se editan tareas en la edición en línea. En este caso, utilice el icono Sangría ![](assets/cs1.png) para crear subtareas.

   * Arrastre y suelte la tarea sobre la tarea que desee designar como tarea principal.

     >[!NOTE]
     >
     >Sólo puede aplicar sangría a las tareas cuando la lista de tareas está ordenada por Número de tarea y cuando no hay agrupaciones aplicadas a la lista de tareas.

### Crear subtareas desde la sección Subtareas {#create-subtasks-from-the-task-subtasks-section}

1. Vaya al proyecto donde desea crear subtareas.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Haga clic en el nombre de la tarea donde desea crear una subtarea.
1. Haga clic en **Subtareas** en el panel izquierdo.
1. Clic **Nueva tarea.**

   Siga los pasos del siguiente artículo para continuar creando la subtarea: [Creación de tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Clic **Guardar tarea.**

## Hacer de una subtarea una tarea principal

1. Vaya al proyecto donde desea convertir una subtarea en una tarea principal.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Seleccione la subtarea que desea convertir en tarea principal.
1. Haga clic en **Anular sangría** icono ![](assets/outdent-icon-nwe-31x29.png) para que la subtarea sea una tarea principal.

   O

   En un teclado estándar inglés QWERTY, presione Opción + &lt; (Mac) o Alt + &lt; (Windows). Otros idiomas pueden utilizar los comandos Opción + . (Mac) o Alt + . (Windows) para anular la sangría.

   >[!NOTE]
   >
   >Solo puede anular la sangría de tareas cuando la lista de tareas esté ordenada por Número de tarea y cuando no haya agrupaciones aplicadas a la lista de tareas.
