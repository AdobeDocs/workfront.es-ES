---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Diccionario de datos de Workfront Data Connect
description: Esta página contiene información sobre la estructura y el contenido de los datos de Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 44342db0a473eac70212d08cedf9ac0f571cda0b
workflow-type: tm+mt
source-wordcount: '8129'
ht-degree: 7%

---

# Diccionario de datos de Workfront Data Connect

Esta página contiene información sobre la estructura y el contenido de los datos de Workfront Data Connect.

>[!NOTE]
>
>Los datos de Data Connect se actualizan cada cuatro horas, por lo que es posible que los cambios recientes no se reflejen inmediatamente.

## Tipos de tabla

Existen varios tipos de tablas que puede utilizar en Data Connect para ver los datos de Workfront de una manera que le proporcione la mayor cantidad de insight.

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

### Nivel de acceso

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Nivel de acceso</td>
            <td>Nivel de acceso</td>
            <td>ACSLVL</td>
            <td>Nivel de acceso</td>
            <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LEGACYACCESSLEVELID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Regla de acceso

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Regla de acceso</td>
            <td>Compartir</td>
            <td>ACSRUL</td>
            <td>Compartir</td>
            <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESORIO</td>
             <td>FK</td>
             <td>Variable basada en ACCESSOROBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo ACCESSOROBJCODE</td>
        </tr>
        <tr>
             <td>ACCESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ANCESTORID</td>
             <td>PK</td>
             <td>Variable basada en ANCESTOROBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo ANCESTOROBJCODE</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SECURITYOBJID</td>
             <td>FK</td>
             <td>Variable basada en SECURITYOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Ruta de aprobación

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ruta de aprobación</td>
            <td>Ruta de aprobación</td>
            <td>ARVPTH</td>
            <td>Aprobación</td>
            <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GLOBALPATHID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Proceso de aprobación

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Proceso de aprobación</td>
            <td>Proceso de aprobación</td>
            <td>ARVPRC</td>
            <td>Proceso de aprobación</td>
            <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Paso de aprobación

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Paso de aprobación</td>
            <td>Paso de aprobación</td>
            <td>ARVSTP</td>
            <td>Fase de aprobación</td>
            <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>FK</td>
             <td>APPROVALPATHS_CURRENT</td>
             <td>APPROVALPATHID</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Estado de la aprobación

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Estado de la aprobación</td>
            <td>Estado de la aprobación</td>
            <td>ARVESTI</td>
            <td>ApproverStatus</td>
            <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVABLEOBJID</td>
             <td>FK</td>
             <td>Variable basada en APPROVABLEOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo APPROVABLEOBJCODE</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DELEGATEUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OVERRIDDENUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSYID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>WILDCARDUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Asignación

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Asignación</td>
            <td>Asignación</td>
            <td>ASSGN</td>
            <td>Asignación</td>
            <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
    </tbody>
</table>

### Esperando aprobaciones

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Esperando aprobaciones</td>
            <td>Esperando aprobaciones</td>
            <td>AWAPVL</td>
            <td>Esperando aprobaciones</td>
            <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSREQUESTID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de solicitud de acceso</td>
        </tr>
        <tr>
             <td>APPROVABLEID</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>APROBADOR</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ESPERANDO APROBACIÓN</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>FK</td>
             <td>DOCUMENTVERSIONS_CURRENT</td>
             <td>DOCUMENTVERSIONID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Línea base

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Línea base</td>
            <td>Línea base</td>
            <td>BLIN</td>
            <td>Línea base</td>
            <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Tarea de línea base

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tarea de línea base</td>
            <td>Tarea de línea base</td>
            <td>BSTSK</td>
            <td>Tarea de línea base</td>
            <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BASELINETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
    </tbody>
</table>

### Tarifa de facturación

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tarifa de facturación</td>
            <td>Tasa o Tasa de anulación</td>
            <td>TARIFA</td>
            <td>Tarifa de facturación</td>
            <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURNT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Registro de facturación

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Registro de facturación</td>
            <td>Registro de facturación</td>
            <td>FACTURA</td>
            <td>Registro de facturación</td>
            <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>INVOICEID</td>
             <td>-</td>
             <td colspan="2">Tabla de factura no admitida actualmente</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Reserva

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Reserva</td>
            <td>Reserva</td>
            <td>RESERVA</td>
            <td>Reserva</td>
            <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>EVENTO_BOOKINGS</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BOOKINGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable basada en TOPOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo TOPOBJCODE</td>
        </tr>
    </tbody>
