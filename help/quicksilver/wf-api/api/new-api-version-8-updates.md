---
content-type: api
navigation-topic: api-navigation-topic
title: Actualizaciones de la versión 8 de la API
description: Vea las actualizaciones de la versión 8 de la API.
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
TQID: https://experienceleague.adobe.com/Vlqf19ewhFl6znlfdKapHUmpLWm0gyXDh7eTH1PrMRo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 492
ht-degree: 100%

---

# Actualizaciones de la versión 8 de la API

## Recursos actualizados

Los siguientes recursos existentes se han actualizado con esta versión de la API de Adobe Workfront. Para ver los recursos nuevos de las versiones 8, consulte [Novedades de la versión 8 de la API](../../wf-api/api/new-api-version-8.md). Los cambios realizados en un recurso se indican de la siguiente manera:

* Las adiciones se enumeran simplemente
* Las eliminaciones se indican con texto tachado
* Los cambios se indican en la nota de después de la tabla

### AccessRequest

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| acción<sup>1</sup>  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Cambios en valores posibles

### AccessRule<sup>1</sup> 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| coreAction<sup>2</sup>  |   |   |   |   |   |   |
| forbiddenActions<sup>2</sup> |   |   |   |   |   |   |
| secondaryActions<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Indicador eliminado: REPORTABLE\
<sup>2</sup> Cambia a valores posibles

### Aprobación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  | resourcePools |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambia a valores posibles\
<sup>2</sup>Indicadores añadidos: DYNAMIC, LAZY_READ y NOT_GROUPABLE

### Asignación

|   |   |   |   | Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### Cliente

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   | getPackagingOptionValue |   |   |
| proofPlan<sup>1</sup> |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### CustomerPreferences

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| nombre<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### DocumentApproval

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| ID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Indicador añadido: NOT_FILTERABLE

### DocumentVersion

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style="table-layout:auto"}

### Grupo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   | propietarios |   |   |   |   |

{style="table-layout:auto"}

### HourType

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| appGlobalID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Indicador añadido: NOT_FILTERABLE

### Iteración

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style="table-layout:auto"}

### Igual

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### Nota

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### OpTask

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | iteración |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| estimación |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambia a valores posibles

### Portafolio

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambia a valores posibles

### Programa

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### Proyecto

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   | resourcePools |   |   | defaultShownTimesheetProjects |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### ProofApproval

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| approverID | aprobador |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID<sup>1</sup> |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Indicador añadido: NOT_FILTERABLE

### QueueDef

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| requestorCoreAction<sup>1</sup> |   |   |   |   |   |   |
| requestorForbiddenActions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### Tarifa

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### ReservedTime

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style="table-layout:auto"}

### ResourceManager

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style="table-layout:auto"}

### Tarea

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambia a valores posibles

### Equipo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| agileMethodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatus |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### Plantilla

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style="table-layout:auto"}

### TemplateTask

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

Actualizar

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### Usuario

|   |   | Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### Trabajo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambia a valores posibles\
<sup>2</sup>Indicadores añadidos: DYNAMIC, LAZY_READ y NOT_GROUPABLE
