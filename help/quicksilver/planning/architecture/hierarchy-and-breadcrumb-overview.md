---
title: Información general de jerarquía y ruta
description: Puede crear varias jerarquías de espacio de trabajo entre los tipos de registro de un espacio de trabajo, después de conectar los tipos de registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 34921b12ad902ba7390e4ea34825331280e7a8d6
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---



# Información general de jerarquía y ruta

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como administrador del espacio de trabajo, puede definir jerarquías flexibles pero estructuradas entre tipos de registros conectados y otros tipos de objetos en Adobe Workfront Planning.

Las jerarquías son conexiones entre tipos de registros o entre tipos de registros y un proyecto de Workfront.

Para obtener información acerca de cómo crear jerarquías, vea [Crear jerarquías de área de trabajo](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Las siguientes son ventajas de utilizar jerarquías en los espacios de trabajo:

* Organizar el trabajo de forma que refleje la forma en que los equipos realmente planean, operan y entregan.
* Para que los usuarios entiendan dónde están, cómo se conectan los tipos de registros y cómo fluye la estrategia en la ejecución, consultando un conjunto de rutas de exploración que indican su lugar en el sistema.
* Para ofrecer una mejor navegación y crear claridad y continuidad en todos los flujos de trabajo.
* Definir flujos que se adapten al funcionamiento de su organización, que admitan flexibilidad y coherencia en todas las etapas de trabajo.

## Consideraciones al trabajar con jerarquías

* Se pueden crear hasta cinco jerarquías para un espacio de trabajo.
* Puede tener hasta 4 tipos de registros y objetos conectados en una jerarquía.
* Sólo se pueden conectar los tipos de objeto siguientes en una jerarquía de espacio de trabajo:
   * Tipos de registro que pertenecen al espacio de trabajo en el que está creando las jerarquías.
   * Proyectos de Workfront. Los proyectos de Workfront no se pueden agregar como principales de otros tipos de registro. Siempre son el último tipo de objeto de una jerarquía.
* No se pueden agregar los siguientes tipos de objeto en una jerarquía:
   * Tipos de registro de otros espacios de trabajo, incluso cuando están configurados como tipos de registro conectables o globales. Puede agregar tipos de registros globales a jerarquías sólo cuando se hayan agregado al espacio de trabajo desde el que está creando la jerarquía.
   * Todos los demás objetos de Workfront.
   * AEM Assets.
* Las jerarquías pueden incluir tipos de registros de Planning y proyectos de Workfront al mismo tiempo.

      Por ejemplo, puede tener un tipo de registro de campaña con Tácticas de planificación y Proyectos de Workfront como elementos secundarios en la misma jerarquía de área de trabajo.
  * Si ya existe una conexión entre los tipos de registro seleccionados, el sistema vuelve a utilizar la conexión existente.
* Si no existe ninguna conexión, Workfront creará una como parte de la configuración de jerarquía.
* La configuración **Crear campo correspondiente en el tipo de registro vinculado** debe estar activada para el campo conectado para los registros y tipos de objeto que desea incluir en una jerarquía.
* No puede eliminar un tipo de registro si forma parte de una jerarquía.
* No puede eliminar un campo de conexión si el tipo de registro al que se hace referencia en el campo forma parte de una jerarquía. Primero debe quitar el tipo de registro de la jerarquía o eliminar la jerarquía antes de poder eliminar el tipo de registro.
* Puede eliminar un campo de búsqueda de un tipo de registro conectado. No se puede recuperar la información del campo.
* Las siguientes son reglas para la configuración de jerarquías:
   * Un tipo de registro solo puede tener un tipo de registro principal en un espacio de trabajo determinado.

     Por ejemplo, un tipo de registro Táctico no puede tener un tipo de registro Campaña y un tipo de registro Objetivo como elemento principal en el mismo espacio de trabajo.
   * Un tipo de registro puede ser el principal en varias jerarquías.

     Por ejemplo, puede tener tres jerarquías diferentes en un espacio de trabajo, y cada una de ellas puede tener Campañas como tipo de registro principal.
   * Un registro se puede conectar a varios registros principales del mismo tipo, cuando se conecta uno a varios o varios a varios tipos de registros.

     Por ejemplo, la táctica A puede pertenecer tanto a la Campaña X como a la Campaña Y.
   * Un tipo de registro sólo puede conectarse a un tipo de registro secundario a la vez. Un tipo de registro secundario también puede ser primario para otro tipo de registro.

     Por ejemplo, un tipo de registro de campaña puede ser el principal de otro tipo de registro en la misma jerarquía (Tácticas), y Tácticas a su vez puede ser el principal de Programas, que puede ser principal de Proyectos.
   * Un tipo de registro no puede ser el principal de una jerarquía y el secundario de otra jerarquía del mismo espacio de trabajo.
   * Los tipos de registros globales pueden aparecer en varios espacios de trabajo dentro de varias jerarquías, una vez añadidos a dichos espacios de trabajo.

     Por ejemplo, si una campaña es un tipo de registro global y forma parte de una jerarquía en Workspace 1, se puede agregar como un tipo de registro existente a Workspace 2 y puede formar parte de una jerarquía allí. Pero no puede formar parte de una jerarquía en Workspace 2 solo cuando se designa como tipo de registro global en Workspace 1, pero no se agrega a Workspace 2.
   * Cuando los tipos de registro conectados forman parte de jerarquías, puede conectar un registro de un tipo de registro secundario a un máximo de 10 registros de un tipo de registro principal.

     Por ejemplo, si crea una jerarquía entre Campañas como principal y Persona como registro secundario, puede conectar la misma persona hasta a 10 campañas.

## Consideraciones al ver rutas

Cuando se crean jerarquías entre tipos de registros, se generan rutas de exploración para los registros que pertenecen a esos tipos de registros.

Por ejemplo, si crea una jerarquía y conecta Campañas con Tácticas, luego con Actividades y después con Proyectos, cuando navega a un registro de cualquiera de los tipos conectados en la jerarquía, puede ver en qué parte de la jerarquía se coloca el registro.

![Ruta de exploración](assets/breadcrumbs-on-project.png)

Tenga en cuenta lo siguiente:

* Si un tipo de registro forma parte de varias jerarquías, puede cambiar entre jerarquías desde la ruta de exploración del registro en la página del registro.
* Si el tipo de registro de una jerarquía tiene varios registros, puede seleccionar registros de la ruta de exploración.
* Las rutas de exploración funcionan en Workfront y Planning.

  Por ejemplo, cuando se mira un proyecto que está conectado a campañas y tácticas de Planning, y también a portafolios y programas de Workfront, puede cambiar entre los tipos de objeto de Planning y Workfront de la ruta de exploración.

  Para obtener más información, vea [Crear jerarquías de área de trabajo](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* Al editar un registro, los cambios son visibles desde todos los espacios de trabajo y todas las jerarquías de las que forma parte el registro.