</table>

### Perfiles de empresa

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Perfiles de empresa</td>
            <td>Perfiles de empresa</td>
            <td>BSNPRF</td>
            <td>BusinessProfile</td>
            <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>BUSINESSPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Regla empresarial

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Regla empresarial</td>
            <td>Regla empresarial</td>
            <td>BSNRUL</td>
            <td>Regla empresarial</td>
            <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Categoría

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Categoría</td>
            <td>Formulario personalizado</td>
            <td>CTGY</td>
            <td>Categoría</td>
            <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Parámetro de categoría

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parámetro de categoría</td>
            <td>Campos de formulario personalizados</td>
            <td>CTGYPA</td>
            <td>Parámetro de categoría</td>
            <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIESPARAMETERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>FK</td>
             <td>PARAMETERGROUPS_CURRENT</td>
             <td>PARAMETERGROUPID</td>
        </tr>
        <tr>
             <td>PARAMETERID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Clasificador

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Clasificador</td>
            <td>Ubicación</td>
            <td>CLSF</td>
            <td>Ubicación</td>
            <td>CLASSIFIER_CURRENT<br>CLASSIFIER_DAILY_HISTORY<br>CLASSIFIER_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Compañía

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Compañía</td>
            <td>Compañía</td>
            <td>CMPY</td>
            <td>Compañía</td>
            <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Trimestre personalizado

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Trimestre personalizado</td>
            <td>Trimestre personalizado</td>
            <td>CSTQRT</td>
            <td>Trimestre personalizado</td>
            <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMQUARTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Enumeración personalizada

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>CustomEnum</td>
            <td>Condición, prioridad, gravedad, estado</td>
            <td>CSTEM</td>
            <td>Enumeración personalizada</td>
            <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMENUMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>
<div>* El tipo de registro se identifica mediante la propiedad enumClass. Los siguientes son los tipos esperados: <br>
<ul><li>CONDITION_OPTASK</li>
<li>CONDITION_PROJ</li>
<li>CONDITION_TASK</li>
<li>PRIORITY_OPTASK</li>
<li>PRIORITY_PROJ</li>
<li>PRIORITY_TASK</li>
<li>SEVERITY_OPTASK</li>
<li>STATUS_OPTASK</li>
<li>STATUS_PROJ</li>
<li>STATUS_TASK</li></ul></div>

### Documento

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Documento</td>
            <td>Documento</td>
            <td>DOCU</td>
            <td>Documento</td>
            <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CHECKEDOUTBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTREQUESTID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de solicitud de documento</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTAFOLIOIDE</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTAFOLIOIDE</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RELEASEVERSIONID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla Versión de lanzamiento</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable basada en TOPOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo TOPOBJCODE</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Aprobación de documento

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Aprobación de documento</td>
            <td>Aprobación de documento</td>
            <td>DOCAPL</td>
            <td>Aprobación de documento</td>
            <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APROBADOR</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCAPPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>REQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Aprobación de documento (NUEVO)

Disponibilidad limitada del cliente

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Aprobación de documento</td>
            <td>Aprobación</td>
            <td>N/D</td>
            <td>N/D</td>
            <td>APPROVAL_CURRENT<br>APPROVAL_DAILY_HISTORY<br>APPROVAL_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APROBADO</td>
             <td>PK</td>
             <td>-</td>
             <td>NOTA: También es el ID del objeto DOCUMENTVERSION al que está asociada la aprobación.</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variable basada en ASSETTYPE</td>
             <td>La clave principal/ID del objeto identificado en el campo ASSETTYPE</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">EAUTHTENANTID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td class="key">PRODUCTID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td class="key">REALCREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Fase de aprobación del documento (NUEVA)

Disponibilidad limitada del cliente

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Fase de aprobación del documento</td>
            <td>Fase de aprobación</td>
            <td>N/D</td>
            <td>N/D</td>
            <td>APPROVAL_STAGE_CURRENT<br>APPROVAL_STAGE_DAILY_HISTORY<br>APPROVAL_STAGE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APROBADO</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>APROBADO</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
    </tbody>
</table>

### Participantes en la fase de aprobación de documentos (NUEVO)

