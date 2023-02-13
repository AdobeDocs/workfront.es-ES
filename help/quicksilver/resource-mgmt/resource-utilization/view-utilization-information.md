---
product-area: resource-management
navigation-topic: resource-utilization
title: Ver información de utilización de recursos
description: Puede ver la utilización de sus recursos mediante el informe Utilización .
author: Alina
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '7758'
ht-degree: 0%

---

# Ver información de utilización de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

Puede ver la utilización de sus recursos mediante el informe Utilización .

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

Debe tener lo siguiente para acceder al informe de uso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver o acceso superior a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos </p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Portafolios</p> </li> 
     <li> <p>Programas</p> </li> 
     <li> <p>Datos financieros si desea ver la información por coste</p> </li> 
    </ul> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso a proyectos, portafolios y programas para acceder a la sección Utilización del área Recursos</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>Administrar el acceso al proyecto para acceder a la sección Utilización de un proyecto</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

Las secciones siguientes describen cómo ver y utilizar la información de utilización.

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

## Resumen del informe de utilización {#overview-of-the-utilization-report}

Con el informe Utilización puede ver el progreso, el coste o los ingresos de un proyecto, programa o portafolio en un solo informe. También puede comparar los ingresos con los costos.

Puede ver el informe Utilización en el área Recursos para mostrar la utilización en varios proyectos, o puede verlo en el nivel de un proyecto para mostrar la utilización de los recursos individuales (funciones de trabajo y usuarios) asociados a ese proyecto.

