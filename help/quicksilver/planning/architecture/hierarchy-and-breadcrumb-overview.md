---
title: Información general de jerarquía y ruta
description: Puede crear varias jerarquías de espacio de trabajo entre los tipos de registro de un espacio de trabajo.
hide: true
hidefromtoc: true
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# Información general de jerarquía y ruta

Como administrador del espacio de trabajo, puede definir jerarquías flexibles pero estructuradas entre tipos de registro y y otros tipos de objetos en Adobe Workfront Planning.

Las jerarquías son conexiones entre tipos de registros. Puede tener hasta 4 tipos de registros y objetos conectados en una jerarquía.

Para obtener información acerca de cómo crear jerarquías, vea [Crear jerarquías de área de trabajo](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Las siguientes son ventajas de utilizar jerarquías en los espacios de trabajo:

* Organizar el trabajo de forma que refleje la forma en que los equipos realmente planean, operan y entregan.
* Para que los usuarios entiendan dónde están, cómo se conectan los tipos de registros y cómo fluye la estrategia en la ejecución, consultando un conjunto de rutas de exploración que indican su lugar en el sistema.
* Para ofrecer una mejor navegación y crear claridad y continuidad en todos los flujos de trabajo.
* Definir flujos que se adapten al funcionamiento de su organización, que admitan flexibilidad y coherencia en todas las etapas de trabajo.

## Consideraciones al trabajar con jerarquías

* Como administrador del espacio de trabajo, puede crear varias jerarquías para un espacio de trabajo.
* Si ya existe una conexión entre los tipos de registro seleccionados, el sistema vuelve a utilizar la conexión existente.
* Si no existe ninguna conexión, Workfront creará automáticamente una como parte de la configuración de jerarquía.
* Las siguientes son reglas para la configuración de jerarquías:
   * Un tipo de registro solo puede tener un tipo de registro principal en un espacio de trabajo determinado.

     Por ejemplo, un tipo de registro Táctico no puede tener un tipo de registro Campaña y un tipo de registro Objetivo como elemento principal en el mismo espacio de trabajo.
   * Un registro se puede conectar a varios registros principales del mismo tipo, cuando se conecta uno a varios o varios a varios tipos de registros.
Por ejemplo, la táctica A puede pertenecer tanto a la Campaña X como a la Campaña Y.
   * Un tipo de registro puede conectarse a varios tipos de registros secundarios.

     Por ejemplo, un tipo de registro de campaña puede ser el principal de varios tipos de registros más, como Tácticas, Pruebas y otros tipos de registros.
   * Las jerarquías pueden incluir tipos de registros de Planning y tipos de objetos de Workfront.

     Por ejemplo, puede tener un tipo de registro de campaña con Tácticas de planificación y Proyectos de Workfront como elementos secundarios.

     <!--asking if ONLY projects are supported here in slack; if yes, make a note to say that only Projects are supported; also add a note about AEM -->
   * Los tipos de registros globales pueden aparecer en varios espacios de trabajo dentro de varias jerarquías. <!--not sure if this AFTER they were added to another workspace; right now, I can see only the current workspace when building one??-->
   * Los tipos de objetos de Workfront también pueden aparecer en varias jerarquías y en diferentes espacios de trabajo.
   * Los tipos de registros globales no pueden formar parte de jerarquías de espacios de trabajo diferentes.

     Por ejemplo, si una campaña es un tipo de registro global y forma parte de una jerarquía en Workspace 1, se puede agregar como un tipo de registro existente a Workspace 2, pero no puede formar parte de una jerarquía allí. <!--verifying that this is not connectable RT and it is about global ones - checking in slack-->
   * Los tipos de registros con conexiones que no crean un campo correspondiente en sus tipos de registros vinculados también pueden formar parte de jerarquías. Las nuevas conexiones que se crean durante la configuración de la jerarquía siempre crearán un campo correspondiente en los tipos de registros vinculados de forma predeterminada.

## Consideraciones al ver rutas

Cuando se crean jerarquías entre tipos de registros, se generan rutas de exploración para los registros que pertenecen a esos tipos de registros.

Por ejemplo, si crea una jerarquía y conecta Campañas con Tácticas y, a continuación, Proyectos, cuando navega a un registro de cualquiera de los tipos conectados en la jerarquía, puede ver en qué parte de la jerarquía se coloca el registro.

Tenga en cuenta lo siguiente:

* Si un tipo de registro forma parte de varias jerarquías en varios espacios de trabajo, puede cambiar entre jerarquías desde la ruta de exploración del registro en la página del registro.
* Las rutas de exploración funcionan en Workfront y Planning.

  Por ejemplo, al ver un proyecto conectado a campañas y tácticas de Planning, así como a portafolios y programas de Workfront, puede cambiar entre las jerarquías de Planning y Workfront desde la ruta de exploración.

  Para obtener más información, vea [Crear jerarquías de área de trabajo](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