Disponibilidad limitada del cliente

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Participante de la fase de aprobación del documento</td>
            <td>Decisiones de aprobación</td>
            <td>N/D</td>
            <td>N/D</td>
            <td>APPROVAL_STAGE_PARTICIPANT_CURRENT<br>APPROVAL_STAGE_PARTICIPANT_DAILY_HISTORY<br>APPROVAL_STAGE_PARTICIPANT_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APROBADO</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>APROBADO</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEPARTICIPANTID/td&gt;
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variable basada en ASSETTYPE</td>
             <td>La clave principal/ID del objeto identificado en el campo ASSETTYPE</td>
        </tr>
        <tr>
             <td class="key">DECISIONUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td class="key">PARTICIPANTID</td>
             <td>FK</td>
             <td class="relatedtable">Variable basada en PARTICIPANTTYPE</td>
             <td>La clave principal/ID del objeto identificado en el campo PARTICIPANTTYPE</td>
        </tr>
        <tr>
             <td class="key">REALREQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">REALUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">REQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">STAGEID</td>
             <td>FK</td>
             <td>APPROVAL_STAGE_CURRENT</td>
             <td>STAGEID</td>
        </tr>
    </tbody>
</table>

### Carpeta de documentos

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Carpeta de documentos</td>
            <td>Carpeta de documentos</td>
            <td>DOCFLD</td>
            <td>DocsFolders</td>
            <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>FK</td>
             <td>LINKEDFOLDERS_CURRENT</td>
             <td>LINKEDFOLDERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>DOCFOLDERID</td>
        </tr>
        <tr>
             <td>PORTAFOLIOIDE</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTAFOLIOIDE</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Metadatos del proveedor de documentos

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Metadatos del proveedor de documentos</td>
            <td>Metadatos del proveedor de documentos</td>
            <td>DOCUMENTO</td>
            <td>DocumentProviderMetadata</td>
            <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERMETAID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Proveedor de documento

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Proveedor de documento</td>
            <td>Proveedor de documento</td>
            <td>DOCPRO</td>
            <td>Proveedor de documento</td>
            <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>FK</td>
             <td>DOCPROVIDERCONFIG_CURRENT</td>
             <td>DOCPROVIDERCONFIGID</td>
        </tr>
        <tr>
             <td>DOCPROVIDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Configuración del proveedor de documentos

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Configuración del proveedor de documentos</td>
            <td>Configuración del proveedor de documentos</td>
            <td>DOCCFG</td>
            <td>DocumentProviderConfig</td>
            <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Versión de documento

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Versión de documento</td>
            <td>Versión de documento</td>
            <td>DOCV</td>
            <td>Versión de documento</td>
            <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">El ID externo en el sistema de almacenamiento externo</td>
        </tr>
        <tr>
             <td>PROOFAPPROVALSTATUSID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de estado de aprobación de pruebas</td>
        </tr>
        <tr>
             <td>PROOFEDBYUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de revisión</td>
        </tr>
        <tr>
             <td>PROOFOWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFSTAGEID</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de fase de revisión</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### tarifa de cambio

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>tarifa de cambio</td>
            <td>tarifa de cambio</td>
            <td>EXTRAER</td>
            <td>tarifa de cambio</td>
            <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Gasto

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gasto</td>
            <td>Gasto</td>
            <td>EXPNS</td>
            <td>Gasto</td>
            <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXPENSEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>FK</td>
             <td>EXPENSETYPES_CURRENT</td>
             <td>EXPENSETYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable basada en TOPBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo TOPBJCODE</td>
        </tr>
    </tbody>
</table>

### Tipo de gasto

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tipo de gasto</td>
            <td>Tipo de gasto</td>
            <td>EXPTYPE</td>
            <td>Tipo de gasto</td>
            <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Grupo

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Grupo</td>
            <td>Grupo</td>
            <td>GRUPO</td>
            <td>Grupo</td>
            <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSLEADERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ROOTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Hora

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Hora</td>
            <td>Hora</td>
            <td>HOUR</td>
            <td>Hora</td>
            <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>TONTO</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXTERNALTIMESHEETID</td>
             <td>-</td>
             <td colspan="2">No es una relación de Workfront; se utiliza para la integración con sistemas externos
Self</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTOVERHEADID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
    </tbody>
</table>

### Tipo de hora

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tipo de hora</td>
            <td>Tipo de hora</td>
            <td>HORA</td>
            <td>Tipo de hora</td>
            <td>HOURTYPES_CURRENT<br>HOURTYPES_DAILY_HISTORY<br>HOURTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Iteración

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Iteración</td>
            <td>Iteración</td>
            <td>ITRN</td>
            <td>Iteración</td>
            <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
    </tbody>
