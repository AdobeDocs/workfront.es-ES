---
title: Información general sobre las limitaciones de objetos de Adobe Workfront Planning
description: Adobe Workfront Planning tiene límites en cuanto a la cantidad de objetos que se pueden crear en la instancia. Existen límites de objetos para mejorar el rendimiento del producto y la experiencia con Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 2%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Información general sobre las limitaciones de objetos de Adobe Workfront Planning

Adobe Workfront Planning tiene límites en cuanto a la cantidad de objetos que se pueden crear en la instancia. Existen límites de objetos para mejorar el rendimiento del producto y la experiencia con Workfront Planning.

En la tabla siguiente se muestran los límites de la cantidad de objetos que se pueden crear en Workfront Planning. Las limitaciones están sujetas a cambios a medida que avanzamos hacia las siguientes fases de desarrollo.

| Objeto de Adobe Workfront Planning | Límite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Número de espacios de trabajo de una instancia de Workfront | 1.000 |
| Número de secciones de un espacio de trabajo | 50 |
| Número de tipos de registro de un espacio de trabajo | 1000 (incluye los tipos de registro de todas las secciones y los que se crean al utilizar una plantilla de espacio de trabajo) |
| Número de registros para un tipo de registro | 50.000 |
| Número de campos para un tipo de registro o taxonomía | 500 |
| Número de caracteres de un campo de texto | 1.000 caracteres |
| Tamaño del archivo que puede pegar en una tabla de tipo de registro | 1 MB |
| Tamaño del archivo que puede importar mediante la API para una tabla de tipo de registro | 1,5 MB |
| Velocidad a la que se pueden realizar solicitudes de API | 200 solicitudes por minuto |
| Número de vistas que un usuario puede crear para un tipo de registro | 100 |

<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.

****************KEEP THIS COMMENTED OUT:
| Size of CSV of Excel file you can import** | 5MB |
**This functionality has been temporarily removed and it will be available at a later date.**********************
-->