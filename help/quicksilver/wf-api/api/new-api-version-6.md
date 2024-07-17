---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 6 de la API
description: Novedades de la versión 6 de la API
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 34%

---

# Novedades de la versión 6 de la API

## Nuevos objetos

### Gerente de recursos

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador | cliente |   |   |   |   | Agregar |
| customerID | proyecto |   |   |   |   | Cuenta |
| projectID | resourceManager |   |   |   |   | Eliminar |
| resourceManagerID | plantilla |   |   |   |   | Obtener |
| templateID |   |   |   |   |   | Informe  |
|   |   |   |   |   |   | Buscar  |


### Ews

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | cargar |   |
| manipular |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Etiqueta personalizada

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   | checkDelete | customLabels | Agregar |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Cuenta |
|   |   |   |   | removeCustomLabel |   | Eliminar |
|   |   |   |   |   |   | Obtener |
|   |   |   |   |   |   | Informe |
|   |   |   |   |   |   | Buscar |


## Objetos actualizados

Cambios en objetos existentes: las adiciones se enumeran simplemente, las eliminaciones tienen tachado, los cambios en los objetos existentes tienen una nota adjunta después de la tabla

### Actualizar

 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> cambios en valores posibles

<sup>2</sup> ha cambiado el atributo hasFilters a true

 

### Aprobación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

Se agregó la validación de fecha <sup>1</sup>

Se agregó el indicador <sup>2</sup> NOT_FILTERABLE

 

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

<sup>1</sup> cambios en valores posibles

 

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

Se cambió <sup>1</sup> a Informable

Se agregó el validador de longitud máxima de <sup>2</sup>

 

### Objeto de servicio de trabajo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

Se agregó la validación de fecha <sup>1</sup>

Se agregó el marcador <sup>2</sup> Not_Filterable

 

### Asignación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Línea base 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

Se agregó el marcador <sup>1</sup> Not_Filterable

 

### Tarea de línea base

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

Se agregó el marcador <sup>1</sup> Not_Filterable

 

### Registro de facturación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> agregó el indicador de campo NO_TIME

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
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatus |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatus |   |
|   |   |   |   |   | taskGroupStatus |   |

{style="table-layout:auto"}

 

Documento 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Tipo de cambio 

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

<sup>1</sup> cambios en valores posibles

 

### Optask (Problema)<sup>1</sup> 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> marcado como RESTAURABLE

Se agregó el marcador <sup>2</sup> Not_Filterable

 

### Proyecto<sup>1</sup> 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| trabajar |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> marcado como RESTAURABLE y RESOURCE_MANAGEABLE

Se agregó el marcador <sup>2</sup> Not_Filterable

 

### Tarea<sup>1</sup>

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> marcado como RESTAURABLE

Se agregó el validador <sup>2</sup> AT_DATE_YEAR_BEFORE

Se agregó el marcador <sup>3</sup> Not_Filterable

 

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

<sup>1</sup> marcado como RESTAURABLE y RESOURCE_MANAGEABLE

### Tarea de plantilla<sup>1</sup> 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> marcado como RESTAURABLE

Se agregó el marcador <sup>2</sup> Not_Filterable

 

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

<sup>1</sup> valores posibles cambiados

<sup>2</sup> ha cambiado los filtros a `[true]`

 

### Anuncio

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
