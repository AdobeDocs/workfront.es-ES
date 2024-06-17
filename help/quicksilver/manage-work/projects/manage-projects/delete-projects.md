---
title: Eliminar proyectos
product-area: projects
navigation-topic: manage-projects
description: Puede eliminar un proyecto si el proyecto y sus datos ya no son necesarios. Como alternativa a eliminar un proyecto, se recomienda editar el proyecto y cambiar el estado a Completo o Inactivo. De este modo, se quitan todas las tareas actuales relacionadas con el proyecto de la lista de tareas de un usuario, pero se guardan todos los datos asociados con el proyecto.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 1%

---

# Eliminar proyectos

<!--Audited: 01/2024-->

Puede eliminar un proyecto si el proyecto y sus datos ya no son necesarios.

Como alternativa a eliminar un proyecto, se recomienda editar el proyecto y cambiar el estado a Completo o Inactivo. De este modo, se quitan todas las tareas actuales relacionadas con el proyecto de la lista de tareas de un usuario, pero se guardan todos los datos asociados con el proyecto.

Puede eliminar un proyecto en una lista de proyectos o en el nivel de proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront*</p> </td> 
   <td> <p>Licencia actual: Plan </p> 
   O
   <p>Nueva licencia: Standard </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuración del nivel de acceso</td> 
   <td> <p>Editar el acceso a los proyectos con capacidad para crear y eliminar proyectos</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Editar acceso a Proyectos, Tareas, Problemas con la capacidad de Eliminar proyectos, tareas y problemas</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront. Para obtener más información sobre los requisitos de acceso, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

* Según la forma en que el administrador de Workfront configure las preferencias de eliminación de proyectos, tareas o problemas en las preferencias de plantilla de horas y horas de la instancia de Workfront, las horas registradas para las tareas, los problemas o el proyecto se gestionarán de una de las siguientes maneras al eliminar el proyecto:

   * Las horas permanecen en la hoja de horas como tiempo general.
   * Las horas se eliminan y se restaurarán si alguna vez se restaura el proyecto.

  Para obtener más información sobre la configuración de las preferencias de eliminación para los problemas de horas de sesión, consulte [Configurar preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Si el proyecto que elimina está vinculado a una iniciativa en el Scenario Planner de Workfront:

   * La iniciativa permanece en el plan, pero se elimina el vínculo al proyecto.
   * Si el proyecto que elimina está vinculado a la única iniciativa publicada de un plan, también se elimina la indicación de que el plan se ha publicado.
   * Si recupera un proyecto eliminado, el proyecto se recupera, pero su vínculo a la iniciativa no se restaura y el área del Planificador de escenarios ya no se muestra en Detalles del proyecto.

     El Scenario Planner requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte [Información general del Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

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
1. Haga clic en **Más** icono ![](assets/qs-more-menu.png) a la derecha del nombre del proyecto y haga clic en **Eliminar proyecto**.

   ![](assets/more-icon-expanded-delete-project-highlighted.png)

1. Clic **Sí, eliminarla**.

   El proyecto se elimina y se almacena en la papelera de reciclaje durante 30 días. El administrador de Workfront puede restaurarla desde la papelera de reciclaje durante este tiempo.

## Restauración de proyectos eliminados

Un administrador de sistema o de grupo puede restaurar proyectos en un plazo de 30 días después de haberlos eliminado, tal como se describe en el artículo [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
