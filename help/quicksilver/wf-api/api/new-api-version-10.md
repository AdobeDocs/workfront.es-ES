---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 10 de la API
description: Recursos actualizados
author: Becky
feature: Workfront API
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 46%

---

# Novedades de la versión 10 de la API

* [Nuevos recursos](#new-resources)
* [Recursos actualizados](#updated-resources)
* [Recursos eliminados](#removed-resources)

## Nuevos recursos {#new-resources}

### ActivityLog

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | AGREGAR |
|   |   |   |   |   |   | RECUENTO |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### Entrada de calendario

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   | AGREGAR |
|   |   |   |   |   |   | RECUENTO  |
|   |   |   |   |   |   | ELIMINAR  |
|   |   |   |   |   |   | EDITAR  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | INFORME  |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### CalendarEntryExternalReference

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   | RECUENTO |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | INFORME  |
|   |   |   |   |   |   | SEARCH  |

{style=&quot;table-layout:auto&quot;}

### ExternalAuthToken

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   | AGREGAR |
|   |   |   |   |   |   | RECUENTO |
|   |   |   |   |   |   | ELIMINAR  |
|   |   |   |   |   |   | EDITAR  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | INFORME  |
|   |   |   |   |   |   | SEARCH  |

{style=&quot;table-layout:auto&quot;}

### LicenseTypeGroupLimit

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| customerID | cliente |   |   |   |   |   |
| groupID | grupo |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedlicense |   |   |   |   |   |   |
| límite de trabajo |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserHomeCalendarPreference

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| customerID | cliente |   |   |   |   | AGREGAR |
| edTime | usuario |   |   |   |   | RECUENTO |
| firstDayOfWeek |   |   |   |   |   | ELIMINAR |
| Identificador |   |   |   |   |   | EDITAR |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | INFORME |
| userID |   |   |   |   |   | SEARCH |
| workDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**Recursos actualizados**

Con esta versión de la API de Workfront se han actualizado los siguientes recursos existentes. Los cambios realizados en un recurso se indican de la siguiente manera:

* Las adiciones simplemente aparecen en la lista
* Las eliminaciones se indican con texto tachado
* Los cambios se enumeran en la nota después de la tabla

### Ruta de aprobación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `¹`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹ Type changed from null to boolean`

### Asignación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| assignPercent `¹` |   |   |   |   |   |   |
| viewByAssignedToUser |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹`validador agregado LESS_THAN_EQUAL

### BudgetedHour

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Preferencias de cliente

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| name `¹` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Cambios en los valores posibles

### DocMetadataLinkGroup

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style=&quot;table-layout:auto&quot;}

### Documento

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### DocumentRequest

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

DocumentVersion

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| externalIntegrationType ¹ |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Cambios en los valores posibles

Gasto

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Grupo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style=&quot;table-layout:auto&quot;}

### LinkedFolder

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| externalIntegrationType¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Cambios en los valores posibles

### OpTask

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| priorityColor |  |  | pendingApproval¹ |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ El tipo cambió de nulo a booleano

### Sección del portal

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|  |  |  | groupIDs |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Portafolio

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| portafolioNetValue |  |  |  |  |  |  |
| portafolioRoi |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Proyecto

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ProofApproval

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| aprobadorDecisión |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Tarifa

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| rateValue ¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

Se ha añadido la MONEDA al validador

### Tarea

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Equipo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| hoursPerPoint ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ validador añadido LESS_THAN

### TeamAssignment

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TeamTask

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Hoja de horas

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Actualizar

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| updateType `¹` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style=&quot;table-layout:auto&quot;}

¹ cambios en possibleValues

### Usuario

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserNote

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| eventType ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ cambios en possibleValues

### Trabajo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval ¹  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ El tipo cambió de nulo a booleano

## Recursos eliminados {#removed-resources}

### ResourceBudgetedHour

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| allocateDate |   |   |   |   |   | AGREGAR  |
| budgetHours |   |   |   |   |   | RECUENTO  |
| Identificador |   |   |   |   |   | ELIMINAR  |
| scheduledBudgetedHours |   |   |   |   |   | EDITAR  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | INFORME  |
| userID |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

 

 

 
