---
title: Información general sobre las limitaciones de objetos de Adobe Workfront Planning
description: Adobe Workfront Planning tiene límites en cuanto a la cantidad de objetos que se pueden crear en la instancia. Existen límites de objetos para mejorar el rendimiento del producto y la experiencia con Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: 9a7ab1928bfd25c197fca65eddfba1bc01977ea7
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 38%

---


<!--keep the 30 connection limit in yellow till Jan 2026-->

# Información general sobre las limitaciones de objetos de Adobe Workfront Planning

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.</span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}


Adobe Workfront Planning tiene límites en cuanto a la cantidad de objetos que se pueden crear en la instancia. Existen límites de objetos para mejorar el rendimiento del producto y la experiencia con Workfront Planning.

En la tabla siguiente se muestran los límites de la cantidad de objetos que se pueden crear en Workfront Planning. Las limitaciones están sujetas a cambios.

| Objeto de Adobe Workfront Planning | Límite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Número de espacios de trabajo de una instancia de Workfront | Ilimitado* |
| Número de secciones de un espacio de trabajo | 50 |
| Número de tipos de registro para un espacio de trabajo | 100 (incluye los tipos de registro de todas las secciones y los que se crean al utilizar una plantilla de espacio de trabajo) |
| Número de registros para un tipo de registro | 25.000 |
| Número de registros de un espacio de trabajo | Selección de planificación: 25 000 <br> Prime de planificación: 500 000 <br> Ultimate de planificación: 1 000 000 |
| Número de registros totales de una instancia de Workfront Planning | Selección de Planning: 500.000 <br> Prime de Planning: 2.000.000 <br> Ultimate de Planning: Unlimited |
| Número de campos para un tipo de registro o taxonomía | 500 |
| Número de caracteres de un campo de texto de una sola línea | 1.000 caracteres |
| Número de caracteres de un campo de párrafo | 10.000 caracteres |
| Número de campos de párrafo para un tipo de registro | 20 campos de párrafo |
| Tamaño del archivo que puede utilizar para importar información en una tabla de tipo de registro | 1 MB |
| Tamaño del archivo que puede utilizar para importar información en una tabla de tipo de registro a través de la API | 1,5 MB |
| Velocidad a la que se pueden realizar solicitudes de API | 200 solicitudes por minuto |
| Número de vistas que un usuario puede crear para un tipo de registro | 100 |
| Tamaño del archivo CSV de Excel que puede importar para crear tipos de registros | 5 MB |
| Número de filas que puede importar en un archivo CSV o de Excel para crear tipos de registros | 25.000 |
| Número de columnas que se pueden importar en un archivo CSV o de Excel para crear tipos de registros | 500 |
| Número de campos de fórmula para un tipo de registro | 20 |
| Número de campos de conexión para un tipo de registro | 30 |
| Número de caracteres en una expresión de campo de fórmula | 50.000 |
| Número de entidades (usuarios, funciones, equipos, empresas y grupos) con las que puede compartir un objeto de Planning | 100 |
| Número de tipos de registro en una jerarquía | 4 |
| Número de jerarquías en un espacio de trabajo | 5 |
| Número de registros de un tipo de registro principal conectados a un registro de un tipo de registro secundario, dentro de una jerarquía | 10 |
| Número de registros conectados a un registro en un tipo de conexión de selección múltiple, sin una jerarquía configurada entre los registros | 500 |

* Recomendamos no tener demasiados espacios de trabajo, ya que podrían resultar difíciles de administrar y los flujos de trabajo podrían estar demasiado fragmentados.

Para obtener información sobre los precios y el empaquetado de Workfront Planning, póngase en contacto con su administrador de cuentas.

<!--
****************KEEP THIS COMMENTED OUT:

**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->
