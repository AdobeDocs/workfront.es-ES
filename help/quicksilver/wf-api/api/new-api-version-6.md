---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 6 de la API
description: Novedades de la versión 6 de la API
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
TQID: https://experienceleague.adobe.com/ZXBvvhz5ObfHlwX2BBBs2-F2DbSmgY4lj8TwWnMCzBM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 513
ht-degree: 100%

---

# Novedades de la versión 6 de la API

## Nuevos objetos

### Gerente de recursos

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| ID | cliente |   |   |   |   | Agregar |
| customerID | proyecto |   |   |   |   | Cuenta |
| projectID | resourceManager |   |   |   |   | Eliminar |
| resourceManagerID | plantilla |   |   |   |   | Obtener |
| templateID |   |   |   |   |   | Informe  |
|   |   |   |   |   |   | Buscar  |


### Ews

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | upload |   |
| control |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Etiqueta personalizada

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Agregar |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Cuenta |
|   |   |   |   | removeCustomLabel |   | Eliminar |
|   |   |   |   |   |   | Obtener |
|   |   |   |   |   |   | Informe |
|   |   |   |   |   |   | Buscar |


## Objetos actualizados

Cambios en objetos existentes: las adiciones se enumeran simplemente, las eliminaciones tienen el texto tachado, los cambios en los objetos existentes se adjuntan en una nota después de la tabla.

### Actualizar

 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Cambios en valores posibles

<sup>2</sup> el atributo hasFilters ha cambiado a true

 

### Aprobación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Se añadió la validación de fecha

<sup>2</sup> Se añadió el indicador NOT_FILTERABLE

 

### Proceso de aprobación

|   | Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Paso de aprobación

 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Cambios en los valores posibles

 

### Ruta de aprobación<sup>1</sup>

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | Agregar |
| approvedStatusLabel |   |   |   |   |   | Cuenta |
| comentario |   |   |   |   |   | Eliminar |
| enteredByID |   |   |   |   |   | Editar |
| entryDate |   |   |   |   |   | Obtener |
| globalPathID |   |   |   |   |   | Informe |
| isPrivate |   |   |   |   |   | Buscar |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| nombre<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Se cambió a Notificable

<sup>2</sup>Se añadió el validador de longitud máxima

 

### Objeto de servicio de trabajo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup>Se añadió la validación de fecha

<sup>2</sup> Se añadió el indicador Not_Filterable

 

### Asignación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Línea de base 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Se añadió el indicador Not_Filterable

 

### Tarea de línea base

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Se añadió el indicador Not_Filterable

 

### Registro de facturación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> añadió el indicador de campo NO_TIME

### Evento de evolución 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### Categoría 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

Enumeración personalizada 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style="table-layout:auto"}

 

Documento 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Tarifa de cambio 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| tarifa<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> ha cambiado el validador de PRECISION de 8 a 9

 

### Integración

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Entrada de cuaderno

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Cambios en los valores posibles

 

### Optask (Problema)<sup>1</sup> 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marcado como RESTORABLE

Se añadió el indicador <sup>2</sup> Not_Filterable

 

### Proyecto<sup>1</sup> 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| trabajo |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marcado como RESTORABLE y RESOURCE_MANAGEABLE

Se añadió el indicador <sup>2</sup> Not_Filterable

 

### Tarea<sup>1</sup>

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marcado como RESTORABLE

<sup>2</sup>Se añadió el validador AT_DATE_YEAR_BEFORE

<sup>3</sup> Se añadió el indicador Not_Filterable

 

### Equipo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Plantilla<sup>1</sup> 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marcado como RESTORABLE y RESOURCE_MANAGEABLE

### Tarea de plantilla<sup>1</sup> 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marcado como RESTORABLE

Se añadió el indicador <sup>2</sup> Not_Filterable

 

### Usuario

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> infractores de MAX_LENGTH

 

### Nota del usuario

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Valores posibles modificados

<sup>2</sup> ha cambiado los filtros a `[true]`

 

### Anuncio

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
