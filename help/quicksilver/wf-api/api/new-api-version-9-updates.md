---
content-type: api
navigation-topic: api-navigation-topic
title: Actualizaciones de la versión 9 de la API
description: Recursos actualizados
author: Becky
feature: Workfront API
role: Developer
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
TQID: https://experienceleague.adobe.com/JAoiJn1kNmwFsYKeuSU67f43wBsgMXCgnMDbcOM-5Kg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 84%

---

# Actualizaciones de la versión 9 de la API

## Recursos actualizados

Los siguientes recursos existentes se han actualizado con esta versión de la API de Adobe Workfront. Para ver los recursos nuevos de la versión 9, visita [Novedades de la versión 9](../../wf-api/api/new-api-version-9.md) de la API y [Novedades de la versión 9 de la API (continuación)](../../wf-api/api/new-api-version-9-continue.md). Los cambios realizados en un recurso se indican de la siguiente manera:

* Las adiciones se enumeran simplemente
* Las eliminaciones se indican con texto tachado
* Los cambios se indican en la nota de después de la tabla

### AgileWork

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |   |  |   |   |  |
| `taskID`<sup>2</sup> |   |   |  |  |  |  |

{style="table-layout:auto"}

<sup>1</sup> Indicador eliminado: REPORTABLE\
Se quitó el marcador <sup>2</sup>: NOT_GROUPABLE

### Aprobación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style="table-layout:auto"}

Asignación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| |   |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `assignUserToRoleOnTasks`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnTasks`<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup> Campo agregado: lockToRole

### CustomerPreferences

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Cambios en possibleValues

### Hora

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `days` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Iteración

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | `moveIssues` |   |   |

{style="table-layout:auto"}

### LayoutTemplates

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### Nota

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `html` |   |   |   |   |   |   |
| `json` |   |   |   |   |   |   |
| `richTextNoteID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### OpTask

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |   |   | `convertToProject` |   |   |
| `isReady` |   |   |   | `convertToTask` |   |   |
| `storyBoardOrder` |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### PresupuestoDeRecursos

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Indicador eliminado: REPORTABLE

### Programación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |   |   |   |   |   |

{style="table-layout:auto"}

### Tarea

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   | `agileWork` |   |   | `convertToProject` |   |   |
|   |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### Equipo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `includeIssues` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TimesheetProfile

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### UIFilter

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `filtersForObjCode` |   |

{style="table-layout:auto"}

### UIView

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `viewsForObjCode` |   |

{style="table-layout:auto"}

### Usuario

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `logTimeInDays` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Trabajo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   | `getWFHomeObjects` |   |   |
