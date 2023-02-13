---
title: Eliminar proyectos
product-area: projects
navigation-topic: manage-projects
description: Puede eliminar un proyecto si este y sus datos ya no son necesarios.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Eliminar proyectos

Puede eliminar un proyecto si este y sus datos ya no son necesarios.

Como alternativa a la eliminación de un proyecto, recomendamos editar el proyecto y cambiar el estado a Completado o Muerto. Esto elimina todas las tareas actuales relacionadas con el proyecto de la lista de tareas de un usuario, pero guarda todos los datos asociados con el proyecto.

## Requisitos de acceso

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks,&nbsp;Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos, Tareas, Problemas con capacidad para Eliminar proyectos, tareas y problemas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para el proyecto, tareas y problemas con la capacidad de Eliminar el proyecto, las tareas y los problemas. </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.
Puede eliminar un proyecto en una lista de proyectos o en el nivel de proyecto.

## Comprender el proceso de eliminación de proyectos

* [Limitaciones para eliminar proyectos](#limitations-for-deleting-projects)
* [El impacto de la eliminación de proyectos](#the-impact-of-deleting-projects)

### Limitaciones para eliminar proyectos  {#limitations-for-deleting-projects}

* Los elementos eliminados se mueven a la Papelera de reciclaje durante 30 días y solo el administrador de Workfront puede recuperarlos.

   Para obtener más información sobre la restauración de objetos, consulte el artículo [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Si el proyecto tiene tareas o problemas con las horas registradas, el administrador de Workfront o del grupo debe permitir la eliminación de estas tareas configurando las Preferencias de tarea y problema en la instancia de Workfront para que pueda eliminar el proyecto que contiene las tareas.

   Para obtener más información sobre cómo habilitar la eliminación de tareas, problemas o proyectos en los que se registran horas, consulte la sección &quot;Eliminación&quot; en [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### El impacto de la eliminación de proyectos {#the-impact-of-deleting-projects}

* Al eliminar un proyecto, se ven afectados otros objetos vinculados a él.

   Los siguientes objetos adjuntos a un proyecto también se eliminan al eliminar un proyecto:

   * Documentos

      No se puede eliminar un proyecto que tenga un documento adjunto que se haya extraído. Para obtener más información sobre la comprobación de documentos, consulte [Ver documentos](../../../documents/managing-documents/check-out-documents.md).

   * Tareas
   * Subtareas
   * Problemas
   * Notas
   * Rutas de aprobación
   * Gastos

* Según la configuración que realice el administrador de Workfront del proyecto, la tarea o las preferencias de eliminación de problemas en las preferencias de horario y hora de la instancia de Workfront, las horas registradas para las tareas, los problemas o el proyecto se gestionan de una de las siguientes formas al eliminar el proyecto:

   * Las horas permanecen en el parte de horas como hora general.
   * Las horas se eliminan y se restauran si el proyecto se restaura.

   Para obtener más información sobre la configuración de las preferencias de eliminación para las horas registradas en los problemas, consulte [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Si el proyecto que elimine está vinculado a una iniciativa del planificador de escenarios de Workfront:

   * La iniciativa sigue en el plan, pero el vínculo con el proyecto es eliminado.
   * Si el proyecto que elimine está vinculado a la única iniciativa publicada de un plan, también se elimina la indicación de que el plan se ha publicado.
   * Si recupera un proyecto eliminado, se recupera el proyecto, pero su vínculo a la iniciativa no se restaura y el área del planificador de escenarios ya no aparece en Detalles del proyecto.

      El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte [Información general del planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md).

      Para obtener información sobre los proyectos vinculados a iniciativas en el planificador de escenarios, consulte [Actualizar o crear proyectos publicando iniciativas en el Planificador de escenarios](../../../scenario-planner/publish-scenarios-update-projects.md).

* Si el proyecto también es una actividad para un objetivo en los objetivos de Workfront:

   * El proyecto se elimina del objetivo. También se elimina el progreso que indica el proyecto en relación con el objetivo.

   * Si recupera el proyecto eliminado, también se restaura el proyecto como actividad del objetivo.

      Esto requiere una licencia adicional. Para obtener información sobre los objetivos de Workfront, consulte [Información general sobre los objetivos de Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

      Para obtener información sobre cómo asociar proyectos con objetivos, consulte [Agregar proyectos a objetivos en Objetivos de Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Eliminación de un proyecto de una lista

Puede eliminar proyectos de una lista de proyectos.

1. Vaya a una lista de proyectos o a un informe de proyecto.
1. Seleccione el proyecto que desee eliminar y haga clic en **Eliminar** en la parte superior de la lista.

1. Haga clic en **Sí, Eliminarlo** para confirmar la eliminación.

   El proyecto se elimina y se almacena en la Papelera de reciclaje durante 30 días. El administrador de Workfront puede restaurarlo desde la Papelera de reciclaje durante este tiempo.

## Eliminar un proyecto en el nivel de proyecto

1. Vaya al proyecto que desee eliminar.
1. Haga clic en el **Más** icono ![](assets/qs-more-menu.png).

1. Haga clic en **Eliminar proyecto**.

1. Haga clic en **Sí, elimínelo**.

   El proyecto se elimina y se almacena en la Papelera de reciclaje durante 30 días. El administrador de Workfront puede restaurarlo desde la Papelera de reciclaje durante este tiempo.

## Restauración de proyectos eliminados

Un administrador de sistemas o grupos puede restaurar proyectos dentro de los 30 días posteriores a su eliminación, tal como se describe en el artículo [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
