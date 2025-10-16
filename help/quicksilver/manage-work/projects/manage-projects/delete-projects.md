---
title: Eliminar proyectos
product-area: projects
navigation-topic: manage-projects
description: Puede eliminar un proyecto si el proyecto y sus datos ya no son necesarios. Como alternativa a eliminar un proyecto, recomendamos editar el proyecto y cambiar el estado a Completado o Inactivo. Todas las tareas actuales relacionadas con el proyecto se quitarán de la lista de tareas de un usuario pero se guardarán todos los datos asociados con dicho proyecto.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 94%

---

# Eliminar proyectos

<!--Audited: 07/2024-->

Puede eliminar un proyecto si el proyecto y sus datos ya no son necesarios.

Como alternativa a eliminar un proyecto, recomendamos editar el proyecto y cambiar el estado a Completado o Inactivo. Todas las tareas actuales relacionadas con el proyecto se quitarán de la lista de tareas de un usuario pero se guardarán todos los datos asociados con dicho proyecto.

Puede eliminar un proyecto en una lista de proyectos o a nivel de proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>paquete de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront</p> </td> 
   <td> <p>Estándar</p>
   <p>Plan</p> 
   </td> 
  </tr> 
    <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a los proyectos con la posibilidad de crear y eliminar proyectos</p> </td> 
  </tr> 
    <td> <p>Permisos de objeto</p> </td> 
   <td> <p>Acceso de edición a proyectos, tareas, problemas con la posibilidad de eliminar proyectos, tareas y problemas</p> </td> 
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
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>New license: Standard </p>
   <p>Current license: Plan </p> 
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configuration</td> 
   <td> <p>Edit access to Projects with ability to Create and Delete projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Comprender el proceso de eliminación de proyectos

* [Limitaciones para eliminar proyectos](#limitations-for-deleting-projects)
* [Impacto de la eliminación de proyectos](#the-impact-of-deleting-projects)

### Limitaciones para eliminar proyectos  {#limitations-for-deleting-projects}

* Los elementos eliminados se moverán a la papelera de reciclaje durante 30 días y solamente el administrador del sistema los puede recuperar.

  Para obtener más información sobre cómo restaurar objetos, consulte el artículo [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Si el proyecto tiene tareas o problemas con las horas registradas, el administrador de grupos o de Workfront debe permitir la eliminación de estas tareas configurando las Preferencias de tareas y problemas en la instancia de Workfront para que pueda eliminar el proyecto que contiene las tareas.

  Para obtener más información sobre cómo habilitar la eliminación de tareas, problemas o proyectos en los que se registran horas, consulte la sección “Eliminación” en [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Impacto de la eliminación de proyectos {#the-impact-of-deleting-projects}

* Al eliminar un proyecto, se ven afectados otros objetos vinculados al proyecto.

  Los siguientes objetos adjuntos a un proyecto también se eliminan cuando se elimina un proyecto:

   * Documentos

     No se puede eliminar un proyecto que tenga un documento adjunto que se haya desprotegido. Para obtener más información sobre cómo desproteger documentos, consulte [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

   * Tareas
   * Subtareas
   * Problemas
   * Actualizaciones
   * Rutas de aprobación
   * Gastos
   * Riesgos
   * Líneas base
   * Información del caso empresarial
   * Información de los detalles de cola
   * Tarifas de facturación
   * Registros de facturación

     No puede eliminar un proyecto que tenga registros de facturación con un estado Facturado. Para obtener más información, consulte [Crear registros de facturación](../../projects/project-finances/create-billing-records.md).

* Según la forma en que el administrador de Workfront haya configurado las preferencias de eliminación de proyectos, tareas o problemas en las preferencias de plantilla de horas y horas de la instancia de Workfront, las horas registradas para las tareas, los problemas o el proyecto se gestionarán de una de las siguientes maneras al eliminar el proyecto:

   * Las horas permanecen en la plantilla de horas como tiempo general.
   * Las horas se eliminan y se restaurarán si el proyecto se restaurara en algún momento.

  Para obtener más información sobre cómo configurar las preferencias de eliminación para las horas registradas para los problemas, consulte [Configurar preferencias de plantilla de horas y de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Si el proyecto que elimina está vinculado a una iniciativa en el Planificador de escenarios de Workfront:

   * La iniciativa permanece en el plan, pero se elimina el vínculo al proyecto.
   * Si el proyecto que elimina está vinculado a la única iniciativa publicada de un plan, también se elimina la indicación de que el plan se ha publicado.
   * Si recupera un proyecto eliminado, el proyecto se recupera, pero su vínculo a la iniciativa no se restaura y el área del Planificador de escenarios ya no se muestra en Detalles del proyecto.

     El Planificador de escenarios requiere una licencia adicional. Para obtener información sobre el Planificador de escenarios de Workfront, consulte [Información general sobre el Planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md).

     Para obtener información sobre los proyectos vinculados a iniciativas en el Planificador de escenarios, consulte [Actualizar o crear proyectos mediante la publicación de iniciativas en el Planificador de escenarios](../../../scenario-planner/publish-scenarios-update-projects.md).

* Si el proyecto también es una actividad para una meta de Workfront Goals:

   * El proyecto se elimina de la meta. También se quita el progreso indicado en la meta por el proyecto.

   * Si recupera el proyecto eliminado, este también se restaurará como la actividad de la meta.

     Se requiere una licencia adicional. Para obtener información sobre Workfront Goals, consulte [Información general sobre Adobe Workfront Goals](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Para obtener información sobre cómo asociar los proyectos con las metas, consulte [Añadir proyectos a metas en Adobe Workfront Goals](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Eliminación de un proyecto de una lista

Puede eliminar proyectos de una lista de proyectos.

1. Ir a una lista de proyectos o a un informe de proyecto.
1. Seleccione el proyecto o proyectos que desee eliminar y, a continuación, haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete-icon.png) de la parte superior de la lista.

1. Haga clic en **Sí, eliminar** para confirmar la eliminación.

   Los proyectos se eliminan y se almacenan en la Papelera de reciclaje durante 30 días. El administrador de Workfront puede restaurar los proyectos eliminados de la Papelera de reciclaje durante este tiempo.

## Eliminación de un proyecto en el nivel de proyecto

1. Vaya al proyecto que desee eliminar.
1. Haga clic en el icono **Más** ![Menú más](assets/qs-more-menu.png) a la derecha del nombre del proyecto y, a continuación, haga clic en **Eliminar proyecto**.

   ![Menú más expandido](assets/more-icon-expanded-delete-project-highlighted.png)

1. Haga clic en **Sí, eliminar**.

   El proyecto se elimina y se almacena en la Papelera de reciclaje durante 30 días. El administrador de Workfront puede restaurarlo de la Papelera de reciclaje durante este tiempo.

## Restauración de proyectos eliminados

Un administrador de sistema o de grupos puede restaurar proyectos durante los 30 días posteriores a su eliminación, como se describe en el artículo [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
