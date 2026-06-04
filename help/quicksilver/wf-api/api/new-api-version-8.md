---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 8 de la API
description: Esta es una lista de recursos que son nuevos en la versión 9 de la API. Para obtener una lista de las actualizaciones realizadas en los recursos de la versión 8, visite Actualizaciones de la versión 8 de la API
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
TQID: https://experienceleague.adobe.com/bKFAN--rVO1yxgFLiyhXolgUBajVGYQxM7pBUuqy3v8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 269
ht-degree: 100%

---

# Novedades de la versión 8 de la API

## Nuevos recursos

Esta es una lista de recursos que son nuevos en la versión 9 de la API. Para obtener una lista de las actualizaciones realizadas en los recursos de la versión 8, visite [Actualizaciones de la versión 8 de la API](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| backlogOrder | cliente |   |   | bulkCopy  |   | COPY |
| color | iteración  |   |   |   |   | COUNT |
| customerID | lastUpdatedBy |   |   |   |   | ELIMINAR |
| estimación | opTask |   |   |   |   | EDIT |
| ID | proyecto |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | REPORT |
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
| deprecationRelease |   |   |   |   |   | COUNT  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**KanbanBoard**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | ELIMINAR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ProofApprovalStatus

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | ADD |
| budgetedHours |   |   |   |   |   | COUNT |
| plannedBudgetedHours |   |   |   |   |   | ELIMINAR |
| projectID |   |   |   |   |   | EDIT |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ResourcePlannerFilter

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | ELIMINAR |
|   |   |   |   |   |   | EDITAR |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### Suscribirse

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | subscribers | ADD |
|   |   |   |   | removeSubscribers |   | COUNT  |
|   |   |   |   | subscribes |   | ELIMINAR |
|   |   |   |   | unsubscribes |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### UserRole

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| roleID | función |   |   |   |   |   |
| timePercentage | usuario |   |   |   |   |   |
| userID |   |   |   |   |   |   |
