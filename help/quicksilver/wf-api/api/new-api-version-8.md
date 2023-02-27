---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 8 de API
description: Esta es una lista de recursos que son nuevos para la versión 9 de la API. Para obtener una lista de las actualizaciones realizadas en los recursos de la versión 8, visite Actualizaciones de la versión 8 de la API
author: Becky
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 32%

---

# Novedades de la versión 8 de API

## Nuevos recursos

Esta es una lista de recursos que son nuevos para la versión 9 de la API. Para obtener una lista de las actualizaciones realizadas en los recursos de la versión 8, visite [Actualizaciones de la versión 8 de la API](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| backlogOrder | cliente |   |   | bulkCopy  |   | COPIAR |
| color | iteración  |   |   |   |   | RECUENTO |
| customerID | lastUpdatedBy |   |   |   |   | ELIMINAR |
| estimación | opTask |   |   |   |   | EDITAR |
| Identificador | proyecto |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | INFORME |
| iterationID | tarea |   |   |   |   | SEARCH |
| lastUpdateDate | equipo |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| historyBoardOrder |   |   |   |   |   |   |
| historyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| tipo |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | RECUENTO  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**KanbanBoard**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   | AGREGAR |
| name |   |   |   |   |   | RECUENTO |
|   |   |   |   |   |   | ELIMINAR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ProofApprovalStatus

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| Identificador |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ResourceBudgetedHour**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| allocateDate |   |   |   |   |   | AGREGAR |
| budgetHours |   |   |   |   |   | RECUENTO |
| scheduledBudgetedHours |   |   |   |   |   | ELIMINAR |
| projectID |   |   |   |   |   | EDITAR |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ResourcePlannerFilter

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   | AGREGAR |
| name |   |   |   |   |   | RECUENTO |
|   |   |   |   |   |   | ELIMINAR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**RichTextNote**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   | RECUENTO |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### Suscribirse

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|  Identificador |   |   |   | addSubscribers | suscriptores | AGREGAR |
|   |   |   |   | removeSubscribers |   | RECUENTO  |
|   |   |   |   | suscripciones |   | ELIMINAR |
|   |   |   |   | cancelar suscripciones |   | GET |
|   |   |   |   |   |   | INFORME |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### UserRole

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| roleID | rol |   |   |   |   |   |
| timePercentage | usuario |   |   |   |   |   |
| userID |   |   |   |   |   |   |