</table>

### Entrada de cuaderno

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Entrada de cuaderno</td>
            <td>Entrada de cuaderno</td>
            <td>JARNLE</td>
            <td>Entrada de cuaderno</td>
            <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>FK</td>
             <td>APPROVERSTATUSES_CURRENT</td>
             <td>APPROVERSTATUSID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">Tabla de registro de auditoría no admitida actualmente</td>
        </tr>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTSHAREID</td>
             <td>-</td>
             <td colspan="2">Tabla de uso compartido de documentos no compatible actualmente</td>
        </tr>
        <tr>
             <td>EDITEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXPENSEID</td>
             <td>FK</td>
             <td>EXPENSES_CURRENT</td>
             <td>EXPENSEID</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>FK</td>
             <td>HOURS_CURRENT</td>
             <td>HOURID</td>
        </tr>
        <tr>
             <td>INITIATIVEID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de iniciativa</td>
        </tr>
        <tr>
             <td>JOURNALENTRIESID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTAFOLIOIDE</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTAFOLIOIDE</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SUBOBJID</td>
             <td>FK</td>
             <td>Variable basada en SUBOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo SUBOBJCODE</td>
        </tr>
        <tr>
             <td>SUBSCRIBEID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable basada en TOPOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo TOPOBJCODE</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Carpeta vinculada

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Carpeta vinculada</td>
            <td>Carpeta vinculada</td>
            <td>LNKFDR</td>
            <td>LinkedFolder</td>
            <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">El ID externo en el sistema de almacenamiento externo</td>
        </tr>
        <tr>
             <td>FOLDERID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>FOLDERID</td>
        </tr>
        <tr>
             <td>LINKEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Hito

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Hito</td>
            <td>Hito</td>
            <td>MILLA</td>
            <td>Hito</td>
            <td>HITOS_ACTUALES<br>HITOS_DIARIOS_HISTORIAL<br>HITOS_EVENTO</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Ruta de hitos

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ruta de hitos</td>
            <td>Ruta de hitos</td>
            <td>MPATH</td>
            <td>Ruta de hitos</td>
            <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Recurso no laboral

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Recurso no laboral</td>
            <td>Recurso no laboral</td>
            <td>NLBR</td>
            <td>Recurso no laboral</td>
            <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCECATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Categoría de recurso no laboral

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Categoría de recurso no laboral</td>
            <td>Categoría de recurso no laboral</td>
            <td>NLBRCY</td>
            <td>Categoría de recurso no laboral</td>
            <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Día no laborable

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Día no laborable</td>
            <td>Excepción de horario</td>
            <td>NO WKD</td>
            <td>Día no laborable</td>
            <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>NONWORKDAYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Nota

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Nota</td>
            <td>Nota</td>
            <td>NOTA</td>
            <td>Nota</td>
            <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHDOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>ATTACHOBJID</td>
             <td>FK</td>
             <td>Variable basada en ATTACHOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en OBJCODE ATTACHOBJCODE</td>
        </tr>
        <tr>
             <td>ATTACHOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ATTACHWORKID</td>
             <td>FK</td>
             <td>WORKITEMS_CURRENT</td>
             <td>WORKITEMID</td>
        </tr>
        <tr>
             <td>ATTACHWORKUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">Tabla de registro de auditoría no admitida actualmente</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>EXTERNALSERVICEID</td>
             <td>-</td>
             <td colspan="2">No es una relación de Workfront; se utiliza para la integración con sistemas externos</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en NOTEOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo NOTEOBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTENDORSEMENTID</td>
             <td>-</td>
             <td colspan="2">Tabla de aprobación no admitida actualmente</td>
        </tr>
        <tr>
             <td>PARENTJOURNALENTRYID</td>
             <td>FK</td>
             <td>JOURNALENTRIES_CURRENT</td>
             <td>JOURNALENTRYID</td>
        </tr>
        <tr>
             <td>PARENTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>PORTAFOLIOIDE</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTAFOLIOIDE</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROOFACTIONID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de acciones de revisión</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de revisión</td>
        </tr>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>FK</td>
             <td>RESERVEDTEXTNOTES_CURRENT</td>
             <td>RICHTEXTNOTEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>THREADID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable basada en TOPOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo TOPOBJCODE</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>


    &lt;/tbody>
</table>

