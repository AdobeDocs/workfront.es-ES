---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Ver horas reales
description: Las horas que inicie sesión en los elementos de trabajo en Adobe Workfront se consideran horas reales.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Ver horas reales

Las horas que inicie sesión en los elementos de trabajo en Adobe Workfront se consideran horas reales.

Las horas reales representan el tiempo real que tardó en completar una tarea, un problema o un proyecto.

Se recomienda registrar las horas en los elementos de trabajo, que son tareas y problemas.

Sin embargo, como administrador de Workfront, también puede permitir que los usuarios registren tiempo en los proyectos, según los flujos de trabajo de su organización.

Para obtener más información sobre cómo configurar el sistema para que los usuarios puedan registrar tiempo en los proyectos, consulte [Configurar las preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Ver o aumentar el acceso a Tareas, Proyectos o Problemas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o aumentar los permisos de una tarea, un proyecto o un problema</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Horas reales en tareas y problemas vs. Horas reales en proyectos

Las Horas reales en tareas y problemas representan el número de horas registradas directamente en las tareas y problemas.

>[!NOTE]
>
>Horas reales de tareas secundarias acumuladas a las horas reales de la tarea principal. La siguiente fórmula se aplica a las horas reales de una tarea principal:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Horas reales para proyectos representa un total de horas reales de todas las tareas del proyecto (incluidas las horas registradas directamente en las tareas principales), todos los problemas del proyecto y las horas reales registradas en el propio proyecto.

La siguiente fórmula se aplica a las horas reales de un proyecto:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Buscar horas reales

Encontrar el valor de Horas reales para un elemento es idéntico para tareas, proyectos y problemas.

Puede encontrar la información de Horas reales sobre las tareas en las siguientes ubicaciones:

* [Horas reales en la sección Detalles](#actual-hours-in-the-details-section)
* [Horas reales en la sección Horas](#actual-hours-in-the-hours-section)
* [Horas reales en los informes](#actual-hours-in-reports)
* [Horas reales en las herramientas de administración de recursos](#actual-hours-in-resource-management-tools)

### Horas reales en la sección Detalles {#actual-hours-in-the-details-section}

Buscar horas reales en la sección Detalles es idéntico en proyectos, tareas y problemas.

Para localizar las horas reales en los detalles de la tarea:

1. Vaya a una tarea para la que desee revisar las horas reales.
1. Haga clic en **Detalles de la tarea** en el panel izquierdo.
1. Haga clic en **Información general** y observe el valor de **Horas reales**.

   Este es el total de horas registradas en esta tarea.

### Horas reales en la sección Horas {#actual-hours-in-the-hours-section}

Buscar horas reales en la sección Horas es idéntico para proyectos, tareas y problemas.

Para localizar las horas reales en la sección Horas

1. Vaya a una tarea para la que desee revisar las horas reales.
1. Haga clic en **Horas** en el panel izquierdo.

   Según la configuración, la sección Horas podría aparecer en **Mostrar más**.

   Muestra una lista de entradas de horas registradas en la tarea.

1. Asegúrese de que la vista **Standard** y la agrupación **Project** se hayan aplicado a esta lista.

   El número que se muestra en la línea de agrupación de la columna **Horas** es el número total de horas reales en la tarea.

### Horas reales en los informes {#actual-hours-in-reports}

Al generar informes sobre tareas, problemas o proyectos, puede mostrar el valor de Horas reales de cada tarea, problema o proyecto en el informe.

Agregar la columna Horas reales a una vista de tareas es similar a crear una vista en un informe.

Para mostrar las horas reales en un informe de tareas:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront y luego haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, elija **Tarea** como objeto.

1. Haga clic en **Agregar columna** y empiece a escribir **Horas reales** cuando se muestre el campo desplegable **Mostrar en esta columna**. Seleccione el campo cuando aparezca en la lista.

1. Haga clic en **Guardar + Cerrar** para guardar el informe.

   La columna Horas reales muestra el número de horas registradas en cada tarea.

### Horas reales en las herramientas de administración de recursos {#actual-hours-in-resource-management-tools}

Si desea ver el progreso del trabajo que los usuarios están realizando en las tareas y problemas que se les han asignado, puede verlos en las siguientes herramientas de Administración de recursos:

* Informe de utilización.\
  Para obtener información sobre el informe de utilización, consulte [Información general sobre el informe de utilización de recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Planificador de recursos.

  Para obtener información sobre cómo ver las horas reales en el Planificador de recursos, consulte [Ver horas disponibles, planificadas y reales o FTE en el Planificador de recursos al usar la vista de usuario](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Hora de registro

Puede registrar tiempo en tareas, problemas y proyectos de varias formas.

Para obtener más información sobre cómo registrar el tiempo en Workfront, consulte [Registrar el tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).
