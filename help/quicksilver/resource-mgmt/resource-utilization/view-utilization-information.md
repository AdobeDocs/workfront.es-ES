---
product-area: resource-management
navigation-topic: resource-utilization
title: Ver información de utilización de recursos
description: Puede ver la utilización de los recursos mediante el informe Utilización.
author: Alina, Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: d2b62f2ec2f52c54129b342d68c336c782601242
workflow-type: tm+mt
source-wordcount: '7854'
ht-degree: 0%

---

# Ver información de utilización de recursos

{{highlighted-preview}}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

Puede ver la utilización de los recursos mediante el informe Utilización.

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

Debe tener lo siguiente para acceder al informe de utilización:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Vea o acceda a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos </p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Portafolios</p> </li> 
     <li> <p>Programas</p> </li> 
     <li> <p>Datos financieros si desea ver información por coste</p> </li> 
    </ul> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Vea el acceso a proyectos, portafolios y programas para acceder a la sección Utilización en el área Recursos</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>Administrar el acceso al proyecto para acceder a la sección Utilización de un proyecto</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

En las secciones siguientes se describe cómo ver y utilizar la información de utilización.

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

## Descripción general del informe Utilización {#overview-of-the-utilization-report}

Mediante el informe Utilización, puede ver el progreso, el coste o los ingresos de un proyecto, programa o portafolio en un solo informe. También puede comparar los ingresos con el coste.

Puede consultar el informe Utilización en el área de Recursos para ver la utilización en varios proyectos o puede consultarlo en el nivel de un proyecto para ver la utilización de los recursos individuales (funciones y usuarios) asociados a ese proyecto.

