---
content-type: api
navigation-topic: api-navigation-topic
title: Actualizaciones de la versión 8 de API
description: Vea las actualizaciones de la versión 8 de la API.
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 34%

---

# Actualizaciones de la versión 8 de API

## Recursos actualizados

Los siguientes recursos existentes se han actualizado con esta versión de la API de Adobe Workfront. Para ver los recursos nuevos de las versiones 8, consulte [Novedades de la versión 8 de la API](../../wf-api/api/new-api-version-8.md). Los cambios realizados en un recurso se indican de la siguiente manera:

* Las adiciones se enumeran simplemente
* Las eliminaciones se indican con texto tachado
* Los cambios se registran en la nota después de la tabla

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

<sup>1</sup> Indicador eliminado: INFORMABLE\
<sup>2</sup> Cambios en valores posibles

### Ruta de aprobación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  | resourcePools |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles\
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

### Preferencias del cliente

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| name<sup>1</sup> |   |   |   |   |   |   |

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

### Me gusta

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
| tasar |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### Portafolio

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Cambios en valores posibles

### Programar

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

### TiempoReservado

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

<sup>1</sup>Cambios en valores posibles

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

<sup>1</sup>Cambios en valores posibles\
<sup>2</sup>Indicadores añadidos: DYNAMIC, LAZY_READ y NOT_GROUPABLE
