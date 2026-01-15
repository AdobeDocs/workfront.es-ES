---
title: Información general sobre tipos de registros
description: Los tipos de registro son los componentes de un espacio de trabajo de Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 47%

---


# Información general de tipos de registro

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

A diferencia de Workfront, donde los tipos de objeto están predefinidos, en Adobe Workfront Planning puede crear sus propios tipos de objeto.

Por ejemplo, en Workfront, los tipos de objeto Programa, Portafolios, Proyecto, Tarea o Problema ya están creados.

Los tipos de objetos de Workfront Planning se denominan &quot;tipos de registros&quot; y existen únicamente cuando los usuarios los crean.

Los tipos de registro son los componentes básicos de un espacio de trabajo de Workfront Planning y debe crearlos todos para poder asociarlos con el flujo de trabajo y otra información.

Los tipos de registros están organizados en espacios de trabajo.

Para obtener más información acerca de los espacios de trabajo, consulte [Creación de espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

## Información general de tipo de registro

En Workfront Planning, puede crear tipos de registros personalizados que den respuesta a las necesidades de su organización.

Para obtener información acerca de cómo crear tipos de registros, consulte [Creación de tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

* Al crear un espacio de trabajo a partir de una plantilla, los tipos de registros se crean en las siguientes secciones del espacio de trabajo:

   * **Tipos de registros operativos**: tipos de registros que representan planes estratégicos, iniciativas o trabajo planificado. Por ejemplo, Campaña, Actividad, Táctica u Oportunidad son tipos de registros operativos.
   * **Taxonomías**: tipos de registros que capturan atributos sobre un tipo de registro operativo. Por ejemplo, Región, Dirección y Público son taxonomías.

  Puede cambiar el nombre de las secciones y los tipos de registro, eliminarlos o crear más.

* Cuando crea un tipo de registro en un espacio de trabajo que ha creado desde cero, puede colocar el tipo de registro en cualquier sección que cree en el espacio de trabajo.
* Cuando crea un tipo de registro, sólo usted y los usuarios a los que concede permisos para acceder al espacio de trabajo y el tipo de registro pueden acceder a él.
* Debe crear un espacio de trabajo para poder crear tipos de registros para ese espacio de trabajo.

  Para obtener información sobre las limitaciones de cuántos tipos de registros puede haber en un espacio de trabajo o una instancia de Workfront, consulte [Información general sobre las limitaciones de objetos de Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).
* Para utilizar tipos de registros en más de un espacio de trabajo, puede designar los tipos de registros como globales o conectables.

   * Los tipos de registros globales se pueden agregar como tipos de registros existentes a otros espacios de trabajo.
   * Los tipos de registros conectables se pueden conectar a desde otros espacios de trabajo.

  Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->