### Integración de objetos

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Integración de objetos</td>
            <td>Integración de objetos</td>
            <td>OBJETO</td>
            <td>ObjectIntegration</td>
            <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LINKEDOBJECTID</td>
             <td>FK</td>
             <td>Variable basada en LINKEDOBJECTCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo LINKEDOBJECTCODE</td>
        </tr>
        <tr>
             <td>OBJECTINTEGRATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>

    &lt;/tbody>
</table>

### Categoría de objetos

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Categoría de objetos</td>
            <td>Categorías de objetos</td>
            <td>OBJCAT</td>
            <td>Categoría de objeto</td>
            <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>OBJECTSCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Tarea operativa/problema

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>OpTask</td>
            <td>Problema, Solicitud</td>
            <td>OPTASK</td>
            <td>Problema</td>
            <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">Tabla de Panel Kanban no admitida actualmente</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">Tabla de definición de cola no admitida actualmente</td>
        </tr>
        <tr>
             <td>QUEUETOPICID</td>
             <td>-</td>
             <td colspan="2">Tabla de temas de colas no admitida actualmente</td>
        </tr>
        <tr>
             <td>RESOLVEOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOLVEPROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOLVETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>RESOLVINGOBJID</td>
             <td>FK</td>
             <td>Variable basada en RESOLVINGOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo RESOLVINGOBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCEOBJID</td>
             <td>FK</td>
             <td>Variable basada en SOURCEOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo SOURCEOBJCODE</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
    </tbody>
</table>

### Parámetro

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parámetro</td>
            <td>Campo personalizado</td>
            <td>PARAM</td>
            <td>Parámetro</td>
            <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERFILTERID</td>
             <td>-</td>
             <td colspan="2">Tabla de filtro de parámetros no compatible actualmente</td>
        </tr>
        <tr>
             <td>PARAMETERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Grupo de parámetros

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Grupo de parámetros</td>
            <td>Sección del formulario</td>
            <td>PARAM</td>
            <td>Grupo de parámetros</td>
            <td>PARAMETERGROUPS_CURRENT<br>PARAMETERGROUPS_DAILY_HISTORY<br>PARAMETERGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Opción del parámetro

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Opción del parámetro</td>
            <td>Opción del parámetro</td>
            <td>POPT</td>
            <td>Opción del parámetro</td>
            <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERID</td>
        </tr>
        <tr>
             <td>PARAMETEROPTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Sección del portal/Informe

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Sección de portal</td>
            <td>Informe</td>
            <td>PTLSEC</td>
            <td>Informe</td>
            <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>FILTERID</td>
             <td>FK</td>
             <td>UIFILTERS_CURRENT</td>
             <td>FILTERID</td>
        </tr>
        <tr>
             <td>GROUPBYID</td>
             <td>FK</td>
             <td>UIGROUPBYS_CURRENT</td>
             <td>GROUPBYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTVIEWEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>PORTALSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCIAS_ACTUALES</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>PUBLICRUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>FK</td>
             <td>REPORTFOLDERS_CURRENT</td>
             <td>REPORTFOLDERID</td>
        </tr>
        <tr>
             <td>RUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SCHEDULEDREPORTID</td>
             <td>-</td>
             <td colspan="2">La tabla de informes programados no se admite actualmente</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>VIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>VIEWID</td>
        </tr>
    </tbody>
</table>

