---
title: Eliminar proyectos
product-area: projects
navigation-topic: manage-projects
description: Puede eliminar un proyecto si el proyecto y sus datos ya no son necesarios.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: 5db9a4869e1321bd268e80f786d157fbb41c0656
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 1%

---

# Eliminar proyectos

Puede eliminar un proyecto si el proyecto y sus datos ya no son necesarios.

Como alternativa a eliminar un proyecto, se recomienda editar el proyecto y cambiar el estado a Completo o Inactivo. De este modo, se quitan todas las tareas actuales relacionadas con el proyecto de la lista de tareas de un usuario, pero se guardan todos los datos asociados con el proyecto.

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
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos, Tareas, Problemas con la capacidad de Eliminar proyectos, tareas y problemas</p> <p><b>NOTA</b></p>

<p>Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para el proyecto, tareas y problemas en el proyecto con capacidad para eliminar el proyecto, las tareas y los problemas. </p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.
Puede eliminar un proyecto en una lista de proyectos o en el nivel de proyecto.

## Comprender el proceso de eliminación de proyectos

* [Limitaciones para eliminar proyectos](#limitations-for-deleting-projects)
* [Impacto de la eliminación de proyectos](#the-impact-of-deleting-projects)

### Limitaciones para eliminar proyectos  {#limitations-for-deleting-projects}

* Los elementos eliminados se trasladan a la papelera de reciclaje durante 30 días y solamente el administrador de Workfront puede recuperarlos.

  Para obtener más información acerca de cómo restaurar objetos, vea el artículo [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Si el proyecto tiene tareas o problemas con las horas registradas, el administrador del grupo o de Workfront debe permitir la eliminación de estas tareas configurando las Preferencias de tareas y problemas en la instancia de Workfront para que pueda eliminar el proyecto que contiene las tareas.

  Para obtener más información sobre cómo habilitar la eliminación de tareas, problemas o proyectos en los que se registran horas, consulte la sección &quot;Eliminación&quot; en [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Impacto de la eliminación de proyectos {#the-impact-of-deleting-projects}

* Al eliminar un proyecto, se afectan otros objetos vinculados al proyecto.

  Los siguientes objetos adjuntos a un proyecto también se eliminan al eliminarlo:

   * Documentos

     No se puede eliminar un proyecto que tenga un documento adjunto que se haya desprotegido. Para obtener más información sobre la retirada de documentos, consulte [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

   * Tareas
   * Subtareas
   * Problemas
   * Actualizaciones
   * Rutas de aprobación
   * Gastos
   * Riesgos
   * Líneas base
   * Información de caso comercial
   * Detalles de cola
   * Tarifas de facturación
   * Registros de facturación

     No puede eliminar un proyecto que tenga Registros de facturación con el estado Facturado. Para obtener más información, consulte [Crear registros de facturación](../../projects/project-finances/create-billing-records.md).

* Según la forma en la que el administrador de Workfront configure las preferencias de eliminación de proyectos, tareas o problemas en las preferencias de plantilla de horas y horas de la instancia de Workfront, las horas registradas para las tareas, los problemas o el proyecto se gestionarán de una de las siguientes maneras al eliminar el proyecto:

   * Las horas permanecen en la hoja de horas como tiempo general.
   * Las horas se eliminan y se restaurarán si alguna vez se restaura el proyecto.

  Para obtener más información sobre la configuración de las preferencias de eliminación para los problemas de horas de sesión, consulte [Configurar preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Si el proyecto que elimina está vinculado a una iniciativa en el Scenario Planner de Workfront:

   * La iniciativa permanece en el plan, pero se elimina el vínculo al proyecto.
   * Si el proyecto que elimina está vinculado a la única iniciativa publicada de un plan, también se elimina la indicación de que el plan se ha publicado.
   * Si recupera un proyecto eliminado, el proyecto se recupera, pero su vínculo a la iniciativa no se restaura y el área del Planificador de escenarios ya no se muestra en Detalles del proyecto.

     El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte [Información general del Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

     Para obtener información sobre los proyectos vinculados a iniciativas en el Scenario Planner, consulte [Actualizar o crear proyectos publicando iniciativas en el Scenario Planner](../../../scenario-planner/publish-scenarios-update-projects.md).

* Si el proyecto también es una actividad para un objetivo en Workfront Goals:

   * El proyecto se elimina de la meta. También se elimina el progreso indicado en la meta por el proyecto.

   * Si recupera el proyecto eliminado, este también se restaurará como la actividad del objetivo.

     Esto requiere una licencia adicional. Para obtener información sobre los objetivos de Workfront, consulte [Información general sobre Adobe Workfront Goals](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Para obtener información sobre cómo asociar proyectos con objetivos, consulte [Agregar proyectos a metas en Adobe Workfront Goals](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Eliminación de un proyecto de una lista

Puede eliminar proyectos de una lista.

1. Ir a una lista de proyectos o a un informe de proyecto.
1. Seleccione el proyecto o proyectos que desee eliminar y haga clic en el botón **Eliminar** icono ![](assets/delete-icon.png) al principio de la lista.

1. Clic **Sí, eliminarla** para confirmar la eliminación.

   Los proyectos se eliminan y se almacenan en la papelera de reciclaje durante 30 días. El administrador de Workfront puede restaurar los proyectos eliminados de la papelera de reciclaje durante este tiempo.

## Eliminar un proyecto en el nivel de proyecto

1. Vaya al proyecto que desee eliminar.
1. Haga clic en **Más** icono ![](assets/qs-more-menu.png), luego haga clic en **Eliminar proyecto**.

   ![](assets/more-icon-expanded-delete-project-highlighted.png)

1. Clic **Sí, eliminarla**.

   El proyecto se elimina y se almacena en la papelera de reciclaje durante 30 días. El administrador de Workfront puede restaurarla desde la papelera de reciclaje durante este tiempo.

## Restauración de proyectos eliminados

Un administrador de sistema o de grupo puede restaurar proyectos en un plazo de 30 días después de haberlos eliminado, tal como se describe en el artículo [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
