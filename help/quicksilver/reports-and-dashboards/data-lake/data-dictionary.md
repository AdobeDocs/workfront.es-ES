---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Diccionario de datos de Data Lake
description: Esta página contiene información sobre la estructura y el contenido de los datos del lago de datos de Workfront.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 81f8477dd26b828c4255c678b36d98789cd81ff8
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 5%

---

# Diccionario de datos del lago de datos Workfront

Esta página contiene información sobre la estructura y el contenido de los datos del lago de datos de Workfront.

>[!NOTE]
>
>Los datos del lago de datos de Workfront se actualizan cada cuatro horas, por lo que es posible que los cambios recientes no se reflejen inmediatamente.

## Tipos de tabla

Existen varios tipos de tablas que puede utilizar para ver los datos de Workfront de una manera que proporcione la mayor cantidad de información.

* **Tabla actual**

  La tabla Actual refleja los datos de forma similar a como existe en Workfront, cada objeto y su estado actual. Sin embargo, se puede navegar con una latencia mucho menor que dentro de Workfront.

* **Tabla de eventos**

  La tabla Evento rastrea cada registro de cambios en Workfront: es decir, cada vez que un objeto cambia de estado, se crea un registro que muestra cuándo se produjo el cambio, quién lo hizo y qué se cambió. Por lo tanto, esta tabla es útil para comparaciones puntuales. Esta tabla sólo incluye registros de los últimos tres años.

* **Tabla de historial diario**

  La tabla Historial diario ofrece una versión abreviada de la tabla Evento, ya que muestra el estado de cada objeto diariamente en lugar de cuando se produjo cada evento individual. Como tal, esta tabla es útil para el análisis de tendencias.

<!-- Custom table -->

## Diagrama de relación de entidad

Los objetos de Workfront (y, por lo tanto, de su lago de datos) se definen no solo por sus valores individuales, sino por sus relaciones con otros objetos. El diagrama de relación de entidades que aparece a continuación proporciona una asignación de alto nivel de las relaciones de objetos en el lago de datos de Workfront. El diagrama se puede ver y descargar mediante el siguiente vínculo:

[Diagrama de relación de entidades del lago de datos Workfront](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

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

La siguiente tabla correlaciona los nombres de objetos en Workfront (así como sus nombres en la interfaz y la API) con sus nombres equivalentes en el lago de datos.

<table>
<thead>
  <tr>
    <th>Nombre de entidad de Workfront</th>
    <th>Referencias de interfaz</th>
    <th>Referencia de API | Etiqueta</th>
    <th>Tablas de lago de datos</th>
    <th>Notas</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Asignación</td>
    <td>Asignación</td>
    <td>ASIGNAR | Asignación</td>
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Condición, prioridad, gravedad, estado</td>
    <td>CSTEM | Enumeración personalizada</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>El tipo de registro se identifica mediante la propiedad enumClass. Los siguientes son los tipos esperados:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
  </tr>
  <tr>
    <td>Documento</td>
    <td>Documento</td>
    <td>DOCU | Documento</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>Versión de documento</td>
    <td>DOCV | Versión del documento</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Grupo</td>
    <td>Grupo</td>
    <td>AGRUPAR | Grupo</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Hora</td>
    <td>Hora</td>
    <td>HOUR | Hora</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tipo de hora</td>
    <td>Tipo de hora</td>
    <td>HORA | Tipo de hora</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Hito</td>
    <td>Hito</td>
    <td>MILLA | Hito</td>
    <td>HITOS_ACTUALES<br>HITOS_DIARIOS_HISTORIAL<br>HITOS_EVENTO</td>
    <td></td>
  </tr>
  <tr>
    <td>MilestonePath</td>
    <td>Ruta de hitos</td>
    <td>MPATH | Ruta de hitos</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Nota</td>
    <td>Nota</td>
    <td>NOTA | Nota</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Problema, Solicitud</td>
    <td>OPTASK | Problema</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portafolio</td>
    <td>Portafolio</td>
    <td>PUERTO | Portfolio</td>
    <td>PORTFOLIO_ACTUALES<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIO_EVENT<br><br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Programar</td>
    <td>Programar</td>
    <td>PRGM | Programa</td>
    <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Proyecto</td>
    <td>Proyecto</td>
    <td>PROYECTO | Proyecto</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Función</td>
    <td>Función</td>
    <td>ROL | Rol</td>
    <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Programación</td>
    <td>Programación</td>
    <td>PROGRAMAR | Programación</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tarea</td>
    <td>Tarea</td>
    <td>TAREA | Tarea</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Equipo</td>
    <td>Equipo</td>
    <td>TEAMOB | Equipo</td>
    <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Hoja de horas</td>
    <td>Hoja de horas</td>
    <td>HOJA TSHET | Hoja de horas</td>
    <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>EVENTO_DE_HOJAS DE HORAS</td>
    <td></td>
  </tr>
  <tr>
    <td>Usuario</td>
    <td>Usuario</td>
    <td>USUARIO | Usuario</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
