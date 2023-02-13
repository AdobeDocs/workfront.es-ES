---
product-area: projects
navigation-topic: manage-tasks
title: Asociar hitos con tareas
description: Puede asociar hitos con tareas para indicar cuándo se alcanzan pasos importantes durante la duración del proyecto.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Asociar hitos con tareas

Puede asociar hitos con tareas para indicar cuándo se alcanzan pasos importantes durante la duración del proyecto.

## Requisitos de acceso

<!--drafted - replace table for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
  <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para la tarea</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Para poder asociar un hito a una tarea, debe existir lo siguiente:

* El administrador de Workfront debe crear una ruta de hitos, tal como se describe en [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Para asociar una ruta de hitos a un proyecto, el proyecto debe estar en estado de Planning o Current.

>[!TIP]
>
>Para obtener la mejor descripción general del progreso de hitos en los proyectos mediante la vista Milestone, debe crear tareas principales y asociarlas a cada fase principal del proyecto. A continuación, asocie estas tareas principales con cada uno de los hitos de la ruta de hitos.

## Asociación de un hito a una tarea

1. Vaya a un proyecto y, a continuación, haga clic en el **Más** icono ![](assets/more-icon.png), luego **Editar**.
1. Al usar la variable **Configuración** , establezca la ruta de hitos que se utilizará en el proyecto.
1. Haga clic en **Guardar**.

   Una vez asociada una ruta de hitos a un proyecto, las tareas se pueden asignar a un hito.

1. Vaya a una tarea y, a continuación, haga clic en la **Más** icono ![](assets/more-icon.png), luego **Editar**.

   Tareas e hitos tienen una relación 1:1. No se puede adjuntar el mismo hito a varias tareas. Cada tarea se puede vincular a un solo hito o cada hito se puede asignar a una tarea.

1. Haga clic en **Configuración** y, a continuación, seleccione un hito en la variable **Milestone** para la tarea.
1. Haga clic en **Guardar**.
1. (Opcional) En una lista de tareas, añada la variable **Iconos de estado** para identificar qué tareas tienen hitos.

   ![](assets/amwt3.png)

1. (Opcional) En una lista de proyectos, seleccione la **Milestone** para identificar el progreso de las tareas de hitos.

   ![Screen_Shot_2018-06-13_at_3.57.56_PM.png](assets/screen-shot-2018-06-13-at-3.57.56-pm-350x57.png)