### Pestaña Portal/Tablero

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Pestaña Portal</td>
            <td>Panel de control</td>
            <td>PTLTAB</td>
            <td>Panel de control</td>
            <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Sección de la ficha de portal

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Sección de la ficha de portal</td>
            <td>Sección de panel</td>
            <td>PRTBSC</td>
            <td>Sección de la ficha de portal</td>
            <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CALENDARPORTALSECTIONID</td>
             <td>-</td>
             <td colspan="2">Sección de portal de calendario no admitida actualmente</td>
        </tr>
        <tr>
             <td>EXTERNALSECTIONID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de secciones externas</td>
        </tr>
        <tr>
             <td>INTERNALSECTIONID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>PORTALSECTIONOBJID</td>
             <td>FK</td>
             <td>Variable basada en PORTALSECTIONOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo PORTALSECTIONOBJCODE</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>FK</td>
             <td>PORTALTABS_CURRENT</td>
             <td>PORTALTABID</td>
        </tr>
        <tr>
             <td>PORTALTABSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Último visor de sección del portal

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>PortalSectionLastViewer</td>
            <td>Últimos visores del informe</td>
            <td>PLSLSV</td>
            <td>PortalSectionLastViewer</td>
            <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>REPORTID</td>
        </tr>
        <tr>
             <td>REPORTLASTVIEWERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>VIEWERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Portafolio

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Portafolio</td>
            <td>Portafolio</td>
            <td>PORT</td>
            <td>Portafolio</td>
            <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">Tabla de informe de valoración no compatible actualmente</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTAFOLIOIDE</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Preferencia

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Preferencia</td>
            <td>Ver, filtrar, agrupar, definición de informe</td>
            <td>PROSET</td>
            <td>Preferencia</td>
            <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Programa

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Programa</td>
            <td>Programa</td>
            <td>PRGM</td>
            <td>Programa</td>
            <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTAFOLIOIDE</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTAFOLIOIDE</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Proyecto

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Proyecto</td>
            <td>Proyecto</td>
            <td>PROJ</td>
            <td>Proyecto</td>
            <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>AEMNATIVEFOLDERTREESREFID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">Tabla de informe de valoración no compatible actualmente</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">Tabla de informe de valoración no compatible actualmente</td>
        </tr>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>POPACCOUNTID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de cuentas POP</td>
        </tr>
        <tr>
             <td>PORTAFOLIOIDE</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTAFOLIOIDE</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">Tabla de definición de cola no admitida actualmente</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>PATROCINADOR</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Usuario de equipo del proyecto

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Usuario de equipo del proyecto</td>
            <td>Usuario de equipo del proyecto</td>
            <td>PUERTO</td>
            <td>Usuario de proyecto</td>
            <td>PROYECTOSUSUARIOS_ACTUALES<br>PROYECTOSUSUARIOS_DIARIOS_HISTORIAL<br>PROYECTOSUSUARIOS_EVENTO</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TMPUSERID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Rol de usuario del equipo del proyecto

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rol de usuario del equipo del proyecto</td>
            <td>Rol de usuario del equipo del proyecto</td>
            <td>PTEAM</td>
            <td>ProjectUserRole</td>
            <td>PROYECTOSUSUARIOSROLES_CURRENT<br>PROYECTOSUSUARIOSROLES_DAILY_HISTORY<br>PROYECTOSUSUARIOSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERSROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tarjeta de tarifas

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tarjeta de tarifas</td>
            <td>Tarjeta de tarifas</td>
            <td>CRTR</td>
            <td>Tarjeta de tarifas</td>
            <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SECURITYROOTID</td>
             <td>FK</td>
             <td>Variable basada en SECURITYOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SOURCEID</td>
             <td>FK</td>
             <td>Variable basada en SOURCEOBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo SOURCEOBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>

    &lt;/tbody>
</table>

