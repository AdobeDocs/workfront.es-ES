---
product-area: projects
navigation-topic: update-work-in-a-project
title: Actualizar estado de la tarea
description: Puede actualizar el estado de una tarea para informar a otros sobre dónde se encuentra la tarea (y el proyecto general) y cómo progresa.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 1%

---

# Actualizar estado de la tarea

Puede actualizar el estado de una tarea para informar a otros sobre dónde se encuentra la tarea (y el proyecto general) y cómo progresa.

Los estados predeterminados son Nuevo, En curso y Completado. El administrador de Adobe Workfront puede agregar estados personalizados para su organización. Para obtener más información, consulte [Creación o edición de un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Puede actualizar manualmente los estados de las tareas o dejar que Workfront los actualice automáticamente cuando se realicen determinadas acciones.

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

## Consideraciones acerca de la actualización del estado de las tareas

* Cuando marca una tarea como Completada, el porcentaje completado de la tarea se actualiza al 100%.
* Los siguientes escenarios existen para tareas principales:
   * No se puede actualizar el estado de una tarea principal a Completo cuando el modo de finalización de resumen del proyecto está establecido en Automático y las subtareas no se han completado.
   * Puede actualizar el estado de una tarea principal a Completo cuando el modo de finalización de resumen del proyecto esté establecido en Manual y las subtareas estén completadas o incompletas.

  Para obtener más información, consulte [Editar proyectos](../manage-projects/edit-projects.md).

## Actualizar manualmente el estado de la tarea

Al actualizar un estado de tarea, también puede escribir una explicación sobre el nuevo estado y cambiar otra información de la tarea, como la fecha de vencimiento.

1. Vaya a una tarea a la que esté asignado para la que desee actualizar el estado.
1. Haga clic en **Estado** en el encabezado de la tarea y seleccione un nuevo estado.
1. (Opcional) Realice una de las siguientes acciones para proporcionar información adicional sobre la actualización y, a continuación, haga clic en **Actualizar** o, si la tarea tiene el **Completar** estado, haga clic en **Listo:**

   * Para añadir una nota sobre la actualización, vaya a **Actualizaciones** y haga clic en **Iniciar una nueva actualización** y, a continuación, escriba la nota.

   * Para notificar la actualización a determinados usuarios, escriba sus nombres en la **Notificar** que aparece al escribir una nota sobre la actualización. Para obtener más información, consulte [Etiquetar a otros en las actualizaciones](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Para actualizar la condición de la tarea, haga clic en **Seleccionar condición** a la derecha del **Notificar** (aparecen al escribir una nota sobre la actualización) y, a continuación, seleccione la condición que mejor refleje la condición actual de la tarea.

   * Para actualizar la fecha de confirmación de la tarea, expanda **Fecha de confirmación** , y seleccione una nueva fecha de compromiso.
   * Para proporcionar una indicación visual de la finalización de la tarea, arrastre la burbuja bajo Porcentaje completado o haga doble clic en ella para introducir un valor porcentual.\
     ![](assets/drag-the-progress-bar-350x155.png)

## Actualizar automáticamente el estado de la tarea

Workfront actualiza automáticamente el estado existente de una tarea a un estado diferente cuando se producen las acciones enumeradas en la siguiente tabla.

>[!NOTE]
>
>Los estados de la tabla siguiente son estados de sistema predeterminados. El administrador de Workfront o de un grupo puede cambiar el nombre de los estados de su instancia de Workfront. Para obtener información sobre la creación y administración de estados en Workfront, consulte [Creación o edición de un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Acción</td> 
   <td>Estado original</td> 
   <td>Nuevo estado</td> 
  </tr> 
  <tr> 
   <td>Actualizar el porcentaje completado de la tarea al 100%</td> 
   <td>Nuevo o en curso</td> 
   <td>Completar</td> 
  </tr> 
  <tr> 
   <td>Actualizar el porcentaje completado de la tarea del 100% a un número inferior</td> 
   <td>Completar</td> 
   <td>En curso</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Haga clic en el botón Iniciar tarea para aceptar el trabajo en una tarea asignada</span> </td> 
   <td><span>Nuevo</span> </td> 
   <td> <p>Cualquier estado asociado con el botón Iniciar tarea en la configuración de Equipo de inicio.</p> <p>Para obtener información sobre cómo reemplazar el botón Trabajar en ello por un botón Iniciar tarea, consulte <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Reemplazar el botón Trabajar en ello por un botón Iniciar</a></span>.</p> <p>Sugerencia: <span>Clic</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">el botón Deshacer</span>después de hacer clic en Iniciar tarea, revierte el estado a Nuevo. </p> </td> 
  </tr> 
 </tbody> 
</table>
