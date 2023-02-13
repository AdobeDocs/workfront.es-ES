---
product-area: projects
navigation-topic: financials
title: Información general sobre la anulación de la función de trabajo Tasas de facturación y el cálculo de ingresos en un proyecto
description: Puede utilizar las tasas de facturación para calcular los ingresos de sus proyectos cuando los multiplique por las horas dedicadas al proyecto. Para obtener más información sobre las tasas de facturación y los ingresos, consulte el artículo Información general sobre facturación e ingresos.
author: Alina
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3644'
ht-degree: 0%

---

# Información general sobre la anulación de la función de trabajo Tasas de facturación y el cálculo de ingresos en un proyecto

Puede utilizar las tasas de facturación para calcular los ingresos de sus proyectos cuando los multiplique por las horas dedicadas al proyecto. Para obtener más información sobre tasas de facturación e ingresos, consulte el artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

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

## Información general sobre las tasas de facturación de funciones del trabajo y los tipos de ingresos por hora de función

Como administrador de Adobe Workfront, puede asociar las tasas de facturación tanto a los usuarios como a las funciones de trabajo.\
Para obtener más información sobre cómo crear usuarios y asociarlos con tasas de facturación, consulte el artículo [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Para obtener más información sobre la creación de funciones de trabajo y su asociación con tasas de facturación, consulte el artículo [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Las tasas de facturación asociadas a los usuarios no se pueden anular.

Las tasas de facturación asociadas con funciones de trabajo se pueden sobrescribir en el nivel de empresa o proyecto.

Para calcular los ingresos de los proyectos en función de las tasas de facturación de las funciones de trabajo, la variable **Tipo de ingresos** de las tareas de los proyectos deberá ser una de las siguientes:

* Rol por hora
* Rol por hora con tope
* Función por hora más fijo

Para obtener más información, consulte **Tipo de ingresos** y tasas de facturación, consulte [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Jerarquía de anulaciones de Tasa de Facturación al calcular Ingresos

Una función de trabajo puede tener asociada una tasa de facturación de las siguientes maneras:

* Como administrador de Workfront, puede definir la tasa de facturación a nivel del sistema asociada a una función de trabajo al crear esa función de trabajo.\
   Para obtener más información sobre la creación de funciones de trabajo, consulte [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Como administrador de Workfront, puede definir la tasa de facturación a nivel de empresa para la misma función de trabajo al crear una empresa.\
   Cuando Workfront calcula los ingresos de los proyectos asociados con esta empresa, la tasa de facturación de la empresa se utiliza cuando la función se asigna a tareas, en lugar de la tasa de facturación a nivel del sistema para esta función de trabajo.\
   Las tasas de puestos de trabajo cambiadas a nivel de empresa afectarán a todos los proyectos asociados con esa empresa.

   >[!NOTE]
   >
   >Si necesita actualizar la tasa de facturación de la empresa, la tasa del proyecto no se actualizará automáticamente. Debe eliminar la empresa del proyecto, actualizar la tasa de la empresa y volver a adjuntar la empresa al proyecto antes de que la nueva tasa de la empresa entre en vigor en el proyecto. Para obtener instrucciones sobre cómo adjuntar una empresa a un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

   Para obtener más información sobre la creación de tasas de facturación de funciones de trabajo específicas de una empresa, consulte [Crear y editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Como administrador de Workfront, puede activar una opción al editar un proyecto para aplicar cambios en las tasas de facturación a nivel de empresa al proyecto cuando los usuarios recalculen manualmente las finanzas del proyecto.\
   Para obtener más información, consulte [Anular tasas de facturación a nivel de proyecto con tasas de facturación a nivel de empresa](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

* Como administrador de proyectos, puede definir la tasa de facturación para la misma función de trabajo a nivel de proyecto.\
   Las tasas de función de trabajo cambiadas en el proyecto solo afectarán a ese proyecto.

   Para obtener información sobre la anulación de tasas de función para el proyecto, consulte [Anular tasas de facturación de rol de trabajo en el nivel de proyecto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Si una función de trabajo está asociada con una tasa de facturación a nivel de sistema, de empresa y de proyecto, Workfront calcula los ingresos de las tareas utilizando la tasa de facturación de la función de trabajo a nivel de proyecto, cuando utiliza las tasas de la función de trabajo. Los ingresos procedentes de todas las tareas se acumulan en los ingresos del proyecto.

## Anular tasas de facturación de rol de trabajo en el nivel de proyecto

Como administrador de proyectos, puede especificar la tasa de facturación de una función de trabajo en un proyecto específico. Esta tasa de facturación a nivel de proyecto anula la tasa de facturación a nivel del sistema para esta función de trabajo. Workfront utiliza la tasa de facturación a nivel de proyecto de la función de trabajo para calcular los ingresos, en lugar de utilizar la tasa de facturación a nivel de sistema.

Para obtener información sobre cómo anular las tasas de facturación de rol de trabajo en el nivel de proyecto, consulte [Anular tasas de facturación de rol de trabajo en el nivel de proyecto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Para obtener más información sobre la función de trabajo que se utiliza para calcular los ingresos del proyecto, consulte la sección &quot;Cálculos de ingresos para tareas basadas en asignaciones de usuario y función&quot; en [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>En el caso de los ingresos reales, las tasas de facturación aplicadas a las horas que se agregan a un registro de facturación marcado como Facturado no deben verse afectadas por las anulaciones de las tasas de facturación que se produzcan después de facturar el registro de facturación.

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

## Información general sobre la sección Tasas de Facturación de un proyecto

Después de especificar las tasas de facturación de anulación de las funciones de trabajo asociadas con el proyecto, puede ver todas las funciones de trabajo y sus anulaciones en la **Tasas de facturación** del proyecto.

Observe la siguiente información en la lista de **Tasas de facturación**:

* [Agrupación de funciones de trabajo](#job-role-grouping)
* [Valor de tasa de facturación del proyecto](#project-billing-rate-value)
* [Valor de tasa de facturación predeterminado](#default-billing-rate-value)
* [Valor de tipo de facturación de la empresa](#company-billing-rate-value)
* [Varios valores y marcos de tiempo de la tasa de facturación](#multiple-billing-rate-values-and-timeframes)

### Agrupación de funciones de trabajo {#job-role-grouping}

Las tasas de facturación se agrupan en el **Tasas de facturación** por sus respectivas funciones de trabajo.

### Valor de tasa de facturación del proyecto {#project-billing-rate-value}

En la línea de agrupación correspondiente a una función de trabajo, observe la tasa de facturación para esa función de trabajo en el nivel de proyecto en la **Tasa de facturación del proyecto** para abrir el Navegador. Si la función de trabajo tiene varias tasas de anulación, la tasa de anulación correspondiente a la fecha actual se muestra en la línea de agrupación de la variable **Tasa de facturación del proyecto** para abrir el Navegador.

### Valor de tasa de facturación predeterminado {#default-billing-rate-value}

En la línea de agrupación de una función de trabajo, observe la tasa de facturación para esa función de trabajo a nivel del sistema en la **Tasa de facturación predeterminada** para abrir el Navegador.

>[!NOTE]
>
>Si hay tasas de facturación de proyectos para una función de trabajo, la variable **Tasa de facturación predeterminada** nunca se aplica al cálculo de ingresos para el proyecto. Solo el **Tasas de facturación del proyecto** se aplican para calcular los ingresos.

### Valor de tipo de facturación de la empresa {#company-billing-rate-value}

En la línea de agrupación de una función de trabajo, observe la tasa de facturación para esa función de trabajo a nivel de empresa en la variable **Tasa de facturación de la empresa** para abrir el Navegador. Esto significa que hay una empresa asociada con este proyecto y que esta función de trabajo tiene una tasa de facturación diferente para esa empresa. Se muestra la tasa de facturación de la empresa, aunque sea la misma que la tasa del proyecto.

>[!NOTE]
>
>Si hay tasas de facturación de proyectos para una función de trabajo, la variable **Tasa de facturación de la empresa** nunca se aplica al cálculo de ingresos para el proyecto. Solo el **Tasas de facturación del proyecto** para calcular ingresos.

### Varios valores y marcos de tiempo de la tasa de facturación {#multiple-billing-rate-values-and-timeframes}

Si tiene varias tasas de facturación de anulación para una función de trabajo específica, se enumeran en la agrupación para esa función de trabajo. Con la edición en línea, puede cambiar las tasas de anulación y la variable **Inicio** **Fecha** y **Fecha final** de las tasas de facturación de anulación en esta pestaña.

>[!NOTE]
>
>No se puede especificar un **Fecha de inicio** para la primera tasa de anulación y no se puede especificar una **Fecha final** para la última tasa de anulación. Workfront supone que la primera tasa de anulación se aplica a todas las horas con una fecha anterior a la del **Fecha final** de la primera anulación y que la última tasa de anulación se aplica para todas las horas con una fecha más reciente que la del **Fecha de inicio** de la última anulación.\
>Si se registra una hora antes de la fecha de inicio planeada del proyecto, se utiliza la primera tasa de facturación.\
>Si se registra una hora después de la Fecha de Finalización Planificada del proyecto, se utiliza la última tasa de facturación.

## Calcular ingresos planificados

* [Calcular los ingresos planeados en función de una anulación única de la tasa de facturación](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Calcular los ingresos planeados en función de varias anulaciones de tasa de facturación](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Distribución de horas planificadas a lo largo de la duración de una tarea](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Calcular los ingresos planeados en función de una anulación única de la tasa de facturación {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Tenga en cuenta lo siguiente cuando calcule los ingresos planeados en función de una anulación única de la tasa de facturación:

* Cuando la variable **Tipo de ingresos** de una tarea es **Función por hora**, Workfront multiplica las horas planificadas de una tarea por la tasa de facturación de la función de trabajo asociada con la tarea para calcular los ingresos planeados de la tarea.

* Cuando la tasa de facturación de la función de trabajo se ha anulado en el nivel de proyecto, Workfront utiliza la tasa de anulación del proyecto para calcular los ingresos planeados.
* Cuando una tarea tiene varias asignaciones, los ingresos planeados se calculan multiplicando la tasa de facturación de la función de trabajo de cada asignación y su respectiva asignación de horas planificadas.

>[!NOTE]
>
>El horario planificado por asignación no es lo mismo que el horario planificado para la tarea, en el caso de varias asignaciones.

Para obtener más información sobre la función de trabajo que se utiliza para calcular los ingresos planeados, consulte la sección &quot;Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuario y función&quot; del artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Calcular los ingresos planeados en función de varias anulaciones de tasa de facturación {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Tenga en cuenta lo siguiente al calcular los ingresos planeados en función de varias anulaciones de Tasa de facturación:

* Cuando la variable **Tipo de ingresos** de una tarea es **Función por hora**, Workfront multiplica las horas planificadas de una tarea por la tasa de facturación de la función de trabajo asociada con la tarea para calcular los ingresos planeados de la tarea.

   Para obtener más información sobre la función de trabajo que se utiliza para calcular los ingresos planeados, consulte la sección &quot;Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuario y función&quot; del artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* En el caso de varias anulaciones de la tasa de facturación, la tasa por la que se multiplican las horas planificadas cambia durante la duración de una tarea. De forma predeterminada, Workfront distribuye las horas planificadas uniformemente durante la duración de una tarea y asigna un número igual de horas para cada día de la tarea. Al calcular **Ingresos planificados** para una tarea, Workfront multiplica la hora planificada por día por la tasa de facturación de ese día. En el caso de múltiples tasas de facturación, esa tasa podría ser diferente cada día.

   Por ejemplo, tiene una tarea con una función por hora **Tipo de ingresos**. La tarea tiene una duración de 5 días y un valor de 40 horas planificadas. Las horas previstas por día son de 8 horas. Asigne una función de trabajo de Project Manager a la tarea y anule la tasa de facturación de esta función de trabajo durante los últimos 3 días de la tarea, de modo que tendrá una tasa de facturación de Rate 1 para los dos primeros días y una tasa de facturación de Rate 2 para los 3 días restantes de la tarea para esta función de trabajo.

   La fórmula que calcula la variable **Ingresos planificados** de esta tarea es:

   ```
   Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
   ```

Para obtener más información sobre cómo encontrar la cantidad de horas programadas por día en Workfront, consulte la sección [Distribución de horas planificadas a lo largo de la duración de una tarea](#distribution-of-planned-hours-across-the-duration-of-a-task) en este artículo.

>[!NOTE]
>
>Si tiene varios asignadores en la tarea, la cantidad de horas planeadas se distribuye primero a cada usuario asignado y, a continuación, a cada día durante la duración de la tarea. En este caso, los ingresos planeados calcularán teniendo en cuenta la cantidad de horas diarias para cada usuario asignado y la tasa de facturación de cada puesto de trabajo que podría cambiar durante la duración de la tarea, en caso de tasas de facturación múltiples.

### Distribución de horas planificadas a lo largo de la duración de una tarea {#distribution-of-planned-hours-across-the-duration-of-a-task}

Tenga en cuenta lo siguiente al comprender la distribución de horas planificadas a lo largo de la duración de una tarea:

* De forma predeterminada, Workfront distribuye las horas planificadas uniformemente durante la duración de una tarea y asigna un número igual de horas planificadas para cada día de la tarea, según la disponibilidad de la programación del proyecto.

   Para obtener más información sobre cómo comprender la distribución de horas planificadas a lo largo de la duración de una tarea, consulte la sección &quot;Explicación de la distribución de horas planificadas a lo largo de la duración de una tarea&quot; en el artículo [Información general sobre las horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

   >[!NOTE]
   >
   >Las horas planificadas por día son la asignación de horas planificadas para cada día durante la duración de la tarea. Si la tarea tiene una asignación, este número también representa las horas planificadas por día por asignación. Si la tarea tiene varias asignaciones, las horas planificadas por día por asignación son diferentes de las horas planificadas por día para la tarea. No hay representación visual en Workfront para las horas planificadas por día por asignación, para tareas con varias asignaciones.
   >
   >
   >Las horas planificadas por día se multiplican por la tasa de facturación de la función de trabajo asignada a la tarea de ese día para calcular los ingresos planificados por día para esa tarea. Una suma de todos los ingresos planificados diarios calculados de esta manera es igual a los ingresos planeados para esa tarea.

## Calcular ingresos reales

* [Calcular los ingresos reales en función de una anulación única de la tasa de facturación](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Calcular los ingresos reales en función de varias anulaciones de tasa de facturación](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Calcular los ingresos reales en función de una anulación única de la tasa de facturación {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Tenga en cuenta lo siguiente cuando calcule los ingresos reales en función de una anulación única de la tasa de facturación:

* Cuando la variable **Tipo de ingresos** de una tarea es **Función por hora**, Workfront multiplica el **Horas reales** de una tarea por la tasa de facturación de la función de trabajo asociada con la tarea para calcular **Ingresos reales** en la tarea. Las horas reales son horas registradas directamente en la tarea.

   Para obtener más información sobre qué rol de trabajo se utiliza para calcular **Ingresos reales**, consulte la sección &quot;Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuario y función&quot; del artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Si la tasa de facturación de la función de trabajo se ha anulado en el nivel de proyecto, Workfront utiliza la tasa de anulación del proyecto para calcular los ingresos reales. Cuando anula la tasa de facturación de la función de trabajo del proyecto, la variable **Ingresos reales** del proyecto se vuelve a calcular automáticamente mediante la nueva tasa ajustada.

   Para obtener información sobre la anulación de tasas de función para el proyecto, consulte [Anular tasas de facturación de rol de trabajo en el nivel de proyecto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Si desea mantener las horas que ya ha iniciado sesión en el proyecto antes de sobrescribir la tasa de facturación original facturada a la tasa original, debe incluirlas en una **Registro de facturación** y debe marcar la variable **Registro de facturación** como **Facturado**. De lo contrario, la función **Ingresos reales** a partir de las horas registradas antes de que se anulara la tasa de facturación para el proyecto, se recalculará utilizando la nueva tasa cuando se vuelvan a calcular las finanzas de los proyectos.\
>Para obtener más información sobre cómo incluir horas en un registro de facturación y marcarlo como **Facturado**, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

### Calcular los ingresos reales en función de varias anulaciones de tasa de facturación {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Tenga en cuenta lo siguiente al calcular los ingresos reales en función de varias anulaciones de Tasa de facturación:

* Cuando la variable **Tipo de ingresos** de una tarea es **Función por hora**, Workfront multiplica el **Horas reales** en la tarea con la tasa de facturación de las funciones de trabajo asignadas a la tarea para calcular **Ingresos reales** en la tarea. Las horas reales son horas registradas directamente en la tarea.

* En el caso de anulaciones de tasas de facturación múltiples, la tasa por la que la variable **Horas reales** se multiplican para calcular la variable **Ingresos reales** puede cambiar durante la duración de una tarea. Workfront utiliza la tasa de facturación de la función de trabajo cuyo lapso de tiempo coincide con la variable **Fecha de entrada** de las horas registradas para que la tarea calcule **Ingresos reales.**

   Por ejemplo, una tarea tiene la variable **Tipo de ingresos** de **Función por hora** y se asigna a la función de trabajo de Project Manager. Anule la tasa de facturación de esta función de trabajo con la tasa 1 para las fechas comprendidas entre el 19 de junio y el 25 de junio. A partir del 26 de junio, anule la tasa de facturación con la tasa 2. Registrar 2 horas para el 20 de junio y 3 horas para el 28 de junio.

   Workfront calcula la variable **Ingresos reales** para esta tarea utilizando la fórmula siguiente:

   ```
   Actual Revenue = 2 * Rate 1 + 3 * Rate 2
   ```

   Para obtener más información sobre qué rol de trabajo se utiliza para calcular **Ingresos reales**, consulte la sección &quot;Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuario y función&quot; del artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## El impacto de las zonas horarias al calcular los ingresos en función de varias tasas de facturación

Los usuarios pueden ver diferentes horas planificadas por día de otros usuarios si se producen diferencias entre ellos y otras entidades en Workfront. Los siguientes escenarios podrían distorsionar la información de horas por día planeadas para un usuario a partir de lo que otro usuario ve:

* Es posible que los dos usuarios tengan sus equipos configurados para dos zonas horarias diferentes
* Los dos perfiles de usuario de Workfront se pueden configurar en dos zonas horarias diferentes
* La zona horaria asociada al perfil del usuario puede ser diferente a la zona horaria del sistema en Workfront
* La zona horaria asociada al perfil del usuario puede ser diferente a la zona horaria de la programación del proyecto.

En estos casos, el número de horas planificadas por día puede ser diferente entre dos usuarios que no comparten la misma configuración para las zonas horarias. También verán diferentes números de ingresos planeados al usar varias anulaciones de tasas de facturación en un proyecto.

* [Calcular los ingresos previstos para los usuarios en diferentes zonas horarias](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Calcular los ingresos reales para los usuarios en diferentes zonas horarias](#calculate-actual-revenue-for-users-in-different-time-zones)

### Calcular los ingresos previstos para los usuarios en diferentes zonas horarias {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Si tiene usuarios en diferentes zonas horarias trabajando en los mismos proyectos, le recomendamos que no cambie las anulaciones de la tasa de facturación de sus proyectos durante la semana. Al hacerlo, puede mostrar una cantidad errónea de ingresos planeados para su proyecto, como resultado de las diferencias horarias entre las zonas horarias de la programación de los usuarios y la zona horaria del sistema de Workfront . La mayoría de las programaciones permiten que los fines de semana se excluyan de los cálculos Horario planificado. Si se produce un cambio en la anulación de la tasa de facturación de una función de trabajo, es mejor que se produzca durante un fin de semana que a mitad de una semana, cuando pueda coincidir con la mitad de la Duración de una tarea.

Tenga en cuenta lo siguiente al calcular los ingresos planeados para usuarios en diferentes zonas horarias:

* Para tareas que tienen un **Tipo de ingresos** de **Función por hora** y se asignan a funciones de trabajo, **Ingresos planificados** se calcula multiplicando la variable **Horas planificadas** de una tarea por la tasa de facturación de la función de trabajo.

* La variable **Horas planificadas** se distribuyen uniformemente en todo el **Duración** de la tarea.

* La variable **Duración** es el periodo de tiempo entre **Inicio planificado** **Fecha** y **Fecha de finalización planeada** de la tarea. Porque la variable **Fecha de inicio planeada** y **Fecha de finalización planeada** de las tareas pueden variar según los husos horarios de los usuarios que vean la tarea, la cantidad de horas programadas por día puede ser diferente para dos usuarios en dos husos horarios diferentes.

* La cantidad de horas planificadas por día no cambia los ingresos planificados de un proyecto si la tasa de facturación de la función de trabajo no cambia, o si solo hay una anulación de la tasa de facturación. En este caso, incluso si dos usuarios de dos zonas horarias diferentes ven diferentes horas planificadas por día, los ingresos planificados generales del proyecto son idénticos entre los dos usuarios.

   Sin embargo, en el caso de varias anulaciones de la tasa de facturación, la variable **Ingresos planificados** del proyecto puede parecer diferente para dos usuarios en dos zonas horarias diferentes, ya que depende de la cantidad de horas planificadas por día (que podría ser diferente para los dos usuarios) y de la anulación de la tasa de facturación (que podría ser diferente para el mismo día, cuando cada usuario está mirando la tarea en su propio huso horario).

* La precisión **Ingresos planificados** cantidad es la que ve el usuario que tiene la misma zona horaria que la de su instancia de Workfront. El administrador de Workfront define la zona horaria de Workfront en el área Información del cliente del sistema.\
   Para obtener más información sobre la definición de la zona horaria del sistema, consulte el artículo [Configurar información básica para el sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Calcular los ingresos reales para los usuarios en diferentes zonas horarias {#calculate-actual-revenue-for-users-in-different-time-zones}

Tenga en cuenta lo siguiente al calcular los ingresos reales para usuarios en diferentes zonas horarias:

* Cuando la variable **Tipo de ingresos** de una tarea es **Función por hora**, Workfront multiplica el **Horas reales** en la tarea con la tasa de facturación de las funciones de trabajo asignadas a la tarea para calcular la **Ingresos reales**. Las horas reales son horas registradas directamente en la tarea.

* En el caso de varias anulaciones de la tasa de facturación, Workfront utiliza la tasa de facturación de la función de trabajo cuyo lapso de tiempo coincide con el **Fecha de entrada** de las horas registradas para que la tarea calcule **Ingresos reales**.

* Porque no hay marca de tiempo en la variable **Fecha de entrada** de horas registradas y no hay una marca de tiempo en los intervalos de fechas de varias anulaciones de tasas de facturación, **Ingresos reales** Los cálculos no se ven afectados por la zona horaria asociada a los usuarios.

Para obtener más información sobre qué rol de trabajo se utiliza para calcular **Ingresos reales**, consulte la sección &quot;Explicación de los cálculos de ingresos para tareas basadas en asignaciones de usuario y función&quot; del artículo [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Volver a calcular las finanzas del proyecto

Las finanzas se calculan en un proyecto a medida que se producen cambios en las horas registradas para el proyecto.

Si las tasas se cambian durante la vida de un proyecto, puede volver a calcular los costes e ingresos del proyecto manualmente mediante la opción Recalcular finanzas de un proyecto. Además, algunas acciones déclencheur un nuevo cálculo automático.

Para obtener más información sobre cómo volver a calcular las finanzas del proyecto, consulte el artículo [Volver a calcular las finanzas del proyecto](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Añadir una nueva tasa de facturación mediante la API

Para agregar una nueva tasa de facturación para una función de trabajo mediante la API, realice una *setRatesForRole* para la variable **Rate** usando el *método PUT*.
La acción y los campos de fecha del **Rate** están disponibles en la versión 8.0 de la API. Si ya tiene varias tasas de facturación definidas para una función de trabajo en un proyecto y desea agregar una nueva tasa de facturación para él con un nuevo intervalo de fechas, debe incluir tanto la tasa existente como la que se agregará en la misma llamada de API. Esto es similar a cómo se actualizan las colecciones de los objetos.

La siguiente llamada de API es un ejemplo en el que **attachmentID** es la variable **ID del proyecto** del proyecto en el que va a añadir la tasa y **RoleID** es la variable **ID de rol de trabajo** para el cual está agregando la nueva tasa de facturación.<pre>{</pre><pre>&quot;attachmentID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachmentObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df00014148cda5136d4b79d09&quot;, </pre><pre>&quot;tasas&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Para obtener más información sobre el uso de la API de Workfront, consulte el artículo [Conceptos básicos de API](https://experience.workfront.com/s/article/API-Basics-638808549).
