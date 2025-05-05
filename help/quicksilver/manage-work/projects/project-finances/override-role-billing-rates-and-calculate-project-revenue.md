---
product-area: projects
navigation-topic: financials
title: Visión General de Sustitución de Tasas de Facturación de Rol y Cálculo de Ingresos en un Proyecto
description: Puede utilizar tarifas de facturación para calcular los ingresos de sus proyectos cuando los multiplique por las horas invertidas en el proyecto. Para obtener más información sobre las tarifas de facturación y los ingresos, consulte el artículo Información general sobre facturación e ingresos.
author: Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '3860'
ht-degree: 99%

---

# Información general sobre cómo anular las tarifas de facturación de funciones y calcular los ingresos en un proyecto

{{highlighted-preview}}

Puede utilizar tarifas de facturación para calcular los ingresos de sus proyectos cuando los multiplique por las horas invertidas en el proyecto. Para obtener más información sobre las tarifas de facturación y los ingresos, consulte el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
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
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## Visión general de tarifas de facturación de funciones y tipos de ingresos de rol por hora

Como administrador de Adobe Workfront, puede asociar las tarifas de facturación tanto con los usuarios como con las funciones.\
Para obtener más información sobre cómo crear usuarios y asociarlos con tarifas de facturación, consulte el artículo [Añadir usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Para obtener más información sobre cómo crear funciones y asociarlas con tarifas de facturación, consulte el artículo [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Las tarifas de facturación asociadas con los usuarios no se pueden anular.

Las tarifas de facturación asociadas con las funciones de trabajo se pueden anular a nivel de compañía o proyecto.

Para calcular los ingresos de los proyectos en función de las tarifas de facturación de las funciones de trabajo, el **Tipo de ingresos** de las tareas de los proyectos debe ser uno de los siguientes:

* Rol por hora
* Rol por hora con límite
* Rol por hora más fijos

Para obtener más información sobre **Tipo de ingresos** y tarifas de facturación, consulte [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## La jerarquía de tarifa de facturación se anula al calcular ingresos

Una función puede tener asociada una tarifa de facturación de las siguientes maneras:

* Como administrador de Workfront, puede definir la tarifa de facturación a nivel del sistema asociada con una función de trabajo al crear dicha función.\
  Para obtener más información sobre cómo crear funciones, consulte [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Como administrador de Workfront, puede definir la tarifa de facturación a nivel de compañía para la misma función de trabajo al crear una compañía.\
  Cuando Workfront calcula los ingresos de los proyectos asociados con esta compañía, la tarifa de facturación de la compañía se utiliza cuando la función se asigna a tareas, en lugar de la tarifa de facturación del sistema para esta función de trabajo.\
  Las tarifas de funciones cambiadas a nivel de compañía afectarán a todos los proyectos asociados con esa compañía.

  >[!NOTE]
  >
  >Si necesita actualizar la tarifa de facturación de la compañía, la tarifa del proyecto no se actualizará automáticamente. Debe quitar la compañía del proyecto, actualizar la tarifa de la compañía y, a continuación, volver a adjuntar la compañía al proyecto antes de que la nueva tarifa de compañía surta efecto en el proyecto. Para obtener instrucciones sobre cómo adjuntar una compañía a un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

  Para obtener más información sobre cómo crear tarifas de facturación de funciones específicas de una compañía, consulte [Crear y editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Como administrador de Workfront, puede habilitar una opción al editar un proyecto para aplicar cambios en las tarifas de facturación a nivel de compañía en el proyecto cuando los usuarios recalculen manualmente las finanzas de un proyecto.\
  Para obtener más información, [Anular las tarifas de facturación a nivel de proyecto con las tarifas de facturación a nivel de compañía](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* Como administrador de Workfront, puede definir tarjetas de tarifas con varias tarifas de facturación por función, según la ubicación y la fecha. Cuando se adjunta una tarjeta de tarifas a un proyecto, todas las funciones (por ubicación, si se utilizan ubicaciones) y sus tarifas de facturación asociadas se añaden a la sección de tarifas de facturación del proyecto. Al adjuntar una tarjeta de tarifas, se anulan las tarifas de facturación existentes en el proyecto.

  Para obtener más información, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) y [Adjuntar una tarjeta de tarifas a un proyecto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* Como gerente del proyecto, puede definir la tarifa de facturación para la mismo función en el nivel de proyecto.\
  Las tarifas de funciones cambiadas en el proyecto solo afectarán a ese proyecto.

  Para obtener información sobre cómo anular las tarifas de funciones para el proyecto, consulte [Anular tarifas de facturación de funciones a nivel de proyecto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Si una función está asociada con una tarifa de facturación en el nivel del sistema, en el nivel de la compañía y en el nivel del proyecto, Workfront calcula los ingresos de las tareas utilizando la tarifa de facturación de la función en el nivel de proyecto, cuando utiliza las taifas de funciones. Los ingresos de todas las tareas se acumulan en los ingresos del proyecto.

## Anular tarifas de facturación de funciones a nivel de proyecto

Como gerente del proyecto, puede especificar cuál es la tarifa de facturación de una función en un proyecto específico. Esta tarifa de facturación en el nivel de proyecto anula la tarifa de facturación en el nivel de sistema para esta función. Workfront utiliza la tarifa de facturación en el nivel de proyecto de la función de trabajo para calcular los ingresos, en lugar de utilizar la tarifa de facturación en el nivel de sistema.

<span class="preview">También puede adjuntar una tarjeta de tarifas al proyecto, que importará las tarifas de facturación de funciones de trabajo de la tarjeta de tarifas en el proyecto.</span>

Para obtener información sobre cómo anular las tarifas de facturación de funciones a nivel del proyecto, consulte [Anular tarifas de facturación de funciones a nivel de proyecto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Para obtener más información sobre qué función se utiliza para calcular los ingresos del proyecto, consulte la sección “Cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones” en [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">Para obtener información sobre cómo adjuntar una tarjeta de tarifas a un proyecto, consulte [Adjuntar una tarjeta de tarifas a un proyecto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>En el caso de los ingresos reales, las tarifas de facturación aplicadas a las horas que se añaden a un Registro de facturación que está marcado como Facturado, no deben verse afectadas por las anulaciones de tarifas de facturación que ocurren después de que se haya facturado el Registro de facturación.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Visión general de la sección de tarifas de facturación de un proyecto

Después de especificar la anulación de las tarifas de facturación para las funciones asociadas con el proyecto, puede ver todas las funciones y sus anulaciones en la pestaña **Tarifas de facturación** del proyecto.

Tenga en cuenta la siguiente información de la lista de **Tarifas de facturación**:

* [Agrupación de funciones](#job-role-grouping)
* [Valor de tarifa de facturación del proyecto](#project-billing-rate-value)
* [Valor de tarifa de facturación predeterminada](#default-billing-rate-value)
* [Valor de tarifa de facturación de la compañía](#company-billing-rate-value)
* [Varios valores de tarifa de facturación y periodos de tiempo](#multiple-billing-rate-values-and-timeframes)

### Agrupación de funciones {#job-role-grouping}

Las tarifas de facturación se agrupan en el área **Tarifas de facturación** según sus respectivas funciones. <span class="preview">Si se adjunta una tarjeta de tarifas al proyecto, las funciones también se agrupan por tarjeta de tarifas. Si las ubicaciones se aplican a las funciones, el nombre de la ubicación se incluye como parte del nombre de la función. Podría tener la misma función en la lista para varias ubicaciones.</span>

### Valor de tarifa de facturación del proyecto {#project-billing-rate-value}

En la línea de agrupación correspondiente a una función, tenga en cuenta la tarifa de facturación para esa función en el nivel de proyecto, en la columna **Tarifa de facturación del proyecto**. Si la función tiene múltiples anulaciones de tarifa, la anulación de la tarifa correspondiente a la fecha actual se mostrará en la línea de agrupación de la columna **Tarifa de facturación del proyecto**.

### Valor de tarifa de facturación predeterminada {#default-billing-rate-value}

En la línea de agrupación de una función, tenga en cuenta la tarifa de facturación de esa función en el nivel de sistema, en la columna **Tarifa de facturación predeterminada**.

>[!NOTE]
>
>Si hay tarifas de facturación del proyecto para una función, la **tarifa de facturación predeterminada** nunca se aplica en el cálculo de los ingresos del proyecto. Para calcular los ingresos solo se aplican las **tarifas de facturación del proyecto**.

### Valor de tarifa de facturación de la compañía {#company-billing-rate-value}

En la línea de agrupación de una función, tenga en cuenta la tarifa de facturación de esa función a nivel de compañía, en la columna **Tarifa de facturación de la compañía**. Esto significa que hay una compañía asociada con este proyecto y que esta función tiene una tarifa de facturación diferente para esa compañía. Se muestra la tarifa de facturación de la compañía, aunque sea la misma que la del proyecto.

>[!NOTE]
>
><span class="preview">Cuando se adjunta una tarjeta de tarifas al proyecto, las **tarifas de facturación de la compañía** no se importan en las tarifas de facturación. Los cálculos se basan en las tarifas de la tarjeta de tarifas o en las tarifas de la compañía para las funciones.</span>
>
>Si hay tarifas de facturación del proyecto para una función, la **tarifa de facturación de la compañía** nunca se aplica en el cálculo de los ingresos del proyecto. Para calcular los ingresos solo se aplican las **tarifas de facturación del proyecto**.

### Varios valores de tarifa de facturación y periodos de tiempo {#multiple-billing-rate-values-and-timeframes}

Si tiene varias anulaciones de tarifas de facturación para una función específica, se enumeran en la agrupación de esa función. Con la edición en línea, puede cambiar la anulación de tarifas y la **Fecha** **de inicio** y la **Fecha de finalización** de la anulación de las tarifas de facturación en esta pestaña.

>[!NOTE]
>
>No puede especificar una **Fecha de inicio** para la primera anulación de tarifa, ni tampoco puede especificar una **Fecha de finalización** para la última anulación de tarifa. Workfront supone que la primera anulación de tarifa se aplica a todas las horas con una fecha anterior a la **Fecha de finalización** de la primera anulación y que la última anulación de tarifa se aplica a todas las horas con una fecha posterior a la **Fecha de inicio** de la última anulación.\
>Si se registra una hora antes de la Fecha planificada de inicio del proyecto, se usa la primera tarifa de facturación.\
>Si se registra una hora después de la Fecha planificada de finalización del proyecto, se usa la última tarifa de facturación.

## Ingresos planificados totales

* [Calcular ingresos planificados según una anulación de tarifa de facturación única](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Calcular ingresos planificados según múltiples anulaciones de tarifas de facturación](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Distribución de horas planificadas a lo largo de la duración de una tarea](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Calcular ingresos planificados según una anulación de tarifa de facturación única {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Tenga en cuenta lo siguiente al calcular los ingresos planificados según una anulación de tarifa de facturación única:

* Cuando el **Tipo de ingresos** de una tarea es **Rol por hora**, Workfront multiplica las horas planificadas de una tarea por la tarifa de facturación de la función asociada con la tarea para calcular los ingresos planificados en la tarea.

* Cuando la tarifa de facturación de la función se ha anulado en el nivel de proyecto, Workfront utiliza la anulación de tarifa del proyecto para calcular los ingresos planificados.
* Cuando una tarea tiene varias asignaciones, los ingresos planificados se calculan multiplicando la tarifa de facturación de la función de cada asignación y su respectiva asignación de horas planificadas.

>[!NOTE]
>
>Las horas planificadas por asignación no son las mismas que las horas planificadas para la tarea, en el caso de varias asignaciones.

Para obtener más información sobre qué función se usa para calcular los ingresos planificados, consulte la sección “Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones” en el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Calcular ingresos planificados según múltiples anulaciones de tarifas de facturación {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Tenga en cuenta lo siguiente al calcular los ingresos planificados según múltiples anulaciones de tarifas de facturación:

* Cuando el **Tipo de ingresos** de una tarea es **Rol por hora**, Workfront multiplica las horas planificadas de una tarea por la tarifa de facturación de la función asociada con la tarea para calcular los ingresos planificados en la tarea.

  Para obtener más información sobre qué función se usa para calcular los ingresos planificados, consulte la sección “Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones” en el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* En caso de múltiples anulaciones de tarifas de facturación, la tarifa por la que se multiplican las horas planificadas cambia durante la duración de una tarea. De forma predeterminada, Workfront distribuye las horas planificadas de forma uniforme a lo largo de la duración de una tarea y asigna un número igual de horas a cada día de la tarea. Al calcular **Ingresos planificados** para una tarea, Workfront multiplica la hora planificada por día por la tasa de facturación de ese día. En caso de múltiples tarifas de facturación, esa tarifa podría ser diferente cada día.

  Por ejemplo, tiene una tarea con un Rol por hora **Tipo de ingresos**. La tarea tiene una duración de 5 días y un valor de horas planificadas de 40 horas. Las horas planificadas por día son 8 horas. Asigne una función de jefe de proyecto a la tarea y anule la tarifa de facturación de esta función durante los últimos 3 días de la tarea, de modo que tendrá una tarifa de facturación 1 para los dos primeros días y una tarifa 2 para los 3 días restantes de la tarea para esta función.

  La fórmula que calcula los **ingresos planificados** de esta tarea es:

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Para obtener más información acerca de cómo encontrar la cantidad de horas planificadas por día en Workfront, consulte la sección [Distribución de horas planificadas entre la duración de una tarea](#distribution-of-planned-hours-across-the-duration-of-a-task) en este artículo.

>[!NOTE]
>
>Si tiene varias personas asignadas en la tarea, la cantidad de horas planificadas se distribuye primero a cada persona asignada y, a continuación, a cada día durante la duración de la tarea. En este caso, los ingresos planificados se calcularán teniendo en cuenta la cantidad de horas diarias para cada asignado y la tasa de facturación de cada función que podría cambiar durante la duración de la tarea, en caso de múltiples tarifas de facturación.

### Distribución de horas planificadas a lo largo de la duración de una tarea {#distribution-of-planned-hours-across-the-duration-of-a-task}

Tenga en cuenta lo siguiente al comprender la distribución de las horas planificadas a lo largo de la duración de una tarea:

* De forma predeterminada, Workfront distribuye las horas planificadas de forma uniforme a lo largo de la duración de una tarea y asigna un número igual de horas planificadas a cada día de la tarea, según la disponibilidad de la programación del proyecto.

  Para obtener más información acerca de cómo distribuir las horas planificadas en la duración de una tarea, consulte la sección “Explicación de la distribución de horas planificadas en la duración de una tarea” en el artículo [Información general sobre las horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >Las horas planificadas por día son la asignación de horas planificadas para cada día durante la duración de la tarea. Si la tarea tiene una asignación, este número representa también las horas planificadas por día y por asignación. Si la tarea tiene varias asignaciones, las horas planificadas por día y asignación son diferentes a las horas planificadas por día para la tarea. No hay representación visual en Workfront para las horas planificadas por día y asignación, para tareas con varias asignaciones.
  >
  >
  >Las horas planificadas por día se multiplican por la tasa de facturación de la función asignada a la tarea para ese día a fin de calcular los ingresos planificados por día para esa tarea. Una suma de todos los ingresos planificados diarios calculados de esta manera es igual a los ingresos planificados para esa tarea.

## Calcular ingresos reales

* [Calcular ingresos reales según una anulación de tarifa de facturación única](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Calcular ingresos reales en función de varias anulaciones de tarifa de facturación](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Calcular ingresos reales en función de una anulación de tarifa de facturación única {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Tenga en cuenta lo siguiente al calcular los ingresos reales en función de una anulación de tarifa de facturación única:

* Si el **Tipo de ingresos** de una tarea es **Rol por hora**, Workfront multiplica las **Horas reales** de una tarea por la tasa de facturación de la función asociada con la tarea para calcular los **Ingresos reales** en la tarea. Las horas reales son horas registradas directamente en la tarea.

  Para obtener más información sobre qué función se usa para calcular los **Ingresos reales**, consulte la sección “Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones” en el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Si la tasa de facturación de la función se ha anulado en el nivel de proyecto, Workfront utiliza la tasa de anulación del proyecto para calcular los ingresos reales. Cuando se anula la tarifa de facturación de la función en el proyecto, los **ingresos reales** del proyecto se recalculan automáticamente usando la nueva tarifa ajustada.

  Para obtener información acerca de cómo anular las tarifas de función para el proyecto, consulte [Anular tarifas de facturación de función en el nivel de proyecto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Si desea conservar las horas en las que ya inició sesión en el proyecto antes de anular la tarifa de facturación original facturada en la tarifa original, debe incluirlas en un **Registro de facturación** y debe marcar el **Registro de facturación** como **Facturado**. De lo contrario, los **ingresos reales** de las horas registradas antes de que se anulara la tarifa de facturación del proyecto se recalcularán usando la nueva tarifa cuando se recalculen las finanzas de los proyectos.\
>Para obtener más información sobre cómo incluir horas en un registro de facturación y marcarlo como **Facturado**, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

### Calcular ingresos reales en función de varias anulaciones de tarifa de facturación {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Tenga en cuenta lo siguiente al calcular los ingresos reales en función de varias anulaciones de tarifas de facturación:

* Cuando el **Tipo de ingresos** de una tarea es **Rol por hora**, Workfront multiplica las **Horas reales** en la tarea con la tasa de facturación de las funciones asignadas a la tarea para calcular los **Ingresos reales** en la tarea. Las horas reales son horas registradas directamente en la tarea.

* En caso de que haya varias anulaciones de tarifas de facturación, la tarifa por la cual se multiplican las **Horas reales** para calcular los **Ingresos reales** podría cambiar durante la duración de una tarea. Workfront usa la tarifa de facturación de la función cuyo lapso de tiempo coincide con la **Fecha de entrada** de las horas registradas para la tarea a fin de calcular los **Ingresos reales.**

  Por ejemplo, una tarea tiene el **Tipo de ingresos** de **Rol por hora** y se asigna a la función de Administrador de proyectos. Anule la tarifa de facturación de esta función con la tarifa 1 para las fechas entre el 19 de junio y el 25 de junio. A partir del 26 de junio, anule la tarifa de facturación con la tarifa 2. Registre 2 horas para el 20 de junio y 3 horas para el 28 de junio.

  Workfront calcula los **ingresos reales** de esta tarea mediante la siguiente fórmula:

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Para obtener más información acerca de qué función se usa para calcular los **Ingresos reales**, consulte la sección “Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones” en el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## El impacto de las zonas horarias al calcular ingresos basados en varias tarifas de facturación

Los usuarios pueden ver diferentes horas planificadas por día de otros usuarios si se producen diferencias de zona horaria entre ellos y otras entidades de Workfront. Los siguientes escenarios podrían distorsionar la información de Horas planificadas por día de un usuario con respecto a lo que otro usuario ve:

* Los dos usuarios pueden tener sus equipos configurados para dos zonas horarias diferentes
* Los dos perfiles de usuario de Workfront pueden establecerse en dos zonas horarias diferentes
* La zona horaria asociada al perfil de usuario puede ser diferente de la zona horaria del sistema en Workfront
* La zona horaria asociada al perfil del usuario puede ser diferente de la zona horaria de la programación del proyecto.

En estos casos, el número de horas planificadas por día puede ser diferente entre dos usuarios que no comparten la misma configuración para las zonas horarias. También verán diferentes números de ingresos planificados cuando usen varias anulaciones de tarifas de facturación en un proyecto.

* [Calcular los ingresos planificados para usuarios en diferentes zonas horarias](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Calcular los ingresos reales para usuarios en diferentes zonas horarias](#calculate-actual-revenue-for-users-in-different-time-zones)

### Calcular los ingresos planificados para usuarios en diferentes zonas horarias {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Si tiene usuarios en diferentes zonas horarias trabajando en los mismos proyectos, le recomendamos que no cambie las anulaciones de tarifas de facturación para sus proyectos durante la semana. Si lo hace, se puede mostrar una cantidad errónea de ingresos planificados para el proyecto, como resultado de las diferencias horarias entre las zonas horarias en la programación de los usuarios y la zona horaria del sistema de Workfront La mayoría de los horarios permiten que los fines de semana se excluyan de los cálculos de Horas planificadas. Si se produce un cambio en la anulación de la tarifa de facturación de una función, es mejor que se produzca durante un fin de semana que a mitad de una semana cuando podría coincidir con la mitad de la duración de una tarea.

Tenga en cuenta lo siguiente al calcular los ingresos planificados para usuarios en diferentes zonas horarias:

* En el caso de las tareas que tienen un **Tipo de ingresos** de **Rol por hora** y que están asignadas a funciones, los **Ingresos planificados** se calculan multiplicando las **Horas planificadas** de una tarea por la tarifa de facturación de la función.

* Las **Horas planificadas** se distribuyen de manera uniforme en la **Duración** de la tarea.

* La **duración** es el período de tiempo entre la **Fecha planificada de inicio** **&#x200B;**&#x200B;y la **Fecha planificada de finalización** de la tarea. Dado que la **Fecha planificada de inicio** y la **Fecha planificada de finalización** de las tareas pueden diferir según las zonas horarias de los usuarios que ven la tarea, la cantidad de horas planificadas por día puede ser diferente para dos usuarios en dos zonas horarias diferentes.

* La cantidad de horas planificadas por día no cambia los ingresos planificados de un proyecto si la tarifa de facturación de la función no cambia, o cuando solo hay una anulación de tarifa de facturación. En este caso, incluso si dos usuarios de dos zonas horarias diferentes ven diferentes horas planificadas por día, los ingresos planificados generales del proyecto son idénticos entre los dos usuarios.

  Sin embargo, en el caso de varias anulaciones de tarifas de facturación, los **Ingresos planificados** generales del proyecto podrían parecer diferentes para dos usuarios en dos zonas horarias diferentes, ya que dependen de la cantidad de Horas planificadas por día (que podría ser diferente para los dos usuarios) y la anulación de tarifas de facturación (que podría ser diferente para el mismo día, cuando cada usuario esté mirando la tarea en su propia zona horaria).

* La cantidad exacta de **Ingresos planificados** es la que ve el usuario que tiene la misma zona horaria que la de la instancia de Workfront. El administrador de Workfront define la zona horaria de Workfront en el área Información del cliente del sistema.\
  Para obtener más información sobre la definición de la zona horaria de su sistema, consulte el artículo [Configurar la información básica del sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Calcular los ingresos reales para usuarios en diferentes zonas horarias {#calculate-actual-revenue-for-users-in-different-time-zones}

Tenga en cuenta lo siguiente al calcular los ingresos reales para usuarios de diferentes zonas horarias:

* Si el **Tipo de ingresos** de una tarea es **Rol por hora**, Workfront multiplica las **Horas reales** en la tarea con la tarifa de facturación de los roles asignados a la tarea para calcular los **Ingresos reales**. Las horas reales son horas registradas directamente en la tarea.

* En caso de varias anulaciones de tarifas de facturación, Workfront usa la tarifa de facturación de la función cuyo lapso de tiempo coincida con la **Fecha de entrada** de las horas registradas para la tarea a fin de calcular los **Ingresos reales**.

* Debido a que no hay una marca de tiempo en la **Fecha de entrada** de las horas registradas y no hay una marca de tiempo en los intervalos de fechas de múltiples anulaciones de tarifas de facturación, los cálculos de **Ingresos reales** no se ven afectados por la zona horaria asociada con los usuarios.

Para obtener más información sobre qué función se usa para calcular los **Ingresos reales**, consulte la sección &quot;Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuarios y funciones&quot; en el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Recalcular las finanzas de un proyecto

Las finanzas se calculan en un proyecto a medida que se producen cambios en las horas registradas para el proyecto.

Si las tarifas se cambian durante la duración de un proyecto, puede recalcular manualmente los costes e ingresos del proyecto mediante la opción Recalcular finanzas en un proyecto. Además, algunas acciones activan un nuevo cálculo automático.

Para obtener más información sobre cómo volver a calcular las las finanzas del proyecto, consulte el artículo [Recalcular las finanzas del proyecto](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Añadir una nueva tarifa de facturación usando la API

Para añadir una nueva tarifa de facturación para una función mediante la API, debe realizar una acción *setRatesForRole* para el objeto **Rate** mediante el *método PUT*.
La acción y los campos de fecha del objeto **Rate** están disponibles en la versión 8.0 de la API.
Si ya tiene varias tarifas de facturación definidas para una función en un proyecto y desea añadirle una nueva tarifa de factura con un nuevo intervalo de fechas, debe incluir tanto la tarifa existente como la tarifa que se añadirá en la misma llamada de API. Es similar a cómo se actualizan las colecciones en los objetos.

La siguiente llamada de API es un ejemplo en el que **attachableID** es el **ID de proyecto** del proyecto donde está añadiendo la tarifa y **RoleID** es el **ID de función** para el cual está añadiendo la nueva tarifa de facturación.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;rates&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Para obtener más información sobre el uso de la API de Workfront, consulte el artículo [Conceptos básicos de la API](https://experience.workfront.com/s/article/API-Basics-638808549).
