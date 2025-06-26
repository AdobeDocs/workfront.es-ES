---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Ver horas reales
description: Las horas que inicie sesión en los elementos de trabajo en Adobe Workfront se consideran horas reales. Las horas reales representan el tiempo real que tardó en completar una tarea, un problema o un proyecto.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 04818bc054c3bab6e6208b6678365549664d1594
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 40%

---

# Ver horas reales

<!-- Audited: 5/2025 -->

Las horas que registre en sus elementos de trabajo en Adobe Workfront se consideran horas reales.

Las horas reales representan el tiempo real que tardó en completar una tarea, un problema o un proyecto.

Se recomienda registrar las horas en los elementos de trabajo, que son tareas y problemas. Sin embargo, como administrador de Workfront, puede permitir que los usuarios también registren tiempo en los proyectos según los flujos de trabajo de su organización.

Para obtener más información sobre cómo permitir que los usuarios registren tiempo en los proyectos, consulte [Configurar preferencias de plantilla de horas y de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
   <p>Nuevo: estándar<p>
   <p>O</p>
   <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a tareas, proyectos o problemas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores a una tarea, proyecto o problema</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Horas reales vs. Horas reales heredadas

Según el área de Workfront desde la que acceda a las horas reales, podrían hacer referencia a una de las siguientes horas registradas:

* En el proyecto, las tareas y los informes y listas de problemas:

   * **Horas reales**: Horas registradas para el proyecto, las tareas o los problemas después de mayo de 2021. Se almacenan en la base de datos de Workfront en horas y su campo de valor es `actualWorkRequiredDouble`.
   * **Horas reales heredadas**: Horas registradas para proyectos, tareas o problemas en cualquier momento, incluso antes de mayo de 2021. Se almacenan en la base de datos de Workfront en minutos y su campo de valor es `actualWorkRequired`. <!--check below and see if you need to add this to the API section - asked on the tech doc task -->

* En el área Detalles del proyecto, tarea o problema:

   * **Horas reales**: Horas registradas en proyectos, tareas o problemas en cualquier momento, incluso antes de mayo de 2021. Corresponden a las horas reales heredadas en informes y listas. Se almacenan en la base de datos de Workfront en minutos y su valor es `actualWorkRequired`.

## Horas reales en tareas y problemas frente a horas reales en proyectos

Las horas reales en tareas y problemas representan el número de horas registradas directamente en las tareas y problemas.

Las horas reales de las tareas secundarias se transfieren a las horas reales de la tarea principal. La siguiente fórmula se aplica a las horas reales de una tarea principal:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Horas reales para proyectos representa un total de horas reales de todas las tareas del proyecto (incluidas las horas registradas directamente en las tareas principales), todos los problemas del proyecto y las horas reales registradas en el propio proyecto.

La siguiente fórmula se aplica a las horas reales de un proyecto:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Buscar horas reales

Encontrar el valor de las horas reales para un elemento es idéntico para tareas, proyectos y problemas.

### Horas reales en la sección Detalles {#actual-hours-in-the-details-section}

Buscar las horas reales en la sección Detalles es idéntico para proyectos, tareas y problemas.

Para localizar las horas reales en los detalles de la tarea:

1. Vaya a una tarea para la que desee revisar las horas reales.
1. En el panel izquierdo, haga clic en **Detalles de la tarea**. Se muestra la sección **Información general**.
1. Busque el valor **Horas reales** en la sección **Tiempo de trabajo**. Este es el total de horas registradas en esta tarea.

### Horas reales en la sección Horas {#actual-hours-in-the-hours-section}

Buscar las horas reales en la sección Horas es idéntico para proyectos, tareas y problemas.

Para localizar las horas reales en la sección Horas:

1. Vaya a una tarea para la que desee revisar las horas reales.

1. En el panel izquierdo, haga clic en **Horas**. Se muestra una lista de las entradas de horas registradas en la tarea, con la columna **Horas** que muestra el número total de horas reales para la tarea.

1. Asegúrese de que la vista **Estándar** y la agrupación **Proyecto** se hayan aplicado a esta lista.

### Horas reales en los informes {#actual-hours-in-reports}

Al generar informes sobre tareas, problemas o proyectos, puede mostrar el valor de Horas reales de cada tarea, problema o proyecto en el informe.

Para mostrar las horas reales en un informe de tareas:

{{step1-to-reports}}

1. En la página **Informes**, haga clic en **Nuevo informe** y, a continuación, elija **Tarea** como objeto.
1. En la esquina inferior derecha de la página, haga clic en **Agregar columna**.
1. En el campo desplegable **Mostrar en esta columna** que aparece, empiece a escribir **Horas reales** y, a continuación, seleccione el campo cuando aparezca en la lista.

1. En la esquina inferior izquierda de la página, haga clic en **Guardar + Cerrar** para guardar el informe.

1. En el cuadro de diálogo **Asigne un nombre a este informe para guardarlo**, escriba un nuevo nombre para el informe y haga clic en **Aplicar**.

### Horas reales en las herramientas de administración de recursos {#actual-hours-in-resource-management-tools}

Si desea ver el progreso del trabajo que los usuarios están realizando en las tareas y problemas que se les han asignado, puede consultarlo en las siguientes herramientas de Administración de recursos:

* El Informe De Utilización.\
  Para obtener más información, consulte [Información general sobre el informe de utilización de recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* El Planificador de recursos.

  Para obtener más información, vea [Ver horas disponibles, planificadas y reales o FTE en el Planificador de recursos al usar la vista de usuario](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Horas reales en la API de Workfront

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

La mayoría de los campos de Workfront que almacenan horas se guardan en la base de datos de Workfront en minutos. Por ejemplo, el nombre del campo Horas planificadas de una tarea es `workRequired` en la base de datos de Workfront y se almacena en minutos.

Debe tener en cuenta la conversión de minutos a horas al acceder a estos campos en llamadas API o en campos o columnas personalizados calculados.

Las horas reales registradas para proyectos, tareas o problemas se almacenan actualmente en la base de datos de Workfront como minutos y su valor es `actualWorkRequired`.

Con la siguiente versión de la API de Workfront programada para su lanzamiento para finales de 2025, según cómo acceda a Horas reales, se pueden almacenar en los siguientes campos y unidades de la base de datos:

* **Horas reales**: Horas registradas para el proyecto, las tareas o los problemas después de mayo de 2021. Se almacenan en la base de datos de Workfront en horas y su campo de valor es `actualWorkRequiredDouble`.

* **Horas reales heredadas**: Horas registradas para proyectos, tareas o problemas en cualquier momento, incluso antes de mayo de 2021. Se almacenan en la base de datos de Workfront en minutos y su valor es `actualWorkRequired`.

Para obtener información sobre cómo usar las horas reales en columnas o campos calculados, consulte [Preguntas más frecuentes sobre informes](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Hora de registro

Puede registrar tiempo en tareas, problemas y proyectos de varias formas.

Para obtener más información, consulte [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).
