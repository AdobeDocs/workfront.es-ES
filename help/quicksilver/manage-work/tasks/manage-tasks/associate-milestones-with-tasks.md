---
product-area: projects
navigation-topic: manage-tasks
title: Asociar hitos a tareas
description: Puede asociar hitos con tareas para indicar cuándo se alcanzan pasos importantes durante la duración del proyecto. Debe asociar una trayectoria del hito a un proyecto antes de poder asociar hitos con tareas del proyecto.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Asociar hitos a tareas

<!--Audited: 01/2024-->

Puede asociar hitos con tareas para indicar cuándo se alcanzan pasos importantes durante la duración del proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>Nueva licencia: Standard</p> 
   <p>Licencia actual: Trabajo o superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas</p> <p><b>NOTA</b>

Si no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para la tarea</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

+++

## Requisitos previos

Para poder asociar un hito a una tarea, debe existir lo siguiente:

* El administrador de Workfront debe crear una ruta de hitos, tal como se describe en [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Debe asociar una ruta de hitos a un proyecto.

  Para obtener más información, consulte [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* Para asociar una trayectoria del hito a un proyecto, el proyecto debe estar en estado Planificación o Actual.

  >[!TIP]
  >
  >Para obtener la mejor descripción general del progreso de los hitos en sus proyectos mediante la vista Hito, debe crear tareas principales y asociarlas a cada fase principal del proyecto. A continuación, asocie estas tareas principales a cada uno de los hitos de la trayectoria del hito.

## Asociar un hito a una tarea

Una vez asociada una trayectoria del hito a un proyecto, se puede asignar un hito a las tareas.

1. Vaya a una tarea, haga clic en el icono **Más** ![](assets/more-icon.png) a la derecha del nombre de la tarea y, a continuación, **Editar**.

   Las tareas y los hitos tienen una relación 1:1. No se puede adjuntar el mismo hito a varias tareas. Cada tarea se puede vincular a un solo hito, o cada hito se puede asignar a una tarea.

1. Haga clic en **Configuración** y, a continuación, seleccione un hito en el campo **Hito** para la tarea.
1. Haga clic en **Guardar**.
1. (Opcional) En una lista de tareas, agregue la columna **Iconos de estado** para identificar qué tareas tienen hitos. El indicador de rombo de hito aparece en la columna Iconos de estado.

   Para obtener más información, consulte [Crear o editar vistas en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![](assets/amwt3.png)

1. (Opcional) Vaya a una lista de proyectos y seleccione la vista **Hito** para identificar el progreso de sus tareas de hito.

   ![](assets/milestone-view-project-list.png)
