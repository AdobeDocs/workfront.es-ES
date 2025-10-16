---
product-area: resource-management
navigation-topic: resource-utilization
title: Ver información de utilización de recursos
description: Puede ver la utilización de sus recursos en el informe Utilización.
author: Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '7259'
ht-degree: 99%

---

# Ver información sobre la utilización de recursos {#view-resource-utilization-information}

>[!CONTEXTUALHELP]
>id="wf-resourcing-utilization"
>title="Informe de utilización"
>abstract="El informe Utilización le permite ver el progreso, el coste o los ingresos de un proyecto, programa o portafolio en un solo informe. También puede comparar los ingresos con el coste."

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

Puede ver la utilización de sus recursos en el informe Utilización.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Vazgen's response about these hours ie below and he asked us to NOT document them:</p>
<p>It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours.</p>
<p>In some cases, like for Planned Hours, it takes them from Assignments</p>
<p>But Budgeted Hours come from projects.</p>
<p>And Actual Hours are their own object - Hour)</p>
</div>
-->

<!--
<p style="color: #dc143c;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This report displays information about the assignments on work items for projects in your environment, like Planned, Actual, and Budgeted Hours, FTE, or Cost.&nbsp;These are hours,&nbsp;FTE, or costs associated with the assignments and not with the tasks and issues themselves.(PRIVATE NOTE:&nbsp;Vazgen's response about these hours: It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours. In some cases, like for Planned Hours, it takes them from Assignments; But Budgeted Hours come from projects. And Actual Hours are their own object - Hour.)</p>
-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td>
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos </p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Portafolios</p> </li> 
     <li> <p>Programas</p> </li> 
     <li> <p>Datos financieros, si desea ver la información por coste</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Acceso de visualización para proyectos, portafolios y programas, y poder acceder a la sección Utilización en el área Asignando recursos</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>Acceso de administración para un proyecto y poder acceder a la sección Utilización del proyecto</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Prerequisites for accessing utilization information</h2>
<p>(NOTE: drafted, replaced with above table)</p>
<p>To access utilization information as described in this section, ensure that the following conditions are met:</p>
<ul>
<li>You have at least&nbsp;View access to the project, program, or portfolio for which you want to view the utilization information.</li>
<li>Your Workfront administrator must grant you at least View access to&nbsp;Financial&nbsp;Data in your Access Level to be able to view cost and revenue information in the Utilization report. The Workfront administrator must enable both View Role Billing & Cost Rates as well as View User Billing &&nbsp;Cost Rates when they grant you the View access to Financial Data. For information about granting access to&nbsp;Financial&nbsp;Data, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. </li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;drafted. No longer the case.) </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Reporting area. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Resourcing area. </p>
</li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is available by default in the Reporting area if the system administrator has not assigned a custom layout template to you. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is available by default in the Resourcing area if the system administrator has not assigned a custom layout template to you. </p>
</li>
</ul>
</div>
-->

## Información general del informe Utilización {#overview-of-the-utilization-report}

El informe Utilización le permite ver el progreso, el coste o los ingresos de un proyecto, programa o portafolio en un solo informe. También puede comparar los ingresos con el coste.

Puede ver el informe Utilización en el área Asignando recursos para ver la utilización en varios proyectos, o puede verlo en el nivel de un proyecto para ver la utilización de los recursos individuales (funciones y usuarios) asociados a ese proyecto.

