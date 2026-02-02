---
product-area: projects
navigation-topic: manage-tasks
title: Asociar hitos a las tareas
description: Puede asociar hitos con tareas para indicar cuándo se alcanzan pasos importantes durante la duración del proyecto. Debe asociar una trayectoria del hito a un proyecto antes de poder asociar hitos con tareas del proyecto.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 90%

---

# Asociar hitos con tareas

<!--Audited: 01/2024-->

Puede asociar hitos con tareas para indicar cuándo se alcanzan pasos importantes durante la duración del proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para la tarea</p></td> 
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
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   <p>Current license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Requisitos previos

Para poder asociar un hito a una tarea, debe existir lo siguiente:

* El administrador de Workfront debe crear una ruta de hitos, tal como se describe en [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Debe asociar una ruta de hitos a un proyecto.

  Para obtener más información, consulte [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* Para asociar una ruta de hitos a un proyecto, el proyecto debe estar en el estado de Planificación o Actual.

  >[!TIP]
  >
  >Para obtener la mejor descripción general del progreso de los hitos en sus proyectos mediante la vista Hito, debe crear tareas principales y asociarlas a cada fase principal del proyecto. A continuación, asocie estas tareas principales a cada uno de los hitos de la ruta de hitos.

## Asociar un hito a una tarea

Una vez asociada una ruta de hitos a un proyecto, se puede asignar un hito a las tareas.

1. Vaya a una tarea y, a continuación, haga clic en el icono **Más** ![Icono de más](assets/more-icon.png) a la derecha del nombre de la tarea y, a continuación, **Editar**.

   Las tareas y los hitos tienen una relación 1:1. No se puede adjuntar el mismo hito a varias tareas. Cada tarea se puede vincular a un solo hito, o cada hito se puede asignar a una tarea.

1. Haga clic en **Configuración** y, a continuación, seleccione un hito en el campo **Hito** para la tarea.
1. Haga clic en **Guardar**.
1. (Opcional) En una lista de tareas, añada la columna **Iconos de estado** para identificar qué tareas tienen hitos. El indicador de hito con forma de rombo aparece en la columna Iconos de estado.

   Para obtener más información, consulte [Crear o editar vistas en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![Iconos de estado](assets/amwt3.png)

1. (Opcional) Vaya a una lista de proyectos y seleccione la vista **Hito** para identificar el progreso de sus tareas de hito.

   ![Lista de proyectos de vista de hito](assets/milestone-view-project-list.png)
