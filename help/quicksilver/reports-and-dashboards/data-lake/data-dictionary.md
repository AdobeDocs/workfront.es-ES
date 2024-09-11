---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Diccionario de datos de Workfront Data Connect
description: Esta página contiene información sobre la estructura y el contenido de los datos de Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 57c08a06a57bebfaa81035e4fe801f3077e6a829
workflow-type: tm+mt
source-wordcount: '4295'
ht-degree: 4%

---

# Diccionario de datos de Workfront Data Connect

Esta página contiene información sobre la estructura y el contenido de los datos de Workfront Data Connect.

>[!NOTE]
>
>Los datos de Data Connect se actualizan cada cuatro horas, por lo que es posible que los cambios recientes no se reflejen inmediatamente.

## Tipos de tabla

Existen varios tipos de tablas que puede utilizar en Data Connect para ver los datos de Workfront de una manera que proporcione la mayor cantidad de información.

* **Tabla actual**

  La tabla Actual refleja los datos de forma similar a como existe en Workfront, cada objeto y su estado actual. Sin embargo, se puede navegar con una latencia mucho menor que dentro de Workfront.

* **Tabla de eventos**

  La tabla Evento rastrea cada registro de cambios en Workfront: es decir, cada vez que un objeto cambia de estado, se crea un registro que muestra cuándo se produjo el cambio, quién lo hizo y qué se cambió. Por lo tanto, esta tabla es útil para comparaciones puntuales. Esta tabla sólo incluye registros de los últimos tres años.

* **Tabla de historial diario**

  La tabla Historial diario ofrece una versión abreviada de la tabla Evento, ya que muestra el estado de cada objeto diariamente en lugar de cuando se produjo cada evento individual. Como tal, esta tabla es útil para el análisis de tendencias.

<!-- Custom table -->

## Diagrama de relación de entidad

Los objetos de Workfront (y, por lo tanto, de su repositorio de datos de Data Connect) se definen no solo por sus valores individuales, sino también por sus relaciones con otros objetos. El diagrama de relación de entidades que aparece a continuación proporciona una asignación de alto nivel de las relaciones de objeto en Data Connect. El diagrama se puede ver y descargar mediante el siguiente vínculo:

