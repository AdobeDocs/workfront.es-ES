---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre la fecha proyectada de finalización de proyectos, tareas y problemas
description: La fecha proyectada de finalización es un indicador calculado en tiempo real de cuándo se completará el proyecto, la tarea o el problema. Cuando el proyecto, tarea o problema se marca como Completado, la Fecha proyectada de finalización cambia a la fecha real de finalización.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: bac9856f3d0946b17e36797262d1a21f093ceadd
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Información general sobre la fecha proyectada de finalización de proyectos, tareas y problemas

La fecha proyectada de finalización es un indicador calculado en tiempo real de cuándo se completará el proyecto, la tarea o el problema. Cuando el proyecto, tarea o problema se marca como Completado, la Fecha proyectada de finalización cambia a la fecha real de finalización.

En las secciones siguientes se describe cómo se determina la fecha proyectada de finalización de los proyectos, las tareas y los problemas, y cómo localizarla.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Nuevo: 
   <ul><li><p>Un colaborador o superior para ver la fecha proyectada de finalización en un informe</p></li> <li><p>Licencia estándar para crear un informe</p></li> </ul>

<p>Actual: 
   <ul><li><p>Revise o suba para ver la fecha proyectada de finalización en un informe</p></li> 
   <li><p>Licencia de planificación para crear un informe</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización o superior a Proyectos</p> <p>Debe tener acceso de edición a informes, paneles y calendarios para crear un informe</p> <p>Debe tener acceso de edición a filtros, vistas y agrupaciones para crear un informe o modificar una vista de lista</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores a un proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Cómo determina Adobe Workfront la fecha proyectada de finalización

La fecha proyectada de finalización es un campo calculado y no se puede cambiar manualmente.

Los criterios utilizados para determinar la fecha proyectada de finalización difieren según el objeto que visualice:

* **Proyectos:** La fecha proyectada de finalización de los proyectos es igual a la fecha proyectada de finalización de la última tarea del proyecto.

  Por ejemplo, un porcentaje completado mayor acerca la fecha proyectada de finalización de la tarea al día actual. Si el estado de la tarea es Nuevo y la fecha planificada de finalización de la tarea está cerca o ha pasado, la fecha proyectada de finalización avanza más hacia el futuro.

* **Tareas:** La fecha proyectada de finalización de las tareas se determina según los siguientes criterios:

   * **Actualizaciones de progreso realizadas en la tarea por el usuario asignado de la tarea:** Las actualizaciones de progreso incluyen cambios en el porcentaje completado y cambios en el estado de la tarea.
   * **Fecha de confirmación:** Si el usuario asignado a la tarea especifica una Fecha de compromiso, la Fecha de finalización prevista cambia para coincidir con la Fecha de compromiso.

     Para obtener más información sobre las fechas de compromiso, consulte el artículo [Resumen de fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Predecesoras:** Si no hay retrasos en las tareas predecesoras, la fecha proyectada de finalización debe coincidir con la fecha planificada de finalización. A medida que se producen retrasos, las tareas dependientes muestran una Fecha proyectada de finalización mayor que la Fecha planificada de finalización.

     Para obtener más información sobre la Fecha planificada de finalización de las tareas, consulte [Información general sobre la fecha planificada de finalización de la tarea](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Cuando la tarea predecesora de una tarea tiene una Fecha real de finalización, las tareas dependientes reciben una Fecha proyectada de finalización como se describe en el siguiente escenario:
  >
  >
  >Si el proyecto tiene la Tarea A, la Tarea B y la Tarea C, y la Tarea B es la sucesora de la Tarea A, la Tarea C es la sucesora de la Tarea B y se agrega una Fecha de finalización real a la Tarea A, la Fecha proyectada de finalización se vuelve a calcular automáticamente para la Tarea B (siempre que la **Tipo de actualización** del proyecto se establece en automático y al cambiar), pero no se recalculará para la Tarea C. Actualmente, Workfront calcula la Fecha proyectada de finalización para las tareas que están un nivel por encima o por debajo de la Tarea actualizada, por motivos de rendimiento. 

* **Problemas:** La fecha proyectada de finalización del problema se ha establecido inicialmente para que coincida con la fecha planificada de finalización del problema.

  Si el usuario asignado del problema especifica una fecha de compromiso, tanto la fecha de finalización prevista como la fecha planificada de finalización cambian para coincidir con la fecha de compromiso.

  Para obtener más información sobre las fechas de compromiso, consulte el artículo [Resumen de fecha de confirmación](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Ver la fecha proyectada de finalización

En los informes puede ver la Fecha proyectada de finalización de proyectos, tareas y problemas. Puede ver la fecha proyectada de finalización de proyectos y tareas en otras áreas de Workfront.

### Ver la fecha proyectada de finalización de un proyecto {#view-the-projected-completion-date-of-a-project}

1. Vaya al proyecto en el que desea ver la fecha proyectada de finalización.
1. Clic **Detalles del proyecto** en el panel izquierdo.
1. Busque el **Fecha proyectada de finalización** en el campo **Información general** > **Fechas del proyecto** sección.

### Ver la fecha proyectada de finalización de una tarea {#view-the-projected-completion-date-of-a-task}

1. Vaya a la tarea en la que desea ver la Fecha proyectada de finalización.
1. Clic **Detalles de tarea** en el panel izquierdo.
1. Busque el **Fecha proyectada de finalización** en el campo **Información general** > **Fechas y restricciones de la tarea** sección.

### Ver la fecha proyectada de finalización de un problema {#view-the-projected-completion-date-of-an-issue}

La fecha proyectada de finalización de los problemas solo se puede ver en el informe de problemas o en la vista de lista. Crear una vista de lista es similar a crear la vista en un informe.

Para crear un informe de problemas que incluya la fecha proyectada de finalización:

1. Cree un informe de problemas, tal como se describe en el artículo [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Seleccione el **Columnas (vista)** pestaña.
1. Clic **Agregar columna** y empiece a escribir **Fecha proyectada de finalización** en el **Mostrar en esta columna:** field.

1. Selecciónelo cuando aparezca en la lista, bajo el icono **Problema** objeto. 
1. Haga clic en **Guardar + Cerrar**.

   El **Fecha proyectada de finalización** en el informe se rellena. 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
