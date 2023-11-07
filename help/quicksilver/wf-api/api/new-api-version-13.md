---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 13 de la API
description: Adobe Workfront publicó la versión 13 de la API el 22 de abril de 2021. La versión 13 de la API incorpora los siguientes cambios con respecto a la versión 12.
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# Novedades de la versión 13 de la API

Adobe Workfront publicó la versión 13 de la API el 22 de abril de 2021. La versión 13 de la API incorpora los siguientes cambios con respecto a la versión 12.

## Recursos añadidos

No se han añadido recursos para la versión 13 de la API.

## Recursos eliminados

No se ha eliminado ningún recurso para la versión 13 de la API.

## Recursos modificados

Se modificaron los siguientes recursos para la versión 13 de la API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">RutaPan</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">Preferencias del cliente</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Grupo </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Proyecto</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Tarea</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Equipo</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Hoja de horas</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">Perfil de hoja de horas</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">UserDelegation</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Trabajo </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

Un objeto AccessLevel está asociado a los usuarios y describe el conjunto de AccessLevelPermissions que determinan a qué puede tener acceso el usuario.

Para obtener más información sobre los niveles de acceso, consulte [Funcionamiento de los niveles de acceso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descripción</b> </p> <p>Se ha añadido el validador MAX_LENGTH, que especifica que la longitud de la descripción no es superior a 4000 caracteres.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RutaPan {#breadcrumb}

Un objeto BreadCrumb representa un elemento en la jerarquía principal/secundario de un elemento de trabajo de Workfront. Las rutas de exploración indican cómo encaja un elemento de trabajo en la mayor estructura de Portfolio, Proyectos, Proyectos y Tareas.

Para obtener más información sobre las rutas de exploración, consulte [Información general sobre las rutas en la nueva experiencia de Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Los códigos de objeto se encuentran en <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">Explorador de API</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

Un objeto BurndownEvent representa un objeto que cambia el agrupamiento de una iteración.

Para obtener más información sobre la evolución, consulte [Evolución](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> <p>Los campos siguientes quitaron el indicador NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Preferencias del cliente {#customerpreferences}

Un objeto CustomerPreferences representa el conjunto de preferencias que un cliente ha establecido para su instancia de Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Se agregaron valores posibles:</p> 
      <ul> 
       <li style="font-weight: normal;">contraseña:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> contraseña:aemAADomain (config.general.aem.adomain) </li> 
       <li style="font-weight: normal;">contraseña:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">contraseña:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">hoja de horas:default.timesheet.restrict.timesheet.edit.owner.admins (config.timesheet.restrict.timesheet.edit.owner.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Acciones</td> 
   <td> <p>Se agregaron las siguientes acciones al recurso Preferencias del cliente.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Toma el argumento:</p> 
      <ul> 
       <li> <p>preferencias (mapa)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Un objeto DocumentVersion representa una versión específica de un archivo (como material escrito, imágenes u otras formas de información).

Para obtener más información sobre las versiones de los documentos, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Se ha agregado el valor posible:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Se ha añadido el indicador NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo  {#group}

Un objeto Group representa un conjunto de usuarios y equipos. Los grupos a menudo representan la estructura departamental.

Para obtener más información sobre los grupos, consulte [Grupos vs. equipos en Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Acciones</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>Esta acción devuelve una matriz de los grupos principales del grupo (grupos de los que es subgrupo el grupo dado).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

El objeto JournalEntry se puede configurar para que registre información sobre campos de objeto específicos cada vez que se modifiquen dichos campos. Cuando un campo está configurado para registrarse como parte del objeto Entrada de cuaderno, se creará una Entrada de cuaderno correspondiente cada vez que se modifique ese campo.

El recurso JournalEntry agregó el indicador REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> <p>Los campos siguientes quitaron el indicador NOT_GROUPABLE:</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>Los siguientes campos han añadido el indicador NOT_FILTERABLE:</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Los administradores de Adobe Workfront o de grupos pueden crear plantillas para personalizar los elementos de diseño en Adobe Workfront. El objeto LayoutTemplate es específico de Adobe Workfront Classic.

Para ver el objeto que representa las plantillas de diseño en la nueva experiencia de Adobe Workfront, consulte [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Descripción</b> </p> <p>Se ha añadido el validador MAX_LENGTH, que especifica que la longitud de la descripción no es superior a 4000 caracteres.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Un objeto LinkedFolder representa una carpeta vinculada desde un proveedor de documentos externo, como Google Drive o Dropbox.

Para obtener más información sobre las carpetas vinculadas, consulte [Vinculación de documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Se ha agregado el valor posible:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>Buscar campos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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
   <td> <p>Campos directos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>Campos directos</p> </td> 
   <td> <p>Se agregaron los campos siguientes al recurso ProofApproval.</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>DecisionDate</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Un objeto QueueDef representa una cola, que es un proyecto que se ha publicado en el área del servicio de asistencia para permitir a los usuarios enviar problemas al mismo.

Para obtener más información sobre las colas de solicitudes, consulte [Crear una cola de solicitudes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Agregado. Los valores posibles son:</p> 
      <ul> 
       <li> <p>0 (después de formularios personalizados)</p> </li> 
       <li> <p>1 (Antes de formularios personalizados)</p> </li> 
      </ul> </li> 
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
   <td> <p>Buscar campos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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

### Hoja de horas {#timesheet}

Un objeto Timesheet representa un parte de horas virtual que permite a los usuarios especificar horas trabajadas reales para tareas, proyectos y tipos de horas generales.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos principales</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Eliminado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Perfil de hoja de horas {#timesheetprofile}

Un objeto Timesheet representa un parte de horas virtual que permite a los usuarios especificar horas trabajadas reales para tareas, proyectos y tipos de horas generales.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Campos directos</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Campos predeterminados</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Agregado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Los administradores de Adobe Workfront o de grupos pueden crear plantillas para personalizar los elementos de diseño en Adobe Workfront. El objeto UITemplate es específico de la nueva experiencia de Adobe Workfront.

Para ver el objeto que representa las plantillas de diseño en Adobe Workfront Classic, consulte [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Acciones</td> 
   <td> <p>Se agregaron las siguientes acciones al recurso UITemplate.</p> 
    <ul> 
     <li> <p><b>migrationCustomersAllLayoutTemplates</b> </p> <p>Toma el argumento:</p> 
      <ul> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrationLayoutTemplates</b> </p> <p>Toma los argumentos:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (booleano)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegation {#userdelegation}

Un objeto UserDelegation representa el acto de delegar el trabajo de un usuario a otro durante un período de tiempo específico.

El objeto UserDelegation agregó el indicador REPORTABLE.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos directos</td> 
   <td> <p>Los campos siguientes quitaron el indicador NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos predeterminados</td> 
   <td> <p>Se agregaron los campos siguientes:</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
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
   <td> <p>Buscar campos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