Para obtener información sobre el acceso y el uso del informe de uso, consulte la [Rastree el progreso, el coste y los ingresos con el informe de uso](#track-progress-cost-and-revenue-with-the-utilization-report) en este artículo.

* [Seguimiento de horas (progreso)](#track-hours-progress)
* [Seguimiento del coste](#track-cost)
* [Seguimiento de ingresos](#track-revenue)
* [Comparar ingresos con costes planificados y reales](#compare-revenue-against-planned-and-actual-costs)

### Seguimiento de horas (progreso) {#track-hours-progress}

Para realizar un seguimiento del progreso, consulte la comparación entre las horas presupuestadas y las programadas y las horas reales.

Al realizar un seguimiento del progreso de un proyecto, programa o portafolio, el progreso respecto a las tareas y los problemas se incluye en el informe Utilización.

La siguiente información está disponible en el informe de uso al rastrear horas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Título de columna al ver horas</strong> </th> 
   <th><strong>Función</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Horas presupuestadas</strong> </td> 
   <td scope="col"> <p>El total de horas presupuestadas para los proyectos incluidos. Puede ver el total de horas presupuestadas para la vida general de los proyectos incluidos o puede ver el total de horas presupuestadas solo para el intervalo de fechas especificado (puede especificar una semana o mes individual). </p> <p>Las horas presupuestadas se rellenan a partir de la información disponible en el nuevo área de Presupuestación de Recursos del Caso de Negocio o el Planificador de Recursos<em>.</em></p> <p>Las horas presupuestadas aparecen en el informe de utilización en cualquiera de las filas siguientes:</p> 
    <ul> 
     <li> Las horas presupuestadas se resumen por rol de trabajo y por usuario individual en el informe de uso de la siguiente manera:<br><strong>Usuario individual:</strong> Las horas presupuestadas se resumen para cada usuario en el informe de utilización. Estas horas presupuestadas están asociadas con las tareas y los problemas a los que se asigna al usuario en los proyectos incluidos. (Puede expandir la fila de la función de trabajo correspondiente para ver una lista de usuarios con esa función de trabajo).<br><strong>Función del trabajo:</strong> Las horas presupuestadas se resumen por función del trabajo en el informe de utilización.<br>Las horas presupuestadas aparecen en una función de trabajo particular como resultado de cualquiera de los siguientes escenarios: 
     <li>La función de trabajo se define como la función de trabajo principal del usuario que está asignado a la tarea o problema en el que está asociado el horario presupuestado. </li> 
       <li>Cuando se ve la información de utilización de un solo proyecto, se utiliza la función de trabajo del usuario asignado a las horas, ya sea que no haya asignación en la tarea o el problema, se asigna a otro usuario sin asignación de función de trabajo, se asigna a otro usuario con una función de trabajo diferente o se asigna otro equipo.</li> 
       <li>Cuando se ve la información de uso de varios proyectos, programas o portafolios, la función de trabajo del usuario asignado a las horas solo se utiliza cuando la función está asignada en una tarea o problema de un proyecto. </li> 
       <li>La función de trabajo se asigna a la tarea o problema que tiene asociado Horario presupuestado y el usuario asignado a la tarea o problema no tiene una función de trabajo definida en el sistema.</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>Horas no asignadas</strong>: Las horas presupuestadas se muestran en el informe de utilización de la sección Horas no asignadas cuando las horas presupuestadas están asociadas con una tarea o problema y no hay ningún usuario o función asignado a la tarea o problema.<br>Esta sección aparece únicamente cuando hay horas en el proyecto que coinciden con esta descripción y cuando se visualiza el informe de utilización por o desde un proyecto. </p> <p>Esta sección aparece únicamente cuando hay horas en el proyecto que coinciden con esta descripción y cuando se visualiza el informe de utilización por o desde un proyecto. </p> </li> 
    </ul> <p>Para obtener más información sobre las horas presupuestadas, consulte la sección "Localizar las horas presupuestadas de un proyecto" en la sección <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender el costo presupuestado del trabajo y las horas presupuestadas para los proyectos</a> artículo.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Horas planificadas</strong> </td> 
   <td scope="col"> <!-- Yay, no errors, warnings, or alerts! -->

<p>
El horario planificado de los proyectos incluidos que están asociados con las asignaciones de cada tarea y problema. Puede ver el total de horas planificadas de todas las asignaciones del proyecto durante toda la vida de los proyectos incluidos, o puede ver el total de horas planificadas solo para el intervalo de fechas especificado (puede especificar una semana o un mes concretos). 
</p>
<p>
<strong>SUGERENCIA </strong>
</p>
<p>
No se tienen en cuenta las horas planificadas de elementos con una duración de 0. 
</p>
<p>
Las horas planificadas en el informe Utilización tienen en cuenta si las horas planificadas se han reasignado a lo largo de la duración de una tarea o problema. 
</p>
<p>
Cuando se modifica la asignación diaria del usuario durante horas mediante el equilibrador de carga de trabajo, los datos del informe Utilización pueden verse afectados si las fechas seleccionadas en el informe Utilización contienen solo una parte de la duración de una tarea o de un problema. 
</p>
<p>
Para obtener información sobre cómo modificar las asignaciones para los usuarios, consulte <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">Administrar asignaciones de usuario en el equilibrador de carga de trabajo</a>.


</p>
<p>
Las horas planificadas aparecen en el informe Utilización en cualquiera de las filas siguientes:
</p>
<ul>

<li>Las horas planificadas se resumen por función del trabajo y por usuario individual en el informe de utilización de la siguiente manera: 
<ul>

<li><strong>Usuario individual</strong>: Las horas planificadas se resumen para cada usuario en el informe de utilización. Estas horas planificadas están asociadas con las tareas y los problemas a los que se asigna al usuario en los proyectos incluidos. (Puede expandir la fila de la función de trabajo correspondiente para ver una lista de usuarios con esa función de trabajo).

<li><strong>Función del trabajo</strong>: Las horas previstas se resumen por función del puesto en el informe de utilización de un solo proyecto.<br>Las horas programadas aparecen en una función de trabajo particular como resultado de cualquiera de los siguientes escenarios:  
<ul>

<li>La función de trabajo se define como la función de trabajo principal del usuario que está asignado a la tarea o problema en el que está asociado el horario planificado.

<li>Cuando se ve la información de utilización de un solo proyecto, las horas asociadas a una función de trabajo no se muestran para la función de trabajo en los siguientes escenarios:   
<ul>

<li>No hay asignación en la tarea o problema

<li>Se asigna un usuario sin asignación de función de trabajo

<li>A un usuario se le asigna una función de trabajo diferente

<li>Se asigna un equipo a la tarea o al problema
</li>   
</ul>

<li>Cuando se ve la información de uso de varios proyectos, programas o portafolios, la función de trabajo del usuario asignado a las horas solo se utiliza cuando la función está asignada en una tarea o problema de un proyecto. Las horas de rol de trabajo no se muestran por separado al ver el informe de uso de varios proyectos.

<li>La función de trabajo se asigna a la tarea o problema que tiene asociado Horario planificado y el usuario asignado a la tarea o problema no tiene una función de trabajo definida en el sistema.
</li>  
</ul>

<li><strong>Horas no asignadas</strong>: Las horas planificadas se muestran en el informe de utilización en la sección Horas no asignadas cuando las horas planificadas están asociadas a una tarea o problema y no hay ningún usuario o función asignado a la tarea o problema. Esta sección aparece únicamente cuando hay horas en el proyecto que coinciden con esta descripción y cuando se visualiza el informe de utilización para un solo proyecto. <br>Para obtener más información sobre las horas programadas, consulte <a href="../../manage-work/tasks/task-information/planned-hours.md">Información general sobre las horas planificadas</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Horas reales</strong> </td> 
   <td> <p> El número total de horas registradas en las tareas, los problemas, <span>y sobre el proyecto</span> para los proyectos incluidos. Puede ver el total de horas reales para la vida total de los proyectos incluidos o puede ver el total de horas reales solo para el intervalo de fechas especificado (puede especificar una semana o mes individual). </p> <p>Advertencia: El informe de utilización incluye las horas registradas en el proyecto, las tareas secundarias, los problemas y las tareas principales que tienen al menos una asignación. No incluye las horas registradas en tareas principales sin asignaciones. Se recomienda no utilizar tareas principales como tareas de trabajo y asignar solo tareas secundarias a los recursos. </p> <p>Las horas reales aparecen en el informe de utilización en cualquiera de las filas siguientes:</p> 
    <ul> 
     <li> Las horas reales se resumen por función del trabajo y por usuario individual en el informe de utilización de un proyecto, de la siguiente manera:<br><strong>Usuario individual:</strong> Las horas reales se muestran en el informe de utilización en la fila del usuario que registró las horas. (Puede expandir la fila de la función de trabajo correspondiente para ver una lista de usuarios con esa función de trabajo que han registrado horas).<br><strong>Función del trabajo:</strong> Las horas reales registradas por los usuarios asociados con esas funciones se resumen en el informe de utilización en la fila de la función de trabajo correspondiente.<br>Las horas reales aparecen en una función de trabajo particular como resultado de cualquiera de los siguientes escenarios: 
      <ul> 
       <li>La función de trabajo se define como la función de trabajo principal del usuario que registró las horas.</li> 
       <li>No hay asignación en la tarea o problema</li> 
       <li>A otro usuario se le asigna sin asignación de función de trabajo</li> 
       <li>A otro usuario se le asigna una función de trabajo diferente</li> 
       <li> <p>Se asigna un equipo.</p> </li> 
      </ul></li>  
     <p>Si el usuario que registra las horas no tiene una función de trabajo asociada con su perfil, la función de trabajo utilizada para el informe de utilización es la función de trabajo asignada a la tarea o problema en el que se registran las horas o la función de trabajo asociada con el propietario principal de la tarea o problema. </p> 
     <li><strong>Otras horas:</strong> Las horas reales se muestran en el informe de utilización en la sección Otras horas, en la fila del usuario que inició sesión en las horas.<br>Las horas aparecen en esta sección cuando el usuario que registró las horas no tiene una función de trabajo definida en el sistema.<br>Esta sección solo aparece cuando hay horas en el proyecto que coinciden con esta descripción. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Varianza presupuestada (para horas)</strong> </td> 
   <td> <p>El total de horas presupuestadas menos el total de horas reales en los proyectos incluidos. Puede ver la varianza presupuestada total para la vida total de los proyectos incluidos o puede ver la varianza presupuestada total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual). </p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de horas presupuestadas es bueno a las horas reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de horas presupuestadas es inferior al de horas reales.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Varianza planificada (para horas)</strong> </td> 
   <td> <p>El total de horas planificadas menos el total de horas reales en los proyectos incluidos. Puede ver la varianza planeada total para la vida general de los proyectos incluidos o puede ver la varianza planeada total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de horas planificadas es bueno a las horas reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de horas planificadas es inferior al de horas reales.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Seguimiento del coste {#track-cost}

Para realizar un seguimiento de los costes, consulte cómo se comparan los costes presupuestados y planeados con los costes reales.

Al rastrear el coste de un proyecto, programa o portafolio, la información en el informe Utilización proviene de las tareas. La información de costes de las tareas siempre está disponible en el informe de utilización. El coste de las tareas se calcula en función del tipo de coste de la tarea. Para obtener información sobre el tipo de coste de las tareas, consulte &quot;Modificación de tipos de coste para tareas individuales&quot; en [Seguimiento de costes](../../manage-work/projects/project-finances/track-costs.md).

Puede mostrar la información de coste en el informe de uso de las siguientes maneras:

* Para una semana o mes determinados, o para el proyecto, programa o portafolio en general.
* Por función o por persona, para proyectos.

La moneda utilizada en el informe de utilización está determinada por la moneda establecida en el proyecto. Para obtener información sobre cómo ajustar la moneda de un proyecto, consulte [Cambiar la moneda del proyecto](../../manage-work/projects/project-finances/change-project-currency.md).

La siguiente información está disponible en el informe de uso al rastrear el costo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Título de columna al visualizar el coste</strong> </th> 
   <th> <p><strong>Función</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Costo presupuestado</strong> </td> 
   <td scope="col"> <p>El costo presupuestado de los proyectos incluidos. Puede ver el total de Coste presupuestado para la duración total de los proyectos incluidos, o puede ver el total de Coste presupuestado solo para el intervalo de fechas especificado (puede especificar una semana o un mes individuales).</p> <p>Dado que el Coste presupuestado en el Informe de uso se centra en el coste por función, el cálculo es el mismo que el Coste de trabajo presupuestado en otras áreas de Workfront. Para obtener información sobre cómo se calcula el coste laboral presupuestado, consulte <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender el costo presupuestado del trabajo y las horas presupuestadas para los proyectos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Costo planificado</strong> </td> 
   <td scope="col"> <p>El coste total previsto de los proyectos incluidos. Puede ver el costo planeado total para la vida general de los proyectos incluidos o puede ver el costo planeado total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> <p>Para obtener información sobre cómo se calcula el coste planeado del proyecto, consulte la sección "Cómo calcula Workfront los costes planeados, presupuestados y reales" del artículo <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Costo real</strong> </td> 
   <td scope="col"> <p>Costo real total de los proyectos incluidos. Puede ver el costo real total para la vida total de los proyectos incluidos o puede ver el costo real total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> <p>Para obtener información sobre cómo se calcula el coste real del proyecto, consulte la sección "Cómo calcula Workfront los costes planeados, presupuestados y reales" del artículo <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Varianza presupuestada (para costo)</strong> </td> 
   <td scope="col"> <p>El costo presupuestado total menos el costo real total en los proyectos incluidos. Puede ver la varianza presupuestada total para la vida total de los proyectos incluidos o puede ver la varianza presupuestada total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el costo presupuestado total es bueno que el costo real.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el costo presupuestado total es menor que el costo real.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Varianza planificada (para costo)</strong> </td> 
   <td> <p>El costo planeado total menos el costo real total en los proyectos incluidos. Puede ver la varianza planeada total para la vida general de los proyectos incluidos o puede ver la varianza planeada total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual). </p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el costo planeado total es bueno que el costo real.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el costo planeado total es menor que el costo real.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Seguimiento de ingresos {#track-revenue}

Puede realizar un seguimiento de los ingresos consultando cómo se comparan los ingresos presupuestados y planeados con los ingresos reales.

Al rastrear los ingresos de un proyecto, programa o portafolio, los ingresos solo de las tareas se incluyen en el informe Utilización .

La información de la siguiente tabla está disponible en el informe de uso al rastrear los ingresos.

Para obtener información sobre los campos específicos y cómo los calcula Workfront, consulte también los siguientes artículos:

* [Seguimiento de costes](../../manage-work/projects/project-finances/track-costs.md)
* [Información general sobre facturación e ingresos](../../manage-work/projects/project-finances/billing-and-revenue-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Título de columna al visualizar ingresos</strong> </th> 
   <th> <strong>Función</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Ingresos presupuestados</strong> </td> 
   <td scope="col"> <p>El total de horas presupuestadas multiplicado por la tasa de facturación de funciones en los proyectos incluidos. Puede ver el total de ingresos presupuestados para la vida general de los proyectos incluidos o puede ver el total de ingresos presupuestados solo para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ingresos planificados</strong> </td> 
   <td scope="col"> <p>Los ingresos planeados en el informe de utilización son los ingresos asociados con las horas planificadas asignadas a los recursos asignados a las tareas del proyecto.</p> <p>Workfront calcula los ingresos previstos del proyecto para el informe de utilización mediante la fórmula siguiente:</p> <p><code>Project Planned Revenue = SUM&nbsp;(All Tasks Planned Revenue)</code> </p> 
   <p><b>NOTA</b>
   <p>Los ingresos planeados del proyecto que se muestran en el informe de utilización difieren de los ingresos planeados que se muestran en el área Detalles del proyecto y en los informes del proyecto. </p> <p>Los ingresos planeados del área Detalles del proyecto reflejan los ingresos de la tarea, así como los ingresos fijos del proyecto. En el Informe de uso, se muestran los ingresos planeados asociados únicamente a las tareas del proyecto. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>Si el proyecto tiene una tarea con 10 horas, asignada a un consultor con una tasa de 20 dólares por hora y el proyecto tiene 100 dólares de ingresos fijos, el informe de utilización muestra 200 dólares para ingresos planificados (los ingresos previstos asociados con las horas de la tarea). La sección Detalles del proyecto muestra 300 $ (los ingresos previstos de la tarea y los ingresos fijos del proyecto). </p> 
     </div> <p>Para obtener más información sobre la tarea y los ingresos planificados del proyecto fuera del informe de utilización, consulte <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</p> </p> <p>La forma en que el informe de utilización calcula y muestra los ingresos planeados para los proyectos incluidos tiene en cuenta el tipo de ingresos establecido en la tarea. </p> <p>Según el tipo de ingresos de cada tarea del proyecto, existen los siguientes escenarios: </p> <p><strong>Ingresos fijos:</strong> Independientemente de las asignaciones de tareas, los ingresos de la tarea siempre se calculan utilizando el importe fijo especificado en la tarea.</p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe de utilización calcula los ingresos planeados para las tareas de ingresos fijos dividiendo los ingresos fijos uniformemente por el número de horas planificadas en la tarea. </p> <p>Por ejemplo, una tarea tiene un ingreso de 200 dólares. Si hay 4 horas planificadas en la tarea, cada hora será de 50 dólares. Esto se distribuye a nivel de usuario y función. Esta distribución es única para el informe de uso.</p> <p><b>NOTA</b>

Si tiene una tarea de ingresos fijos y no hay horas planificadas para la tarea, los ingresos no se muestran en el informe de uso porque no hay forma de distribuirlos a las horas. Si tiene horas planificadas en tareas con ingresos fijos y sin asignaciones, los ingresos se muestran como ingresos no asignados. </p> <p><strong>Función por hora:</strong> Los ingresos de la tarea se calculan utilizando la tasa de facturación establecida para una función específica, multiplicada por el número de horas planificadas asociadas a dicha función. Workfront utiliza la fórmula siguiente:</p> <p>Rol Ingresos planificados por hora = SUM(Horario planificado desde el rol en todas las tareas) * Rol Tasa de Facturación</code></p> <p><strong>Por hora del usuario:</strong> Los ingresos de la tarea se calculan utilizando la tasa de facturación establecida para un usuario específico, multiplicada por el número de horas planificadas asociadas a ese usuario. Workfront utiliza la fórmula siguiente:</p> <p>Ingresos planificados por hora de usuario = SUM(Horario planificado por los usuarios en todas las tareas) * Tasa de facturación del usuario</code> </p> <p><b>Función por hora o usuario por hora más fijo</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe de utilización calcula los ingresos planeados dividiendo los ingresos fijos uniformemente por el número de horas planificadas en la tarea. </p> <p>Existen los siguientes casos: </p>
<ul>
<li> <p><strong>Función Por Hora Más Fijo:</strong> Los ingresos de la tarea se calculan utilizando la tasa de facturación establecida para una función específica, multiplicada por el número de horas planificadas asociadas a la función. Además, se agrega una cantidad fija especificada en la tarea a la tasa de rol. Workfront utiliza la fórmula siguiente:</p> <p>Rol por hora más ingresos planificados fijos = [SUM(Horario planificado desde la función en todas las tareas) * Tasa de facturación de funciones] + SUM(Importe fijo o límite de la tarea/Horario planificado de la tarea)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Usuario Por Hora Más Fijo:</strong> La tasa de facturación establecida para un usuario específico, multiplicada por el número de horas programadas en la tarea de ese usuario. Además, se agrega a la tasa de usuario una cantidad fija especificada en la tarea. Workfront utiliza la fórmula siguiente:</p> <p>Ingresos planificados por hora del usuario más ingresos fijos = [SUM(Horario planificado del usuario en todas las tareas) * Tasa de facturación del usuario] + SUM(Importe fijo o límite de la tarea/Horario planificado de la tarea)</code> </p> </li>
</ul> <p><b>Función o usuario por hora con límite</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, si los ingresos planeados exceden el límite, la cantidad por encima del importe del límite se considera ingresos fijos. Los ingresos planeados se calculan dividiendo los ingresos fijos uniformemente por el número de horas planificadas en la tarea y, a continuación, añadiendo a ellos el importe de límite y la función o los ingresos por hora del usuario. <br></p> <p>Existen los siguientes casos: </p>
<ul>
<li> <p><strong>Función por hora con límite:</strong> Las tareas se facturan por hora como en Función por hora, pero tienen un límite máximo que puede especificar. Workfront utiliza la fórmula siguiente:</p> <p>Función por hora con límite de ingresos previstos = [SUM(Horario planificado desde la función en todas las tareas y problemas) * Tasa de facturación de funciones] + Importe de límite de la tarea + SUMA(Importe sobre el importe de límite/Horas previstas de la tarea)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Usuario por hora con límite:</strong> Las tareas se facturan por hora como en Usuario por hora, pero tienen un límite máximo que puede especificar. Workfront utiliza la fórmula siguiente: </p> <p>Ingresos planificados por hora del usuario con límite = [SUM(Horario planificado del usuario en todas las tareas) * Tasa de facturación del usuario] + Importe de límite de la tarea + SUMA(Importe sobre el importe de límite/Horas previstas de la tarea)</code> </p> </li>
</ul> <p>Para obtener más información sobre la función o el usuario que se tiene en cuenta al calcular los ingresos previstos, consulte <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>Ingresos reales</strong> </td> 
   <td> <p>Ingresos reales es el ingreso asociado con las horas reales de las tareas. <span>y del proyecto</span>. Para obtener más información sobre los ingresos reales, consulte la sección "Seguimiento de ingresos" en el artículo <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a>.</p>

<p>La forma en que el informe de utilización calcula los ingresos reales de los proyectos incluidos difiere según el tipo de ingresos establecido en la tarea, de la siguiente manera:</p> <p><strong>Ingresos fijos:</strong> Independientemente de las asignaciones de tareas, los ingresos de la tarea siempre se calculan utilizando el importe fijo especificado en la tarea.</p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los ingresos reales dividiendo los ingresos fijos de manera uniforme por el número de horas registradas en la tarea. </p> <p> </p> <p>Por ejemplo, una tarea tiene un ingreso real de 200 dólares. Si hay 4 horas reales en la tarea, cada hora sería 50 dólares. Esto se distribuye a nivel de usuario y función. Esta distribución es única para el informe de uso.</p> <p><b>NOTA</b>

Si tiene una tarea de ingresos fijos y no hay horas reales en la tarea, los ingresos reales no se muestran en el informe de uso porque no hay forma de distribuir las horas. </p> <p><strong>Función por hora:</strong> Los ingresos de la tarea se calculan utilizando la tasa de facturación establecida para una función específica, multiplicada por el número de horas planificadas.</p> <p>Workfront utiliza la fórmula siguiente:</p> <p>Rol Ingresos por hora reales = SUM(Horario real desde el rol en todas las tareas) * Rol Tasa de Facturación</code> </p> <p><strong>Por hora del usuario:</strong> Los ingresos de la tarea se calculan utilizando la tasa de facturación establecida para un usuario específico, multiplicada por el número de horas registradas con la tarea de ese usuario. Workfront utiliza la fórmula siguiente:</p> <p>Ingresos reales por hora del usuario = SUM(Horario real del usuario en todas las tareas) * Tasa de facturación del usuario</code></p> <p><b>Función o usuario por hora más fijo</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los ingresos reales dividiendo los ingresos fijos de manera uniforme por el número de horas registradas en la tarea. </p> <p>Existen los siguientes casos: </p>
<ul>
<li> <p><strong>Función Por Hora Más Fijo:</strong> La tasa de facturación establecida para una función específica, multiplicada por el número de horas registradas en la tarea desde un usuario con esa función. Además, se agrega una cantidad fija especificada en la tarea a la tasa de rol. </p> <p>Workfront utiliza la fórmula siguiente:</p> <p>Rol por hora más ingresos reales fijos = [SUM(Horario real desde la función en todas las tareas) * Tasa de facturación de funciones] + SUM(Importe fijo o límite de la tarea/Horario real de la tarea)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Usuario Por Hora Más Fijo:</strong> La tasa de facturación establecida para un usuario específico, multiplicada por el número de horas registradas con la tarea de ese usuario. Además, se agrega a la tasa de usuario una cantidad fija especificada en la tarea. </p> <p>Workfront utiliza la fórmula siguiente:</p> <p>Ingresos reales por hora más fijos = [SUM(Horario real desde la función en todas las tareas) * Tasa de facturación del usuario] + SUM(Cantidad fija o máxima de la tarea/Horario de usuario de la tarea)</code> </p> </li>
</ul> <p><b>Función o usuario por hora con límite</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, si los ingresos planeados exceden el límite, la cantidad por encima del importe del límite se considera ingresos fijos. Los ingresos planeados se calculan dividiendo los ingresos fijos uniformemente por el número de horas planificadas en la tarea y, a continuación, añadiendo a ellos el importe de límite y la función o los ingresos por hora del usuario. <br></p> <p>Existen los siguientes escenarios:</p>
<ul>
<li> <p><strong>Función por hora con límite:</strong> Las tareas se facturan por hora como en Función por hora, pero tienen un límite máximo que puede especificar. Workfront utiliza la fórmula siguiente:</p> <p>Función por hora con límite de ingresos reales = [SUM(Horario real desde el rol en todas las tareas y problemas) * Tasa de Facturación de Rol] + Importe de límite de la tarea + SUMA(Importe sobre el importe de límite/horas reales de la tarea)</code></p> </li>
</ul>
<ul>
<li> <p><strong>Usuario por hora con límite:</strong> Las tareas se facturan por hora como en Usuario por hora, pero tienen un límite máximo que puede especificar.</p> <p> Workfront utiliza la fórmula siguiente:</p> <p>Ingresos reales por hora del usuario con límite = [SUM(Horario real desde el rol en todas las tareas y problemas) * Tasa de facturación del usuario] + Importe de límite de la tarea + SUMA(Importe sobre el importe de límite/horas reales de la tarea)</code> </p> </li>
</ul>
<div>
<p><strong>Ingresos del proyecto</strong>: Los ingresos asociados con las horas registradas en el proyecto se calculan teniendo en cuenta la cantidad de Facturación por hora de la función de trabajo principal del usuario que registra la hora. No se recomienda iniciar sesión en el proyecto. </p>
<p><b>NOTA</b>

Si el usuario no está asociado a una función de trabajo o si la Facturación por hora de la función principal es cero, Workfront calcula los ingresos reales utilizando la cantidad Facturación por hora para el usuario. Si el usuario no tiene una cantidad de Facturación por hora en su perfil, los ingresos reales son cero. </p>
</div> </td>
</tr> 
  <tr> 
   <td><strong>Varianza presupuestada (para ingresos)</strong> </td> 
   <td> <p>El total de ingresos reales menos ingresos presupuestados en los proyectos incluidos.<br>Puede ver la varianza presupuestada total para la vida total de los proyectos incluidos o puede ver la varianza presupuestada total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de ingresos presupuestados es bueno respecto a los ingresos reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de ingresos presupuestados es menor que el de ingresos reales.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Varianza planificada (para Ingresos)</strong> </td> 
   <td> <p>El total de ingresos reales menos el total de ingresos planeados en los proyectos incluidos.<br>Puede ver la varianza planeada total para la vida general de los proyectos incluidos o puede ver la varianza planeada total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual). </p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de ingresos planeados es bueno que el de ingresos reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de ingresos planeados es menor que el de ingresos reales.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### Comparar ingresos con costes planificados y reales {#compare-revenue-against-planned-and-actual-costs}

Puede consultar el Coste planeado o real junto con los Ingresos planeados. También se muestra el margen (%) (el margen se calcula como Ingresos - Coste/Ingresos).

La siguiente información está disponible en el informe de utilización cuando se comparan los ingresos con los costes planeados y reales:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Título de columna al visualizar ingresos frente a coste (planificado)</strong> </th> 
   <th> <strong>Función</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Costo planificado</strong> </td> 
   <td scope="col"> El coste total previsto de los proyectos incluidos. Puede ver el costo planeado total para la vida general de los proyectos incluidos o puede ver el costo planeado total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual). </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ingresos planificados</strong> </td> 
   <td scope="col"> <p>Ingresos planificados es el ingreso asociado con las horas planificadas de las tareas. </p> <p>La forma en que el informe de utilización calcula y muestra los ingresos planeados para los proyectos incluidos varía en función del tipo de ingresos establecido en la tarea, como se describe en la sección <a href="#track-revenue" class="MCXref xref">Seguimiento de ingresos</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Margen</strong> </td> 
   <td scope="col"> <p>El porcentaje de margen se calcula de la siguiente manera:</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>NOTA</b>

Si Ingresos planeados es igual a 0, el margen se muestra como 0. </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>Título de columna al visualizar ingresos frente a coste (real)</strong> </p>  </td> 
   <td scope="col"><p><strong>Función</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Costo real</strong> </td> 
   <td scope="col"> <p>Costo real total de los proyectos incluidos. Puede ver el costo real total para la vida total de los proyectos incluidos o puede ver el costo real total solo para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ingresos reales</strong> </td> 
   <td> <p>Los ingresos reales son los ingresos asociados con las horas reales de las tareas.</p> <p>Los ingresos reales se muestran en el informe de utilización solo después de que la tarea esté marcada como Completa o Listo (o un estado que coincida con Completada).</p> <p>La forma en que el informe de utilización calcula los ingresos reales de los proyectos incluidos difiere según el tipo de ingresos establecido en la tarea, como se describe en la <a href="#track-revenue" class="MCXref xref">Seguimiento de ingresos</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Margen</strong> </td> 
   <td> <p>El porcentaje de margen se calcula de la siguiente manera:</p> <p>Ingresos reales - Costo real / Ingresos reales * 100. </p> <p><b>NOTA</b>

Si Ingresos reales es igual a 0, el margen se muestra como 0. </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## Rastree el progreso, el coste y los ingresos con el informe de uso {#track-progress-cost-and-revenue-with-the-utilization-report}

Puede realizar un seguimiento del progreso o el coste de un proyecto, programa o portafolio.

Puede mostrar información sobre el informe de utilización de una determinada semana o mes, o sobre la duración total de los proyectos.

Para realizar un seguimiento del progreso o el coste de uno o más proyectos con un informe de uso:

1. Realice una de las siguientes acciones, en función de si está viendo la información de utilización de un proyecto individual, varios proyectos, un programa o un portafolio:

   * Para ver la información de uso de un solo proyecto:

      1. Vaya a un proyecto para el que desee ver la información de utilización y, a continuación, haga clic en **Mostrar más> Utilización**.
      1. La información de uso se muestra automáticamente al ver un proyecto individual y no es necesario aplicar un filtro.\
         Si desea filtrar el informe de uso, puede aplicar un filtro y luego hacer clic en **Ejecutar**.\
         Para obtener información sobre cómo filtrar el informe de uso, consulte la sección [Filtrar la información de utilización](#filter-utilization-information) en este artículo.\
         La información de uso se muestra para usuarios y funciones individuales (los usuarios se agrupan dentro de su función asociada).
   * Para ver la información de uso de varios proyectos:

      1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recurso**, luego **Utilización** en el panel izquierdo.
      1. Aplique un filtro al informe Utilización y haga clic en **Ejecutar**.\
         Debe especificar uno o más proyectos en el filtro antes de ejecutar el informe de uso. Para obtener información sobre cómo filtrar el informe de uso, consulte la sección [Filtrar la información de utilización](#filter-utilization-information) en este artículo.\
         La información de uso se muestra para funciones y proyectos individuales (las funciones se agrupan dentro de su proyecto asociado).
   * Para ver la información de utilización de un programa:

      1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recurso**, luego **Utilización** en el panel izquierdo y haga clic en el botón **Show**>**Programas**.
      1. Aplique un filtro al informe Utilización y haga clic en **Ejecutar**.\
         Debe especificar uno o más programas en el filtro antes de ejecutar el informe de uso. Para obtener información sobre cómo filtrar el informe de uso, consulte la sección [Filtrar la información de utilización](#filter-utilization-information) en este artículo.\
         La información sobre la utilización se muestra para proyectos y programas individuales (los proyectos se agrupan dentro de su programa asociado).
   * Para ver la información de utilización de un portafolio:

      1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recurso**, luego **Utilización** en el panel izquierdo y haga clic en **Show**>**Portfolio**.
      1. Aplique un filtro al informe Utilización y haga clic en **Ejecutar**.\
         Debe especificar uno o más portafolios en el filtro antes de ejecutar el informe de uso. Para obtener información sobre cómo filtrar el informe de uso, consulte la sección [Filtrar la información de utilización](#filter-utilization-information) en este artículo.\
         La información de uso se muestra para proyectos, programas y portafolios individuales (los proyectos se agrupan dentro de su programa asociado y los programas se agrupan dentro de su portafolio asociado).




1. En la esquina superior derecha del informe de utilización, haga clic en el botón **Ver** menú desplegable y, a continuación, seleccione una de las siguientes opciones:

   * **Costo**
   * **Horas**
   * **Ingresos**
   * **Ingresos contra costo (planificados)**
   * **Ingresos frente a costos (reales)**.

   La opción que seleccione determina qué columnas e información están disponibles en el informe. Para obtener más información sobre la información disponible en cada columna, consulte la tabla en el paso 5.\
   ![](assets/utilization-view-dropdown.png)

1. (Opcional) Seleccione el intervalo de fechas en el que se muestra la información de uso. Puede mostrar la información de una semana o mes determinados a la izquierda del **General** para abrir el Navegador. La información del proyecto, programa o portafolio general siempre se muestra en la **General** para abrir el Navegador.\
   Para obtener más información, consulte la sección [Ajustar el intervalo de fechas para el que se muestra la información](#adjust-the-date-range-for-which-information-is-displayed) en este artículo.

1. (Opcional) Haga clic en el título de cualquier columna para ordenar el informe de utilización según la información de esa columna. La ordenación solo funciona cuando se incluyen varios elementos en el informe. Por ejemplo, puede ordenar los resultados del informe cuando esté viendo más de un proyecto (o portafolio o programa). Los resultados no se pueden ordenar cuando se está viendo un solo proyecto (o un portafolio o un programa) a la vez.
1. Utilice la información de la sección [Resumen del informe de utilización](#overview-of-the-utilization-report) en este artículo para obtener más información sobre cada columna del informe Utilización.

## Filtrar la información de utilización {#filter-utilization-information}

Puede filtrar el contenido mostrado en un informe de uso de un proyecto. Puede filtrar por tareas, problemas, funciones y datos personalizados. Al aplicar un filtro al informe de utilización, el informe de utilización contiene información basada en los criterios seleccionados.

Puede crear un filtro o aplicar uno que haya creado anteriormente.

* [Crear o modificar un filtro](#create-or-modify-a-filter)
* [Aplicar un filtro guardado](#apply-a-saved-filter)
* [Duplicar un filtro](#duplicate-a-filter)
* [Cambiar el nombre de un filtro](#rename-a-filter)
* [Eliminar un filtro](#delete-a-filter)

### Crear o modificar un filtro {#create-or-modify-a-filter}

Al crear un filtro, todos los usuarios de Workfront que tengan acceso al informe de Utilización también tendrán acceso al filtro que cree. Del mismo modo, cuando se modifica un filtro existente, este se modifica para todos los usuarios que tengan acceso al informe Utilización.

Para crear o modificar un filtro:

1. Para filtrar la información de utilización de un solo proyecto, vaya al proyecto para el que desee filtrar la información de utilización y, a continuación, haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para filtrar la información de utilización de varios proyectos, de un programa o de un portafolio, haga clic en el icono del menú principal ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, **Recurso**, **Utilización** en el panel izquierdo y, a continuación, **Show**>**Programas** o **Portfolio** o **Proyectos**.

1. Haga clic en el **Filtro** para mostrar las opciones de filtro.

1. (Condicional) Para modificar un filtro existente, haga clic en el **Filtro** menú desplegable y, a continuación, seleccione el filtro que desee modificar.
1. Especifique la siguiente información para crear o modificar el filtro:

   * **Portfolio:** Empiece escribiendo el nombre del portafolio que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
      Repita este proceso para incluir información de varios portafolios en el informe Utilización .\
      Para incluir todos los portafolios del sistema en el filtro, haga clic en **Agregar todo**. (Esta opción solo está disponible si tiene menos de 10 portafolios en el sistema).

   * **Programas:** Comience a escribir el nombre del programa que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
      Repita este proceso para incluir información de varias tareas en el informe Utilización .\
      Si ya ha designado portafolios en el filtro, el programa que especifique debe proceder de las carteras ya incluidas en el filtro. En caso contrario, los datos del programa no se incluyen en el informe de utilización.\
      Para incluir todos los programas de su sistema en el filtro, haga clic en **Agregar todo**. (Esta opción solo está disponible si tiene menos de 20 programas en el sistema).

   * **Proyectos:** Empiece escribiendo el nombre del proyecto que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
      Repita este proceso para incluir información de varios proyectos en el informe Uso .\
      Si ya ha designado portafolios o programas en el filtro, el proyecto que especifique debe pertenecer a uno de los portafolios o programas que ya estén incluidos en el filtro. Si no es así, los datos del proyecto no se incluyen en el informe de utilización.\
      Para incluir todos los proyectos del sistema en el filtro, haga clic en **Agregar todo**. (Esta opción solo está disponible si tiene menos de 250 proyectos en el sistema).

   * **Tareas:** Empiece escribiendo el nombre de la tarea que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
      Repita este proceso para incluir información de varias tareas en el informe Utilización .\
      Si ya ha designado portafolios, programas o proyectos en el filtro, la tarea que especifique debe proceder de uno de los portafolios, programas o proyectos que ya estén incluidos en el filtro. Si no es así, los datos de la tarea no se incluyen en el informe de utilización.

   * **Problemas:** Comience a escribir el nombre del problema que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
      Repita este proceso para incluir información de varios problemas en el informe de utilización.\
      Si ya ha designado portafolios, programas o proyectos en el filtro, el problema que especifique debe proceder de uno de los portafolios, programas o proyectos que ya estén incluidos en el filtro. Si no es así, los datos del problema no se incluyen en el informe de utilización.\
      La información de costes por problemas no siempre se incluye en el informe de utilización. Para obtener más información sobre cuándo se incluye la información de costos para problemas en el informe de uso, consulte la sección [Rastree el progreso, el coste y los ingresos con el informe de uso](#track-progress-cost-and-revenue-with-the-utilization-report) en este artículo.

   * **Funciones:** Empiece escribiendo el nombre de la función que desea que se represente en el Informe de uso y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable. Repita este proceso para incluir funciones adicionales.\
      El informe de utilización contiene información solamente sobre las funciones que especifique. Por ejemplo, una tarea contiene 10 horas reales. 6 de estas horas provienen de una función de Designer y 4 de una función de desarrollador. Si filtra el informe de uso por función de Designer, se excluirán del informe las 4 horas que provengan de la función de desarrollador.

   * **Agregar regla de filtro:** Haga clic en **Agregar regla de filtro**, haga clic en el primer campo y comience a escribir el nombre del campo sobre el que desea filtrar. Si el campo está disponible, se rellena para cada objeto al que se puede asociar. Haga clic en el nombre del campo para agregarlo al filtro.

      >[!IMPORTANT]
      >
      >Debe escribir el nombre del campo y no la etiqueta del campo. La etiqueta de campo aparece en un formulario personalizado adjunto a un objeto. Para obtener información sobre la diferencia entre la etiqueta y el nombre de un campo personalizado, consulte  [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

      Para obtener más información sobre los campos que se ven en las columnas, consulte [Glosario de terminología de Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
      Elija el filtro y los modificadores de condición para el filtro. Los modificadores disponibles se describen en [Modificadores de filtro y condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Para crear un nuevo filtro, haga clic en **Guardar filtro**.\
   O\
   Para modificar un filtro existente, haga clic en la flecha desplegable situada junto al **Guardar filtro** y haga clic en **Guardar nuevo filtro**.\
   En el **Nombre del filtro** , especifique un nombre para el filtro y haga clic en **Guardar**.\
   El área Utilización se filtra con la información incluida en el filtro.

### Aplicar un filtro guardado {#apply-a-saved-filter}

1. Para aplicar un filtro en el Informe de uso para un solo proyecto, vaya al proyecto para el que desee filtrar y haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para aplicar un filtro en el Informe de uso para varios proyectos, para un programa o para un portafolio, haga clic en el botón **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, **Recurso**, **Utilización** en el panel izquierdo y, a continuación, **Show**>**Programas** o **Portfolio** o **Proyectos**.

1. Haga clic en **Filtros guardados** y, a continuación, seleccione el filtro que desee aplicar en el menú desplegable.

### Duplicar un filtro {#duplicate-a-filter}

1. Para duplicar un filtro en el Informe de uso para un solo proyecto, vaya al proyecto para el que desee duplicar el filtro y, a continuación, haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para duplicar un filtro en el Informe de uso para varios proyectos, para un programa o para un portafolio, haga clic en el botón **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recurso**, luego **Utilización** en el panel izquierdo.

1. Haga clic en **Filtros guardados**, pase el ratón sobre el filtro que desea duplicar en el menú desplegable y, a continuación, haga clic en el **Duplicar** icono.

   ![](assets/utilization-filter-duplicate.png)\
   Se muestra el cuadro de diálogo Duplicar filtro.

1. En el **Nombre del filtro** , especifique un nombre para el nuevo filtro y haga clic en **Guardar**.

### Cambiar el nombre de un filtro {#rename-a-filter}

Al cambiar el nombre de un filtro, todos los usuarios de Workfront que tengan acceso al informe de utilización verán el nuevo nombre que elija.

Para cambiar el nombre de un filtro:

1. Para cambiar el nombre de un filtro en el Informe de uso para un solo proyecto, vaya al proyecto para el que desee cambiar el nombre del filtro y, a continuación, haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para cambiar el nombre de un filtro en el Informe de uso para varios proyectos, para un programa o para un portafolio, haga clic en el botón **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recurso**, luego **Utilización** en el panel izquierdo.

1. Haga clic en **Filtros guardados**, pase el ratón sobre el filtro que desea duplicar en el menú desplegable y, a continuación, haga clic en el **Cambiar nombre** icono.\
   ![](assets/utilization-filter-rename.png)\
   Aparecerá el cuadro de diálogo Cambiar nombre de filtro.

1. En el **Nombre del filtro** , especifique un nombre para el nuevo filtro y haga clic en **Guardar**.

### Eliminar un filtro {#delete-a-filter}

Al eliminar un filtro, este se elimina para todos los usuarios de Workfront que tengan acceso al informe de uso.

Para eliminar un filtro:

1. Para eliminar un filtro en el Informe de uso de un solo proyecto, vaya al proyecto para el que desea eliminar el filtro y, a continuación, haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para eliminar un filtro en el Informe de uso para varios proyectos, para un programa o para un portafolio, haga clic en el botón **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recurso**, luego **Utilización** en el panel izquierdo.

1. Haga clic en **Filtros guardados**, pase el ratón sobre el filtro que desea duplicar en el menú desplegable y, a continuación, haga clic en el **Eliminar** icono.

   ![](assets/utilization-filter-delete.png)

1. Haga clic en **Eliminar** cuando se le pregunte si desea eliminar el filtro.

## Ajustar el intervalo de fechas para el que se muestra la información {#adjust-the-date-range-for-which-information-is-displayed}

Puede ajustar el intervalo de fechas en el que se muestra la información de utilización. Puede seleccionar una fecha anterior o futura. Los cambios que realice solo serán visibles para usted.

1. Para ajustar el intervalo de fechas del Informe de uso para un solo proyecto, vaya al proyecto para el que desee ajustar el intervalo de fechas y, a continuación, haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para ajustar el intervalo de fechas del informe Utilización para varios proyectos, para un programa o para un portafolio, haga clic en el botón **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recurso**, luego **Utilización** en el panel izquierdo.

1. Haga clic en el intervalo de fechas junto al **Exportar** botón.

   La semana actual está seleccionada de forma predeterminada.

1. Seleccione entre las siguientes opciones:

   * **Semana:** Seleccione esta opción para seleccionar una semana determinada (de domingo a sábado).
   * **Mes:** Seleccione esta opción para seleccionar un mes determinado.

   El intervalo de fechas seleccionado se muestra en el informe de utilización, a la izquierda del informe **General** para abrir el Navegador.\
   Workfront recuerda si desea ver una vista de semana o mes. La próxima vez que acceda al informe de utilización, se mostrará la semana actual o el mes actual, según la opción que seleccione.

## Exportar información de utilización

Puede exportar información de uso de un proyecto, programa o portafolio desde Workfront. La información solo se puede exportar en los formatos XLSX, TSV y PDF.

Cuando se visualiza en Microsoft Excel, los números negativos se muestran entre paréntesis.

Para exportar información de utilización:

1. Para exportar la información de utilización de un solo proyecto, vaya al proyecto para el que desea exportar la información de utilización y, a continuación, haga clic en el botón **Utilización** (en función de la configuración de diseño, puede encontrarse en la sección **Más** ).

   O

   Para exportar la información de utilización de varios proyectos, de un programa o de un portafolio, haga clic en el botón **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recurso**, luego **Utilización** en el panel izquierdo.

1. Haga clic en **Exportar**, situado en la esquina superior izquierda del **Utilización** pestaña .

1. Seleccione entre las siguientes opciones:

   * **PDF:** Exporta el informe en formato de PDF. Este es el formato recomendado si planea imprimir el informe.\
      Seleccione: **Letra - Vertical**, **Carta - Horizontal** o **Otros tamaños** (proporciona opciones para exportar en legal (8,5&quot; x 14&quot;), libro mayor (11&quot; x 17&quot;) y A4).\
      Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el disco duro.

   * **Excel:** Exporta el informe en formato XLSX. Este es el formato recomendado si planea seguir analizando los datos en Excel.\
      Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el disco duro.

   * **Delimitado por tabulaciones:** Exporta el informe en formato TSV. Este es el formato recomendado si planea importar los datos en software de terceros para un análisis más detallado.\
      Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el disco duro.

1. Lea la información del artículo [Exportar datos](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) para comprender cómo utilizar el archivo exportado.

## Ver información de utilización en un gráfico

Los datos se pueden visualizar desde el informe Utilización en una vista de gráfico.

1. Para ver un informe de utilización de un solo proyecto en formato de gráfico, vaya al proyecto que desee ver y, a continuación, haga clic en **Mostrar más> Utilización** en el panel izquierdo.

   O

   Para ver un informe de uso en formato de gráfico para varios proyectos, para un programa o para un portafolio, haga clic en **Informes** en la barra de navegación global para ir al área de informes y, a continuación, haga clic en la **Utilización** pestaña .

1. En la esquina superior derecha del informe de utilización, haga clic en el botón **Gráfico** icono.\
   ![](assets/utilization-chart.png)\
   El informe Utilización se muestra en una vista de gráfico.

1. (Opcional) Configure esta opción para mostrar Proyectos, Programas o Portfolio seleccionando la opción adecuada en la **Show** menú desplegable.
1. (Opcional) Pase el ratón sobre un punto específico en el tiempo del informe para ver los datos de ese momento.

   ![](assets/utilization-chart-hover-350x176.png)

1. (Opcional) Ajuste los filtros para decidir qué información se muestra en el gráfico. Para obtener información sobre el ajuste de filtros, consulte la sección [Filtrar la información de utilización](#filter-utilization-information) en este artículo.
1. (Opcional) Configure el intervalo de tiempo del informe de gráfico, tal como se describe en la sección [Ajustar el intervalo de fechas para el que se muestra la información](#adjust-the-date-range-for-which-information-is-displayed) en este artículo.
