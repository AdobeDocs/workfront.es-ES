---
content-type: api
navigation-topic: api-navigation-topic
title: Novedades de la versión 6 de la API
description: Novedades de la versión 6 de la API
author: John
feature: Workfront API
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 2ec05c03a5bfa842008870ca47fb617b81fd6ebd
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 42%

---

# Novedades de la versión 6 de la API

## Nuevos objetos

### Gerente de recursos

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador | cliente |   |   |   |   | Agregar |
| customerID | proyecto |   |   |   |   | Cuenta |
| projectID | resourceManager |   |   |   |   | Eliminar |
| resourceManagerID | plantilla |   |   |   |   | Get |
| templateID |   |   |   |   |   | Informe  |
|   |   |   |   |   |   | Buscar  |


### Ews

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | cargar |   |
| handle |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Etiqueta personalizada

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| Identificador |   |   |   | checkDelete | customLabels | Agregar |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Cuenta |
|   |   |   |   | removeCustomLabel |   | Eliminar |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Informe |
|   |   |   |   |   |   | Buscar |


## Objetos actualizados

Cambios en objetos existentes: las adiciones se enumeran simplemente, las eliminaciones se han eliminado, los cambios en las ya existentes tienen una nota adjunta después de la tabla

### Actualizar

 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID² |   |

{style=&quot;table-layout:auto&quot;}

¹ Cambios en los valores posibles

² El atributo hasFilters ha cambiado a true

 

### Ruta de aprobación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate¹ |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Se agregó la validación de fecha

² Se ha añadido el indicador NOT_FILTERABLE

 

### Proceso de aprobación

|   | Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|---|
|  |  | `attachedApprovalPaths` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Paso de aprobación

 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| approvalType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Cambios en posibles valores

 

### Ruta de aprobación¹

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | Agregar |
| approvedStatusLabel |   |   |   |   |   | Cuenta |
| comentario |   |   |   |   |   | Eliminar |
| enteredByID |   |   |   |   |   | Editar |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | Informe |
| isPrivate |   |   |   |   |   | Buscar |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Cambiado a Informable

² Se ha agregado el validador de longitud máxima

 

### Objeto de servicio de trabajo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| constraintDate¹ |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired² |   |   |   | workItemStatusLabels  |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Validación de fecha agregada

² Se Ha Agregado Un Indicador No Filtrable

 

### Asignación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Línea base 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Indicador no filtrable añadido

 

### Tarea de línea base

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Indicador no filtrable añadido

 

### Registro de facturación

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| billingDate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ se ha añadido el indicador de campo NO_TIME

### Evento de pérdida 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style=&quot;table-layout:auto&quot;}

 

### Categoría 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style=&quot;table-layout:auto&quot;}

 

Enumeración personalizada 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatus |   |
|   |   |   |   | ispossibleToUnlockStatus | projectGroupStatus |   |
|   |   |   |   |   | taskGroupStatus |   |

{style=&quot;table-layout:auto&quot;}

 

Documento 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

tarifa de cambio 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| tasa¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Se ha cambiado el validador de PRECISION para 8 a 9

 

### Integración

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Entrada de cuaderno

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Cambios en posibles valores

 

### Optask (Problema)¹ 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Marcado como RESTAURABLE

² Se Ha Agregado Un Indicador No Filtrable

 

### Proyecto¹ 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| trabajo |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Marcado como RESTAURABLE y RESOURCE_MANAGEABLE

² Se Ha Agregado Un Indicador No Filtrable

 

### Tarea¹

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| constraintDate² |   |   |   |   |   |   |
| workRequired3 |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Marcado como RESTAURABLE

² Se agregó el validador AT_DATE_YEAR_BEFORE

Se Ha Añadido Un Indicador No Filtrable

 

### Equipo

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Plantilla¹ 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Marcado como RESTAURABLE y RESOURCE_MANAGEABLE

### Tarea de plantilla¹ 

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Marcado como RESTAURABLE

² Se Ha Agregado Un Indicador No Filtrable

 

### Usuario

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| myInfo¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Violadores de MAX_LENGTH

 

### Nota del usuario

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
| eventType¹ |   |   |   |   | myNotifications² |   |

{style=&quot;table-layout:auto&quot;}

¹ Valores posibles modificados

² tiene filtros modificados en `[true]`

 

### Anuncio

| Campos | Referencias | Colecciones | Buscar | Acciones | Consultas | Operaciones |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