Para obtener información sobre cómo acceder y usar el informe Utilización, consulte la sección [Seguimiento de progreso, coste e ingresos con el informe Utilización](#track-progress-cost-and-revenue-with-the-utilization-report) en este artículo.

### Seguimiento de horas (progreso) {#track-hours-progress}

Puede realizar un seguimiento del progreso viendo una comparación de las horas presupuestadas y las horas planificadas con las horas reales.

Con el seguimiento del progreso de un proyecto, programa o portafolio, el progreso de tanto tareas como problemas se incluye en el informe Utilización.

La siguiente información está disponible en el informe Utilización cuando se lleva el seguimiento de las horas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Título de columna al ver las horas</strong> </th> 
   <th><strong>Función</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Horas presupuestadas</strong> </td> 
   <td scope="col"> <p>Total de horas presupuestadas en los proyectos incluidos. Puede ver el total de horas presupuestadas para la duración global de los proyectos incluidos, o puede ver el total de horas presupuestadas solo para el intervalo de fecha especificado (puede especificar una semana o mes individual). </p> <p>Las horas presupuestadas se rellenan a partir de la información disponible en el área Presupuestación de recursos del caso empresarial o del Planificador de recursos<em>.</em></p> <p>Las horas presupuestadas aparecen en el informe Utilización en cualquiera de las siguientes filas:</p> 
    <ul> 
     <li> Las horas presupuestadas se resumen por función y por usuario individual en el informe Utilización, de la siguiente manera:<br><strong>Usuario individual:</strong> las horas presupuestadas se resumen para cada usuario en el informe Utilización. Estas horas presupuestadas están asociadas con las tareas y problemas que se han asignado al usuario en los proyectos incluidos. (Puede expandir la fila de la función correspondiente para ver una lista de usuarios con esa función).<br><strong>Función:</strong> las horas presupuestadas se resumen por función en el informe Utilización.<br>Las horas presupuestadas aparecen en una función en particular como resultado de cualquiera de los siguientes escenarios:
     <ul>
     <li>La función se define como la función principal del usuario asignado a la tarea o al problema con el que están asociadas las horas presupuestadas. </li> 
       <li>Cuando se ve la información de utilización de un solo proyecto, se usa la función del usuario asignado a las horas, tanto si no hay asignación en la tarea o el problema, si se asigna a otro usuario sin ninguna asignación de función, si se asigna a otro usuario con una función diferente o si se asigna otro equipo.</li> 
       <li>Cuando se ve la información de utilización de varios proyectos, programas o portafolios, la función del usuario asignado a las horas se usa únicamente cuando la función está asignada a una tarea o problema de un proyecto. </li> 
       <li>La función se asigna a la tarea o problema que tiene asociadas horas presupuestadas y el usuario asignado a la tarea o problema no tiene una función definida en el sistema.</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>Horas sin asignar</strong>: las horas presupuestadas se muestran en el informe de utilización, en la sección Horas sin asignar, cuando dichas horas se han asociado a una tarea o problema que no tiene asignado ningún usuario o función.<br>Esta sección solo aparece cuando hay horas en el proyecto que coinciden con esta descripción y cuando se ve el informe de utilización por proyecto o desde un proyecto. </p> <p>Esta sección solo aparece cuando hay horas en el proyecto que coinciden con esta descripción y cuando se ve el informe de utilización por proyecto o desde un proyecto. </p> </li> 
    </ul> <p>Para obtener más información sobre las horas presupuestadas, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md#locate-the-budgeted-hours-of-a-project">Localizar las horas presupuestadas de un proyecto</a> en <a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md">Comprender el coste de mano de obra presupuestado y las horas presupuestadas de los proyectos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Horas planificadas</strong> </td> 
   <td scope="col">
<p>
Horas planificadas en los proyectos incluidos asociados a las asignaciones de cada tarea y problema. Se puede ver el total de horas planificadas de todas las asignaciones del proyecto correspondientes a toda la vida de los proyectos incluidos o bien el total de horas planificadas solo para el intervalo de fecha especificado (se puede especificar una semana o mes concretos).
</p>
<p>
<strong>SUGERENCIA </strong>
</p>
<p>
No se tienen en cuenta las horas planificadas de elementos que tienen una duración de 0. 
</p>
<p>
Las horas planificadas del informe de utilización tienen en cuenta si estas se han reasignado a lo largo de la duración de una tarea o problema. 
</p>
<p>
Cuando se ha modificado la asignación diaria de horas del usuario mediante el Distribuidor de cargas de trabajo, los datos del informe de utilización pueden verse afectados si las fechas seleccionadas en dicho informe contienen únicamente una parte de la duración de una tarea o problema. 
</p>
<p>
Para obtener información sobre la modificación de asignaciones para usuarios, consulte <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo</a>.


</p>
<p>
Las horas planificadas aparecen en el informe de utilización en cualquiera de las filas siguientes:
</p>
<ul>

<li>Las horas planificadas se resumen por función y por usuario individual en el informe de utilización, de la siguiente manera: 
<ul>

<li><strong>Usuario individual</strong>: las horas planificadas se resumen para cada usuario en el informe de utilización. Estas horas planificadas están asociadas a las tareas y problemas a los que se ha asignado al usuario en los proyectos incluidos. (Puede expandir la fila de la función correspondiente para ver una lista de usuarios con esa función).

<li><strong>Función</strong>: las horas planificadas se resumen por función en el informe de utilización de un solo proyecto.<br>Las horas planificadas aparecen en una función en particular como resultado de cualquiera de los siguientes escenarios:  
<ul>

<li>La función se define como función principal del usuario asignado a la tarea o problema al que se han asociado las horas planificadas.

<li>Cuando se consulta la información de utilización de un solo proyecto, las horas asociadas a una función no se muestran para la función en los siguientes casos:   
<ul>

<li>No hay ninguna asignación en la tarea o problema

<li>Se asigna un usuario sin asignación de función

<li>Se asigna a un usuario una función diferente

<li>Se asigna un equipo a una tarea o problema
</li>   
</ul>

<li>Cuando se ve la información de utilización de varios proyectos, programas o portafolios, la función del usuario asignado a las horas se usa únicamente cuando la función está asignada a una tarea o problema de un proyecto. Las horas de la función no se muestran por separado al ver el informe de utilización de varios proyectos.

<li>La función se asigna a la tarea o problema que tiene horas planificadas asociadas y el usuario asignado a la tarea o problema no tiene una función definida en el sistema.
</li>  
</ul>

<li><strong>Horas sin asignar</strong>: las horas planificadas se muestran en el informe de utilización en la sección Horas sin asignar cuando las horas planificadas se han asociado a una tarea o problema que no tiene ningún usuario o función asignado. Esta sección aparece únicamente cuando hay horas en el proyecto que coinciden con esta descripción y cuando se visualiza el informe de utilización de un solo proyecto. <br>Para obtener más información sobre las horas planificadas, consulte <a href="../../manage-work/tasks/task-information/planned-hours.md">Información general sobre las horas planificadas</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Horas reales</strong> </td> 
   <td> <p> Total de horas registradas en las tareas, problemas, <span> y en el proyecto </span> de los proyectos incluidos. Se puede ver el total de horas reales correspondientes a toda la vida de los proyectos incluidos o bien el total de horas reales solo para el intervalo de fecha especificado (se puede especificar una semana o mes individual). </p> <p><strong>Advertencia:</strong> El informe de utilización incluye las horas registradas en el proyecto, las tareas secundarias, los problemas y las tareas principales que tienen al menos una asignación. Sin embargo, no incluye las horas registradas en las tareas principales sin asignaciones. Se recomienda no utilizar tareas principales como tareas de trabajo y asignar solo tareas secundarias a los recursos. </p> <p>Las horas reales aparecen en el informe de utilización en cualquiera de las filas siguientes:</p> 
    <ul> 
     <li> Las horas reales se resumen por función y por usuario individual en el informe de utilización de un proyecto, de la siguiente manera:<br><strong>Usuario individual:</strong> las horas reales se muestran en el informe de utilización en la fila del usuario que ha registrado las horas. (Puede expandir la fila de la función correspondiente para ver una lista de los usuarios con esa función que han registrado horas).<br><strong>Función:</strong> las horas reales registradas por los usuarios asociados a esas funciones se resumen en el informe de utilización en la fila de la función correspondiente.<br>Las horas reales aparecen en una función en particular como resultado de cualquiera de los siguientes escenarios: 
      <ul> 
       <li>La función se define como función principal del usuario que ha registrado las horas</li> 
       <li>No hay ninguna asignación en la tarea o problema</li> 
       <li>Se asigna otro usuario sin asignación de función</li> 
       <li>Se asigna a otro usuario una función diferente</li> 
       <li> <p>Se asigna un equipo</p> </li> 
      </ul></li>  
     <p>Si el usuario que registra las horas no tiene una función asociada a su perfil, la función utilizada para el informe de utilización es la función asignada a la tarea o problema en el que se registran las horas o la función asociada al propietario principal de la tarea o problema. </p> 
     <li><strong>Otras horas:</strong> las horas reales se muestran en el informe de utilización en la sección Otras horas, en la fila del usuario que ha registrado las horas.<br>Las horas aparecen en esta sección cuando el usuario que ha registrado las horas no tiene una función definida en el sistema.<br>Esta sección solo aparece cuando hay horas en el proyecto que coinciden con esta descripción. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Variación presupuestada (para horas)</strong> </td> 
   <td> <p>Total de horas presupuestadas menos el total de horas reales en los proyectos incluidos. Puede ver la variación presupuestada total para la vida general de los proyectos incluidos o solo para el intervalo de fechas especificado (puede especificar una semana o mes concretos). </p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de horas presupuestadas es mayor que las horas reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de horas presupuestadas es menor que las horas reales.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Variación planificada (para horas)</strong> </td> 
   <td> <p>Total de horas planificadas menos el total de horas reales en los proyectos incluidos. Puede consultar la variación total planificada para la vida útil total de los proyectos incluidos o puede consultar la variación total planificada solo para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de horas planificadas es mayor que las horas reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de horas planificadas es menor que las horas reales.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Realizar un seguimiento de los costes {#track-cost}

Puede realizar un seguimiento de los costes observando la comparación del coste presupuestado y el coste planificado con los costes reales.

Al realizar el seguimiento del coste de un proyecto, programa o portafolio, la información del informe de Utilización procede de las tareas. La información de costes de las tareas siempre está disponible en el informe Utilización. El coste de las tareas se calcula según el tipo de coste de la tarea. Para obtener información acerca del tipo de coste de las tareas, consulte [Cómo calcula Workfront los tipos de coste de las tareas](/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-cost-types-for-tasks) en [Realizar un seguimiento de los costes](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

Puede mostrar la información de los costes en el informe de Utilización de las siguientes maneras:

* Para una semana o mes determinados, o para el proyecto, programa o portafolio general
* Por función o por personas, para proyectos

La moneda del informe de utilización viene determinada por la moneda definida en el proyecto. Para obtener información sobre cómo ajustar la moneda de un proyecto, consulte [Cambiar la moneda del proyecto](../../manage-work/projects/project-finances/change-project-currency.md).

La siguiente información está disponible en el informe de Utilización al realizar el seguimiento de los costes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Título de columna al ver el coste</strong> </th> 
   <th> <p><strong>Función</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Coste presupuestado</strong> </td> 
   <td scope="col"> <p>Costo presupuestado de los proyectos incluidos. Puede consultar el coste presupuestado total de la vida general de los proyectos incluidos o el coste presupuestado total solo para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> <p>Dado que el coste presupuestado en el informe de Utilización se centra en el coste por función, el cálculo es el mismo que el Coste de mano de obra presupuestado dentro de otras áreas de Workfront. Para obtener información sobre cómo se calcula el Coste de mano de obra presupuestado, consulte <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender el coste presupuestado de la mano de obra y las horas presupuestadas para proyectos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Coste planificado</strong> </td> 
   <td scope="col"> <p>Coste total planificado de los proyectos incluidos. Puede ver el coste total planificado para la vida útil general de los proyectos incluidos o puede ver el coste total planificado solamente para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> <p>Tenga en cuenta que para las vistas de semana, mes y trimestre, los costes planificados se calculan como un promedio del período elegido cuando las tarifas de coste de las funciones o usuarios son efectivas por fecha.</p><p>Para obtener información sobre cómo se calcula el coste planificado del proyecto, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">Cómo calcula Workfront los costes planificados, presupuestados y reales</a> en <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">Realizar un seguimiento de los costes</a>.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"><strong>Coste real</strong> </td> 
   <td scope="col"> <p>Coste real total de los proyectos incluidos. Puede ver el coste real total de la vida útil general de los proyectos incluidos o puede ver el coste real total solamente para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> <p>Para obtener información sobre cómo se calcula el coste real del proyecto, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">Cómo calcula Workfront los costes planificados, presupuestados y reales</a> en <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">Realizar un seguimiento de los costes</a>.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Variación presupuestada (para coste)</strong> </td> 
   <td scope="col"> <p>Coste presupuestado total menos el coste real total de los proyectos incluidos. Puede ver la variación presupuestada total para la vida general de los proyectos incluidos o solo para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el coste presupuestado total es mayor que el coste real.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el coste presupuestado total es menor que el coste real.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Variación planificada (de coste)</strong> </td> 
   <td> <p>Coste total planificado menos el coste real total de los proyectos incluidos. Puede consultar la variación total planificada para la vida útil total de los proyectos incluidos o puede consultar la variación total planificada solo para el intervalo de fechas especificado (puede especificar una semana o mes concretos). </p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el coste total planificado es mayor que el coste real.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el coste total planificado es menor que el coste real.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Seguimiento de ingresos {#track-revenue}

Puede realizar un seguimiento de los ingresos consultando cómo se comparan los ingresos presupuestados y planificados con los ingresos reales.

Al realizar un seguimiento de los ingresos de un proyecto, programa o portafolio, solo los ingresos de las tareas se incluyen en el informe de utilización.

La información de la siguiente tabla está disponible en el informe de utilización al realizar el seguimiento de los ingresos.

Para obtener información sobre los campos específicos y cómo los calcula Workfront, consulte también [Seguimiento de costes](../../manage-work/projects/project-finances/track-costs.md) e [Información general sobre facturación e ingresos](../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Título de columna al ver los ingresos</strong> </th> 
   <th> <strong>Función</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Ingresos presupuestados</strong> </td> 
   <td scope="col"> <p>El total de horas presupuestadas multiplicado por la tarifa de facturación de función en los proyectos incluidos. Puede ver el total de ingresos presupuestados para la duración global de los proyectos incluidos, o puede ver el total de ingresos presupuestados solo para el intervalo de fecha especificado (puede especificar una semana o mes individual).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ingresos planificados</strong> </td> 
   <td scope="col"> <p>Los ingresos planificados en el informe Utilización son los ingresos asociados con las horas planificadas asignadas a los recursos asignados a las tareas del proyecto.</p> <p>Workfront calcula los ingresos planificados del proyecto para el informe Utilización mediante la siguiente fórmula:</p> <p><code>Project Planned Revenue = SUM (All Tasks Planned Revenue)</code> </p> 
   <p><b>NOTA</b>
   <p>Los ingresos planificados del proyecto que se muestran en el informe Utilización difieren de los ingresos planificados que se muestran en el área Detalles del proyecto y en los informes del proyecto. </p> <p>Los ingresos planificados en el área de Detalles del proyecto reflejan los ingresos de la tarea así como los ingresos fijos del proyecto. Los ingresos planificados en el informe Utilización muestran los ingresos planificados asociados únicamente a las tareas del proyecto. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>Si el proyecto tiene 1 tarea con 10 horas asignada a un consultor con una tasa horaria de 20 dólares y el proyecto tiene 100 dólares de ingresos fijos, el informe Utilización muestra 200 dólares para los ingresos planificados (los ingresos planificados asociados con las horas de la tarea). La sección Detalles del proyecto muestra 300 dólares (los ingresos planificados de la tarea y los ingresos fijos del proyecto). </p> 
     </div> <p>Para obtener más información sobre los ingresos planificados de la tarea y del proyecto fuera del informe Utilización, consulte <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</p> </p> <p>La forma en que el informe Utilización calcula y muestra los ingresos planificados para los proyectos incluidos tiene en cuenta el tipo de ingresos establecido en la tarea. </p> <p>Según el tipo de ingresos de cada tarea del proyecto, existen los siguientes escenarios: </p> <p><strong>Ingresos fijos:</strong> independientemente de las asignaciones de tareas, los ingresos de la tarea siempre se calculan utilizando el importe fijo especificado en la tarea.</p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los ingresos planificados para las tareas de ingresos fijos dividiendo los ingresos fijos equitativamente por el número de horas planificadas en la tarea. </p> <p>Por ejemplo, una tarea tiene unos ingresos de 200 dólares. Si hay 4 horas planificadas en la tarea, cada hora sería 50 dólares. Esto se distribuye en el nivel de usuario y función. Esta distribución es exclusiva del informe Utilización.</p> <p><b>NOTA</b>

Si tiene una tarea de ingresos fijos y no hay horas planificadas para la tarea, los ingresos no se mostrarán en el informe Utilización porque no hay forma de distribuirlos entre las horas. Si tiene horas planificadas en las tareas con ingresos fijos y ninguna asignación, los ingresos se mostrarán como ingresos sin asignar. </p> <p><strong>Función por hora:</strong> los ingresos de la tarea se calculan usando la tarifa de facturación establecida para un rol específico, multiplicada por el número de horas planificadas asociadas con ese rol. Workfront utiliza la fórmula siguiente:</p> <p><code>Ingresos planificados por rol por hora = SUMA (horas planificadas del rol en todas las tareas) * Tarifa de facturación del rol</code></p><p><b>NOTA:</b> La tarifa de facturación por hora de la fórmula tiene en cuenta cualquier cambio de la fecha en vigor de la tarifa.</p>   <p><strong>Usuario por hora:</strong> los ingresos de la tarea se calculan usando la tarifa de facturación establecida para un usuario específico, multiplicada por el número de horas planificadas asociadas con ese usuario. Workfront utiliza la fórmula siguiente:</p> <p><code>Ingresos planificados por usuario por hora = SUMA (horas planificadas de los usuarios en todas las tareas) * Tarifa de facturación de usuario</code> </p> <p><b>NOTA:</b> La tarifa de facturación por hora de la fórmula tiene en cuenta cualquier cambio de la fecha en vigor de la tarifa.</p> <p><b>Rol por hora más fijos o Usuario por hora más fijos</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los ingresos planificados, dividiendo los ingresos fijos de forma uniforme por el número de horas planificadas de la tarea. </p> <p>Se dan los siguientes casos: </p>
<ul>
<li> <p><strong>Función por hora más fijo:</strong> los ingresos de la tarea se calculan usando la tarifa de facturación establecida para una función específica, multiplicada por el número de horas planificadas asociadas con la función. Además, se añade a la tarifa de usuario una cantidad fija especificada en la tarea. Workfront utiliza la fórmula siguiente:</p> <p><code>Función por hora más ingresos planificados fijos = [SUMA(Horas planificadas de la función en todas las tareas) * Tasa de facturación de la función] + SUMA(Importe límite o fijo de la tarea/Horas planificadas de la tarea)</code> </p> </li>
<li> <p><strong>Usuario por hora más fijos:</strong> la tarifa de facturación establecida para un usuario específico, multiplicada por el número de horas planificadas en la tarea de ese usuario. Además, se añade a la tarifa de usuario una cantidad fija especificada en la tarea. Workfront utiliza la fórmula siguiente:</p> <p><code>Usuario por hora más ingresos planificados fijos = [SUMA(Horas planificadas del usuario en todas las tareas) * Tarifa de facturación del usuario] + SUMA(Importe límite o fijo de la tarea/Horas planificadas de la tarea)</code> </p> </li>
</ul> <p><b>Función o usuario por hora con límite</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, si los ingresos planificados superan el límite, el importe por encima del importe del límite se considera ingresos fijos. Los ingresos planificados se calculan dividiendo los ingresos fijos de forma equitativa por el número de horas planificadas en la tarea y, a continuación, añadiéndole el importe del límite y los ingresos por hora del usuario o función. <br></p> <p>Se dan los siguientes casos: </p>
<ul>
<li> <p><strong>Función por hora con límite:</strong> las tareas se facturan por hora como en Función por hora, pero tienen un límite máximo que puede especificar. Workfront utiliza la fórmula siguiente:</p> <p><code>Función por hora con ingresos planificados con límite = [SUMA(Horas planificadas de la función en todas las tareas y problemas) * Tasa de facturación de la función] + Importe límite de la tarea + SUMA(Importe que excede el importe de límite/Horas planificadas de la tarea)</code> </p> </li>
<li> <p><strong>Usuario por hora con límite:</strong> las tareas se facturan por hora como en Usuario por hora, pero tienen un límite máximo que puede especificar. Workfront utiliza la fórmula siguiente: </p> <p><code>Usuario por hora con ingresos planificados con límite = [SUMA(Horas planificadas del usuario en todas las tareas) * Tasa de facturación de usuario] + Importe límite de la tarea + SUMA(Importe que excede el importe de límite/Horas planificadas de la tarea)</code> </p> </li>
</ul> <p>Para obtener más información sobre qué función o usuario se tiene en cuenta al calcular los ingresos planificados, consulte <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>Ingresos reales</strong> </td>
   <td> <p>Los ingresos reales son los ingresos asociados con las horas reales de las tareas y del proyecto. Para obtener más información sobre los ingresos reales, consulte <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#track-revenue-amounts">Rastrear importes de ingresos</a> en <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md">Información general sobre facturación e ingresos</a>.</p>

<p>La forma en que el informe Utilización calcula los ingresos reales de los proyectos incluidos difiere según el tipo de ingresos establecido en la tarea, de la siguiente manera:</p> <p><strong>Ingresos fijos:</strong> independientemente de las asignaciones de tareas, los ingresos de la tarea siempre se calculan utilizando el importe fijo especificado en la tarea.</p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los ingresos reales dividiendo los ingresos fijos de forma uniforme por el número de horas registradas en la tarea. </p> <p> </p> <p>Por ejemplo, una tarea tiene unos ingresos reales de 200 $. Si hay 4 horas reales en la tarea, cada hora sería 50 $. Esto se distribuye en el nivel de usuario y función. Esta distribución es exclusiva del informe Utilización.</p> <p><b>NOTA</b>

Si tiene una tarea de ingresos fijos y no hay horas reales en la tarea, los ingresos reales no se mostrarán en el informe Utilización porque no hay forma de distribuirlos entre las horas. </p> <p><strong>Función por hora:</strong> los ingresos de la tarea se calculan usando la tarifa de facturación establecida para una función específica, multiplicada por el número de horas reales.</p> <p>Workfront utiliza la fórmula siguiente:</p> <p><code>Función por hora con ingresos reales = SUMA(horas reales de las funciones en todas las tareas) * Tarifa de facturación de función</code> </p> <p><b>NOTA:</b> La tarifa de facturación por hora de la fórmula tiene en cuenta cualquier cambio de la fecha en vigor de la tarifa.</p> <p><strong>Usuario por hora:</strong> los ingresos de la tarea se calculan usando la tarifa de facturación establecida para un usuario específico, multiplicada por el número de horas registradas en la tarea de ese usuario. Workfront utiliza la fórmula siguiente:</p> <p><code>Hora de usuario con ingresos reales = SUMA(horas reales de usuario en todas las tareas) * Tarifa de facturación de usuario</code></p> <p><b>NOTA:</b> La tarifa de facturación por hora de la fórmula tiene en cuenta cualquier cambio de la fecha en vigor de la tarifa.</p> <p><b>Función o usuario por hora más fijos</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los ingresos reales dividiendo los ingresos fijos de forma uniforme por el número de horas registradas en la tarea. </p> <p>Se dan los siguientes casos: </p>
<ul>
<li> <p><strong>Función por hora más fijos:</strong> la tarifa de facturación establecida para una función específica, multiplicada por el número de horas registradas en la tarea de un usuario con esa función. Además, se añade a la tarifa de usuario una cantidad fija especificada en la tarea. </p> <p>Workfront utiliza la fórmula siguiente:</p> <p><code>Función por hora más ingresos reales fijos = [SUMA(Horas reales de la función en todas las tareas) * Tarifa de facturación de la función] + SUMA(Importe límite o fijo de la tarea/Horas reales de la tarea)</code> </p> </li>
<li> <p><strong>Usuario por hora más fijos:</strong> la tarifa de facturación establecida para un usuario específico, multiplicada por el número de horas registradas en la tarea de ese usuario. Además, se añade a la tarifa de usuario una cantidad fija especificada en la tarea. </p> <p>Workfront utiliza la fórmula siguiente:</p> <p><code>Usuario por hora más ingresos reales fijos = [SUMA(Horas reales de la función en todas las tareas) * Tarifa de facturación del usuario] + SUMA(Importe límite o fijo de la tarea/Horas del usuario de la tarea)</code> </p> </li>
</ul> <p><b>Función o usuario por hora con límite</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, si los ingresos planificados superan el límite, el importe por encima del importe del límite se considera ingresos fijos. Los ingresos planificados se calculan dividiendo los ingresos fijos de forma equitativa por el número de horas planificadas en la tarea y, a continuación, añadiéndole el importe del límite y los ingresos por hora del usuario o función. <br></p> <p>Se dan los siguientes casos:</p>
<ul>
<li> <p><strong>Función por hora con límite:</strong> las tareas se facturan por hora como en Función por hora, pero tienen un límite máximo que puede especificar. Workfront utiliza la fórmula siguiente:</p> <p><code>Función por hora con límite de ingresos reales = [SUMA(Horas reales de la función en todas las tareas y problemas) * Tarifa de facturación de la función] + Importe límite de la tarea + SUMA(Importe que excede del importe límite/Horas reales de la tarea)</code></p> </li>
<li> <p><strong>Usuario por hora con límite:</strong> las tareas se facturan por hora como en Usuario por hora, pero tienen un límite máximo que puede especificar.</p> <p> Workfront utiliza la fórmula siguiente:</p> <p><code>Usuario por hora con límite de ingresos reales = [SUMA(Horas reales de la función en todas las tareas y problemas) * Tarifa de facturación de usuario] + Importe límite de la tarea + SUMA(Importe que excede del importe límite/Horas reales de la tarea)</code> </p> </li>
</ul>
<p><strong>Ingresos del proyecto</strong>: los ingresos asociados con las horas registradas en el proyecto se calculan teniendo en cuenta la cantidad de Facturación por hora de la función principal del usuario que registra el tiempo. No se recomienda registrar el tiempo en el proyecto. </p>
<p><b>NOTA</b>

Si el usuario no está asociado a una función o si la facturación por hora de la función principal es cero, Workfront calcula los ingresos reales utilizando la cantidad de facturación por hora para el usuario. Si el usuario no tiene un importe de facturación por hora en su perfil, los ingresos reales son cero. </p>
</td> 
  </tr> 
  <tr> 
   <td><strong>Variación presupuestada (para ingresos)</strong> </td> 
   <td> <p>Ingresos reales totales, menos ingresos presupuestados en los proyectos incluidos.<br>Puede ver la variación presupuestada total para la duración total de los proyectos incluidos o puede ver la variación presupuestada total solo para el intervalo de fechas especificado (puede especificar una semana o un mes concretos).</p> <p>Si el valor es positivo, se muestra en verde. Esto indica que los ingresos presupuestados totales son mayores que los ingresos reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que los ingresos presupuestados totales son menores que los ingresos reales.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Variación planificada (para ingresos)</strong> </td> 
   <td> <p>Ingresos reales totales menos los ingresos planificados totales en los proyectos incluidos.<br>Puede ver la variación total planificada para la duración total de los proyectos incluidos o puede ver la variación total planificada solo para el intervalo de fechas especificado (puede especificar una semana o un mes concretos). </p> <p>Si el valor es positivo, se muestra en verde. Esto indica que los ingresos planificados totales son mayores que los ingresos reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que los ingresos planificados totales son menores que los ingresos reales.</p> </td>
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### Comparación de los ingresos con los costes planificados y reales {#compare-revenue-against-planned-and-actual-costs}

Puede ver el coste planificado o real junto con los ingresos planificados. También se muestra el margen (%) (el margen se calcula como Ingresos - Coste / Ingresos).

La siguiente información está disponible en el informe de utilización al comparar los ingresos con los costes planificados y reales:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Título de columna al ver ingresos frente a costes (planificados)</strong> </th> 
   <th> <strong>Función</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Coste planificado</strong> </td> 
   <td scope="col"> Coste total planificado de los proyectos incluidos. Puede ver el coste total planificado para la vida útil general de los proyectos incluidos o puede ver el coste total planificado solamente para el intervalo de fechas especificado (puede especificar una semana o mes concretos). </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ingresos planificados</strong> </td> 
   <td scope="col"> <p>Ingresos planificados son los ingresos asociados con las horas planificadas de las tareas. </p> <p>La forma en que el informe de utilización calcula y muestra los ingresos planificados para los proyectos incluidos difiere según el tipo de ingresos configurado en la tarea, como se describe en la sección <a href="#track-revenue" class="MCXref xref">Seguimiento de ingresos</a> de este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Margen</strong> </td> 
   <td scope="col"> <p>El porcentaje de margen se calcula de la siguiente manera:</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>NOTA</b>

Si los ingresos planificados son iguales a 0, el margen se muestra como 0. </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>Título de columna al ver ingresos frente a costes (reales)</strong> </p>  </td> 
   <td scope="col"><p><strong>Función</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Coste real</strong> </td> 
   <td scope="col"> <p>Coste real total de los proyectos incluidos. Puede ver el coste real total de la vida útil general de los proyectos incluidos o puede ver el coste real total solamente para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ingresos reales</strong> </td> 
   <td> <p>Los ingresos reales son los ingresos asociados con las horas reales de las tareas.</p> <p>Los ingresos reales solo se muestran en el informe de utilización una vez que la tarea se ha marcado como Finalizada o Listo (o un estado que equivale a Finalizada).</p> <p>La forma en que el informe de utilización calcula los ingresos reales de los proyectos incluidos depende del tipo de ingresos establecido en la tarea, tal como se describe en la sección <a href="#track-revenue" class="MCXref xref">Seguimiento de ingresos</a> de este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Margen</strong> </td> 
   <td> <p>El porcentaje de margen se calcula de la siguiente manera:</p> <p>Ingresos reales - Coste real/Ingresos reales x 100. </p> <p><b>NOTA</b>

Si los ingresos reales son iguales a 0, el margen se muestra como 0. </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## Realice un seguimiento del progreso, el coste y los ingresos con el informe de utilización {#track-progress-cost-and-revenue-with-the-utilization-report}

Puede realizar un seguimiento del progreso o el coste de un proyecto, programa o portafolio.

Puede mostrar información sobre el informe de utilización de una semana o mes determinados, o sobre la duración total de los proyectos.

Para realizar un seguimiento del progreso o el coste de uno o más proyectos con un informe de utilización:

1. Realice una de las siguientes acciones, en función de si está viendo la información de utilización de un proyecto individual, varios proyectos, un programa o un portafolio:

   * Para ver la información de utilización de un solo proyecto:

      1. Vaya a un proyecto cuya información de utilización desee ver y, a continuación, haga clic en **Utilización** en el panel izquierdo.
      1. La información de utilización se muestra automáticamente cuando se visualiza un proyecto individual y no es necesario aplicar un filtro.\
         Si desea filtrar el informe de utilización, puede aplicar un filtro y luego hacer clic en **Ejecutar**.\
         Para obtener información sobre cómo filtrar el informe de utilización, consulte [Filtrar información de utilización](#filter-utilization-information) en este artículo.\
         La información de utilización se muestra para usuarios y funciones individuales (los usuarios se agrupan dentro de su función asociada).

   * Para ver la información de utilización de varios proyectos:

     {{step1-to-utilization-report}}

      1. Aplique un filtro al informe de utilización y, a continuación, haga clic en **Ejecutar**.
Debe especificar uno o varios proyectos en el filtro antes de ejecutar el informe de utilización. Para obtener información sobre cómo filtrar el informe de utilización, consulte [Filtrar información de utilización](#filter-utilization-information) en este artículo.\
         La información de utilización se muestra para funciones y proyectos individuales (las funciones se agrupan dentro de su proyecto asociado).

   * Para ver la información de utilización de un programa:

     {{step1-to-utilization-report}}

      1. Haga clic en **Mostrar**>**Programas**.
      1. Aplique un filtro al informe de utilización y, a continuación, haga clic en **Ejecutar**.\
         Debe especificar uno o más programas en el filtro antes de ejecutar el informe de utilización. Para obtener información sobre cómo filtrar el informe de utilización, consulte [Filtrar información de utilización](#filter-utilization-information) en este artículo.\
         La información de utilización se muestra para proyectos y programas individuales (los proyectos se agrupan dentro de su programa asociado).

   * Para consultar la información de utilización de un portafolio:

     {{step1-to-utilization-report}}

      1. Haga clic en **Mostrar**>**Portafolio**.
      1. Aplique un filtro al informe de utilización y, a continuación, haga clic en **Ejecutar**.\
         Debe especificar uno o más portafolios en el filtro antes de ejecutar el informe de utilización. Para obtener información sobre cómo filtrar el informe de utilización, consulte [Filtrar información de utilización](#filter-utilization-information) en este artículo.\
         La información de utilización se muestra para proyectos, programas y portafolios individuales (los proyectos se agrupan dentro de su programa asociado y los programas se agrupan dentro de su portafolio asociado).

1. En la esquina superior derecha del informe de utilización, haga clic en **Ver** y, a continuación, seleccione una de las siguientes opciones en el menú:

   * **Coste**
   * **Horas**
   * **Ingresos**
   * **Ingresos frente a costes (planificados)**
   * **Ingresos frente a costes (reales)**

   La opción que seleccione determina qué columnas e información están disponibles en el informe.
   ![Ver opciones](assets/utilization-view-dropdown.png)

1. (Opcional) Seleccione el intervalo de fechas para el que se muestra la información de utilización. Puede mostrar información de una semana o mes determinados a la izquierda de la columna **General**. La información general del proyecto, programa o portafolio siempre se muestra en la columna **General**.\
   Para obtener más información, consulte [Ajustar el intervalo de fechas para el que se muestra información](#adjust-the-date-range-for-which-information-is-displayed) en este artículo.

1. (Opcional) Haga clic en cualquier título de columna para ordenar el informe de utilización por la información de esa columna. La ordenación solo funciona cuando se incluyen varios elementos en el informe. Por ejemplo, puede ordenar los resultados del informe cuando esté viendo más de un proyecto (o portafolio o programa). No puede ordenar los resultados cuando solo está viendo un proyecto (o un portafolio o un programa) a la vez.
1. Use la información de la sección [Información general sobre el informe de utilización](#overview-of-the-utilization-report) de este artículo para obtener información sobre cada columna del informe de utilización.

## Filtrar información de utilización {#filter-utilization-information}

Puede filtrar el contenido que se muestra en un informe de utilización de un proyecto. Puede filtrar por tareas, problemas, funciones y datos personalizados. Al aplicar un filtro, el informe de utilización contiene información basada en los criterios seleccionados.

Puede crear un nuevo filtro o aplicar un filtro que haya creado anteriormente.

### Creación o modificación de un filtro {#create-or-modify-a-filter}

Al crear un filtro, todos los usuarios de Workfront que tienen acceso al informe de utilización también tienen acceso al filtro que cree. Del mismo modo, cuando se modifica un filtro existente, este se modifica para todos los usuarios que tengan acceso al informe de utilización.

Para crear o modificar un filtro:

1. Abra el informe de utilización.
Consulte [Seguimiento del progreso, los costes y los ingresos con el informe de utilización](#track-progress-cost-and-revenue-with-the-utilization-report) para hacerlo.

1. Haga clic en el icono **Filtro** para mostrar las opciones de filtro.
1. (Condicional) Para modificar un filtro existente, haga clic en el menú desplegable **Filtro** y, a continuación, seleccione el filtro que desee modificar.
1. Especifique la siguiente información para crear o modificar el filtro:

   * **Portafolios:** empiece a escribir el nombre del portafolio que contiene la información que desea incluir en el informe de utilización y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable\
     Repita este proceso para incluir información de varios portafolios en el informe de utilización.\
     Para incluir todos los portafolios del sistema en el filtro, haga clic en **Añadir todo**. (Esta opción solo está disponible si tiene menos de 10 portafolios en el sistema).

   * **Programas:** escriba el nombre del programa que contiene la información que desea incluir en el informe de utilización y, a continuación, haga clic en el nombre en la lista desplegable.\
     Repita este proceso para incluir información de varias tareas en el informe de utilización.\
     Si ya ha designado portafolios en el filtro, el programa que especifique debe proceder de los portafolios ya incluidos en el filtro. Si no es así, los datos del programa no se incluyen en el informe de utilización.\
     Para incluir todos los programas del sistema en el filtro, haga clic en **Añadir todo**. (Esta opción solo está disponible si tiene menos de 20 programas en el sistema).

   * **Proyectos:** escriba el nombre del proyecto que contiene la información que desea incluir en el informe de utilización y, a continuación, haga clic en el nombre en la lista desplegable.\
     Repita este proceso para incluir información de varios proyectos en el informe de utilización.\
     Si ya ha designado portafolios o programas en el filtro, el proyecto que especifique debe pertenecer a uno de los portafolios o programas ya incluidos en el filtro. Si no es así, los datos del proyecto no se incluyen en el informe de utilización.\
     Para incluir todos los proyectos del sistema en el filtro, haga clic en **Añadir todo**. (Esta opción solo está disponible si tiene menos de 250 proyectos en el sistema).

   * **Tareas:** escriba el nombre de la tarea que contiene la información que desea incluir en el informe de utilización y, a continuación, haga clic en el nombre en la lista desplegable.\
     Repita este proceso para incluir información de varias tareas en el informe de utilización.\
     Si ya ha designado portafolios, programas o proyectos en el filtro, la tarea que especifique debe proceder de uno de los portafolios, programas o proyectos ya incluidos en el filtro. Si no es así, los datos de la tarea no se incluyen en el informe de utilización.

   * **Problemas:** escriba el nombre del problema que contiene la información que desea incluir en el informe de utilización y, a continuación, haga clic en el nombre en la lista desplegable.\
     Repita este proceso para incluir información de varios problemas en el informe de utilización.\
     Si ya ha designado portafolios, programas o proyectos en el filtro, el problema que especifique debe ser de uno de los portafolios, programas o proyectos ya incluidos en el filtro. Si no es así, los datos del problema no se incluyen en el informe de utilización.\
     La información de costes de los problemas no siempre se incluye en el informe de utilización. Para obtener más información sobre cuándo se incluye la información de costes de los problemas en el informe de utilización, consulte [Seguimiento del progreso, los costes y los ingresos con el informe de utilización](#track-progress-cost-and-revenue-with-the-utilization-report) en este artículo.

   * **Funciones:** escriba el nombre de la función que desea que se represente en el informe de utilización y, a continuación, haga clic en el nombre en la lista desplegable. Repita este proceso para incluir funciones adicionales.
El Informe de utilización contiene información solo sobre las funciones especificadas. Por ejemplo, una tarea contiene 10 horas reales. Seis de esas horas son de una función de Diseñador y cuatro de una función de Desarrollador. Si filtra el Informe de utilización por función para Diseñador, las cuatro horas que proceden de la función Desarrollador se excluyen del informe.

   * **Agregar regla de filtro:** haga clic en **Agregar regla de filtro**, haga clic en el campo de texto y empiece a escribir el nombre del campo por el que desea filtrar. Si el campo está disponible, se rellena para cada objeto donde se puede asociar. Haga clic en el nombre del campo para añadirlo al filtro.

     >[!IMPORTANT]
     >
     >Debe escribir el nombre del campo y no la etiqueta del campo. La etiqueta de campo se muestra en un formulario personalizado adjunto a un objeto. Para obtener información acerca de la diferencia entre la etiqueta y el nombre de un campo personalizado, vea [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

     Para obtener más información sobre los campos que se ven en las columnas, consulte [Glosario de terminología de Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
     Elija los modificadores de filtro y condición para el filtro. Los modificadores disponibles se describen en [Modificadores de filtro y condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Para crear un nuevo filtro, haga clic en **Guardar filtro**.\
   O\
   Para modificar un filtro existente, haga clic en la flecha situada junto al botón **Guardar filtro** y, a continuación, haga clic en **Guardar nuevo filtro**.
En el campo **Nombre del filtro**, escriba un nombre para el filtro y haga clic en **Guardar**.
El área Utilización se filtra con la información incluida en el filtro.

### Aplicar un filtro guardado {#apply-a-saved-filter}

1. Abra el informe de utilización.
Consulte [Seguimiento del progreso, los costes y los ingresos con el informe de utilización](#track-progress-cost-and-revenue-with-the-utilization-report) para hacerlo.

1. Haga clic en **Filtros guardados** y, a continuación, seleccione el filtro que desee aplicar en la lista desplegable.

### Duplicar un filtro {#duplicate-a-filter}

1. Abra el informe de utilización.
Consulte [Seguimiento del progreso, los costes y los ingresos con el informe de utilización](#track-progress-cost-and-revenue-with-the-utilization-report) para hacerlo.

1. Haga clic en **Filtros guardados**, pase el puntero por encima del filtro que quiere duplicar y haga clic en el icono **Duplicar**.

   ![Icono duplicado](assets/utilization-filter-duplicate.png)

   Se muestra el cuadro de diálogo Duplicar filtro.

1. En el campo **Nombre del filtro**, escriba un nombre para el nuevo filtro y haga clic en **Guardar**.

### Cambiar el nombre de un filtro {#rename-a-filter}

Al cambiar el nombre de un filtro, todos los usuarios de Workfront que tengan acceso al informe de utilización verán el nuevo nombre introducido.

Para cambiar el nombre de un filtro, haga lo siguiente:

1. Abra el informe de utilización.
Consulte [Seguimiento del progreso, los costes y los ingresos con el informe de utilización](#track-progress-cost-and-revenue-with-the-utilization-report) para hacerlo.

1. Haga clic en **Filtros guardados**, pase el puntero por encima del filtro cuyo nombre desea cambiar y haga clic en el icono **Cambiar nombre**.

   ![Cambiar el nombre del icono de filtro](assets/utilization-filter-rename.png)

   Aparece el cuadro de diálogo Cambiar el nombre de un filtro.

1. En el campo **Nombre del filtro**, escriba un nombre para el nuevo filtro y haga clic en **Guardar**.

### Eliminación de un filtro {#delete-a-filter}

Al eliminar un filtro, este se elimina para todos los usuarios de Workfront que tengan acceso al informe de utilización.

Para eliminar un filtro, haga lo siguiente:

1. Abra el informe de utilización.
Consulte [Seguimiento del progreso, los costes y los ingresos con el informe de utilización](#track-progress-cost-and-revenue-with-the-utilization-report) para hacerlo.

1. Haga clic en **Filtros guardados**, pase el puntero por encima del filtro que quiere eliminar y haga clic en el icono **Eliminar**.

   ![Icono Eliminar](assets/utilization-filter-delete.png)

1. Haga clic en **Eliminar** cuando se le pregunte si desea eliminar el filtro.

## Ajuste el intervalo de fechas para el que se muestra información {#adjust-the-date-range-for-which-information-is-displayed}

Puede ajustar el intervalo de fechas para el que se muestra la información de utilización. Puede seleccionar una fecha pasada o futura. Nadie más podrá ver los cambios que realice.

1. Abra el informe de utilización.
Consulte [Realizar un seguimiento del progreso, los costes y los ingresos con el informe de utilización](#track-progress-cost-and-revenue-with-the-utilization-report) para hacerlo.

1. Haga clic en el intervalo de fecha que está junto al botón **Exportar**.

   La semana actual está seleccionada de forma predeterminada.

1. Elija entre las siguientes opciones:

   * **Semana:** seleccione esta opción para seleccionar una semana determinada (de domingo a sábado).
   * **Mes:** seleccione esta opción para seleccionar un mes determinado.

   El intervalo de fecha que seleccione se mostrará en el informe de utilización, a la izquierda de la columna **Global**.\
   Workfront recuerda si desea ver una vista de semana o de mes. La próxima vez que acceda al informe de utilización, se mostrará la semana o el mes actuales, según la opción que seleccione.

## Exportar información de utilización

Puede exportar información de utilización de un proyecto, programa o portafolio desde Workfront. La información solo se puede exportar en los formatos XLSX, TSV y PDF.

Cuando se ven en Microsoft Excel, los números negativos se muestran entre paréntesis.

Para exportar información de utilización, haga lo siguiente:

1. Abra el informe de utilización.
Consulte [Realizar un seguimiento del progreso, los costes y los ingresos con el informe de utilización](#track-progress-cost-and-revenue-with-the-utilization-report) para hacerlo.

1. Haga clic en **Exportar** en la parte superior izquierda del informe.

1. Seleccione entre las siguientes opciones:

   * **PDF:** exporta el informe en formato PDF. Este es el formato recomendado si planea imprimir el informe.\
     Seleccione **Carta - Vertical**, **Carta - Horizontal** u **Otros tamaños** (proporciona opciones para exportar en Legal (8,5 x 14&quot;), Libro mayor (11 x 17&quot;) y A4).
Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el equipo.

   * **Excel:** exporta el informe en formato XLSX. Este es el formato recomendado si planea analizar más a fondo los datos en Excel.
Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el equipo.

   * **Delimitado por tabuladores:** exporta el informe en formato TSV. Este es el formato recomendado si planea importar los datos en software de terceros para un análisis más amplio.
Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el equipo.

1. Lea la información del artículo [Exportar datos](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) para saber cómo usar el archivo exportado.

## Ver información de utilización en un gráfico

Puede visualizar los datos del informe de utilización en una vista de gráfico.

1. Abra el informe de utilización.
Consulte [Realizar un seguimiento del progreso, los costes y los ingresos con el informe de utilización](#track-progress-cost-and-revenue-with-the-utilization-report) para hacerlo.

1. En la esquina superior derecha del informe de utilización, haga clic en el icono **Gráfico**.

   ![Icono del gráfico](assets/utilization-chart.png)

   El informe de utilización se mostrará en una vista de gráfico.

1. (Opcional) Para configurar el gráfico para mostrar proyectos, programas o portafolios, seleccione la opción adecuada en el menú desplegable **Mostrar**.
1. (Opcional) Pase el puntero por encima de un momento específico del informe para ver los datos de ese momento.

   ![Pase el puntero por encima de un punto de datos](assets/utilization-chart-hover.png)

1. (Opcional) Ajuste los filtros para cambiar la información que se muestra en el gráfico. Para obtener información acerca de cómo ajustar los filtros, consulte [Información sobre la utilización de filtros](#filter-utilization-information) en este artículo.
1. (Opcional) Configure el lapso de tiempo del informe de gráfico, tal como se describe en [Ajustar el intervalo de fecha para el cual se muestra la información](#adjust-the-date-range-for-which-information-is-displayed) en este artículo.