Para obtener información sobre el acceso y el uso del informe Utilización, consulte la [Realice un seguimiento del progreso, los costes y los ingresos con el informe Utilización](#track-progress-cost-and-revenue-with-the-utilization-report) de este artículo.

* [Seguimiento de horas (progreso)](#track-hours-progress)
* [Seguimiento del coste](#track-cost)
* [Seguimiento de ingresos](#track-revenue)
* [Comparar ingresos con costos planificados y reales](#compare-revenue-against-planned-and-actual-costs)

### Seguimiento de horas (progreso) {#track-hours-progress}

Puede realizar un seguimiento del progreso si consulta cómo se comparan las horas presupuestadas y planificadas con las horas reales.

Al rastrear el progreso de un proyecto, programa o portafolio, el progreso de ambas tareas y problemas se incluye en el informe Utilización.

La siguiente información está disponible en el informe Utilización al rastrear las horas:

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
   <td scope="col"> <p>Total de horas presupuestadas en los proyectos incluidos. Puede ver el total de horas presupuestadas para la vida general de los proyectos incluidos o puede ver el total de horas presupuestadas solo para el intervalo de fechas especificado (puede especificar una semana o mes individual). </p> <p>Las horas presupuestadas se rellenan a partir de la información disponible en el nuevo área de Presupuestación de recursos del caso comercial o del Planificador de recursos<em>.</em></p> <p>Las horas presupuestadas aparecen en el informe Utilización en cualquiera de las siguientes filas:</p> 
    <ul> 
     <li> Las horas presupuestadas se resumen por rol y por usuario individual en el informe Utilización, de la siguiente manera:<br><strong>Usuario individual:</strong> Las horas presupuestadas se resumen para cada usuario en el informe de utilización. Estas horas presupuestadas están asociadas con las tareas y problemas que se asignan al usuario en los proyectos incluidos. (Puede expandir la fila del rol correspondiente para ver una lista de usuarios con ese rol).<br><strong>Rol:</strong> Las horas presupuestadas se resumen por rol en el informe de utilización.<br>Las horas presupuestadas aparecen en un rol concreto como resultado de cualquiera de los siguientes escenarios: 
     <li>La función de trabajo se define como la función de trabajo principal del usuario asignado a la tarea o al problema donde están asociadas las horas presupuestadas. </li> 
       <li>Cuando se ve la información de utilización de un solo proyecto, se utiliza la función de trabajo del usuario asignado a las horas tanto si no hay asignación en la tarea o el problema, si se asigna a otro usuario sin asignación de función de trabajo, si se asigna a otro usuario con una función de trabajo diferente o si se asigna otro equipo.</li> 
       <li>Cuando se visualiza la información de utilización de varios proyectos, programas o portafolios, la función del usuario asignado a las horas se utiliza únicamente cuando la función está asignada a una tarea o problema de un proyecto. </li> 
       <li>La función del puesto se asigna a la tarea o al problema que tiene asociadas horas presupuestadas y el usuario asignado a la tarea o al problema no tiene una función del puesto definida en el sistema.</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>Horas sin asignar</strong>: las horas presupuestadas se muestran en el informe de utilización de la sección Horas sin asignar cuando las horas presupuestadas están asociadas a una tarea o un problema y no hay ningún usuario o rol asignado a la tarea o al problema.<br>Esta sección solo aparece cuando hay horas en el proyecto que coinciden con esta descripción y cuando se visualiza el informe de utilización de un proyecto o desde él. </p> <p>Esta sección solo aparece cuando hay horas en el proyecto que coinciden con esta descripción y cuando se visualiza el informe de utilización de un proyecto o desde él. </p> </li> 
    </ul> <p>Para obtener más información sobre las horas presupuestadas, consulte la sección "Localizar las horas presupuestadas de un proyecto" en la <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender el costo laboral presupuestado y las horas presupuestadas de los proyectos</a> artículo.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Horas planificadas</strong> </td> 
   <td scope="col"> <!-- Yay, no errors, warnings, or alerts! -->

<p>
Horas planificadas en los proyectos incluidos asociados con las asignaciones de cada tarea y problema. Puede ver el total de horas planificadas de todas las asignaciones del proyecto durante la vida general de los proyectos incluidos o puede ver el total de horas planificadas sólo para el intervalo de fechas especificado (puede especificar una semana o mes concretos). 
</p>
<p>
<strong>SUGERENCIA </strong>
</p>
<p>
No se tienen en cuenta las horas planificadas de elementos que tienen una duración de 0. 
</p>
<p>
Las horas planificadas en el informe Utilización tienen en cuenta si las horas planificadas se han reasignado a lo largo de la duración de una tarea o problema. 
</p>
<p>
Cuando se modifica la asignación diaria de horas del usuario mediante el Distribuidor de cargas de trabajo, los datos del informe Utilización pueden verse afectados si las fechas seleccionadas en el informe Utilización contienen únicamente una parte de la Duración de una tarea o un problema. 
</p>
<p>
Para obtener información sobre la modificación de asignaciones para los usuarios, consulte <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo</a>.


</p>
<p>
Las horas planificadas aparecen en el informe Utilización en cualquiera de las filas siguientes:
</p>
<ul>

<li>Las horas planificadas se resumen por rol y por usuario individual en el informe de utilización, de la siguiente manera: 
<ul>

<li><strong>Usuario individual</strong>: las horas planificadas se resumen para cada usuario en el informe de utilización. Estas horas planificadas están asociadas con las tareas y problemas que se le asignan al usuario en los proyectos incluidos. (Puede expandir la fila del rol correspondiente para ver una lista de usuarios con ese rol).

<li><strong>Rol</strong>: las horas planificadas se resumen por función del puesto en el informe de utilización de un solo proyecto.<br>Las horas planificadas aparecen en un rol en particular como resultado de cualquiera de los siguientes escenarios:  
<ul>

<li>La función del puesto se define como la función del puesto principal del usuario asignado a la tarea o al problema donde están asociadas las horas planificadas.

<li>Cuando se consulta la información de utilización de un solo proyecto, las horas asociadas a un rol no se muestran para el rol en los siguientes casos:   
<ul>

<li>No hay ninguna asignación en la tarea o el problema

<li>Se asigna un usuario sin asignación de rol

<li>A un usuario se le asigna una función diferente

<li>Se asigna un equipo a la tarea o al problema
</li>   
</ul>

<li>Cuando se visualiza la información de utilización de varios proyectos, programas o portafolios, la función del usuario asignado a las horas se utiliza únicamente cuando la función está asignada a una tarea o problema de un proyecto. Las horas de la función no se muestran por separado al ver el informe Utilización de varios proyectos.

<li>La función del puesto se asigna a la tarea o al problema que tiene horas planificadas asociadas y el usuario asignado a la tarea o al problema no tiene una función del puesto definida en el sistema.
</li>  
</ul>

<li><strong>Horas sin asignar</strong>: las horas planificadas se muestran en el informe de utilización de la sección Horas sin asignar cuando las horas planificadas están asociadas a una tarea o un problema y no hay ningún usuario o función asignado a la tarea o al problema. Esta sección aparece únicamente cuando hay horas en el proyecto que coinciden con esta descripción y cuando se visualiza el informe de utilización de un solo proyecto. <br>Para obtener más información sobre las horas planificadas, consulte <a href="../../manage-work/tasks/task-information/planned-hours.md">Resumen de horas planificadas</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Horas reales</strong> </td> 
   <td> <p> El total de horas registradas en las tareas, problemas, <span>y en el proyecto</span> para los proyectos incluidos. Puede ver el total de horas reales para la vida general de los proyectos incluidos o puede ver el total de horas reales solo para el intervalo de fechas especificado (puede especificar una semana o mes individual). </p> <p>Advertencia: El informe de utilización incluye las horas registradas en el proyecto, las tareas secundarias, los problemas y las tareas principales que tienen al menos una asignación. No incluye las horas registradas en tareas principales sin asignaciones. Se recomienda no utilizar tareas principales como tareas de trabajo y asignar solo tareas secundarias a los recursos. </p> <p>Horas reales aparece en el informe de utilización en cualquiera de las filas siguientes:</p> 
    <ul> 
     <li> Las horas reales se resumen por rol y por usuario individual en el informe de utilización de un proyecto, de la siguiente manera:<br><strong>Usuario individual:</strong> Las horas reales se muestran en el informe de utilización, en la fila del usuario que ha registrado las horas. (Puede expandir la fila de la función correspondiente para ver una lista de los usuarios con esa función de trabajo que han registrado horas).<br><strong>Rol:</strong> Las horas reales registradas por los usuarios asociados con esos roles se resumen en el informe de utilización, en la fila del rol correspondiente.<br>Las horas reales aparecen en un rol concreto como resultado de cualquiera de los siguientes escenarios: 
      <ul> 
       <li>La función de trabajo se define como la función de trabajo principal del usuario que ha registrado las horas.</li> 
       <li>No hay ninguna asignación en la tarea o el problema</li> 
       <li>Se asigna otro usuario sin asignación de rol</li> 
       <li>A otro usuario se le asigna una función diferente</li> 
       <li> <p>Se asigna un equipo.</p> </li> 
      </ul></li>  
     <p>Si el usuario que registra las horas no tiene una función de trabajo asociada a su perfil, la función de trabajo utilizada para el informe Utilización es la función de trabajo asignada a la tarea o al problema en el que se registran las horas o la función de trabajo asociada al propietario principal de la tarea o el problema. </p> 
     <li><strong>Otras horas:</strong> Las horas reales se muestran en el informe de utilización de la sección Otras horas, en la fila del usuario que ha iniciado sesión en las horas.<br>Las horas aparecen en esta sección cuando el usuario que ha registrado las horas no tiene una función de trabajo definida en el sistema.<br>Esta sección solo aparece cuando hay horas en el proyecto que coinciden con esta descripción. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Desviación presupuestada (para horas)</strong> </td> 
   <td> <p>Total de horas presupuestadas menos el total de horas reales en los proyectos incluidos. Puede ver la desviación presupuestada total para la vida general de los proyectos incluidos o puede ver la desviación presupuestada total sólo para el intervalo de fechas especificado (puede especificar una semana o mes concretos). </p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de horas presupuestadas es bueno que el de las horas reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de horas presupuestadas es menor que las horas reales.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Desviación planificada (para horas)</strong> </td> 
   <td> <p>Total de horas planificadas menos el total de horas reales en los proyectos incluidos. Puede consultar la desviación total planificada para la vida útil total de los proyectos incluidos o puede consultar la desviación total planificada sólo para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de horas planificadas son buenas a las horas reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de horas planificadas es menor que las horas reales.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Seguimiento del coste {#track-cost}

Puede realizar un seguimiento de los costos observando la comparación del costo presupuestado y el costo planificado con los costos reales.

Al realizar el seguimiento del coste de un proyecto, programa o portafolio, la información del informe Utilización procede de las tareas. La información de costes de las tareas siempre está disponible en el informe Utilización. El coste de las tareas se calcula según el tipo de coste de la tarea. Para obtener información sobre el tipo de coste de las tareas, consulte &quot;Modificación de tipos de coste para tareas individuales&quot; en [Seguimiento de costes](../../manage-work/projects/project-finances/track-costs.md).

Puede mostrar la información de costes en el informe Utilización de las siguientes maneras:

* Para una semana o mes determinados, o para el proyecto, programa o portafolio general.
* Por rol o por individuo, para proyectos.

La moneda utilizada en el informe de utilización viene determinada por la moneda establecida en el proyecto. Para obtener información sobre cómo ajustar la moneda de un proyecto, consulte [Cambiar la divisa del proyecto](../../manage-work/projects/project-finances/change-project-currency.md).

La siguiente información está disponible en el informe Utilización al realizar el seguimiento de Costes:

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
   <td scope="col"><strong>Costo presupuestado</strong> </td> 
   <td scope="col"> <p>Costo presupuestado de los proyectos incluidos. Puede consultar el coste presupuestado total de la vida general de los proyectos incluidos o el coste presupuestado total solo para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> <p>Dado que el coste presupuestado en el informe Utilización se centra en el coste por función, el cálculo es el mismo que el coste laboral presupuestado dentro de otras áreas de Workfront. Para obtener información sobre cómo se calcula el costo laboral presupuestado, consulte <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprender el costo laboral presupuestado y las horas presupuestadas de los proyectos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Costo planificado</strong> </td> 
   <td scope="col"> <p>Costo total planificado de los proyectos incluidos. Puede ver el costo total planificado para la vida general de los proyectos incluidos o puede ver el costo total planificado solamente para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> <p><span class="preview">Tenga en cuenta que para las vistas de semana, mes y trimestre, los costes planificados se calculan como un promedio del periodo elegido cuando las tasas de coste de los roles de trabajo o usuarios son efectivas por fecha.</span></p><p>Para obtener información sobre cómo se calcula el costo planificado del proyecto, consulte la sección "Cómo calcula Workfront los costos planificados, presupuestados y reales" en el artículo <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Costo real</strong> </td> 
   <td scope="col"> <p>Costo real total de los proyectos incluidos. Puede ver el costo real total de la vida general de los proyectos incluidos o puede ver el costo real total solamente para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> <p>Para obtener información sobre cómo se calcula el costo real del proyecto, consulte la sección "Cómo calcula Workfront los costos planificados, presupuestados y reales" en el artículo <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Seguimiento de costes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Desviación presupuestada (de costo)</strong> </td> 
   <td scope="col"> <p>Costo presupuestado total menos el costo real total de los proyectos incluidos. Puede ver la desviación presupuestada total para la vida general de los proyectos incluidos o puede ver la desviación presupuestada total sólo para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el costo presupuestado total es bueno que el costo real.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el costo presupuestado total es menor que el costo real.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Desviación planificada (de costo)</strong> </td> 
   <td> <p>Costo total planificado menos el costo real total de los proyectos incluidos. Puede consultar la desviación total planificada para la vida útil total de los proyectos incluidos o puede consultar la desviación total planificada sólo para el intervalo de fechas especificado (puede especificar una semana o mes concretos). </p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el costo total planificado es bueno que el costo real.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el costo total planificado es menor que el costo real.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Seguimiento de ingresos {#track-revenue}

Puede realizar un seguimiento de los ingresos consultando cómo se comparan los ingresos presupuestados y planificados con los ingresos reales.

Al rastrear los ingresos de un proyecto, programa o portafolio, solo los ingresos de las tareas se incluyen en el informe Utilización.

La información de la siguiente tabla está disponible en el informe Utilización al realizar el seguimiento de los ingresos.

Para obtener información sobre los campos específicos y cómo los calcula Workfront, consulte también los siguientes artículos:

* [Seguimiento de costes](../../manage-work/projects/project-finances/track-costs.md)
* [Resumen de facturación e ingresos](../../manage-work/projects/project-finances/billing-and-revenue-overview.md)

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
   <td scope="col"> <p>El total de horas presupuestadas multiplicado por la tarifa de facturación de rol en los proyectos incluidos. Puede consultar el total de ingresos presupuestados para la vida general de los proyectos incluidos o puede consultar el total de ingresos presupuestados solo para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ingresos planificados</strong> </td> 
   <td scope="col"> <p>Ingresos planificados en el informe Utilización son los ingresos asociados con las horas planificadas asignadas a los recursos asignados a las tareas del proyecto.</p> <p>Workfront calcula los ingresos planificados del proyecto para el informe Utilización mediante la siguiente fórmula:</p> <p><code>Project Planned Revenue = SUM&nbsp;(All Tasks Planned Revenue)</code> </p> 
   <p><b>NOTA</b>
   <p>Los ingresos planificados del proyecto que se muestran en el informe Utilización difieren de los ingresos planificados que se muestran en el área Detalles del proyecto y en los informes de proyecto. </p> <p>Los ingresos planificados en el área de Detalles del proyecto reflejan los ingresos de la tarea y los ingresos fijos del proyecto. Los ingresos planificados en el informe Utilización muestran los ingresos planificados asociados únicamente a las tareas del proyecto. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>Si el proyecto tiene 1 tarea con 10 horas, asignada a un consultor con una tasa horaria de 20 dólares y el proyecto tiene 100 dólares de ingresos fijos, el informe Utilización muestra 200 dólares para los ingresos planificados (los ingresos planificados asociados con las horas de la tarea). La sección Detalles del proyecto muestra 300 $ (los ingresos planificados de la tarea y los ingresos fijos del proyecto). </p> 
     </div> <p>Para obtener más información sobre la tarea y los ingresos planificados del proyecto fuera del informe de utilización, consulte <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Resumen de facturación e ingresos</a>.</p> </p> <p>La forma en que el informe Utilización calcula y muestra los ingresos planificados para los proyectos incluidos tiene en cuenta el tipo de ingresos establecido en la tarea. </p> <p>Según el tipo de ingresos de cada tarea del proyecto, existen los siguientes escenarios: </p> <p><strong>Ingresos fijos:</strong> Independientemente de las asignaciones de tareas, los ingresos de la tarea siempre se calculan utilizando el importe fijo especificado en la tarea.</p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los ingresos planificados para tareas de ingresos fijos dividiendo los ingresos fijos equitativamente por el número de horas planificadas en la tarea. </p> <p>Por ejemplo, una tarea tiene unos ingresos de 200 dólares. Si hay 4 horas planificadas en la tarea, cada hora sería 50 $. Se distribuye en los niveles de usuario y rol. Esta distribución es exclusiva del informe Utilización.</p> <p><b>NOTA</b>

Si tiene una tarea de ingresos fijos y no hay horas planificadas para la tarea, los ingresos no se muestran en el informe de utilización porque no hay forma de distribuirlos entre las horas. Si tiene horas planificadas en tareas con ingresos fijos y sin asignaciones, los ingresos se muestran como ingresos sin asignar. </p> <p><strong>Rol por hora:</strong> Los ingresos de la tarea se calculan a partir de la tarifa de facturación establecida para un rol específico, multiplicada por el número de horas planificadas asociadas a ese rol. Workfront utiliza la fórmula siguiente:</p> <p><code>Ingresos planificados por hora de rol = SUMA(Horas planificadas de la función en todas las tareas) * Tasa de facturación de rol</code></p><p><span class="preview"><b>NOTA:</b> La tarifa por hora de facturación de la fórmula tiene en cuenta cualquier cambio de fecha en vigor de la tarifa.</span></p>   <p><strong>Usuario por hora:</strong> Los ingresos de la tarea se calculan usando la tarifa de facturación establecida para un usuario específico, multiplicada por el número de horas planificadas asociadas con ese usuario. Workfront utiliza la fórmula siguiente:</p> <p><code>Ingresos planificados por hora por usuario = SUMA(Horas planificadas de los usuarios en todas las tareas) * Tasa de facturación del usuario</code> </p> <p><span class="preview"><b>NOTA:</b> La tarifa por hora de facturación de la fórmula tiene en cuenta cualquier cambio de fecha en vigor de la tarifa.</span></p> <p><b>Rol por hora o usuario por hora más fijos</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los ingresos planificados dividiendo los ingresos fijos de forma uniforme por el número de horas planificadas de la tarea. </p> <p>Se dan los siguientes casos: </p>
<ul>
<li> <p><strong>Rol por hora más fijos:</strong> Los ingresos de la tarea se calculan mediante la tarifa de facturación establecida para un rol específico, multiplicada por el número de horas planificadas asociadas al rol. Además, se agrega a la tasa de rol una cantidad fija especificada en la tarea. Workfront utiliza la fórmula siguiente:</p> <p><code>Rol por hora más ingresos planificados fijos = [SUM(Horas planificadas de la función en todas las tareas) * Tasa de facturación de la función] + SUMA(Importe máximo o fijo de la tarea/Horas planificadas de la tarea)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Usuario por hora más fijos:</strong> La tarifa de facturación establecida para un usuario específico, multiplicada por el número de horas planificadas en la tarea de ese usuario. Además, se agrega a la tasa de usuario una cantidad fija especificada en la tarea. Workfront utiliza la fórmula siguiente:</p> <p><code>Usuario por hora más ingresos planificados fijos = [SUM(Horas planificadas del usuario en todas las tareas) * Tarifa de facturación del usuario] + SUMA(Importe máximo o fijo de la tarea/Horas planificadas de la tarea)</code> </p> </li>
</ul> <p><b>Rol o usuario por hora con tope</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, si los ingresos planificados superan el límite, el importe por encima del importe del límite se considera ingresos fijos. Los ingresos planificados se calculan dividiendo los ingresos fijos de forma equitativa por el número de horas planificadas en la tarea y, a continuación, añadiendo a eso el importe del límite y el rol o los ingresos por hora del usuario. <br></p> <p>Se dan los siguientes casos: </p>
<ul>
<li> <p><strong>Rol por hora con tope:</strong> Las tareas se facturan por hora como en el Rol por hora, pero tienen un importe máximo de límite que puede especificar. Workfront utiliza la fórmula siguiente:</p> <p><code>Rol por hora con ingresos planificados de tope = [SUMA(Horas planificadas del rol en todas las tareas y problemas) * Tasa de facturación del rol] + Importe límite de la tarea + SUMA(Importe sobre el importe límite / Horas planificadas de la tarea)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Usuario por hora con tope:</strong> Las tareas se facturan por hora como en Usuario por hora, pero tienen un importe máximo que puede especificar. Workfront utiliza la fórmula siguiente: </p> <p><code>Usuario por hora con ingresos planificados máximos = [SUM(Horas planificadas del usuario en todas las tareas) * Tarifa de facturación del usuario] + Importe límite de la tarea + SUMA(Importe sobre el importe límite / Horas planificadas de la tarea)</code> </p> </li>
</ul> <p>Para obtener más información sobre qué rol o usuario se tiene en cuenta al calcular los ingresos planificados, consulte <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Resumen de facturación e ingresos</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>Ingresos reales</strong> </td> 
   <td> <p>Ingresos reales son los ingresos asociados con las horas reales de las tareas <span>y del proyecto</span>. Para obtener más información sobre los ingresos reales, consulte la sección "Seguimiento de importes de ingresos" en el artículo <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Resumen de facturación e ingresos</a>.</p>

<p>La forma en que el informe Utilización calcula los ingresos reales de los proyectos incluidos difiere según el tipo de ingresos establecido en la tarea, de la siguiente manera:</p> <p><strong>Ingresos fijos:</strong> Independientemente de las asignaciones de tareas, los ingresos de la tarea siempre se calculan utilizando el importe fijo especificado en la tarea.</p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los Ingresos reales dividiendo uniformemente los Ingresos fijos por el número de horas registradas en la tarea. </p> <p> </p> <p>Por ejemplo, una tarea tiene unos ingresos reales de 200 $. Si hay 4 horas reales en la tarea, cada hora sería 50 $. Se distribuye en los niveles de usuario y rol. Esta distribución es exclusiva del informe Utilización.</p> <p><b>NOTA</b>

Si tiene una tarea de ingresos fijos y no hay horas reales en la tarea, los ingresos reales no se muestran en el informe de utilización porque no hay forma de distribuir las horas. </p> <p><strong>Rol por hora:</strong> Los ingresos de la tarea se calculan mediante la tarifa de facturación establecida para un rol específico, multiplicada por el número de horas reales.</p> <p>Workfront utiliza la fórmula siguiente:</p> <p><code>Ingresos reales por hora de rol = SUMA(Horas reales de rol en todas las tareas) * Tasa de facturación de rol</code> </p> <p><span class="preview"><b>NOTA:</b> La tarifa por hora de facturación de la fórmula tiene en cuenta cualquier cambio de fecha en vigor de la tarifa.</span></p> <p><strong>Usuario por hora:</strong> Los ingresos de la tarea se calculan utilizando la tasa de facturación establecida para un usuario específico, multiplicada por el número de horas registradas en la tarea desde ese usuario. Workfront utiliza la fórmula siguiente:</p> <p><code>Ingresos reales por hora de usuario = SUMA(Horas reales de los usuarios en todas las tareas) * Tarifa de facturación de usuario</code></p> <p><span class="preview"><b>NOTA:</b> La tarifa por hora de facturación de la fórmula tiene en cuenta cualquier cambio de fecha en vigor de la tarifa.</span></p> <p><b>Rol o usuario por hora más fijos</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, el informe Utilización calcula los Ingresos reales dividiendo uniformemente los Ingresos fijos por el número de horas registradas en la tarea. </p> <p>Se dan los siguientes casos: </p>
<ul>
<li> <p><strong>Rol por hora más fijos:</strong> Tarifa de facturación establecida para un rol específico, multiplicada por el número de horas registradas en la tarea de un usuario con ese rol. Además, se agrega a la tasa de rol una cantidad fija especificada en la tarea. </p> <p>Workfront utiliza la fórmula siguiente:</p> <p><code>Rol por hora más ingresos reales fijos = [SUM(Horas reales desde el rol en todas las tareas) * Tasa de facturación del rol] + SUMA(Importe máximo o fijo de la tarea / Horas reales de la tarea)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Usuario por hora más fijos:</strong> La tarifa de facturación establecida para un usuario específico, multiplicada por el número de horas registradas en la tarea desde ese usuario. Además, se agrega a la tasa de usuario una cantidad fija especificada en la tarea. </p> <p>Workfront utiliza la fórmula siguiente:</p> <p><code>Usuario por hora más ingresos reales fijos = [SUM(Horas reales de la función en todas las tareas) * Tarifa de facturación del usuario] + SUMA(Importe máximo o fijo de la tarea/Horas de usuario de la tarea)</code> </p> </li>
</ul> <p><b>Rol o usuario por hora con tope</b> </p> <p><b>IMPORTANTE</b>

A diferencia de otras áreas de Workfront, si los ingresos planificados superan el límite, el importe por encima del importe del límite se considera ingresos fijos. Los ingresos planificados se calculan dividiendo los ingresos fijos de forma equitativa por el número de horas planificadas en la tarea y, a continuación, añadiendo a eso el importe del límite y el rol o los ingresos por hora del usuario. <br></p> <p>Existen los siguientes escenarios:</p>
<ul>
<li> <p><strong>Rol por hora con tope:</strong> Las tareas se facturan por hora como en el Rol por hora, pero tienen un importe máximo de límite que puede especificar. Workfront utiliza la fórmula siguiente:</p> <p><code>Rol por hora con tope Ingresos reales = [SUMA(Horas reales desde el rol en todas las tareas y problemas) * Tasa de facturación del rol] + Importe límite de la tarea + SUMA(Importe sobre el importe límite / Horas reales de la tarea)</code></p> </li>
</ul>
<ul>
<li> <p><strong>Usuario por hora con tope:</strong> Las tareas se facturan por hora como en Usuario por hora, pero tienen un importe máximo que puede especificar.</p> <p> Workfront utiliza la fórmula siguiente:</p> <p><code>Usuario por hora con ingresos reales máximos = [SUMA(Horas reales de la función en todas las tareas y problemas) * Tarifa de facturación del usuario] + Importe límite de la tarea + SUMA(Importe sobre el importe límite / Horas reales de la tarea)</code> </p> </li>
</ul>
<div>
<p><strong>Ingresos del proyecto</strong>: los ingresos asociados con las horas registradas en el proyecto se calculan teniendo en cuenta la cantidad Facturación por hora del rol de trabajo principal del usuario que registra el tiempo. No se recomienda registrar el tiempo en el proyecto. </p>
<p><b>NOTA</b>

Si el usuario no está asociado a un rol o si la facturación por hora del rol principal es cero, Workfront calcula los ingresos reales utilizando la cantidad Facturación por hora para el usuario. Si el usuario no tiene un importe de facturación por hora en su perfil, los ingresos reales son cero. </p>
</div> </td>
</tr> 
  <tr> 
   <td><strong>Desviación presupuestada (para ingresos)</strong> </td> 
   <td> <p>Ingresos reales totales menos ingresos presupuestados en los proyectos incluidos.<br>Puede ver la desviación presupuestada total para la vida general de los proyectos incluidos o puede ver la desviación presupuestada total sólo para el intervalo de fechas especificado (puede especificar una semana o mes concretos).</p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de ingresos presupuestados es bueno que el de ingresos reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de ingresos presupuestados es menor que los ingresos reales.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Desviación planificada (para ingresos)</strong> </td> 
   <td> <p>Ingresos reales totales menos los ingresos planificados totales en los proyectos incluidos.<br>Puede consultar la desviación total planificada para la vida útil total de los proyectos incluidos o puede consultar la desviación total planificada sólo para el intervalo de fechas especificado (puede especificar una semana o mes concretos). </p> <p>Si el valor es positivo, se muestra en verde. Esto indica que el total de ingresos planificados es bueno respecto a los ingresos reales.</p> <p>Si el valor es negativo, se muestra en rojo. Esto indica que el total de ingresos planificados es menor que los ingresos reales.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### Comparar ingresos con costos planificados y reales {#compare-revenue-against-planned-and-actual-costs}

Puede ver el costo planificado o real junto con los ingresos planificados. También se muestra el margen (%) (el margen se calcula como Ingresos - Coste / Ingresos).

La siguiente información está disponible en el informe Utilización al comparar los ingresos con los costes planificados y reales:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Título de columna al ver ingresos frente a costo (planificado)</strong> </th> 
   <th> <strong>Función</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Costo planificado</strong> </td> 
   <td scope="col"> Costo total planificado de los proyectos incluidos. Puede ver el costo total planificado para la vida general de los proyectos incluidos o puede ver el costo total planificado solamente para el intervalo de fechas especificado (puede especificar una semana o mes individual). </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ingresos planificados</strong> </td> 
   <td scope="col"> <p>Ingresos planificados son los ingresos asociados con las horas planificadas de las tareas. </p> <p>La forma en que el informe Utilización calcula y muestra los ingresos planificados para los proyectos incluidos difiere según el tipo de ingresos establecido en la tarea, como se describe en la sección <a href="#track-revenue" class="MCXref xref">Seguimiento de ingresos</a> de este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Margen</strong> </td> 
   <td scope="col"> <p>El porcentaje de margen se calcula de la siguiente manera:</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>NOTA</b>

Si los ingresos planificados son iguales a 0, el margen se muestra como 0. </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>Título de columna al ver ingresos frente a costo (real)</strong> </p>  </td> 
   <td scope="col"><p><strong>Función</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Costo real</strong> </td> 
   <td scope="col"> <p>Costo real total de los proyectos incluidos. Puede ver el costo real total de la vida general de los proyectos incluidos o puede ver el costo real total solamente para el intervalo de fechas especificado (puede especificar una semana o mes individual).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Ingresos reales</strong> </td> 
   <td> <p>Ingresos reales son los ingresos asociados con las horas reales de las tareas.</p> <p>Los ingresos reales solo se muestran en el informe Utilización una vez que la tarea se ha marcado como Finalizada o Listo (o un estado que equivale a Finalizada).</p> <p>La forma en que el informe Utilización calcula los ingresos reales de los proyectos incluidos difiere según el tipo de ingresos establecido en la tarea, tal como se describe en la sección <a href="#track-revenue" class="MCXref xref">Seguimiento de ingresos</a> de este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Margen</strong> </td> 
   <td> <p>El porcentaje de margen se calcula de la siguiente manera:</p> <p>Ingresos Reales - Coste Real / Ingresos Reales * 100. </p> <p><b>NOTA</b>

Si los ingresos reales son iguales a 0, el margen se muestra como 0. </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## Realice un seguimiento del progreso, los costes y los ingresos con el informe Utilización {#track-progress-cost-and-revenue-with-the-utilization-report}

Puede realizar un seguimiento del progreso o el coste de un proyecto, programa o portafolio.

Puede mostrar información sobre el informe Utilización de una semana o mes determinados, o sobre la duración total de los proyectos.

Para realizar un seguimiento del progreso o el coste de uno o más proyectos con un informe de Utilización:

1. Realice una de las siguientes acciones, en función de si está viendo la información de utilización de un proyecto individual, varios proyectos, un programa o un portafolio:

   * Para consultar la información de utilización de un solo proyecto:

      1. Vaya a un proyecto cuya información de utilización desee consultar y, a continuación, haga clic en **Mostrar más> Utilización**.
      1. La información de utilización se muestra automáticamente cuando se visualiza un proyecto individual y no es necesario aplicar un filtro.\
         Si desea filtrar el informe Utilización, puede aplicar un filtro y, a continuación, hacer clic en **Ejecutar**.\
         Para obtener información sobre cómo filtrar el informe Utilización, consulte la sección [Filtrar información de utilización](#filter-utilization-information) en este artículo.\
         La información de utilización se muestra para usuarios y funciones individuales (los usuarios se agrupan dentro de su función asociada).

   * Para consultar la información de utilización de varios proyectos:

      1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos**, entonces **Utilización** en el panel izquierdo.
      1. Aplique un filtro al informe Utilización y haga clic en **Ejecutar**.\
         Debe especificar uno o varios proyectos en el filtro antes de ejecutar el informe de utilización. Para obtener información sobre cómo filtrar el informe Utilización, consulte la sección [Filtrar información de utilización](#filter-utilization-information) en este artículo.\
         La información de utilización se muestra para roles y proyectos individuales (los roles se agrupan dentro de su proyecto asociado).

   * Para consultar la información de utilización de un programa:

      1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos**, entonces **Utilización** en el panel izquierdo y haga clic en **Mostrar**>**Programas**.
      1. Aplique un filtro al informe Utilización y haga clic en **Ejecutar**.\
         Debe especificar uno o más programas en el filtro antes de ejecutar el informe de utilización. Para obtener información sobre cómo filtrar el informe Utilización, consulte la sección [Filtrar información de utilización](#filter-utilization-information) en este artículo.\
         La información de utilización se muestra para proyectos y programas individuales (los proyectos se agrupan dentro de su programa asociado).

   * Para consultar la información de utilización de un portafolio:

      1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos**, entonces **Utilización** en el panel izquierdo y haga clic en **Mostrar**>**Portfolio**.
      1. Aplique un filtro al informe Utilización y haga clic en **Ejecutar**.\
         Debe especificar uno o más portafolios en el filtro antes de ejecutar el informe de utilización. Para obtener información sobre cómo filtrar el informe Utilización, consulte la sección [Filtrar información de utilización](#filter-utilization-information) en este artículo.\
         La información de utilización se muestra para proyectos, programas y portafolios individuales (los proyectos se agrupan dentro de su programa asociado y los programas se agrupan dentro de su portafolio asociado).

1. En la esquina superior derecha del informe Utilización, haga clic en **Ver** menú desplegable y, a continuación, seleccione una de las siguientes opciones:

   * **Costo**
   * **Horas**
   * **Ingresos**
   * **Ingresos contra costo (planificados)**
   * **Ingresos contra costo (reales)**.

   La opción que seleccione determina qué columnas e información están disponibles en el informe. Para obtener más información sobre la información disponible en cada columna, consulte la tabla del paso 5.\
   ![](assets/utilization-view-dropdown.png)

1. (Opcional) Seleccione el intervalo de fechas para el que se muestra la información de utilización. Puede mostrar información de una semana o mes determinados a la izquierda del **General** columna. La información del proyecto, programa o portafolio general siempre se muestra en la **General** columna.\
   Para obtener más información, consulte la sección [Ajuste el intervalo de fechas para el que se muestra información](#adjust-the-date-range-for-which-information-is-displayed) en este artículo.

1. (Opcional) Haga clic en cualquier título de columna para ordenar el informe de utilización por la información de esa columna. La ordenación solo funciona cuando se incluyen varios elementos en el informe. Por ejemplo, puede ordenar los resultados del informe cuando esté viendo más de un proyecto (o portafolio o programa). No puede ordenar los resultados cuando solo está viendo un proyecto (o un portafolio o un programa) a la vez.
1. Utilice la información de la sección [Descripción general del informe Utilización](#overview-of-the-utilization-report) en este artículo para obtener más información sobre cada columna del informe Utilización.

## Filtrar información de utilización {#filter-utilization-information}

Puede filtrar el contenido que se muestra en un informe de utilización de un proyecto. Puede filtrar por tareas, problemas, funciones y datos personalizados. Al aplicar un filtro al informe Utilización, el informe Utilización contiene información basada en los criterios seleccionados.

Puede crear un filtro o aplicar un filtro que haya creado anteriormente.

* [Creación o modificación de un filtro](#create-or-modify-a-filter)
* [Aplicar un filtro guardado](#apply-a-saved-filter)
* [Duplicación de un filtro](#duplicate-a-filter)
* [Cambiar nombre de filtro](#rename-a-filter)
* [Eliminación de un filtro](#delete-a-filter)

### Creación o modificación de un filtro {#create-or-modify-a-filter}

Al crear un filtro, todos los usuarios de Workfront que tienen acceso al informe Utilización también tienen acceso al filtro que cree. Del mismo modo, cuando se modifica un filtro existente, este se modifica para todos los usuarios que tengan acceso al informe Utilización.

Para crear o modificar un filtro:

1. Para filtrar la información de utilización de un solo proyecto, vaya al proyecto para el que desea filtrar dicha información y haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para filtrar la información de utilización de varios proyectos, de un programa o de un portafolio, haga clic en el icono Menú principal ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, **Recursos**, **Utilización** en el panel izquierdo, **Mostrar**>**Programas** o **Portfolio** o **Proyectos**.

1. Haga clic en **Filtrar** para mostrar las opciones de filtro.

1. (Condicional) Para modificar un filtro existente, haga clic en **Filtrar** menú desplegable y, a continuación, seleccione el filtro que desea modificar.
1. Especifique la siguiente información para crear o modificar el filtro:

   * **Portfolio:** Empiece escribiendo el nombre del portafolio que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
     Repita este proceso para incluir información de varios portafolios en el informe Utilización.\
     Para incluir todos los portafolios del sistema en el filtro, haga clic en **Añadir todo**. (Esta opción solo está disponible si tiene menos de 10 portafolios en el sistema).

   * **Programas:** Empiece escribiendo el nombre del programa que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
     Repita este proceso para incluir información de varias tareas en el informe Utilización.\
     Si ya ha designado portafolios en el filtro, el programa que especifique debe proceder de los portafolios ya incluidos en el filtro. Si no es así, los datos del programa no se incluyen en el informe Utilización.\
     Para incluir todos los programas del sistema en el filtro, haga clic en **Añadir todo**. (Esta opción sólo está disponible si tiene menos de 20 programas en el sistema.)

   * **Proyectos:** Empiece escribiendo el nombre del proyecto que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
     Repita este proceso para incluir información de varios proyectos en el informe Utilización.\
     Si ya ha designado portafolios o programas en el filtro, el proyecto que especifique debe pertenecer a uno de los portafolios o programas ya incluidos en el filtro. Si no es así, los datos del proyecto no se incluyen en el informe de utilización.\
     Para incluir todos los proyectos del sistema en el filtro, haga clic en **Añadir todo**. (Esta opción solo está disponible si tiene menos de 250 proyectos en el sistema).

   * **Tareas:** Comience a escribir el nombre de la tarea que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
     Repita este proceso para incluir información de varias tareas en el informe Utilización.\
     Si ya ha designado portafolios, programas o proyectos en el filtro, la tarea que especifique debe proceder de uno de los portafolios, programas o proyectos ya incluidos en el filtro. Si no es así, los datos de la tarea no se incluyen en el informe Utilización.

   * **Problemas:** Empiece escribiendo el nombre del problema que contiene la información que desea incluir en el informe Utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.\
     Repita este proceso para incluir información de varios problemas en el informe Utilización.\
     Si ya ha designado portafolios, programas o proyectos en el filtro, el problema que especifique debe ser de uno de los portafolios, programas o proyectos ya incluidos en el filtro. Si no es así, los datos del problema no se incluyen en el informe Utilización.\
     La información de costes de los problemas no siempre se incluye en el informe Utilización. Para obtener más información sobre cuándo se incluye la información de coste de los problemas en el informe Utilización, consulte la sección [Realice un seguimiento del progreso, los costes y los ingresos con el informe Utilización](#track-progress-cost-and-revenue-with-the-utilization-report) en este artículo.

   * **Funciones:** Comience a escribir el nombre de la función que desea que se represente en el informe de utilización y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable. Repita este proceso para incluir funciones adicionales.\
     El Informe de utilización contiene información sólo sobre las funciones especificadas. Por ejemplo, una tarea contiene 10 horas reales. 6 de esas horas son de una función Diseñador y 4 de una función Desarrollador. Si filtra el Informe de utilización por función para Designer, las 4 horas que provienen de la función Desarrollador se excluyen del informe.

   * **Agregar regla de filtro:** Clic **Agregar regla de filtro**, haga clic en el primer campo y, a continuación, empiece a escribir el nombre del campo por el que desea filtrar. Si el campo está disponible, se rellena para cada objeto donde se puede asociar. Haga clic en el nombre del campo para añadirlo al filtro.

     >[!IMPORTANT]
     >
     >Debe escribir el nombre del campo y no la etiqueta del campo. La etiqueta de campo se muestra en un formulario personalizado adjunto a un objeto. Para obtener información sobre la diferencia entre la etiqueta y el nombre de un campo personalizado, consulte  [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

     Para obtener más información sobre los campos que se ven en las columnas, consulte [Glosario de terminología de Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
     Elija los modificadores de filtro y condición para el filtro. Los modificadores disponibles se describen en [Modificadores de filtro y condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Para crear un nuevo filtro, haga clic en **Guardar filtro**.\
   O\
   Para modificar un filtro existente, haga clic en la flecha desplegable situada junto al **Guardar filtro** y luego haga clic en **Guardar nuevo filtro**.\
   En el **Nombre del filtro** , especifique un nombre para el filtro y haga clic en **Guardar**.\
   El área Utilización se filtra con la información incluida en el filtro.

### Aplicar un filtro guardado {#apply-a-saved-filter}

1. Para aplicar un filtro en el informe de utilización a un solo proyecto, vaya al proyecto para el que desea filtrar y, a continuación, haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para aplicar un filtro en el Informe de utilización para varios proyectos, para un programa o para un portafolio, haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, **Recursos**, **Utilización** en el panel izquierdo, **Mostrar**>**Programas** o **Portfolio** o **Proyectos**.

1. Clic **Filtros guardados**, a continuación, seleccione el filtro que desee aplicar en el menú desplegable.

### Duplicación de un filtro {#duplicate-a-filter}

1. Para duplicar un filtro en el informe de utilización para un solo proyecto, vaya al proyecto para el que desea duplicar el filtro y, a continuación, haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para duplicar un filtro en el Informe de utilización para varios proyectos, para un programa o para un portafolio, haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos**, entonces **Utilización** en el panel izquierdo.

1. Clic **Filtros guardados**, pase el ratón sobre el filtro que desea duplicar en el menú desplegable y, a continuación, haga clic en **Duplicar** icono.

   ![](assets/utilization-filter-duplicate.png)\
   Se muestra el cuadro de diálogo Duplicar filtro.

1. En el **Nombre del filtro** , especifique un nombre para el nuevo filtro y haga clic en **Guardar**.

### Cambiar nombre de filtro {#rename-a-filter}

Cuando cambie el nombre de un filtro, todos los usuarios de Workfront que tengan acceso al informe Utilización verán el nuevo nombre que elija.

Para cambiar el nombre de un filtro:

1. Para cambiar el nombre de un filtro en el Informe de utilización para un solo proyecto, vaya al proyecto para el que desea cambiar el nombre del filtro y, a continuación, haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para cambiar el nombre de un filtro en el Informe de utilización para varios proyectos, para un programa o para un portafolio, haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos**, entonces **Utilización** en el panel izquierdo.

1. Clic **Filtros guardados**, pase el ratón sobre el filtro que desea duplicar en el menú desplegable y, a continuación, haga clic en **Cambiar nombre** icono.\
   ![](assets/utilization-filter-rename.png)\
   Aparece el cuadro de diálogo Cambiar nombre de filtro.

1. En el **Nombre del filtro** , especifique un nombre para el nuevo filtro y haga clic en **Guardar**.

### Eliminación de un filtro {#delete-a-filter}

Al eliminar un filtro, este se elimina para todos los usuarios de Workfront que tengan acceso al informe Utilización.

Para eliminar un filtro:

1. Para eliminar un filtro en el Informe de utilización para un solo proyecto, vaya al proyecto para el que desea eliminar el filtro y, a continuación, haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para eliminar un filtro en el Informe de utilización para varios proyectos, para un programa o para un portafolio, haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos**, entonces **Utilización** en el panel izquierdo.

1. Clic **Filtros guardados**, pase el ratón sobre el filtro que desea duplicar en el menú desplegable y, a continuación, haga clic en **Eliminar** icono.

   ![](assets/utilization-filter-delete.png)

1. Clic **Eliminar** cuando se le pregunte si desea eliminar el filtro.

## Ajuste el intervalo de fechas para el que se muestra información {#adjust-the-date-range-for-which-information-is-displayed}

Puede ajustar el intervalo de fechas para el que se muestra la información de utilización. Puede seleccionar una fecha pasada o futura. Los cambios que realice solo serán visibles para usted.

1. Para ajustar el intervalo de fechas del Informe de utilización para un solo proyecto, vaya al proyecto para el que desea ajustar el intervalo de fechas y haga clic en **Mostrar más>Utilización** en el panel izquierdo.

   O

   Para ajustar el intervalo de fechas del informe Utilización para varios proyectos, un programa o un portafolio, haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos**, entonces **Utilización** en el panel izquierdo.

1. Haga clic en el intervalo de fecha situado junto a la variable **Exportar** botón.

   La semana actual está seleccionada de forma predeterminada.

1. Seleccione entre las siguientes opciones:

   * **Semana:** Seleccione esta opción para seleccionar una semana determinada (de domingo a sábado).
   * **Mes:** Seleccione esta opción para seleccionar un mes determinado.

   El intervalo de fechas que seleccione se mostrará en el informe de utilización, a la izquierda del **General** columna.\
   Workfront recuerda si desea ver una vista de semana o de mes. La próxima vez que acceda al informe de utilización, se mostrará la semana o el mes actuales, según la opción que seleccione.

## Exportar información de utilización

Puede exportar información de utilización de un proyecto, programa o portafolio desde Workfront. La información sólo se puede exportar en los formatos XLSX, TSV y PDF.

Cuando se ven en Microsoft Excel, los números negativos se muestran entre paréntesis.

Para exportar información de utilización:

1. Para exportar la información de utilización de un solo proyecto, vaya al proyecto para el que desea exportar la información de utilización y, a continuación, haga clic en **Utilización** (en función de la configuración de diseño, se encuentra en la pestaña **Más** pestaña).

   O

   Para exportar la información de utilización de varios proyectos, de un programa o de un portafolio, haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos**, entonces **Utilización** en el panel izquierdo.

1. Clic **Exportar**, situado en la esquina superior izquierda de la **Utilización** pestaña.

1. Seleccione entre las siguientes opciones:

   * **PDF:** Exporta el informe en formato de PDF. Este es el formato recomendado si planea imprimir el informe.\
     Seleccione una de las opciones **Carta - Vertical**, **Carta - Horizontal**, o **Otros tamaños** (proporciona opciones para exportar en legal (8,5&quot; x 14&quot;), libro mayor (11&quot; x 17&quot;) y A4).\
     Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el disco duro.

   * **Excel:** Exporta el informe en formato XLSX. Este es el formato recomendado si planea analizar más a fondo los datos en Excel.\
     Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el disco duro.

   * **Delimitado por tabuladores:** Exporta el informe en formato TSV. Este es el formato recomendado si planea importar los datos en software de terceros para un análisis más amplio.\
     Según el sistema operativo que utilice, puede tener la opción de abrir o guardar el archivo. Abra el archivo con la aplicación asociada o guárdelo en el disco duro.

1. Lea la información del artículo [Exportación de datos](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) para comprender cómo utilizar el archivo exportado.

## Ver información de utilización en un gráfico

Puede visualizar los datos del informe Utilización en una vista de gráfico.

1. Para ver un informe de utilización de un solo proyecto en formato de gráfico, vaya al proyecto que desee ver y, a continuación, haga clic en **Mostrar más> Utilización** en el panel izquierdo.

   O

   Para ver un informe de utilización en formato de gráfico para varios proyectos, para un programa o para un portafolio, haga clic en **Informes** en la barra de navegación global para ir al área de Informes y luego haga clic en el botón **Utilización** pestaña.

1. En la esquina superior derecha del informe Utilización, haga clic en **Gráfico** icono.\
   ![](assets/utilization-chart.png)\
   El informe de utilización se muestra en una vista de gráfico.

1. (Opcional) Configúrelo para mostrar Proyectos, Programas o Portfolio seleccionando la opción adecuada en la **Mostrar** menú desplegable.
1. (Opcional) Pase el ratón sobre un momento específico del informe para ver los datos de ese momento.

   ![](assets/utilization-chart-hover-350x176.png)

1. (Opcional) Ajuste los filtros para decidir qué información se muestra en el gráfico. Para obtener información sobre cómo ajustar los filtros, consulte la sección [Filtrar información de utilización](#filter-utilization-information) en este artículo.
1. (Opcional) Configure el lapso de tiempo del informe del gráfico, tal como se describe en la sección [Ajuste el intervalo de fechas para el que se muestra información](#adjust-the-date-range-for-which-information-is-displayed) en este artículo.
