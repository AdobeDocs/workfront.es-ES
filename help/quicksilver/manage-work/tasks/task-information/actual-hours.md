---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Ver horas reales
description: Las horas que inicie sesión en los elementos de trabajo en Adobe Workfront se consideran horas reales. Las horas reales representan el tiempo real que tardó en completar una tarea, un problema o un proyecto.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 27%

---

# Ver horas reales

<!-- Audited: 5/2025 -->

Las horas que registre en sus elementos de trabajo en Adobe Workfront se consideran horas reales.

Las horas reales representan el tiempo real que tardó en completar una tarea, un problema o un proyecto.

Se recomienda registrar las horas en los elementos de trabajo, que son tareas y problemas. Sin embargo, como administrador de Workfront, puede permitir que los usuarios también registren tiempo en los proyectos según los flujos de trabajo de su organización.

Para obtener más información sobre cómo permitir que los usuarios registren tiempo en los proyectos, consulte [Configurar preferencias de plantilla de horas y de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Estándar<p>
   <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Ver o aumentar el acceso a Tareas, Proyectos o Problemas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores a una tarea, proyecto o problema</p></td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks, Projects, or Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a task, a project, or an issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Horas reales vs. Horas reales heredadas

Según el área de Workfront desde la que acceda a las horas reales, podrían hacer referencia a una de las siguientes horas registradas:

* En el proyecto, las tareas y los informes y listas de problemas:

   * **Horas reales**: Horas registradas para el proyecto, las tareas o los problemas entre mayo de 2021 y hoy. Se almacenan en la base de datos de Workfront en horas y su campo de valor es `actualWorkRequiredDouble`.
   * **Horas reales heredadas**: Horas registradas para proyectos, tareas o problemas en cualquier momento, entre cualquier fecha anterior a mayo de 2021 y hoy. Se almacenan en la base de datos de Workfront en minutos y su valor es `actualWorkRequired`.

     Las horas registradas actualmente actualizarán las horas reales y las horas reales heredadas.

     >[!IMPORTANT]
     >
     >El costo real del proyecto utiliza las horas reales heredadas para calcular.

* En el área de detalles del proyecto, tarea o problema, las horas reales se podrían mostrar en los siguientes campos:

   * **Horas reales**: en la ficha Detalles, se trata de horas registradas en proyectos, tareas o problemas entre mayo de 2021 y hoy. Se almacenan en la base de datos de Workfront en horas y su campo de valor es `actualWorkRequiredDouble`.
   * **Horas reales**: en un formulario personalizado de proyecto, tarea o problema, cuando se accede a ellas mediante un campo personalizado de referencia de campo nativo que hace referencia al campo nativo Horas reales. Son horas registradas en proyectos, tareas o problemas entre cualquier fecha anterior a mayo de 2021 y la fecha actual. Se almacenan en la base de datos de Workfront en horas y su campo de valor es `actualWorkRequiredDouble`.

     Las horas registradas actualmente actualizarán las horas reales y las horas reales heredadas.

>[!NOTE]
>
>Se recomienda utilizar el campo Horas reales siempre que sea posible, ya que el campo Horas reales heredadas podría mostrar horas imprecisas debido a la forma en que se redondean los incrementos cuando las horas se almacenan en minutos.

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
1. (Opcional y condicional) Si la referencia del campo nativo Horas reales se agregó a un formulario personalizado de proyecto, tarea o problema, vaya al formulario personalizado y busque las Horas reales en el campo personalizado. Es el total de horas registradas para el objeto.

### Horas reales en la sección Horas {#actual-hours-in-the-hours-section}

Buscar las horas reales en la sección Horas es idéntico para proyectos, tareas y problemas.

Para localizar las horas reales en la sección Horas de una tarea:

1. Vaya a una tarea para la que desee revisar las horas reales.

1. En el panel izquierdo, haga clic en **Horas**. Se muestra una lista de las entradas de horas registradas en la tarea, con la columna **Horas** que muestra el número total de horas reales para la tarea.

1. Asegúrese de que la vista **Estándar** y la agrupación **Proyecto** se hayan aplicado a esta lista.
1. Las horas reales de la tarea se mostrarán en la línea de agrupación de la columna **Horas reales**.

### Horas reales y Horas reales heredadas en los informes

Al generar informes sobre tareas, problemas o proyectos, puede mostrar en el informe los valores de Horas reales y Horas reales heredadas para cada tarea, problema o proyecto.

Para obtener información sobre la diferencia entre las horas reales y las horas reales heredadas, consulte la sección [Horas reales vs. horas reales heredadas](#actual-hours-vs-legacy-actual-hours) en este artículo.

Para mostrar las horas reales y las horas reales heredadas en un informe de tareas:

{{step1-to-reports}}

1. En la página **Informes**, haga clic en **Nuevo informe** y, a continuación, elija **Tarea** como objeto.
1. En la esquina inferior derecha de la página, haga clic en **Agregar columna**.
1. En el campo desplegable **Mostrar en esta columna**, empiece a escribir **Horas reales** y, a continuación, seleccione el campo cuando aparezca en la lista.
1. Repita el paso anterior para agregar el campo **Horas reales heredadas** al informe.

1. En la esquina inferior izquierda de la página, haga clic en **Guardar + Cerrar** para guardar el informe.

1. En el cuadro de diálogo **Asigne un nombre a este informe para guardarlo**, escriba un nuevo nombre para el informe y haga clic en **Aplicar**.
1. Repita los mismos pasos para un proyecto o informe de problemas.

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

Con la siguiente versión de la API de Workfront programada para su lanzamiento para finales de 2025, las horas reales se almacenan en los siguientes campos y unidades de la base de datos:

* **Horas reales**: Horas registradas para el proyecto, las tareas o los problemas después de mayo de 2021. Se almacenan en la base de datos de Workfront en horas y su campo de valor es `actualWorkRequiredDouble`.
* **Horas reales heredadas**: Horas registradas para proyectos, tareas o problemas en cualquier momento, incluso antes de mayo de 2021. Se almacenan en la base de datos de Workfront en minutos y su valor es `actualWorkRequired`.

Para obtener información sobre las versiones de API, consulte [Versiones de API y programación de soporte](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>El costo real del proyecto utiliza las horas reales heredadas para calcular.

Para obtener información sobre cómo usar las horas reales en columnas o campos calculados, consulte [Preguntas más frecuentes sobre informes](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Hora de registro

Puede registrar tiempo en tareas, problemas y proyectos de varias formas.

Para obtener más información, consulte [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).
