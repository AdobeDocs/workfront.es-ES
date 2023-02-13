---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre la fecha de finalización prevista para proyectos, tareas y problemas
description: La fecha de finalización prevista es un indicador calculado en tiempo real de cuándo se completará el proyecto, la tarea o el problema. Cuando el proyecto, la tarea o el problema se marcan como Finalizado, la Fecha de Finalización Prevista cambia a la fecha de la Fecha de Finalización Real.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Información general sobre la fecha de finalización prevista para proyectos, tareas y problemas

La fecha de finalización prevista es un indicador calculado en tiempo real de cuándo se completará el proyecto, la tarea o el problema. Cuando el proyecto, la tarea o el problema se marcan como Finalizado, la Fecha de Finalización Prevista cambia a la fecha de la Fecha de Finalización Real.

Las secciones siguientes describen cómo se determina la fecha de finalización prevista para proyectos, tareas y problemas, y cómo localizarla.

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
   <td> 
   <p>For current licenses: 
   <ul><li><p>Contributor or higher to view the Projected Completion Date in a report</p></li> <li><p>A Standard license to create a report</p></li> </ul>
   
   <p>For legacy licenses: 
   <ul><li><p>Review or higher to view the Projected Completion Date in a report</p></li> 
   <li><p>A Plan license to create a report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>You must have Edit access to Reports, Dashboards, Calendars to create a report</p> <p>You must have Edit access to Filters, Views, Groupings to create a report or modify a list view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Revise o superior para ver la Fecha de finalización prevista en un informe</p> <p>Una licencia de plan para crear un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver o acceder más a Proyectos</p> <p>Debe tener acceso de edición a informes, tableros y calendarios para crear un informe</p> <p>Debe tener acceso de edición a filtros, vistas y agrupamientos para crear un informe o modificar una vista de lista</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores de un proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Cómo determina Adobe Workfront la fecha de finalización prevista

La fecha de finalización prevista es un campo calculado y no se puede cambiar manualmente.

Los criterios utilizados para determinar la fecha de finalización prevista difieren, según el objeto que esté viendo:

* **Proyectos:** La fecha de finalización prevista para los proyectos es igual a la fecha de finalización prevista de la última tarea del proyecto.
* **Tareas:** La fecha de finalización prevista para las tareas se determina según los siguientes criterios:

   * **Actualizaciones de progreso realizadas en la tarea por el usuario asignado de la tarea:** Las actualizaciones de progreso incluyen cambios en el porcentaje de finalización y cambios en el estado de la tarea.
   * **Fecha de confirmación:** Si el usuario asignado de la tarea especifica una fecha de finalización, la fecha de finalización prevista cambia para coincidir con la fecha de finalización.

      Para obtener más información sobre fechas de confirmación, consulte el artículo [Resumen de la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Predecesores:** Si no hay retrasos en las tareas predecesoras, la fecha de finalización prevista debe coincidir con la fecha de finalización planificada. A medida que se producen retrasos, las tareas dependientes muestran una Fecha de finalización prevista buena a la Fecha de finalización planeada.

      Para obtener más información sobre la fecha de finalización prevista de las tareas, consulte [Descripción general de la tarea Fecha de finalización planificada](../../../manage-work/tasks/task-information/task-planned-completion-date.md).
   >[!IMPORTANT]
   >
   >Cuando el predecesor de una tarea tiene una Fecha de Finalización Real, las tareas dependientes reciben una Fecha de Finalización Prevista como se describe en el siguiente escenario:
   >
   >
   >Si el proyecto tiene la tarea A, la tarea B y la tarea C, y la tarea B es la sucesora de la tarea A, la tarea C es la sucesora de la tarea B y se añade una fecha de finalización real a la tarea A, la fecha de finalización prevista se vuelve a calcular automáticamente para la tarea B (siempre que la tarea B se vuelva a calcular) **Tipo de actualización** del proyecto está establecido en Automático y En Cambio), pero no se volverá a calcular para la Tarea C. Actualmente, Workfront calcula la fecha de finalización prevista para las tareas que están un nivel más arriba o más abajo que la Tarea actualizada, por motivos de rendimiento. 

* **Problemas:**el problema Fecha de finalización prevista se configura inicialmente para que coincida con el problema Fecha de finalización planeada.

   Si el usuario asignado del problema especifica una fecha de confirmación, tanto la Fecha de finalización prevista como la Fecha de finalización planeada cambiarán para coincidir con la Fecha de finalización.

   Para obtener más información sobre fechas de confirmación, consulte el artículo [Resumen de la fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Ver la fecha de finalización prevista

Puede ver en los informes la fecha de finalización prevista de los proyectos, las tareas y los problemas. Puede ver la Fecha de finalización prevista de los proyectos y tareas en otras áreas de Workfront. 

* [Ver la fecha de finalización prevista de un proyecto](#view-the-projected-completion-date-of-a-project)
* [Ver la fecha de finalización prevista de una tarea](#view-the-projected-completion-date-of-a-task)
* [Ver la fecha de finalización prevista de un problema](#view-the-projected-completion-date-of-an-issue)

### Ver la fecha de finalización prevista de un proyecto {#view-the-projected-completion-date-of-a-project}

1. Vaya al proyecto en el que desea ver la fecha de finalización prevista.
1. Haga clic en **Detalles del proyecto** en el panel izquierdo.
1. Busque la variable **Fecha de finalización prevista** en el campo **Información general** para obtener más información.

### Ver la fecha de finalización prevista de una tarea {#view-the-projected-completion-date-of-a-task}

1. Vaya a la tarea donde desee ver la fecha de finalización prevista.
1. Haga clic en **Detalles de la tarea** en el panel izquierdo.
1. Busque la variable **Fecha de finalización prevista** en el campo **Información general** para obtener más información.

### Ver la fecha de finalización prevista de un problema {#view-the-projected-completion-date-of-an-issue}

Puede ver la fecha de finalización prevista para los problemas únicamente en un informe de problemas o en una vista de lista. Crear una vista de lista es similar a crear la vista en un informe.

Para crear un informe de problemas que incluya la fecha de finalización prevista:

1. Cree un informe de problemas, tal como se describe en el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Seleccione el **Columnas (Vista)** pestaña .
1. Haga clic en **Agregar columna** y empiece a escribir **Fecha de finalización prevista** en el **Mostrar en esta columna:** campo .

1. Selecciónela cuando aparezca en la lista, en la sección **Problema** objeto. 
1. Haga clic en **Guardar + Cerrar**.

   La variable **Fecha de finalización prevista** en el informe se rellena. 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
