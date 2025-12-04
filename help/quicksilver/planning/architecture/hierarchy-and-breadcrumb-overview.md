---
title: Información general de jerarquía y ruta
description: Puede crear varias jerarquías de espacio de trabajo entre los tipos de registro de un espacio de trabajo.
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
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

Las siguientes son ventajas de utilizar jerarquías en los espacios de trabajo:

* Organizar el trabajo de forma que refleje la forma en que los equipos realmente planean, operan y entregan.
* Los usuarios entienden dónde están, cómo se conectan los tipos de registros y cómo fluye la estrategia en la ejecución al hacer referencia a un conjunto de rutas de exploración que indican su lugar en el sistema.
* Ofrezca una mejor navegación y cree claridad y continuidad en todos los flujos de trabajo.
* Las jerarquías no aplican una estructura rígida definida por el sistema y, en su lugar, le permiten definir flujos que se ajustan a cómo funciona su organización, lo que admite flexibilidad y coherencia en todas las etapas de trabajo.

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
   * Los tipos de registros globales pueden aparecer en varios espacios de trabajo dentro de varias jerarquías.
   * Los tipos de objetos de Workfront también pueden aparecer en varias jerarquías y en diferentes espacios de trabajo.
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * Los tipos de registros con conexiones que no crean un campo correspondiente en sus tipos de registros vinculados también pueden formar parte de jerarquías. Las nuevas conexiones que se crean durante la configuración de la jerarquía siempre crearán un campo correspondiente en los tipos de registros vinculados de forma predeterminada.

## Consideraciones al ver rutas


