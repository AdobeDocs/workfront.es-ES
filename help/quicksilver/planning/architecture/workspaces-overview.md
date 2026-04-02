---
title: Información general sobre espacios de trabajo
description: Un espacio de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning para que coincidan con los flujos de trabajo de las unidades organizativas.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
source-git-commit: f4d7484145226eb85bc547e582438e5202dec023
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 78%

---

# Información general sobre espacios de trabajo

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Un espacio de trabajo es un conjunto de tipos de registros que utiliza una unidad organizativa y representa el ciclo de vida y los procesos de trabajo de la unidad. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning.


![Cuenta de administrador de página de aterrizaje de espacios de trabajo](assets/workspaces-landing-page-admin-account.png)

## Consideraciones sobre espacios de trabajo

* Puede crear espacios de trabajo para unidades organizativas específicas dentro de su organización, de modo que coincidan con el modo único en que funciona cada unidad.
* Workfront Planning no incluye espacios de trabajo preconfigurados. Debe crearlos de acuerdo con las necesidades de su organización.
* Puede crear espacios de trabajo de las siguientes maneras:

   * Desde cero
   * Mediante una plantilla. Las plantillas contienen un número preconfigurado de tipos de registro y sus campos.
   * Uso de Planning Designer con tecnología de IA. Esta función se encuentra actualmente en Beta.
   * <span class="preview">Usando un paquete de plantillas de área de trabajo múltiple.</span>

  Para obtener más información, consulte [Creación de espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

* Los espacios de trabajo son marcos en los que trabajan las unidades organizativas (un equipo, un grupo, un departamento o una división). No se pueden asociar a campos. Solo los tipos de registro dentro de un espacio de trabajo pueden asociarse con campos.

  Para obtener más información, vea [Información general sobre los tipos de registro](/help/quicksilver/planning/architecture/overview-of-record-types.md).
* Según la licencia de Workfront, los espacios de trabajo se muestran en las siguientes pestañas del área de planificación:

   * Para los administradores del sistema, los espacios de trabajo se muestran en las siguientes pestañas:

      * **Espacios de trabajo en los que trabajo**: muestra los espacios de trabajo que ha creado o los que se han compartido con usted.
      * **Otros espacios de trabajo**: muestra todos los demás espacios de trabajo del sistema.

   * Para el resto de los usuarios, los espacios de trabajo que han creado otros y los que otros han compartido con ellos se muestran en el área Espacios de trabajo.

* Los tipos de registro que contiene un espacio de trabajo deben reflejar el ciclo de vida laboral y los conceptos de una unidad organizativa.

  Por ejemplo, si los objetos de trabajo de una unidad son campañas, productos y regiones, el espacio de trabajo de esa unidad debe contener los tipos de registro de Campaña, Producto y Región.
* Cuando crea un espacio de trabajo, solo usted tiene permiso para acceder a él y administrarlo. Debe compartirlo con otros usuarios para que puedan colaborar con usted en el mismo espacio.

  Para obtener más información, vea [Uso compartido de un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md).

  Los administradores del sistema pueden gestionar todos los espacios de trabajo, incluso los que no hayan creado.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Existen límites en cuanto a la cantidad de objetos de espacio de trabajo que se pueden crear en la instancia de Workfront Planning. Para obtener más información, consulte [Información general sobre limitaciones de objetos de Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).
