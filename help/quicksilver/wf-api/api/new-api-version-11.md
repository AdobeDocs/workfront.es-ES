---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 11 de la API
description: ReportableBudgedHour se ha agregado a la API de Adobe Workfront como un recurso para la creación de informes. Incluye campos de referencia, campos principales y campos predeterminados que están ausentes en BudgetedHour.
author: John
feature: Workfront API
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
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

* [ReportBudgetedHour](#reportablebudgetedhour)

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
     <li style="font-weight: bold;">descriptor de acceso</li> 
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

### ReportBudgetedHour {#reportablebudgetedhour}

ReportableBudgedHour se ha agregado a la API de Adobe Workfront como un recurso para la creación de informes. Incluye campos de referencia, campos principales y campos predeterminados que están ausentes en BudgetedHour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocateDate </p> <p>La fecha de asignación es el primer día (un domingo) de la semana para el que se presupuestaron las horas en el planificador de recursos.</p> </li> 
     <li> <p style="font-weight: bold;">budgetHours </p> <p>Las horas presupuestadas son horas que el gestor de recursos presupuesta para el trabajo que los recursos necesitan completar en los proyectos</p> </li> 
     <li> <p style="font-weight: bold;">Identificador </p> <p>ID de Workfront único asignado a un objeto específico de la hora presupuestada de informes.</p> </li> 
     <li style="font-weight: bold;">scheduledBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>ID de Workfront único asignado a un proyecto específico.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>ID de Workfront único asignado a una función de trabajo específica.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>ID de Workfront único asignado a un usuario específico.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">proyecto</p> <p>Proyecto al que está asociada una ReportBudgetedHour.</p> </li> 
     <li> <p style="font-weight: bold;">rol</p> <p>Función de trabajo a la que está asociada una ReportBudgetedHour.</p> </li> 
     <li> <p style="font-weight: bold;">usuario</p> <p>Usuario al que está asociada una ReportBudgetedHour.</p> </li> 
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

No se eliminaron recursos para la API v11.

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
     <li><a href="#approvalprocess" class="MCXref xref">Proceso de aprobación</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Asignación</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">BaselineTask</a> </li> 
     <li><a href="#category" class="MCXref xref">Categoría</a> </li> 
     <li><a href="#company" class="MCXref xref">Compañía</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Cliente</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">Preferencias de cliente</a> </li> 
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
     <li><a href="#reservedtime" class="MCXref xref">ReservvedTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">Riesgo</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">Informe programado</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">Tarea</a> </li> 
     <li><a href="#team" class="MCXref xref">Equipo</a> </li> 
     <li><a href="#template" class="MCXref xref">Plantilla</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">Asignación de plantilla</a> </li> 
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
   <td> <p>Los siguientes campos agregaron el posible valor BUDGETING_INFORMATION . Esto permite a los usuarios con permiso editar prioridades y horas de presupuesto en el planificador.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">prohibidaActions</li> 
     <li style="font-weight: bold;">secundarioActions  </li> 
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
     <li> <p style="font-weight: bold;">acción</p> <p>Se ha añadido el valor posible BUDGETING_INFORMATION. Esto permite a los usuarios con permiso editar prioridades y horas de presupuesto en el planificador.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Un objeto AccessRule representa un conjunto de reglas en niveles de acceso personalizados que determina cómo pueden compartir los usuarios los proyectos que crean.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>Los siguientes campos agregaron el posible valor BUDGETING_INFORMATION . Esto permite a los usuarios con permiso editar prioridades y horas de presupuesto en el planificador.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">prohibidaActions</li> 
     <li style="font-weight: bold;">secundarioActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Ruta de aprobación {#approval}

Un elemento de trabajo determinado, como una tarea, un documento o un parte de horas, puede requerir que un supervisor u otro usuario cierre la sesión en el elemento de trabajo. Un objeto Approval representa la acción de cerrar sesión en un elemento de trabajo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos directos<p style="font-weight: normal;">Los siguientes campos agregaron los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no pueden establecerse antes del año 1900 o después de 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los siguientes campos a la API pública para transparencia en el cálculo de EAC (Estimación al completarse).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">También conocido como el Valor Ganado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de la tarea que realmente se completó en el momento en que se calcula esta métrica. Para las tareas, CPTR = Porcentaje real completado x Presupuesto de la tarea. Para Proyectos, BCWP = SUM(valores BCWP de todas las tareas principales e individuales).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">También conocido como valor planeado, el costo presupuestado del trabajo programado (BCWS) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de la tarea que debería haberse completado en el momento en que se calcula esta métrica. Para las tareas, BCWS = Porcentaje completado planeado x Presupuesto de tareas. Para proyectos, BCWS = SUM(valores BCWS de todas las tareas principales e individuales).</p></li>
    </ul><p style="font-weight: normal;">Los campos siguientes agregaron el posible valor ET. Este valor representa la unidad de tiempo Meses transcurridos, que hace referencia a meses sin tener en cuenta los fines de semana ni los días festivos.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Los campos siguientes agregaron el indicador MONEDA</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Los campos siguientes se eliminaron del objeto Approval .</p>
    <ul>
     <li style="font-weight: bold;">reserveTimeID</li>
     <li style="font-weight: bold;">línea de tiempoExceptionInfo</li>
    </ul><p style="font-weight: normal;">Se ha añadido el campo siguiente al objeto Approval .</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reserveTime</p> <p style="font-weight: normal;">Eliminado del objeto Approval  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Se agrega al objeto Approval.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

Un objeto ApprovalPath es una rama de un proceso de aprobación. Las rutas de aprobación se basan en el estado del objeto al que está asociado el proceso de aprobación.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Se ha agregado el valor posible ET. Este valor representa la unidad de tiempo Meses transcurridos, que hace referencia a meses sin tener en cuenta los fines de semana ni los días festivos.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Proceso de aprobación {#approvalprocess}

Un objeto ApprovalProcess es una aprobación de varios pasos que puede asociarse a un proyecto, tarea o problema.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo y es un parámetro booleano que tiene un valor de true si un objeto está activo y de false si no lo está. Los objetos que se establecen como Activo aparecen en los menús desplegables y en los campos de avance de tipo y se pueden adjuntar a otros objetos. Los objetos que no se establecen en Activo no están visibles en los menús desplegables ni en los campos de tipo anterior para adjuntarlos a otros objetos.  </p> </li> 
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

Un objeto de asignación representa la conexión entre un elemento de trabajo y el usuario, equipo o grupo que está asignado para trabajar en él.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">Se ha agregado el valor posible ET. Este valor representa la unidad de tiempo Meses transcurridos, que hace referencia a meses sin tener en cuenta los fines de semana ni los días festivos.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BaselineTask {#baselinetask}

Las líneas de base son instantáneas de cómo se veía el rendimiento de un proyecto en un momento dado. Almacenan información clave sobre el proyecto, como fechas clave, progreso, costos y valores de ingresos. Cuando se crea una línea de base, la información de la tarea también se captura en las tareas de línea de base de esa línea de base.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Se ha agregado el valor posible ET. Este valor representa la unidad de tiempo Meses transcurridos, que hace referencia a meses sin tener en cuenta los fines de semana ni los días festivos.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoría {#category}

Un objeto Category es un formulario personalizado. Puede crear informes para este objeto y mostrarlos también en otros informes de objeto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo y es un parámetro booleano que tiene un valor de true si un objeto está activo y de false si no lo está. Los objetos que se establecen como Activo aparecen en los menús desplegables y en los campos de avance de tipo y se pueden adjuntar a otros objetos. Los objetos que no se establecen en Activo no están visibles en los menús desplegables ni en los campos de tipo anterior para adjuntarlos a otros objetos.  </p> </li> 
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

Un objeto Company representa una organización que consta de una colección de personas. Las empresas están asociadas a un usuario o a un proyecto.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo y es un parámetro booleano que tiene un valor de true si un objeto está activo y de false si no lo está. Los objetos que se establecen como Activo aparecen en los menús desplegables y en los campos de avance de tipo y se pueden adjuntar a otros objetos. Los objetos que no se establecen en Activo no están visibles en los menús desplegables ni en los campos de tipo anterior para adjuntarlos a otros objetos.  </p> </li> 
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
   <td> <p style="font-weight: normal;">Se agregaron las siguientes acciones al objeto CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> <p>Se agregaron las siguientes consultas al objeto CustomEnum</p> 
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
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Se han añadido valores posibles: </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (Condiciones del proyecto)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (Condiciones de la tarea)</li> 
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
   <td> <p style="font-weight: normal;">Se agregaron las siguientes acciones al objeto Cliente</p> 
    <ul> 
     <li style="font-weight: bold;">targetsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Preferencias de cliente {#customerpreferences}

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
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Se han añadido valores posibles:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy (Requisitos de complejidad de las contraseñas)</li> 
       <li style="font-weight: normal;"> password:password.MinimumLength (longitud mínima de la contraseña)</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout (tiempo de espera de sesión móvil)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (Tiempo de espera del usuario desactivado)</li> 
       <li style="font-weight: normal;">parte de horas:default.timesheet.manualrole (función de control manual)</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole (config.proofhq.defaultnonrecipientguestrole)  </li> 
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
   <td> <p>Se agregaron las siguientes acciones al objeto Document .</p> 
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
   <td> <p>Se agregaron los campos siguientes al objeto Iteration .</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">puntos completados</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Plantilla de diseño {#layout-template}

Un objeto de plantilla de diseño representa una disposición concreta de elementos de diseño, como el menú principal, el panel de navegación o el área principal. Las plantillas de diseño se pueden asignar a usuarios, equipos, grupos o funciones de trabajo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">Se ha agregado este campo y es un parámetro booleano que tiene el valor "true" si una plantilla de diseño está configurada para mostrar marcas de hora para fechas de vencimiento en la lista de trabajo y el calendario, y "false" si se establece para ocultar marcas de hora.  </p> </li> 
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

Un hito es un marcador de una tarea que indica que es un punto clave del proyecto. Generalmente se utiliza para denotar un acontecimiento significativo, como la finalización de una fase del proyecto o un conjunto de actividades críticas. Un objeto MilestonePath es una colección de hitos.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo y es un parámetro booleano que tiene un valor de true si un objeto está activo y de false si no lo está. Los objetos que se establecen como Activo aparecen en los menús desplegables y en los campos de avance de tipo y se pueden adjuntar a otros objetos. Los objetos que no se establecen en Activo no están visibles en los menús desplegables ni en los campos de tipo anterior para adjuntarlos a otros objetos.  </p> </li> 
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

Un objeto Note es un comentario o actualización realizados en un objeto Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>Se agregaron los campos siguientes al objeto Note .</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>gustar</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Un objeto OpTask se conoce comúnmente como Problema. Un problema es un elemento de trabajo que normalmente indica que hay un problema que impide la finalización de una tarea o proyecto. Un problema también puede ser una solicitud de asistencia técnica. Los cambios de pedidos, solicitudes y errores también son problemas.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos directos<p style="font-weight: normal;">Los siguientes campos agregaron los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no se pueden establecer antes del año 1900 o después de 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los campos siguientes a OpTask.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">ID de Workfront único de un objeto de placa Kanban.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">Porcentaje completado es un parámetro que devuelve la cantidad completa de un problema, como porcentaje.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">trabajo  </li>
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
     <li style="font-weight: bold;"> <p>trabajo</p> <p style="font-weight: normal;">Eliminado</p> </li> 
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
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Se ha agregado un posible valor TYAH (Typeforward).</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Este campo se agregó y hace referencia al código de objeto de un objeto al que se hace referencia. Los códigos de objeto de todos los objetos se encuentran en la <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.  </p> </li> 
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
     <li style="font-weight: bold;"> <p>descripción</p> <p style="font-weight: normal;">Se ha añadido el validador MAX_LENGTH, que especifica que la longitud de la descripción no supera los 4000 caracteres.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programar {#program}

Un objeto Program es un subconjunto dentro de un portafolio, donde proyectos similares se pueden agrupar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>descripción</p> <p style="font-weight: normal;">Se ha añadido el validador MAX_LENGTH, que especifica que la longitud de la descripción no supera los 4000 caracteres.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo y es un parámetro booleano que tiene un valor de true si un objeto está activo y de false si no lo está. Los objetos que se establecen como Activo aparecen en los menús desplegables y en los campos de avance de tipo y se pueden adjuntar a otros objetos. Los objetos que no se establecen en Activo no están visibles en los menús desplegables ni en los campos de tipo anterior para adjuntarlos a otros objetos.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">Se ha añadido el validador MAX_LENGTH, que especifica que la longitud del nombre no supera los 255 caracteres.  </p> </li> 
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

Los proyectos son elementos de trabajo dentro de Workfront y son un componente principal de la forma en que Workfront ayuda a las personas a hacer su trabajo. Un objeto Project representa un grupo de tareas con un objetivo específico común.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos directos<p style="font-weight: normal;">Los siguientes campos agregaron los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no se pueden establecer antes del año 1900 o después de 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los siguientes campos a la API pública para transparencia en el cálculo de EAC (Estimación al completarse).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">También conocido como el Valor Ganado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de la tarea que realmente se completó en el momento en que se calcula esta métrica. Para las tareas, CPTR = Porcentaje real completado x Presupuesto de la tarea. Para Proyectos, BCWP = SUM(valores BCWP de todas las tareas principales e individuales).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">También conocido como valor planeado, el costo presupuestado del trabajo programado (BCWS) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de la tarea que debería haberse completado en el momento en que se calcula esta métrica. Para las tareas, BCWS = Porcentaje completado planeado x Presupuesto de tareas. Para proyectos, BCWS = SUM(valores BCWS de todas las tareas principales e individuales).</p></li>
    </ul><p style="font-weight: normal;">Los campos siguientes agregaron el indicador MONEDA</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Se quitó el siguiente campo del objeto Project.</p>
    <ul>
     <li style="font-weight: bold;">línea de tiempoExceptionInfo</li>
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
     <li style="font-weight: bold;"> <p>isApendingdecisions</p> <p style="font-weight: normal;">Se ha añadido este campo y es un parámetro booleano que tiene el valor true si una prueba está a la espera de una decisión y false si no lo está.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área de asistencia técnica para permitir a los usuarios enviarle problemas.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>Los siguientes campos agregaron el posible valor BUDGETING_INFORMATION . Esto permite a los usuarios con permiso editar prioridades y horas de presupuesto en el planificador.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbioredActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservvedTime {#reservedtime}

Un objeto ReservedTime representa los días especificados en la hora personal de un usuario, lo que indica que este no estará disponible para el trabajo.

El recurso ReservedTime agregó el indicador REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>Los campos siguientes eliminaron el indicador NOT_GROUPABLE.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>El siguiente campo se ha eliminado del objeto ReservedTime.</p> 
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

El recurso ResourcePlannerFilter agregó el indicador SHARABLE. No se han realizado otros cambios en el objeto.

### Riesgo {#risk}

Un objeto Risk representa un posible evento que puede impedir que un proyecto termine a tiempo o dentro del presupuesto. Se añaden riesgos a los proyectos en la fase de planificación para identificar posibles obstáculos antes de la aprobación de cualquier trabajo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p>Se agregaron los campos siguientes al objeto Risk :</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">ID del usuario que creó originalmente el objeto.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Fecha en la que un usuario envió un objeto en Workfront.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>El parámetro Última fecha de actualización devolverá esa fecha en la que se realizó la última actualización en un objeto,</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Última actualización por ID es un parámetro que devolverá el ID de usuario del último usuario que actualizó el objeto.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> <p style="font-weight: normal;">Se agregaron los siguientes campos de referencia al objeto RIsk.</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Informe programado {#scheduledreport}

Un objeto ScheduledReport representa un informe que se ha configurado para su envío programado.

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

Un objeto ScoreCardQuestion representa una pregunta que se ha agregado a un informe de valoración. Estas preguntas suelen ser determinadas por el administrador de Portfolio y sus respuestas permiten al administrador comprender cómo se alinea un proyecto con los objetivos del portafolio.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Se ha agregado un posible valor TYAH (Typeforward)  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tarea {#task}

Un objeto Task representa un elemento de trabajo que debe realizarse como paso hacia el logro de un objetivo final (completar un proyecto).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Campos directos<p style="font-weight: normal;">Los siguientes campos agregaron los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no se pueden establecer antes del año 1900 o después de 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los siguientes campos a la API pública para transparencia en el cálculo de EAC (Estimación al completarse).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">También conocido como el Valor Ganado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de la tarea que realmente se completó en el momento en que se calcula esta métrica. Para las tareas, CPTR = Porcentaje real completado x Presupuesto de la tarea. Para Proyectos, BCWP = SUM(valores BCWP de todas las tareas principales e individuales).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">También conocido como valor planeado, el costo presupuestado del trabajo programado (BCWS) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de la tarea que debería haberse completado en el momento en que se calcula esta métrica. Para las tareas, BCWS = Porcentaje completado planeado x Presupuesto de tareas. Para proyectos, BCWS = SUM(valores BCWS de todas las tareas principales e individuales).</p></li>
    </ul><p style="font-weight: normal;">Los campos siguientes agregaron el posible valor ET. Este valor representa la unidad de tiempo Meses transcurridos, que hace referencia a meses sin tener en cuenta los fines de semana ni los días festivos.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">El siguiente campo se ha eliminado del objeto Task .</p>
    <ul>
     <li style="font-weight: bold;">reserveTimeID</li>
    </ul><p style="font-weight: normal;">Se ha agregado el siguiente campo al objeto Task .</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reserveTime</p> <p style="font-weight: normal;">Eliminado  </p> </li> 
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
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Este campo se agregó al objeto Equipo. El tipo de estimación ágil determina cómo se calcula la carga de trabajo de un artículo. Si se estima en horas, entonces es el número de horas planeadas que se agregan al artículo. Si se estima en puntos, cada punto agregará un número de horas planificadas al artículo en función de cómo se establezcan los puntos (el valor predeterminado es de 8 horas). Los valores posibles de Tipo de estimación ágil son:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (puntos de artículo)</li> 
       <li style="font-weight: normal;">HORAS (Horas)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (Horas como puntos)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Plantilla {#template}

Un objeto Template representa un patrón para un proyecto. Los proyectos se pueden crear desde Plantillas para ahorrar tiempo. Una plantilla contiene un equipo y tareas, que se copiarán en un proyecto cuando se utilice la plantilla.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Se ha añadido este campo y es un parámetro booleano que tiene un valor de true si un objeto está activo y de false si no lo está. Los objetos que se establecen como Activo aparecen en los menús desplegables y en los campos de avance de tipo y se pueden adjuntar a otros objetos. Los objetos que no se establecen en Activo no están visibles en los menús desplegables ni en los campos de tipo anterior para adjuntarlos a otros objetos.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>todas las prioridades</p> <p style="font-weight: normal;">Agregado</p> </li> 
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

### Asignación de plantilla {#templateassignment}

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
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">Se ha agregado el valor posible ET. Este valor representa la unidad de tiempo Meses transcurridos, que hace referencia a meses sin tener en cuenta los fines de semana ni los días festivos.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Un objeto TemplateTask representa una tarea que forma parte de una plantilla. Las tareas de plantilla se convierten en tareas del proyecto en el que se utiliza la plantilla.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> <p style="font-weight: normal;">Los campos siguientes agregaron el posible valor ET. Este valor representa la unidad de tiempo Meses transcurridos, que hace referencia a meses sin tener en cuenta los fines de semana ni los días festivos.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos de colección</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>todas las prioridades</p> <p style="font-weight: normal;">Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Hoja de horas {#timesheet}

Un objeto de parte de horas representa un panel de tiempo virtual que permite a los usuarios introducir horas reales trabajadas para tareas, proyectos y tipos de horas generales.

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

Los elementos de trabajo de Workfront se pueden actualizar para mantener a los usuarios informados del estado actual. Un objeto Update representa una de estas actualizaciones. Los usuarios pueden introducir actualizaciones o crearlas en el sistema Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">Se ha añadido un valor posible, referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Consultas</td> 
   <td> <p style="font-weight: normal;">Se agregaron las siguientes consultas al objeto Update .</p> 
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
   <td> <p style="font-weight: normal;">Se agregaron las siguientes acciones al objeto Usuario .</p> 
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
   <td> <p style="font-weight: normal;">Se agregaron las siguientes acciones al objeto Usuario .</p> 
    <ul> 
     <li style="font-weight: bold;">thankMyNotifications</li> 
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
   <td colspan="2">Campos directos<p style="font-weight: normal;">Los siguientes campos agregaron los validadores AT_DATE_BEFORE_YEAR y AT_DATE_AFTER_YEAR. Estos validadores especifican que las fechas de los objetos asociados no se pueden establecer antes del año 1900 o después de 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Se agregaron los siguientes campos a la API pública para transparencia en el cálculo de EAC (Estimación al completarse).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">También conocido como el Valor Ganado, el Costo presupuestado del trabajo realizado (CPTR) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de la tarea que realmente se completó en el momento en que se calcula esta métrica. Para las tareas, CPTR = Porcentaje real completado x Presupuesto de la tarea. Para Proyectos, BCWP = SUM(valores BCWP de todas las tareas principales e individuales).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">También conocido como valor planeado, el costo presupuestado del trabajo programado (BCWS) es una métrica de rendimiento del proyecto que representa el costo presupuestado de la cantidad de la tarea que debería haberse completado en el momento en que se calcula esta métrica. Para las tareas, BCWS = Porcentaje completado planeado x Presupuesto de tareas. Para proyectos, BCWS = SUM(valores BCWS de todas las tareas principales e individuales).</p></li>
    </ul><p style="font-weight: normal;">Los campos siguientes agregaron el posible valor ET. Este valor representa la unidad de tiempo Meses transcurridos, que hace referencia a meses sin tener en cuenta los fines de semana ni los días festivos.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Se quitó el siguiente campo del objeto Work .</p>
    <ul>
     <li style="font-weight: bold;">reserveTimeID</li>
    </ul><p style="font-weight: normal;">Se agregó el siguiente campo al objeto Work .</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Campos de referencia</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reserveTime</p> <p style="font-weight: normal;">Eliminado  </p> </li> 
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