### Carpeta de informe

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Carpeta de informe</td>
            <td>Carpeta de informe</td>
            <td>RPTFDR</td>
            <td>Carpeta de informe</td>
            <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Recuento de estadísticas de vista de informe

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Recuento de estadísticas de vista de informe</td>
            <td>Recuento de estadísticas de vista de informe</td>
            <td>PLSVST</td>
            <td>PortalSectionStatisticsInfo</td>
            <td>REPORTVIEWSTATISTICCOUNTS_CURRENT<br>REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>REPORTVIEWSTATISTICCOUNTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Horas presupuestadas reportables

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Horas presupuestadas reportables</td>
            <td>Horas presupuestadas reportables</td>
            <td>RPBGHR</td>
            <td>Hora presupuestadas</td>
            <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REPORTABLEBUDGETEDHOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tiempo reservado/PTO

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tiempo reservado</td>
            <td>Tiempo libre (personal)</td>
            <td>RESVT</td>
            <td>Días libres</td>
            <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Gerente de recursos

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gerente de recursos</td>
            <td>Gerente de recursos</td>
            <td>RESMGR</td>
            <td>Gerente de recursos</td>
            <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>Identificador</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOURCEMANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Conjunto de recursos

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Conjunto de recursos</td>
            <td>Conjunto de recursos</td>
            <td>RSPL</td>
            <td>Conjunto de recursos</td>
            <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Nota de texto enriquecido

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Nota de texto enriquecido</td>
            <td>Nota de texto enriquecido</td>
            <td>RHNOTE</td>
            <td>Nota de texto enriquecido</td>
            <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Valor de parámetro de texto enriquecido

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Valor de parámetro de texto enriquecido</td>
            <td>Valor de parámetro de texto enriquecido</td>
            <td>RCHVAL</td>
            <td>RichTextParameterValue</td>
            <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERVALUEID</td>
             <td>-</td>
             <td colspan="2">Actualmente no se admite la tabla de valores de parámetros</td>
        </tr>
        <tr>
             <td>RICHTEXTPARAMETERVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Riesgo

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Riesgo</td>
            <td>Riesgo</td>
            <td>RIESGO</td>
            <td>Riesgo</td>
            <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ARRIESGADO</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>RISKTYPEID</td>
             <td>FK</td>
             <td>RISKTYPES_CURRENT</td>
             <td>RISKTYPEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Tipo de riesgo

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tipo de riesgo</td>
            <td>Tipo de riesgo</td>
            <td>RSKTYPE</td>
            <td>Tipo de riesgo</td>
            <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RISKTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Función

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Función</td>
            <td>Función</td>
            <td>ROL</td>
            <td>Función</td>
            <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">No se admitirá la tabla de plantillas de diseño</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Programación

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Programación</td>
            <td>Programación</td>
            <td>PROGRAMAR</td>
            <td>Programación</td>
            <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Aprobador de paso

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Aprobador de paso</td>
            <td>Aprobador de paso</td>
            <td>SPAPVR</td>
            <td>Aprobador de fase</td>
            <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tarea

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tarea</td>
            <td>Tarea</td>
            <td>TASK</td>
            <td>Tarea</td>
            <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">Tabla de Panel Kanban no admitida actualmente</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">Tabla de reglas de periodicidad no admitida actualmente</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>FK</td>
             <td>RESERVEDTIMES_CURRENT</td>
             <td>RESERVEDTIMEID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>SUBMITTEDBYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### Tarea predecesora

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tarea predecesora</td>
            <td>Predecesora</td>
            <td>PRED</td>
            <td>Predecesora</td>
            <td>PREDECESORAS_ACTUALES<br>PREDECESORAS_DAILY_HISTORY<br>PREDECESORAS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>Identificador</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREDECESORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Equipo

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Equipo</td>
            <td>Equipo</td>
            <td>TEAMOB</td>
            <td>Equipo</td>
            <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">No se admitirá la tabla de plantillas de diseño</td>
        </tr>
        <tr>
             <td>MYWORKVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REQUESTSVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Miembro del equipo

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Miembro del equipo</td>
            <td>Otros equipos, miembro del equipo</td>
            <td>TEAMMB</td>
            <td>Miembro del equipo</td>
            <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>TEAMMEMBERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Rol de miembro del equipo

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rol de miembro del equipo</td>
            <td>Rol de miembro del equipo</td>
            <td>TEAMMR.</td>
            <td>Rol de miembro del equipo</td>
            <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>TEAMMEMBERROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Plantilla

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Plantilla</td>
            <td>Plantilla, Plantilla de proyecto</td>
            <td>TMPL</td>
            <td>Plantilla</td>
            <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">Tabla de informe de valoración de entrega no compatible actualmente</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">Tabla de definición de cola no admitida actualmente</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Asignación de tarea de plantilla

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Asignación de tarea de plantilla</td>
            <td>Asignación de plantilla</td>
            <td>TASSGN</td>
            <td>Asignación de plantilla</td>
            <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">En este momento no se admite la tabla cronometrable de equipo</td>
        </tr>
        <tr>
             <td>TEMPLATEASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### Tarea de plantilla

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tarea de plantilla</td>
            <td>Tarea de plantilla</td>
            <td>TTSK</td>
            <td>Tarea de plantilla</td>
            <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">Tabla de reglas de periodicidad no admitida actualmente</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>IDENTIFICADOR DE EQUIPO</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">En este momento no se admite la tabla cronometrable de equipo</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Tarea de plantilla predecesora

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tarea de plantilla predecesora</td>
            <td>Predecesora de plantilla</td>
            <td>TPRED</td>
            <td>Predecesora</td>
            <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PREDECESORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEPREDECESSORID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Moneda de KPI de fase temporal

Disponibilidad limitada del cliente

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Moneda de KPI de fase temporal</td>
            <td>KPI de fase temporal</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_CURRENCY_CURRENT<br>TIMEPHASED_CURRENCY_DAILY_HISTORY<br>TIMEPHASED_CURRENCY_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTAFOLIOIDE</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTAFOLIOIDE</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Se añadirá en breve</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDCURRENCYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Duración de KPI de fase temporal

