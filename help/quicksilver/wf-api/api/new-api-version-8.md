---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 8 de la API
description: Esta es una lista de recursos que son nuevos en la versión 9 de la API. Para obtener una lista de las actualizaciones realizadas en los recursos de la versión 8, visite Actualizaciones de la versión 8 de la API
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 29%

---

# Novedades de la versión 8 de la API

## Nuevos recursos

Esta es una lista de recursos que son nuevos en la versión 9 de la API. Para obtener una lista de las actualizaciones realizadas en los recursos de la versión 8, visite [Actualizaciones de la versión 8 de la API](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| backlogOrder | cliente |   |   | bulkCopy  |   | COPIAR |
| color | iteración  |   |   |   |   | RECUENTO |
| customerID | lastUpdatedBy |   |   |   |   | ELIMINAR |
| tasar | opTask |   |   |   |   | EDITAR |
| Identificador | proyecto |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | INFORME |
| iterationID | tarea |   |   |   |   | SEARCH |
| lastUpdateDate | equipo |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| tipo |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | RECUENTO  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**Panel Kanban**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   | AÑADIR |
| name |   |   |   |   |   | RECUENTO |
|   |   |   |   |   |   | ELIMINAR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ProofApprovalStatus

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**MetadatosDeArchivoDeRevisión**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| Identificador |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**HoraPresupuestadaDeRecursos**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | AÑADIR |
| budgetHours |   |   |   |   |   | RECUENTO |
| plannedBudgetedHours |   |   |   |   |   | ELIMINAR |
| projectID |   |   |   |   |   | EDITAR |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ResourcePlannerFilter

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   | AÑADIR |
| name |   |   |   |   |   | RECUENTO |
|   |   |   |   |   |   | ELIMINAR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   | RECUENTO |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### Suscribirse

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | suscriptores | AÑADIR |
|   |   |   |   | removeSubscribers |   | RECUENTO  |
|   |   |   |   | suscribe |   | ELIMINAR |
|   |   |   |   | cancela la suscripción |   | GET |
|   |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### UserRole

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| roleID | función |   |   |   |   |   |
| timePercentage | usuario |   |   |   |   |   |
| userID |   |   |   |   |   |   |
