---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Ver horas reales
description: Las horas en las que inicia sesión en los elementos de trabajo en Adobe Workfront se consideran horas reales.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Ver horas reales

Las horas en las que inicia sesión en los elementos de trabajo en Adobe Workfront se consideran horas reales.

Las horas reales representan el tiempo real que se tardó en completar una tarea, un problema o un proyecto.

Recomendamos que las horas se registren en elementos de trabajo, que son tareas y problemas.

Sin embargo, como administrador de Workfront, también puede permitir que los usuarios inicien sesión en los proyectos, en función de los flujos de trabajo de su organización.

Para obtener más información sobre cómo configurar el sistema para permitir que los usuarios inicien sesión en los proyectos, consulte [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Requisitos de acceso

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
   <td> <p>Ver o tener más acceso a Tareas, Proyectos o Problemas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores de una tarea, un proyecto o un problema</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Horas reales en tareas y problemas frente a horas reales en proyectos

Las horas reales en tareas y problemas representan el número de horas registradas directamente en las tareas y los problemas.

>[!NOTE]
>
>Las horas reales de las tareas secundarias se acumulan hasta las horas reales en la tarea principal. La siguiente fórmula se aplica para las horas reales en una tarea principal:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Las horas reales para los proyectos representan un total de horas reales de todas las tareas del proyecto (incluidas las horas registradas directamente en las tareas principales), todos los problemas del proyecto y las horas reales registradas en el propio proyecto.

La siguiente fórmula se aplica para las horas reales de un proyecto:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Buscar horas reales

Encontrar el valor de horas reales para un artículo es idéntico para tareas, proyectos y problemas.

Puede encontrar la información Horario real sobre las tareas en las siguientes ubicaciones:

* [Horas reales en la sección Detalles](#actual-hours-in-the-details-section)
* [Horas reales en la sección Horas](#actual-hours-in-the-hours-section)
* [Horas reales en los informes](#actual-hours-in-reports)
* [Horas reales en las herramientas de administración de recursos](#actual-hours-in-resource-management-tools)

### Horas reales en la sección Detalles {#actual-hours-in-the-details-section}

La búsqueda de horas reales en la sección Detalles es idéntica para proyectos, tareas y problemas.

Para localizar horas reales en Detalles de la tarea:

1. Vaya a una tarea para la que desee revisar las horas reales.
1. Haga clic en **Detalles de la tarea** en el panel izquierdo.
1. Haga clic en **Información general** y observe la **Horas reales** valor.

   Es el total de horas registradas en esta tarea.

### Horas reales en la sección Horas {#actual-hours-in-the-hours-section}

La búsqueda de horas reales en la sección Horas es idéntica para proyectos, tareas y problemas.

Para localizar las horas reales en la sección Horas :

1. Vaya a una tarea para la que desee revisar las horas reales.
1. Haga clic en **Horas** en el panel izquierdo.

   Según la configuración, la sección Horas podría aparecer en **Mostrar más**.

   Esto muestra una lista de entradas de hora registradas en la tarea.

1. Asegúrese de que la variable **Estándar** y **Proyecto** se aplican a esta lista.

   El número que se muestra en la línea de agrupación para la variable **Horas** es el número total de horas reales en la tarea.

### Horas reales en los informes {#actual-hours-in-reports}

Al crear informes de tareas, problemas o proyectos, puede mostrar el valor de horas reales para cada tarea, problema o proyecto en el informe.

Añadir la columna Horas reales a una vista de tareas es similar a generar una vista en un informe.

Para mostrar horas reales en un informe de tareas:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, elija **Tarea** como objeto.

1. Haga clic en **Agregar columna** y empiece a escribir **Horas reales** cuando la variable **Mostrar en esta columna** se muestra el campo desplegable . Seleccione el campo cuando aparezca en la lista.

1. Haga clic en **Guardar + Cerrar** para guardar el informe.

   La columna Hora real muestra el número de horas registradas en cada tarea.

### Horas reales en las herramientas de administración de recursos {#actual-hours-in-resource-management-tools}

Si desea ver el progreso del trabajo que los usuarios están realizando en sus tareas y problemas asignados, puede verlo en las siguientes herramientas de Administración de recursos:

* Informe de uso.\
   Para obtener información sobre el informe de utilización, consulte [Resumen del informe de Utilización de Recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Planificador de recursos.

   Para obtener información sobre la visualización de horas reales en el planificador de recursos, consulte [Ver las horas disponibles, planificadas y reales o FTE en el Planificador de recursos al utilizar la vista Usuario](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Tiempo de registro

Puede iniciar sesión en tareas, problemas y proyectos de varias formas.

Para obtener más información sobre cómo iniciar sesión en Workfront, consulte [Tiempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).