Disponibilidad limitada del cliente

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Duración de KPI de fase temporal</td>
            <td>KPI de fase temporal</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_DURATION_CURRENT<br>TIMEPHASED_DURATION_DAILY_HISTORY<br>TIMEPHASED_DURATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTAFOLIOIDE</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTAFOLIOIDE</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Se añadirá en breve</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDDURATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Plantilla de horas

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Plantilla de horas</td>
            <td>Plantilla de horas</td>
            <td>TSHET</td>
            <td>Plantilla de horas</td>
            <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>EVENTO_DE_HOJAS DE HORAS</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APROBADOR</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Perfil de hoja de horas

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Perfil de hoja de horas</td>
            <td>Perfil de hoja de horas</td>
            <td>TSPRO</td>
            <td>Perfil de hoja de horas</td>
            <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APROBADOR</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Filtro de IU

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Filtro de IU</td>
            <td>Filtro</td>
            <td>UIFT</td>
            <td>Filtro</td>
            <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCIAS_ACTUALES</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>UIFILTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Agrupar por IU

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Agrupar por IU</td>
            <td>Agrupación</td>
            <td>UIGB</td>
            <td>Agrupación</td>
            <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCIAS_ACTUALES</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>UIGROUPBYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Plantilla de IU

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Plantilla de IU</td>
            <td>Plantilla de diseño</td>
            <td>UITMPL</td>
            <td>Plantilla de diseño</td>
            <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Vista de IU

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Vista de IU</td>
            <td>Ver</td>
            <td>UIVIEW</td>
            <td>Ver</td>
            <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCIAS_ACTUALES</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>UIVIEWID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Usuario

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Usuario</td>
            <td>Usuario</td>
            <td>USER</td>
            <td>Usuario</td>
            <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DEFAULTHOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>DELEGATIONTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EAUTHUSERID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMETEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>IDENTIFICADOR DE EQUIPO</td>
        </tr>
        <tr>
             <td>LASTENTEREDNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LATESTUPDATENOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">No se admitirá la tabla de plantillas de diseño</td>
        </tr>
        <tr>
             <td>MANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">No se admitirá la tabla de perfiles de portal</td>
        </tr>
        <tr>
             <td>PREFLUIDO</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>UMUSERID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
    </tbody>
</table>

### Delegación de usuario

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Delegación de usuario</td>
            <td>Delegación de usuario</td>
            <td>USRDEL</td>
            <td>Delegación de usuario</td>
            <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>FROMUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TOUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERDELEGATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Grupo de usuarios

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Grupo de usuarios</td>
            <td>Otros grupos</td>
            <td>USRGPS</td>
            <td>Grupo de usuarios</td>
            <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERSGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Ubicación del usuario

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ubicación del usuario</td>
            <td>Ubicación del usuario</td>
            <td>USRLOC</td>
            <td>UserLocation</td>
            <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Rol de usuario

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rol de usuario</td>
            <td>Otras funciones</td>
            <td>USRROL</td>
            <td>Rol de usuario</td>
            <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>FK</td>
             <td>USERROLESET_CURRENT</td>
             <td>USERROLESETID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Valor de preferencia de usuario

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Valor de preferencia de usuario</td>
            <td>Preferencia del usuario</td>
            <td>USERPF</td>
            <td>Preferencia del usuario</td>
            <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERPREFVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Conjunto de roles de usuario

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UserRoleSet</td>
            <td>Conjunto de roles de usuario</td>
            <td>URSET</td>
            <td>UserRoleSet</td>
            <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PRIMARYROLEID</td>
             <td>FK</td>
             <td>ROLES_ACTUALES</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Decisiones de los usuarios

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UsersDecisions</td>
            <td>Decisiones de los usuarios</td>
            <td>USRDEC</td>
            <td>Decisiones de los usuarios</td>
            <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>USERDECISIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Elemento de trabajo

<table>
    <thead>
        <tr>
            <th>Nombre de entidad de Workfront</th>
            <th>Referencias de interfaz</th>
            <th>Referencia de API</th>
            <th>Etiqueta de API</th>
            <th>Vistas del lago de datos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>WorkItem</td>
            <td>Elemento de trabajo</td>
            <td>WRKITM</td>
            <td>WorkItem</td>
            <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Clave principal/externa</th>
            <th>Tipo</th>
            <th>Tabla relacionada</th>
            <th>Campo relacionado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable basada en OBJCODE</td>
             <td>La clave principal/ID del objeto identificado en el campo OBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">No es una relación; se utiliza con fines de aplicación interna</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>WORKITEMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>
