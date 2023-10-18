---
product-area: projects
navigation-topic: update-work-in-a-project
title: Ver y actualizar el porcentaje completado de las tareas
description: Puede actualizar el porcentaje completado de una tarea para indicar el progreso que ha realizado en la tarea hacia completarla.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Ver y actualizar el porcentaje completado de las tareas

Puede actualizar el porcentaje completado de una tarea para indicar el progreso que ha realizado en la tarea hacia completarla.

## Requisitos de acceso

<!--drafted for P&P:

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

Debe tener el siguiente acceso para actualizar las tareas manualmente:

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
   <td> <p>Editar acceso a Tareas</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para la tarea</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.


## Áreas en las que se puede actualizar el porcentaje completado de una tarea

Puede actualizar el porcentaje completado de una tarea en cualquiera de las siguientes áreas:

* **En una lista de tareas**: puede actualizar el porcentaje completado de una tarea cuando se muestre la columna Porcentaje completado.\
  Para obtener más información sobre la edición en línea, consulte [Edición en línea de elementos en una lista en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **En la vista Hito**: puede actualizar el porcentaje completado de una tarea al utilizar la vista de Hito en una lista de proyectos o un informe de proyecto. Para obtener más información, consulte [Uso de la vista de Hito](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Al actualizar la tarea**: puede actualizar la opción de porcentaje completado de una tarea al añadir una actualización a la tarea.

  >[!IMPORTANT]
  >
  >Esta opción solo se muestra después de activar la opción Mostrar porcentaje completado.\
  >Para habilitar la barra de actualización de porcentaje completado para las tareas, haga lo siguiente:
  >
  >1. Vaya a la **Principal** menu>su nombre>**Más** junto a su nombre >**Editar** > seleccionar **Mostrar porcentaje completado al actualizar el estado**.\
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >

* **En el encabezado de la tarea**: puede actualizar el porcentaje completado de una tarea en el encabezado de la tarea. Para obtener más información, consulte [Editar tareas](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## Consideraciones acerca de la actualización del porcentaje completado de una tarea

* Cuando marca una tarea como 100% completada, el estado de la tarea se actualiza a Completada.
* Los siguientes escenarios existen para tareas principales:
   * No se puede actualizar el porcentaje completado de una tarea principal al 100% cuando el modo de finalización de resumen del proyecto está establecido en automático y las subtareas no se han completado.
   * Puede actualizar el porcentaje completado de una tarea principal al 100% cuando el modo de finalización de resumen del proyecto esté establecido en Manual y las subtareas estén completadas o incompletas.

  Para obtener más información, consulte [Editar proyectos](../manage-projects/edit-projects.md).

## Actualizar el porcentaje completado de una tarea

1. Vaya a cualquiera de las siguientes áreas de Workfront:

   * Una lista de tareas
   * Una lista de proyectos y aplicar la vista de Hito
   * Una tarea, accediendo a la página de tareas
1. Busque el **Porcentaje completado** para la tarea cuyo porcentaje completado desee actualizar.
1. Haga clic dentro del campo Porcentaje completado y escriba un número entre 0 y 100

   O

   Haga clic en y arrastre **Porcentaje completado** al número necesario para indicar la cantidad de la tarea que ha completado.

   >[!NOTE]
   >
   >Cuando indique que se ha completado el 100 % de la tarea, el estado de la tarea también se actualizará a Completada.


1. Pulse Intro en el teclado para guardar el porcentaje completado.

