---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 11 de la API
description: ReportableBudgedHour se ha agregado a la API de Adobe Workfront como recurso para la creación de informes. Incluye campos de referencia, campos principales y campos predeterminados que están ausentes en BudgetedHour.
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 2%

---

# Novedades de la versión 11 de la API

* [Recursos añadidos](#added-resources)
* [Recursos eliminados](#removed-resources)
* [Recursos modificados](#modified-resources)

## Recursos añadidos {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReportableBudgetedHour](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accessorID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">Identificador</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accesorio</li> 
     <li style="font-weight: bold;">cliente</li> 
     <li style="font-weight: bold;">usuario  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principales</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">Identificador</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">Identificador</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">cliente  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principales</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">Identificador</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">Identificador</li> 
     <li style="font-weight: bold;">restrictLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">cliente  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principales</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">Identificador</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ReportableBudgetedHour {#reportablebudgetedhour}

ReportableBudgedHour se ha agregado a la API de Adobe Workfront como recurso para la creación de informes. Incluye campos de referencia, campos principales y campos predeterminados que están ausentes en BudgetedHour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>La fecha de asignación es el primer día (un domingo) de la semana para el que se presupuestaron las horas en el Planificador de recursos.</p> </li> 
     <li> <p style="font-weight: bold;">budgetHours </p> <p>Horas presupuestadas son horas que el administrador de recursos asigna al trabajo que los recursos necesitan completar en los proyectos</p> </li> 
     <li> <p style="font-weight: bold;">Identificador </p> <p>ID único de Workfront asignado a un objeto específico de hora presupuestada para informes.</p> </li> 
     <li style="font-weight: bold;">plannedBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>ID único de Workfront asignado a un proyecto específico.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>ID único de Workfront asignado a un rol específico.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>ID único de Workfront asignado a un usuario específico.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">proyecto</p> <p>Proyecto al que está asociada una ReportableBudgetedHour.</p> </li> 
     <li> <p style="font-weight: bold;">rol</p> <p>La función a la que está asociada una ReportBudgetedHour.</p> </li> 
     <li> <p style="font-weight: bold;">usuario</p> <p>Usuario con el que está asociado ReportableBudgetedHour.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principales</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">Identificador</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operaciones</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">RECUENTO</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">INFORME </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Recursos eliminados {#removed-resources}

No se ha eliminado ningún recurso para la API v11.

## Recursos modificados {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">Ruta de aprobación</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Asignación</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">BaselineTask</a> </li> 
     <li><a href="#category" class="MCXref xref">Categoría</a> </li> 
     <li><a href="#company" class="MCXref xref">Compañía</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Cliente</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">Preferencias del cliente</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Documento</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Iteración</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Plantilla de diseño</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilestonePath</a> </li> 
     <li><a href="#note" class="MCXref xref">Nota</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Parámetro</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portafolio</a> </li> 
     <li><a href="#program" class="MCXref xref">Programar</a> </li> 
     <li><a href="#project" class="MCXref xref">Proyecto</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">TiempoReservado</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">Riesgo</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">InformeProgramado</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">Tarea</a> </li> 
     <li><a href="#team" class="MCXref xref">Equipo</a> </li> 
     <li><a href="#template" class="MCXref xref">Plantilla</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">Hoja de horas</a> </li> 
     <li><a href="#update" class="MCXref xref">Actualizar</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">Trabajo </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

Un objeto AccessLevelPermissions representa un conjunto de permisos. Este conjunto de permisos se puede asociar a un nivel de acceso.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>En los campos siguientes se ha añadido el posible valor BUDGETING_INFORMATION. Esto permite a los usuarios con permiso editar prioridades y presupuestar horas en el planificador.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Si un usuario no tiene acceso a un objeto de Workfront que necesite, puede solicitar acceso a ese objeto. El objeto AccessRequest representa esta solicitud.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">acción</p> <p>Se ha añadido el posible valor BUDGETING_INFORMATION. Esto permite a los usuarios con permiso editar prioridades y presupuestar horas en el planificador.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Un objeto AccessRule representa un conjunto de reglas en niveles de acceso personalizados que determina cómo los usuarios pueden compartir los proyectos que crean.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>En los campos siguientes se ha añadido el posible valor BUDGETING_INFORMATION. Esto permite a los usuarios con permiso editar prioridades y presupuestar horas en el planificador.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Ruta de aprobación {#approval}

Un elemento de trabajo determinado, como una tarea, un documento o una plantilla de horas, puede requerir que un supervisor u otro usuario firme el elemento de trabajo. Un objeto Approval representa la acción de cerrar sesión en un elemento de trabajo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos directos<p style="font-weight: normal;">En los campos siguientes se han añadido los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no pueden establecerse antes del año 1900 o después del 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los siguientes campos a la API pública para mantener la transparencia en el cálculo de EAC (Estimar al finalizar).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">También conocido como Valor acumulado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de tarea que realmente se completó en el momento en que se calcula esta métrica. Para las tareas, CPTR = Porcentaje real completado x Presupuesto de tareas. Para Proyectos, CPTR = SUMA (valores CPTR de todas las tareas principales e individuales).</p></li>
     <li><p style="font-weight: bold;">CPTP</p><p style="font-weight: normal;">También conocido como Valor planificado, el Costo presupuestado del trabajo programado (CPTP) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de tarea que debería haberse completado en el momento en que se calcula esta métrica. Para tareas, CPTP = Porcentaje planificado completado x Presupuesto de tareas. Para los proyectos, CPTP = SUMA (valores CPTP de todas las tareas principales e individuales).</p></li>
    </ul><p style="font-weight: normal;">Los siguientes campos han añadido el posible valor ET. Este valor representa la unidad de tiempo de los meses transcurridos, que hace referencia a meses sin tener en cuenta fines de semana o festivos.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Los siguientes campos han añadido el indicador CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Los campos siguientes se han eliminado del objeto Approval.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">Se agregó el siguiente campo al objeto Approval.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Eliminado del objeto Approval  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Se ha agregado al objeto Approval.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

Un objeto ApprovalPath es una rama dentro de un proceso de aprobación. Las rutas de aprobación se basan en el estado del objeto al que está asociado el proceso de aprobación.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Se ha añadido el posible valor ET. Este valor representa la unidad de tiempo de los meses transcurridos, que hace referencia a meses sin tener en cuenta fines de semana o festivos.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

Un objeto ApprovalProcess es una aprobación de varios pasos que puede asociarse a un proyecto, tarea o problema.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo, que es un parámetro booleano con un valor true si un objeto está activo y false si no lo está. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos. Los objetos no definidos como Activos no son visibles en los menús desplegables ni en los campos de escritura anticipada para adjuntarlos a otros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Asignación {#assignment}

Un objeto de asignación representa la conexión entre un elemento de trabajo y el usuario, equipo o grupo asignado para trabajar en él.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">Se ha añadido el posible valor ET. Este valor representa la unidad de tiempo de los meses transcurridos, que hace referencia a meses sin tener en cuenta fines de semana o festivos.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BaselineTask {#baselinetask}

Las líneas de base son instantáneas del aspecto que tuvo el rendimiento de un proyecto en un momento determinado. Almacenan información clave sobre el proyecto, como fechas clave, progreso, valores de costes e ingresos. Cuando se crea una línea de base, la información de la tarea también se captura en las tareas de línea de base de esa línea de base.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Se ha añadido el posible valor ET. Este valor representa la unidad de tiempo de los meses transcurridos, que hace referencia a meses sin tener en cuenta fines de semana o festivos.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoría {#category}

Un objeto Category es un formulario personalizado. Se pueden generar informes para este objeto y mostrarlos en otros informes de objetos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo, que es un parámetro booleano con un valor true si un objeto está activo y false si no lo está. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos. Los objetos no definidos como Activos no son visibles en los menús desplegables ni en los campos de escritura anticipada para adjuntarlos a otros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Compañía {#company}

Un objeto Company representa una organización formada por una colección de personas. Las compañías están asociadas a un usuario o a un proyecto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo, que es un parámetro booleano con un valor true si un objeto está activo y false si no lo está. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos. Los objetos no definidos como Activos no son visibles en los menús desplegables ni en los campos de escritura anticipada para adjuntarlos a otros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Acciones</td> 
   <td> <p style="font-weight: normal;">Se agregaron las acciones siguientes al objeto CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> <p>Se agregaron las consultas siguientes al objeto CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente {#customer}

Un objeto Customer representa una organización que utiliza una instancia de Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Se agregaron valores posibles: </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (Condiciones del proyecto)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (condiciones de tarea)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (Condiciones del problema)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>Acciones</td> 
   <td> <p style="font-weight: normal;">Se agregaron las siguientes acciones al objeto Customer</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Preferencias del cliente {#customerpreferences}

Un objeto CustomerPreferences representa el conjunto de preferencias que un cliente ha establecido para su instancia de Workfront.

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Se agregaron valores posibles:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy (Requisitos de complejidad de contraseña)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (Longitud mínima de contraseña)</li> 
       <li style="font-weight: normal;">contraseña:mobileSessionTimeout (tiempo de espera de sesión móvil)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (Tiempo libre del usuario)</li> 
       <li style="font-weight: normal;">hoja de horas:default.timesheet.manualrole (función de control manual)</li> 
       <li style="font-weight: normal;">prueba:defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">prueba:defaultNonRecipientGuestRole (config.proofhq.defaultnonrecipientguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Acciones</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Documento {#document}

Un objeto Document representa un archivo (como material escrito, imágenes u otras formas de información).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Acciones</td> 
   <td> <p>Se agregaron las siguientes acciones al objeto Document.</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Iteración {#iteration}

Un objeto Iteration representa una sola iteración Agile. Las iteraciones son períodos de tiempo discretos que se utilizan para planificar y completar historias de Agile.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>Se han añadido los campos siguientes al objeto Iteration.</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">puntos completados</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Plantilla de diseño {#layout-template}

Un objeto de plantilla de diseño representa una disposición concreta de elementos de diseño, como el menú principal, el panel de navegación o el área de Inicio. Las plantillas de diseño se pueden asignar a usuarios, equipos, grupos o funciones del puesto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">Este campo se ha añadido y es un parámetro booleano que tiene un valor de true si una plantilla de diseño está configurada para mostrar marcas de hora para las fechas de vencimiento en la Lista de trabajos y el Calendario, y de false si está configurada para ocultar marcas de hora.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### MilestonePath {#milestonepath}

Un hito es un marcador en una tarea que indica que es un punto clave en el proyecto. Generalmente se utiliza para denotar un evento significativo, como la finalización de una fase del proyecto o un conjunto de actividades críticas. Un objeto MilestonePath es una colección de hitos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo, que es un parámetro booleano con un valor true si un objeto está activo y false si no lo está. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos. Los objetos no definidos como Activos no son visibles en los menús desplegables ni en los campos de escritura anticipada para adjuntarlos a otros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Nota {#note}

Un objeto Note es un comentario o una actualización realizada sobre un objeto Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>Se agregaron los campos siguientes al objeto Note.</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>me gusta</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Un objeto OpTask suele conocerse como Problema. Un problema es un elemento de trabajo que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Un problema también puede ser una solicitud del servicio de asistencia. Las solicitudes de cambio, las solicitudes y los errores también son problemas.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos directos<p style="font-weight: normal;">En los campos siguientes se han añadido los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no pueden establecerse antes del año 1900 o después del 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los campos siguientes a OpTask.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">El ID de Workfront único de un objeto del Panel Kanban.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">Porcentaje completado es un parámetro que devuelve la cantidad completada de un problema en forma de porcentaje.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">trabajar  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Buscar campos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>trabajar</p> <p style="font-weight: normal;">Eliminado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Acciones</td> 
   <td> <p>Se agregaron las siguientes acciones al objeto OpTask</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parámetro {#parameter}

Un objeto Parameter es un campo personalizado.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Se ha agregado el posible valor TYAH (Escritura anticipada).</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Este campo se ha añadido y hace referencia al código de objeto de un objeto al que se hace referencia. Los códigos de objeto de todos los objetos se encuentran en <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portafolio {#portfolio}

Un objeto Portfolio es una colección de proyectos que compiten por los mismos recursos, normalmente dinero o personas para completarlos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Se ha añadido el validador MAX_LENGTH, que especifica que la longitud de la descripción no es superior a 4000 caracteres.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programar {#program}

Un objeto Program es un subconjunto de un portafolio en el que se pueden agrupar proyectos similares.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Se ha añadido el validador MAX_LENGTH, que especifica que la longitud de la descripción no es superior a 4000 caracteres.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo, que es un parámetro booleano con un valor true si un objeto está activo y false si no lo está. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos. Los objetos no definidos como Activos no son visibles en los menús desplegables ni en los campos de escritura anticipada para adjuntarlos a otros objetos.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">Se ha añadido el validador MAX_LENGTH, que especifica que la longitud del nombre no es superior a 255 caracteres.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Proyecto {#project}

Los proyectos son elementos de trabajo dentro de Workfront y son un bloque de creación principal en la forma en que Workfront ayuda a las personas a realizar su trabajo. Un objeto Project representa un grupo de tareas con un objetivo común y específico.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos directos<p style="font-weight: normal;">En los campos siguientes se han añadido los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no pueden establecerse antes del año 1900 o después del 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los siguientes campos a la API pública para mantener la transparencia en el cálculo de EAC (Estimar al finalizar).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">También conocido como Valor acumulado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de tarea que realmente se completó en el momento en que se calcula esta métrica. Para las tareas, CPTR = Porcentaje real completado x Presupuesto de tareas. Para Proyectos, CPTR = SUMA (valores CPTR de todas las tareas principales e individuales).</p></li>
     <li><p style="font-weight: bold;">CPTP</p><p style="font-weight: normal;">También conocido como Valor planificado, el Costo presupuestado del trabajo programado (CPTP) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de tarea que debería haberse completado en el momento en que se calcula esta métrica. Para tareas, CPTP = Porcentaje planificado completado x Presupuesto de tareas. Para los proyectos, CPTP = SUMA (valores CPTP de todas las tareas principales e individuales).</p></li>
    </ul><p style="font-weight: normal;">Los siguientes campos han añadido el indicador CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">El campo siguiente se quitó del objeto Project.</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ProofApproval {#proofapproval}

Un objeto ProofApproval representa una aprobación que está conectada directamente a una prueba.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitedDecision</p> <p style="font-weight: normal;">Este campo se ha añadido y es un parámetro booleano que tiene un valor de true si una prueba espera una decisión y de false si no lo tiene.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área del servicio de asistencia para permitir a los usuarios enviar problemas al mismo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>En los campos siguientes se ha añadido el posible valor BUDGETING_INFORMATION. Esto permite a los usuarios con permiso editar prioridades y presupuestar horas en el planificador.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### TiempoReservado {#reservedtime}

Un objeto ReservedTime representa los días especificados en la hora personal de un usuario, lo que indica que el usuario no estará disponible para trabajar.

El recurso ReservedTime ha añadido el indicador REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>Los campos siguientes quitaron el indicador NOT_GROUPABLE.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>El campo siguiente se ha eliminado del objeto ReservedTime.</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>tarea</p> <p style="font-weight: normal;">Eliminado  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operaciones</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>EDITAR</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

Un objeto ResourcePlannerFilter es un conjunto de reglas que determinan qué elementos se mostrarán en el Planificador de recursos.

El recurso ResourcePlannerFilter agregó el indicador SHARABLE. No se han producido otros cambios en el objeto.

### Riesgo {#risk}

Un objeto Risk representa un posible evento que puede impedir que un proyecto finalice a tiempo o dentro del presupuesto. Se añaden riesgos a los proyectos en la fase de planificación para identificar posibles obstáculos antes de la aprobación de cualquier trabajo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>Se agregaron los campos siguientes al objeto Riesgo:</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">El ID del usuario que creó originalmente el objeto.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>La fecha en la que un usuario envió un objeto en Workfront.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>El parámetro Fecha de última actualización devolverá esa fecha en la que se realizó la última actualización en un objeto,</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Última actualización por identificador es un parámetro que devuelve el identificador del último usuario que actualizó el objeto.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> <p style="font-weight: normal;">Se agregaron los campos de referencia siguientes al objeto Risk.</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### InformeProgramado {#scheduledreport}

Un objeto ScheduledReport representa un informe que se ha configurado para que se programe su envío.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">Se agregaron los siguientes valores posibles:</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Un objeto ScoreCardQuestion representa una pregunta que se ha agregado a un informe de valoración. Estas preguntas suelen ser determinadas por el gestor del Portfolio, y sus respuestas le permiten comprender cómo se ajusta un proyecto a los objetivos del portafolio.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Se ha agregado el posible valor TYAH (Escritura anticipada)  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tarea {#task}

Un objeto Task representa un elemento de trabajo que debe realizarse como un paso hacia el logro de un objetivo final (completar un proyecto).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos directos<p style="font-weight: normal;">En los campos siguientes se han añadido los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no pueden establecerse antes del año 1900 o después del 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los siguientes campos a la API pública para mantener la transparencia en el cálculo de EAC (Estimar al finalizar).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">También conocido como Valor acumulado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de tarea que realmente se completó en el momento en que se calcula esta métrica. Para las tareas, CPTR = Porcentaje real completado x Presupuesto de tareas. Para Proyectos, CPTR = SUMA (valores CPTR de todas las tareas principales e individuales).</p></li>
     <li><p style="font-weight: bold;">CPTP</p><p style="font-weight: normal;">También conocido como Valor planificado, el Costo presupuestado del trabajo programado (CPTP) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de tarea que debería haberse completado en el momento en que se calcula esta métrica. Para tareas, CPTP = Porcentaje planificado completado x Presupuesto de tareas. Para los proyectos, CPTP = SUMA (valores CPTP de todas las tareas principales e individuales).</p></li>
    </ul><p style="font-weight: normal;">Los siguientes campos han añadido el posible valor ET. Este valor representa la unidad de tiempo de los meses transcurridos, que hace referencia a meses sin tener en cuenta fines de semana o festivos.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">El campo siguiente se ha eliminado del objeto Task.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">Se agregó el siguiente campo al objeto Task.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Eliminado  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Equipo {#team}

Un objeto Team es una colección de usuarios que se pueden asignar a un elemento de trabajo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Este campo se ha añadido al objeto Equipo. El tipo de estimación de Agile determina cómo se calcula la carga de trabajo de una historia. Si se estima en horas, este es el número de horas planificadas que se añaden a la historia. Si se estima en puntos, cada punto agregará un número de horas planificadas a la historia en función de cómo se establezcan los puntos (el valor predeterminado es de 8 horas). Los valores posibles para el tipo de estimación de Agile son:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (puntos de la historia)</li> 
       <li style="font-weight: normal;">HORAS (horas)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (horas como puntos)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Plantilla {#template}

Un objeto Template representa un patrón para un objeto Project. Los proyectos se pueden crear a partir de Plantillas para ahorrar tiempo. Una plantilla contiene un equipo y tareas, que se copiarán en un proyecto cuando se utilice la plantilla.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo, que es un parámetro booleano con un valor true si un objeto está activo y false si no lo está. Los objetos que se definen como Activos aparecen en menús desplegables y campos de escritura anticipada y pueden adjuntarse a otros objetos. Los objetos no definidos como Activos no son visibles en los menús desplegables ni en los campos de escritura anticipada para adjuntarlos a otros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateAssignment {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">Se ha añadido el posible valor ET. Este valor representa la unidad de tiempo de los meses transcurridos, que hace referencia a meses sin tener en cuenta fines de semana o festivos.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Un objeto TemplateTask representa un objeto Task que forma parte de un objeto Template. Las Tareas de plantilla pasan a ser Tareas en el Proyecto en el que se utiliza la Plantilla.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p style="font-weight: normal;">Los siguientes campos han añadido el posible valor ET. Este valor representa la unidad de tiempo de los meses transcurridos, que hace referencia a meses sin tener en cuenta fines de semana o festivos.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Hoja de horas {#timesheet}

Un objeto Timesheet representa un parte de horas virtual que permite a los usuarios especificar horas trabajadas reales para tareas, proyectos y tipos de horas generales.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos principales</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">Eliminado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Actualizar {#update}

Los elementos de trabajo de Workfront se pueden actualizar para mantener a los usuarios informados del estado actual. Un objeto Update representa una de estas actualizaciones. Los usuarios pueden introducir actualizaciones o el sistema de Workfront puede crearlas.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">Se ha agregado un posible valor referenceObjectCustomData (enum.updatetype.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> <p style="font-weight: normal;">Se agregaron las siguientes consultas al objeto Update.</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Acciones</td> 
   <td> <p style="font-weight: normal;">Se agregaron las siguientes acciones al objeto User.</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Acciones</td> 
   <td> <p style="font-weight: normal;">Se agregaron las siguientes acciones al objeto User.</p> 
    <ul> 
     <li style="font-weight: bold;">acceptMyNotifications</li> 
     <li style="font-weight: bold;">unknownAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Trabajo  {#work}

Un objeto Work es una interfaz común que heredan Task y OpTask, y comparte código común entre ambos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos directos<p style="font-weight: normal;">En los campos siguientes se han añadido los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no pueden establecerse antes del año 1900 o después del 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los siguientes campos a la API pública para mantener la transparencia en el cálculo de EAC (Estimar al finalizar).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">También conocido como Valor acumulado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de tarea que realmente se completó en el momento en que se calcula esta métrica. Para las tareas, CPTR = Porcentaje real completado x Presupuesto de tareas. Para Proyectos, CPTR = SUMA (valores CPTR de todas las tareas principales e individuales).</p></li>
     <li><p style="font-weight: bold;">CPTP</p><p style="font-weight: normal;">También conocido como Valor planificado, el Costo presupuestado del trabajo programado (CPTP) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de tarea que debería haberse completado en el momento en que se calcula esta métrica. Para tareas, CPTP = Porcentaje planificado completado x Presupuesto de tareas. Para los proyectos, CPTP = SUMA (valores CPTP de todas las tareas principales e individuales).</p></li>
    </ul><p style="font-weight: normal;">Los siguientes campos han añadido el posible valor ET. Este valor representa la unidad de tiempo de los meses transcurridos, que hace referencia a meses sin tener en cuenta fines de semana o festivos.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">El campo siguiente se ha eliminado del objeto de trabajo.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">Se ha añadido el siguiente campo al objeto de trabajo.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Eliminado  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
