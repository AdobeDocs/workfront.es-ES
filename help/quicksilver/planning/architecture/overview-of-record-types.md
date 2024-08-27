---
title: Información general sobre tipos de registros
description: Los tipos de registro son los componentes básicos de un espacio de trabajo de Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 83c716dea3815ed9a2ce4c3d0598ef42b128de87
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---


# Resumen de tipos de registro

{{planning-important-intro}}

A diferencia de Workfront, donde los tipos de objeto están predefinidos, en Adobe Workfront Planning puede crear sus propios tipos de objeto. Por ejemplo, en Workfront ya se han creado los tipos de objeto Programa, Portfolio, Proyecto, Tarea o Problema.

Los tipos de objetos de Workfront Planning se denominan &quot;tipos de registros&quot; y existen únicamente cuando los usuarios los crean. Los tipos de registro son los componentes básicos de un espacio de trabajo de Workfront Planning. Para obtener información acerca de los espacios de trabajo, vea [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

## Resumen del tipo de registro

En Workfront Planning, puede crear tipos de registros personalizados que satisfagan las necesidades de su organización.

Para obtener información acerca de cómo crear tipos de registros, vea [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

* Al crear un espacio de trabajo a partir de una plantilla, los tipos de registro se crean en las siguientes secciones del espacio de trabajo:

   * **Tipos de registros operativos**: tipos de registros que representan planes estratégicos, iniciativas o trabajo planificado. Por ejemplo, Campaña, Actividad, Táctica u Oportunidad son tipos de registros operativos.
   * **Taxonomías**: tipos de registro que capturan atributos sobre un tipo de registro operativo. Por ejemplo, Región, Dirección y Audiencia son taxonomías.

* Cuando crea un tipo de registro en un espacio de trabajo que ha creado desde cero, puede colocar el tipo de registro en cualquier sección que cree en el espacio de trabajo.
* Cuando crea un tipo de registro, sólo usted y los usuarios a los que concede permisos para acceder al espacio de trabajo pueden ver el tipo de registro.
* Debe crear un espacio de trabajo para poder crear tipos de registros para el espacio de trabajo.
* Puede tener un total de 1.000 tipos de registros en un espacio de trabajo, independientemente de cuántas secciones tenga el espacio de trabajo. Esto incluye los tipos de registro que crea desde cero o que se crean al utilizar una plantilla.


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