[Diagrama de relación de entidad de Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>El diagrama de relación de entidades es un trabajo en curso; como tal, es solo para fines de referencia y está sujeto a cambios.

## Tipos de fecha

Existen varios objetos de fecha que proporcionan información sobre cuándo se producen eventos específicos.

* `DL_LOAD_TIMESTAMP`: esta fecha se usa como referencia interna y refleja cuándo se cargaron los datos en la tabla Historial actual, Evento o Diario. Esta fecha no debe utilizarse para el análisis de datos y se prevé eliminarla durante la fase beta del lago de datos de Workfront.
* `CALENDAR_DATE`: esta fecha solo está presente en la tabla Historial diario. Esta tabla proporciona un registro del aspecto de los datos a las 11:59 UTC para cada fecha especificada en `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: esta fecha está presente en las tablas Evento e Historial diario y registra exactamente cuándo un registro cambió _a_ el valor que tiene en la fila actual.
* `END_EFFECTIVE_TIMESTAMP`: esta fecha está presente en las tablas Evento e Historial diario y registra exactamente cuándo un registro cambió _de_ el valor de la fila actual a un valor de una fila diferente. Para permitir el intervalo entre consultas en `BEGIN_EFFECTIVE_TIMESTAMP` y `END_EFFECTIVE_TIMESTAMP`, este valor nunca es nulo, aunque no haya ningún valor nuevo. En el caso de que un registro siga siendo válido (es decir, el valor no haya cambiado), `END_EFFECTIVE_TIMESTAMP` tendrá el valor 2300-01-01.

## Tabla de terminología

La siguiente tabla correlaciona los nombres de objetos en Workfront (así como sus nombres en la interfaz y la API) con sus nombres equivalentes en Data Connect.

<table>
  <thead>
    <tr>
        <th>Nombre de entidad de Workfront</th>
        <th>Referencias de interfaz</th>
        <th>Referencia de API | Etiqueta</th>
        <th>Tablas de lago de datos</th>
        <th>Opciones</th>
        <th>Campo de relaciones</th>
        <th>Tabla y campo de relaciones</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>Nivel de acceso</td>
        <td>Nivel de acceso</td>
        <td>ACSLVL | Nivel de acceso</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td></td>
        <td>ACCESSLEVELID (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Self<br>No es una relación; se usa con fines de aplicación interna<br>USER_CURRENT | USERID<br>No es una relación; se usa con fines de aplicación interna<br>El identificador del objeto identificado en el campo OBJCODE<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Regla de acceso</td>
        <td>Compartir</td>
        <td>ACRÚL | Compartir</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td></td>
        <td>ACCESSORID <br>ACCESSRULEID (self) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>Id. del objeto identificado en el campo ACCESSOROBJCODE<br>Self<br>Id. del objeto identificado en el campo ANCESTOROBJCODE<br>USERS_CURRENT | USERID<br>El identificador del objeto identificado en el campo SECURITYOBJCODE<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Ruta de aprobación</td>
        <td>Ruta de aprobación</td>
        <td>ARVPTH | Aprobación</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td></td>
        <td>APPROVALPATHID (self) <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>PROCESOS DE APROBACIÓN_ACTUAL | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>No es una relación; se usa con fines de aplicación interna<br>USERS_CURRENT | USERID<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Proceso de aprobación</td>
        <td>Proceso de aprobación</td>
        <td>ARVPRC | Proceso de aprobación</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID (propio) <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Paso de aprobación</td>
        <td>Paso de aprobación</td>
        <td>ARVSTP | Fase de aprobación</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td></td>
        <td>APPROVALPATHID <br>APPROVALSTEPID (self) <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>ApproverStatus</td>
        <td>Estado de la aprobación</td>
        <td>ARVESTI | ApproverStatus</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td></td>
        <td>APPROVERSTATUSID (self)<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>Identificador del objeto identificado en el campo APPROVABLEOBJCODE<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>No es una relación; se usa con fines de aplicación interna<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Asignación</td>
        <td>Asignación</td>
        <td>ASIGNAR | Asignación</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td></td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID (self)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self<br>CATEGORIES_CURRENT | Actualmente no se admite la tabla de clasificador CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TEAM_CURRENT | IDENTIFICADOR DE EQUIPO<br></td>
    </tr>
    <tr>
        <td>Esperando aprobaciones</td>
        <td>Esperando aprobaciones</td>
        <td>AWAPVL | Esperando aprobación</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td></td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>ESPERANDO APROBACIÓN (AUTO) <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>La tabla de solicitud de acceso no se admite actualmente<br>No es una relación; se usa para propósitos de aplicaciones internas<br>USERS_CURRENT | USERID<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJECTS_CURRENT | PROJECTID<br>ROLES_CURRENT | ROLEID<br>USERS_CURRENT | USERID<br>No es una relación; se usa con fines de aplicación interna<br>TASKS_CURRENT | TASKID<br>TEAMS_CURRENT | TEAMID<br>HOJAS DE HORAS_CURRENT | TIMESHEETID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Línea base</td>
        <td>Línea base</td>
        <td>BLIN | Línea base</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td></td>
        <td>BASELINEID (self)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Tarea de línea base</td>
        <td>Tarea de línea base</td>
        <td>BSTSK | Tarea prevista</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td></td>
        <td>BASELINEID<br>BASELINETASKID (self) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>No es una relación; se usa con fines de aplicación interna<br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>Tarifa de facturación</td>
        <td>Tasa o Tasa de anulación</td>
        <td>TARIFA | Tarifa de facturación</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td></td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID (self)<br>ROLEID <br>SOURCERATECARDID <br>SYSID <br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | Actualmente no se admite la tabla de clasificador ASSIGNMENTID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Actualmente no se admite la tabla de categorías de recursos no laborales<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>Identificador del objeto identificado en el campo OBJCODE<br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>ROLES_CURRENT | ROLEID <br>RATECARD_CURRENT | RATECARDID <br>No es una relación; se usa con fines de aplicación interna <br>TEMPLATES_CURNT | TEMPLATEID<br>USERS_CURRENT | USERID<br></td>
    </tr>
    <tr>
        <td>Registro de facturación</td>
        <td>Registro de facturación</td>
        <td>FACTURA | Registro de facturación</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td></td>
        <td>BILLINGRECORDID (self)<br>CATEGORYID<br>EXCHANGERATEID <br>INVOICEID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Actualmente no se admite la tabla de facturas <br>USERS_CURRENT | USERID <br>PROYECTOS_ACTUALES | PROJECTID   <br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Reservas</td>
        <td>Reservas</td>
        <td>RESERVA | Reserva</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>EVENTO_BOOKINGS</td>
        <td></td>
        <td>BOOKINGID (self)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Actualmente no se admite la tabla de categorías de recursos no laborales<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>Identificador del objeto identificado en el campo OBJOBJCODE<br>PROJECTS_CURRENT | PROJECTID <br>No es una relación; se usa con fines de aplicación interna<br>TASKS_CURRENT | TASKID     <br>PLANTILLAS_ACTUALES | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Identificador del objeto identificado en el campo TOPOBJCODE</td>
    </tr>
    <tr>
        <td>Categoría</td>
        <td>Formulario personalizado</td>
        <td>CTGY | Categoría</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td></td>
        <td>CATEGORYID (SÍ MISMO)<br>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Parámetro de categoría</td>
        <td>Campos de formulario personalizados</td>
        <td>CTGYPA | Parámetro de categoría</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td></td>
        <td>CATEGORIESPARAMETERID (self)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID    <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | No se admite actualmente la tabla de grupo de parámetros CATEGORYID<br>PARAMETERS_CURRENT | PARAMETERID    <br>No es una relación; se usa con fines de aplicación interna<br></td>
    </tr>
    <tr>
        <td>Compañía</td>
        <td>Compañía</td>
        <td>CMPY | Compañía</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>COMPANYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Trimestre personalizado</td>
        <td>Trimestre personalizado</td>
        <td>CSTQRT | Trimestre personalizado</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td></td>
        <td>CUSTOMQUARTERID (self) <br>SYSID</td>
        <td>Self<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>Condición, prioridad, gravedad, estado</td>
        <td>CSTEM | Enumeración personalizada</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
        <td>El tipo de registro se identifica mediante la propiedad enumClass. Los siguientes son los tipos esperados:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>Documento</td>
        <td>Documento</td>
        <td>DOCU | Documento</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASERSIONID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID<br>USERID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Self<br>No se admite la tabla de solicitud de documentos actualmente<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>Variable según el valor DOCOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Actualmente no se admite la tabla Versión de lanzamiento<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Variable en función del valor TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Aprobación de documento</td>
        <td>Aprobación de documento</td>
        <td>DOCAPL | Aprobación de documento</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td></td>
        <td>APPROVERID<br>DOCAPPROVALID (self)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | USERID <br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID <br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Carpeta de documentos</td>
        <td>Carpeta de documentos</td>
        <td>DOCFLD | DocsFolders</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td></td>
        <td>DOCFOLDERID (self)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br>PROGRAMID    <br>ID DE PROYECTO<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CURRENT | PORTFOLIOID <br>PROGRAM_CURRENT | PROGRAMID    <br>PROYECTOS_ACTUALES | PROJECTID <br>No es una relación; se usa con fines de aplicación interna<br>TASKS_CURRENT | TASKID     <br>PLANTILLAS_ACTUALES | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>DocumentProviderMetadata</td>
        <td>Metadatos del documento proporcionado</td>
        <td>DOCUMENTO | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td></td>
        <td>DOCPROVIDERMETAID (self) <br>SYSID</td>
        <td>Self<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>Proveedor de documento</td>
        <td>DOCPRO | Proveedor de documentos</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td></td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID (self)<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | USERID    <br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>Configuración del proveedor de documentos</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td></td>
        <td>DOCPROVIDERCONFIGID (self)<br>SYSID</td>
        <td>Self<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>Versión de documento</td>
        <td>DOCV | Versión del documento</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td></td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURRENT | USERID<br>ID externo<br>Actualmente no se admite la tabla de estado de aprobación de pruebas<br>USER_CURRENT | USERID<br>Actualmente no se admite la tabla de revisión<br>USER_CURRENT | Actualmente no se admite la tabla USERID<br>Proof Stage</td>
    </tr>
    <tr>
        <td>tarifa de cambio</td>
        <td>tarifa de cambio</td>
        <td>EXTRAER | Tipo de cambio</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td></td>
        <td>EXCHANGERATEID (self)<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>Self<br>PROYECTOS_CURRENT | PROJECTID <br>No es una relación; se usa con fines de aplicación interna <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>Gasto</td>
        <td>Gasto</td>
        <td>EXPNS | Gasto</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td></td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID (self) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Self <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | USERID <br>Identificador del objeto identificado en el campo OBJCODE <br>PROJECTS_CURRENT | PROJECTID <br>No es una relación; se usa con fines de aplicación interna<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Identificador del objeto identificado en el campo TOPOBJCODE</td>
    </tr>
    <tr>
        <td>Tipo de gasto</td>
        <td>Tipo de gasto</td>
        <td>EXPTYPE | Tipo de gasto</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>OBJID <br>SYSID  </td>
        <td>No es una relación; se usa para aplicaciones internas<br>Self<br>El identificador del objeto identificado en el campo OBJCODE <br>No es una relación; se usa para aplicaciones internas  </td>
    </tr>
    <tr>
        <td>Grupo</td>
        <td>Grupo</td>
        <td>AGRUPAR | Grupo</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td></td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | No se admitirá la tabla USERID<br>Self<br>Layout Template<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Hora</td>
        <td>Hora</td>
        <td>HOUR | Hora</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td></td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br> TASKID<br>TIMESHEETID</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | La tabla de clasificador CATEGORYID<br>no se admite actualmente<br>No es una relación; se usa para propósitos de aplicaciones internas<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>No es una relación de Workfront; se usa para la integración con sistemas externos<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>No es una relación; se usa con fines de aplicación interna<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TIMESHEET_CURRENT | TIMESHEETID</td>
    </tr>
    <tr>
        <td>Tipo de hora</td>
        <td>Tipo de hora</td>
        <td>HORA | Tipo de hora</td>
        <td>HOURTYPES_CURRENT</td>
        <td></td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>No es una relación; se usa con fines de aplicación interna<br>Self<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Iteración</td>
        <td>Iteración</td>
        <td>ITRN | Iteración</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (self)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID <br>Self<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>No es una relación; se usa con fines de aplicación interna<br>TEAMS_CURRENT | IDENTIFICADOR DE EQUIPO</td>
    </tr>
    <tr>
        <td>Entrada de cuaderno</td>
        <td>Entrada de cuaderno</td>
        <td>JARNLE | Entrada de diario</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td></td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIATIVEID<br>JOURNALENTRIEID (self)<br>OBJID<br>OPTASKID{11 4}PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>SUBOBJID<br>SUBSCRIBEID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TIMESHEETID<br>TOPOBJID<br>USERID<br></td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>Actualmente no se admite la tabla de registros de auditoría<br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTS_CURRENT | No se admite la tabla de uso compartido de documentos <br>DOCUMENTID actualmente <br>USERS_CURRENT | USERID<br>EXPENSES_CURRENT | EXPENSEID<br>HOURS_CURRENT | No se admite actualmente la tabla de iniciativa HOURID<br>Self<br>Id. del objeto identificado en el campo OBJCODE<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>El identificador del objeto identificado en el campo SUBOBJCODE<br>Actualmente no se admite la tabla de suscripción<br>No es una relación; se usa para aplicaciones internas<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>HOJAS DE HORAS_CURRENT | TIMESHEETID<br>Identificador del objeto identificado en el campo TOPOBJCODE<br>USERS_CURRENT | USERID<br></td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td></td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (self)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>ID externo<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>No es una relación; se usa con fines de aplicación interna  </td>
    </tr>
    <tr>
        <td>Hito</td>
        <td>Hito</td>
        <td>MILLA | Hito</td>
        <td>HITOS_ACTUALES<br>HITOS_DIARIOS_HISTORIAL<br>HITOS_EVENTO</td>
        <td></td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | MILESTONEID</td>
    </tr>
    <tr>
        <td>MilestonePath</td>
        <td>Ruta de hitos</td>
        <td>MPATH | Ruta de hitos</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>RecursoNoLaboral</td>
        <td>Recurso no laboral</td>
        <td>NLBR | Recurso no laboral</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (self)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | La tabla USERID <br>Categoría de recursos no laborales no se admite en este momento <br>No es una relación; se usa para fines de aplicaciones internas    </td>
    </tr>
    <tr>
        <td>Día no laborable</td>
        <td>Excepción de horario</td>
        <td>NO WKD | Día no laborable</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td></td>
        <td>NONWORKDAYID (self)<br>OBJID <br>SCHEDULEID <br>SYSID <br>USERID  </td>
        <td>Self<br>Identificador del objeto identificado en el campo OBJCODE <br>SCHEDULES_CURRENT | SCHEDULEID <br>No es una relación; se usa con fines de aplicación interna <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Nota</td>
        <td>Nota</td>
        <td>NOTA | Nota</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td></td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID{1 PARENTJOURNALENTRYID<br>PARENTNOTEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>PROOFACTIONID<br>PROOFID<br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>THREADID<br>TIMESHEETID<br>TOPOBJID<br>USERID<br></td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>Variable según ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | Actualmente no se admite la tabla USERID<br>Audit Record<br>COMPANIES_CURRENT | ID DE EMPRESA <br>DOCUMENT_CURRENT | DOCUMENTID<br>No es una relación de Workfront; se usa para la integración con sistemas externos<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>Variable según NOTEOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>Actualmente no se admite la tabla de endoso<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Actualmente no se admite la tabla de acción de revisión<br>Actualmente no se admite la tabla de revisión<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTE_CURRENT | NOTEID<br>TIMESHEET_CURRENT | TIMESHEETID<br>Variable según TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Integración de objetos</td>
        <td>Integración de objetos</td>
        <td>OBJETO | ObjectIntegration</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td></td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (propio)<br>OBJID <br>SYSID  </td>
        <td>El identificador del objeto identificado en el campo LINKEDOBJECTCODE <br>Self<br>El identificador del objeto identificado en el campo OBJCODE <br>No es una relación; se usa para propósitos de aplicación interna  </td>
    </tr>
    <tr>
        <td>Categoría de objetos</td>
        <td>Categorías de objetos</td>
        <td>OBJCAT | Categoría de objeto</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>El identificador del objeto identificado en el campo OBJCODE <br>No es una relación; se usa para propósitos de aplicación interna  </td>
    </tr>
    <tr>
        <td>OpTask</td>
        <td>Problema, Solicitud</td>
        <td>OPTASK | Problema</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUS DEFID<br>QUEUETOPICID<br>RESOLVEOPTASKID<br>RESOLVEPROJECTID<br>RESOLVETASKID<br>RESOLVINGOBJID<br>ROLEID<br>SOURCEOBJID<br>SOURCETASKID<br>SUBMITTEDBYID<br>TEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | Actualmente no se admite la tabla del Panel Kanban de ITERATIONID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>No se admite actualmente la tabla de definición de cola<br>Actualmente no se admite la tabla de temas de cola<br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | TASKID<br>Variable según RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>Variable según SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | IDENTIFICADOR DE EQUIPO<br></td>
    </tr>
    <tr>
        <td>Parámetro</td>
        <td>Campo personalizado</td>
        <td>PARAM | Parámetro</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td></td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>Actualmente no se admite la tabla de filtro de parámetros<br>Self<br>No es una relación; se usa con fines de aplicación interna  </td>
    </tr>
    <tr>
        <td>Opción del parámetro</td>
        <td>Opción del parámetro</td>
        <td>POPT | Opción de parámetro</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td></td>
        <td>PARAMETERID<br>PARAMETEROPTIONID (self) <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>Self <br>No es una relación; se usa con fines de aplicación interna  </td>
    </tr>
    <tr>
        <td>Sección de portal</td>
        <td>Informe</td>
        <td>PTLSEC | Informe</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID (self)<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VISID EWID</td>
        <td>No es una relación; se usa con fines de aplicación interna <br>USERS_CURRENT | USERID <br>UIFILTERS_CURRENT | FILTERID<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Identificador del objeto identificado en el campo OBJOBJCODE<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | USERID <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | La tabla de informes programados del ID de usuario <br>no se admite actualmente<br>No es una relación; se usa para fines de aplicaciones internas <br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>Pestaña Portal</td>
        <td>Panel de control</td>
        <td>PTLTAB | Tablero</td>
        <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        <td></td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID (self)<br>SYSID<br>USERID</td>
        <td>No es una relación; se usa con fines de aplicación interna <br>USERS_CURRENT | No se admitirá la tabla USERID <br>Portal Profile <br>Self<br>No es una relación; se usa para propósitos de aplicaciones internas <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Sección de la ficha de portal</td>
        <td>Sección de panel</td>
        <td>PRTBSC | Sección de ficha de portal</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td></td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABSECTIONID (self)<br>SYSID</td>
        <td>No se admite actualmente la sección de portal del calendario<br>No se admite actualmente la tabla de secciones externas<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>Identificador del objeto identificado en el campo PORTALSECTIONOBJCODE<br>PORTALTABS_CURRENT | PORTALTABID<br>Self<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>Últimos visores del informe</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td></td>
        <td>REPORTID<br>REPORTLASTVIEWERID (self)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID (self)<br>No es una relación; se usa con fines de aplicación interna<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portafolio</td>
        <td>Portafolio</td>
        <td>PUERTO | Portfolio</td>
        <td>PORTFOLIO_ACTUALES<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIO_EVENT<br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>No se admite la tabla de cuadro de mando actualmente<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>Preferencia</td>
        <td>Ver, filtrar, agrupar, definición de informe</td>
        <td>PROSET | Preferencia</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>PREFERENCEID (self) <br>SYSID  </td>
        <td>No es una relación; se usa con fines de aplicación interna<br>Self <br>No es una relación; se usa con fines de aplicación interna  </td>
    </tr>
    <tr>
        <td>Programar</td>
        <td>Programar</td>
        <td>PRGM | Programa</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>Self</td>
    </tr>
    <tr>
        <td>Proyecto</td>
        <td>Proyecto</td>
        <td>PROYECTO | Proyecto</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br>POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUEID<br>RECURSO CEPOOLID<br>SCHEDULEID<br>SPONSORID<br>SUBMITTEDBYID<br>TEAMID<br>TEMPLATEID</td>
        <td>No es una relación de Workfront; se usa para la integración con sistemas externos<br>Actualmente no se admite la tabla de cuadro de mandos<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>Actualmente no se admite la tabla de informe de valoración<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>USER_CURRENT | USERID<br>Actualmente no se admite la tabla de cuentas POP<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Self<br>No se admite actualmente la tabla de definición de cola<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>RateCard</td>
        <td>Tarjeta de tarifas</td>
        <td>CRTR |Tarjeta de tarifa</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td></td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID (self) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID    <br>Self<br>Id. del objeto identificado en el campo SECURITYOBJCODE <br>Id. del objeto identificado en el campo SOURCEOBJCODE<br>No es una relación; se usa para fines de aplicación interna  </td>
    </tr>
    <tr>
        <td>Carpeta de informe</td>
        <td>Carpeta de informe</td>
        <td>RPTFDR | Carpeta de informe</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td></td>
        <td>REPORTFOLDERID (self) <br>SYSID  </td>
        <td>El propio <br>no es una relación; se usa con fines de aplicación interna  </td>
    </tr>
    <tr>
        <td>Tiempo reservado</td>
        <td>Tiempo libre (personal)</td>
        <td>RESVT | Tiempo libre</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td></td>
        <td>RESERVEDTIMEID (propio) <br>SYSID<br>TASKID<br>USERID  </td>
        <td>Self<br>No es una relación; se usa con fines de aplicación interna<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Conjunto de recursos</td>
        <td>Conjunto de recursos</td>
        <td>RSPL | Conjunto de recursos</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Self<br>No es una relación; se usa para fines de aplicaciones internas  </td>
    </tr>
    <tr>
        <td>Nota de texto enriquecido</td>
        <td>Nota de texto enriquecido</td>
        <td>RHNOTE | Nota de texto enriquecido</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td></td>
        <td>RICHTEXTNOTEID (self) <br>SYSID  </td>
        <td>El propio <br>no es una relación; se usa con fines de aplicación interna  </td>
    </tr>
    <tr>
        <td>Valor de parámetro de texto enriquecido</td>
        <td>Valor de parámetro de texto enriquecido</td>
        <td>RCHVAL | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td></td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID (self) <br>SYSID  </td>
        <td>La tabla Valor de parámetro no se admite actualmente<br>Self <br>No es una relación; se usa con fines de aplicación interna  </td>
    </tr>
    <tr>
        <td>Riesgo</td>
        <td>Riesgo</td>
        <td>RIESGO | Riesgo</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID <br>ID DE PROYECTO <br>RISKID (SÍ)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | USERID <br>PROYECTOS_ACTUALES | PROJECTID   <br>Self<br>RISKTYPES_CURRENT | RISKTYPEID<br>No es una relación; se usa con fines de aplicación interna<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Tipo de riesgo</td>
        <td>Tipo de riesgo</td>
        <td>RSKTYPE | Tipo de riesgo</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td></td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>Self<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Función</td>
        <td>Función</td>
        <td>ROL | Rol</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | No se admitirá la tabla USERID<br>Plantilla de diseño<br>RATECARD_CURRENT | RATECARDID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Programación</td>
        <td>Programación</td>
        <td>PROGRAMAR | Programación</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>Aprobador de etapa</td>
        <td>Aprobador de etapa</td>
        <td>SPAPVR | Aprobador de fase</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td></td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID (self)<br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>ROLES_CURRENT | ROLEID<br>Self<br>No es una relación; se usa para aplicaciones internas <br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Tarea</td>
        <td>Tarea</td>
        <td>TAREA | Tarea</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID TEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENCERULEID<br>REJECTIONISSUEID<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID<br>TEAMID<br>TEMPLATETASKID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | Actualmente no se admite la tabla del Panel Kanban de ITERATIONID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | PROJECTID<br>Actualmente no se admite la tabla de reglas de periodicidad<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | USERID<br>Self<br>TEAM_CURRENT | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br></td>
    </tr>
    <tr>
        <td>Tarea predecesora</td>
        <td>Predecesora</td>
        <td>PRED | Predecesora</td>
        <td>PREDECESORAS_ACTUALES<br>PREDECESORAS_DAILY_HISTORY<br>PREDECESORAS_EVENT</td>
        <td></td>
        <td>ID (propio)<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>Self<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID <br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Equipo</td>
        <td>Equipo</td>
        <td>TEAMOB | Equipo</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>No se admitirá la tabla de plantillas de diseño<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | USERID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Miembro del equipo</td>
        <td>Otros equipos, miembro del equipo</td>
        <td>TEAMMB | Miembro del equipo</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td></td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID (self)<br>USERID</td>
        <td>No es una relación; se usa con fines de aplicación interna <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>TeamMemberRole</td>
        <td>Rol de miembro del equipo</td>
        <td>TEAMMR. | Rol de miembro del equipo</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td></td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID (self)<br>USERID</td>
        <td>ROLES_ACTUALES | ROLEID <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Plantilla</td>
        <td>Plantilla</td>
        <td>TMPL | Plantilla</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>SYNSID 14}TEAMID<br>TEMPLATEID (self)<br></td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Actualmente no se admite la tabla de definición de cola<br>SCHEDULES_CURRENT | SCHEDULEID <br>No es una relación; se usa con fines de aplicación interna <br>TEAMS_CURRENT | TEAMID<br>Self</td>
    </tr>
    <tr>
        <td>Asignación de plantilla</td>
        <td>Asignación de plantilla</td>
        <td>TASSGN | Asignación de plantilla</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td></td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (self)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>Identificador del objeto identificado en el campo OBJCODE<br>ROLES_CURRENT | ROLEID<br>No es una relación; se usa para aplicaciones internas<br>TEAMS_CURRENT | Actualmente no se admite la tabla de tiempo de equipo TEAMID<br>Self<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br></td>
    </tr>
    <tr>
        <td>Tarea de plantilla</td>
        <td>Tarea de plantilla</td>
        <td>TTSK | Tarea de plantilla</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td></td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEID<br>TASKID (self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>Actualmente no se admite la tabla de reglas de periodicidad<br>ROLES_CURRENT | ROLEID<br>No es una relación; se usa con fines de aplicación interna<br>TEAMS_CURRENT | TEAMID<br>Actualmente no se admite la tabla de tiempo disponible del equipo<br>TEMPLATES_CURRENT | TEMPLATEID<br>Self</td>
    </tr>
    <tr>
        <td>Tarea de plantilla predecesora</td>
        <td>Predecesora de plantilla</td>
        <td>TPRED | Predecesora</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td></td>
        <td>PREDECESSORID<br>SUCCESSORID <br>TEMPLATEPREDECESSORID (self)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>Self<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Hoja de horas</td>
        <td>Hoja de horas</td>
        <td>HOJA TSHET | Hoja de horas</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>EVENTO_DE_HOJAS DE HORAS</td>
        <td></td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Perfil de hoja de horas</td>
        <td>Perfil de hoja de horas</td>
        <td>TSPRO | Perfil de hoja de horas</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td></td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (self)</td>
        <td>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>No es una relación; se usa con fines de aplicación interna<br>Self</td>
    </tr>
    <tr>
        <td>Filtro de IU</td>
        <td>Filtro</td>
        <td>UIFT | Filtrar</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID (self)</td>
        <td>No es una relación; se usa con fines de aplicación interna<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Identificador del objeto identificado en el campo OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>No es una relación; se usa con fines de aplicación interna <br>Self</td>
    </tr>
    <tr>
        <td>Agrupar por IU</td>
        <td>Agrupación</td>
        <td>UIGB | Agrupación</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td></td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID (self)</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>No es una relación; se usa con fines de aplicación interna <br>Self</td>
    </tr>
    <tr>
        <td>Plantilla de IU</td>
        <td>Plantilla de diseño</td>
        <td>UITMPL | Plantilla de diseño</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID (self)</td>
        <td>No es una relación; se usa con fines de aplicación interna<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Identificador del objeto identificado en el campo OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>No es una relación; se usa con fines de aplicación interna <br>Self</td>
    </tr>
    <tr>
        <td>Vista de IU</td>
        <td>Ver</td>
        <td>UIVIEW | Ver</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td></td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID (self)</td>
        <td>No es una relación; se usa con fines de aplicación interna<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Identificador del objeto identificado en el campo OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>No es una relación; se usa con fines de aplicación interna <br>Self</td>
    </tr>
    <tr>
        <td>Usuario</td>
        <td>Usuario</td>
        <td>USUARIO | Usuario</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td></td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID <br>PORTALPROFILEID<br>PREFUID<br>PRIVATERATECARDID<br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UUMUSERID</td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | ID DE EMPRESA <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>No es una relación; se usa con fines de aplicación interna<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>No se admitirá la tabla de plantillas de diseño<br>USER_CURRENT | No se admitirá la tabla USERID<br>Perfil de portal<br>No es una relación; se usa para aplicaciones internas<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br>No es una relación; se usa con fines de aplicación interna</td>
    </tr>
    <tr>
        <td>Delegación de usuario</td>
        <td>Delegación de usuario</td>
        <td>USRDEL | Delegación de usuario</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td></td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID (self)</td>
        <td>USERS_CURRENT | USERID<br>No es una relación; se usa con fines de aplicación interna <br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>Grupo de usuarios</td>
        <td>Otros grupos</td>
        <td>USRGPS | Grupo de usuarios</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td></td>
        <td>GROUPID <br>SYSID<br>USERID <br>USERSGROUPID (self)</td>
        <td>GROUPS_CURRENT | GROUPID <br>No es una relación; se usa con fines de aplicación interna<br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>Rol de usuario</td>
        <td>Otros roles</td>
        <td>USRROL | Función de usuario</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td></td>
        <td>ROLEID <br>SYSID<br>USERID    <br>USERROLESETID<br>USERSROLEID (self)</td>
        <td>ROLES_ACTUALES | ROLEID <br>No es una relación; se usa con fines de aplicación interna<br>USERS_CURRENT | USERID    <br>USERROLESET_CURRENT | USERROLESETID<br>Self</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | Preferencia de usuario</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td></td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID (self)</td>
        <td>No es una relación; se usa con fines de aplicación interna<br>USERS_CURRENT | USERID    <br>Propio</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>URSET | UserRoleSet</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td></td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID (self)</td>
        <td>ROLES_ACTUALES | ROLEID <br>No es una relación; se usa con fines de aplicación interna<br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>UsersDecisions</td>
        <td>Decisiones de los usuarios</td>
        <td>USRDEC | Decisiones de usuarios</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td></td>
        <td>USERDECISIONID (self)<br>SYSID <br>USERID  </td>
        <td>Self<br>No es una relación; se usa con fines de aplicación interna <br>USERS_CURRENT | USERID </td>
    </tr>
    <tr>
        <td>WorkItem</td>
        <td>Elemento de trabajo</td>
        <td>WRKITM | WorkItem</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td></td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>ID DE PROYECTO <br>SYSID<br>TASKID    <br>ID DE USUARIO <br>WORKITEMID (propio)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br>Identificador del objeto identificado en el campo OBJOBJCODE<br>OPTASK_CURRENT | OPTASKID    <br>PROYECTOS_ACTUALES | PROJECTID <br>No es una relación; se usa con fines de aplicación interna<br>TASKS_CURRENT | TASKID    <br>USUARIOS_ACTUALES | USERID    <br>Automático </td>
    </tr>
  </tbody>
</table>
