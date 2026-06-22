---
title: Información general sobre espacios de trabajo
description: Un espacio de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning para que coincidan con los flujos de trabajo de las unidades organizativas.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
TQID: https://experienceleague.adobe.com/Hh1Gh4ex1dLrPhsmqiLv3x5NAU0yKzIwcsV4hEogXTo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 516
ht-degree: 60%

---

# Información general sobre espacios de trabajo

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después del lanzamiento en Vista previa, las mismas funciones también están disponibles mensualmente en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Un espacio de trabajo es un conjunto de tipos de registros que utiliza una unidad organizativa y representa el ciclo de vida y los procesos de trabajo de la unidad. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning.

<!--update screenshot with production, it was broken at Preview-->

![Cuenta de administrador de página de aterrizaje de espacios de trabajo](assets/workspaces-landing-page-admin-account.png)

## Consideraciones sobre espacios de trabajo

* Puede crear espacios de trabajo para unidades organizativas específicas dentro de su organización, de modo que coincidan con el modo único en que funciona cada unidad.
* Workfront Planning no incluye espacios de trabajo preconfigurados. Debe crearlos de acuerdo con las necesidades de su organización.
* Puede crear espacios de trabajo de las siguientes maneras:

   * Desde cero
   * Mediante una plantilla. Las plantillas contienen un número preconfigurado de tipos de registro y sus campos.
   * Uso de Planning Designer con tecnología de IA. Esta función se encuentra actualmente en Beta.
   * Uso de un paquete de plantillas de varios espacios de trabajo.

  Para obtener más información, consulte [Creación de espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

* Los espacios de trabajo son marcos en los que trabajan las unidades organizativas (un equipo, un grupo, un departamento o una división). No se pueden asociar a campos. Solo los tipos de registro dentro de un espacio de trabajo pueden asociarse con campos.

  Para obtener más información, vea [Información general sobre los tipos de registro](/help/quicksilver/planning/architecture/overview-of-record-types.md).
* Los espacios de trabajo se muestran en las siguientes pestañas del área de Planning:

   * **Espacios de trabajo en los que trabajo**: muestra los espacios de trabajo que ha creado o los que se han compartido con usted.
   * **Otros espacios de trabajo**: muestra todos los demás espacios de trabajo del sistema. Solo está disponible para administradores de sistemas.
   * <span class="preview">**Espacios de trabajo de ejemplo**: muestra ejemplos integrados de espacios de trabajo de prácticas recomendadas. No puede editar los espacios de trabajo ni los tipos de registro, ni agregar registros o campos, pero puede agregar, editar y compartir vistas con otros usuarios.</span>

  >[!NOTE]
  >
  ><span class="preview">Recomendamos no editar los espacios de trabajo de ejemplo, sino usarlos como referencia para crear los suyos propios. Utilice el paquete de plantillas de varios espacios de trabajo para crear espacios de trabajo idénticos a los mostrados en la pestaña Espacios de trabajo de ejemplo. Para obtener más información, consulte la sección &quot;Crear varios espacios de trabajo mediante un paquete de plantillas de varios espacios de trabajo de prácticas recomendadas&quot; en el artículo [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md). </span>

<!--
No longer the case - they match now: 

* For all other users:

* **Workspaces I'm on**: Workspaces they created (for Standard-license users) and workspaces others shared with them display in the Workspaces area.

<div class="preview"> 

* **Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.

</div>
-->



* Los tipos de registro que contiene un espacio de trabajo deben reflejar el ciclo de vida laboral y los conceptos de una unidad organizativa.

  Por ejemplo, si los objetos de trabajo de una unidad son campañas, productos y regiones, el espacio de trabajo de esa unidad debe contener los tipos de registro de Campaña, Producto y Región.
* Cuando crea un espacio de trabajo, solo usted tiene permiso para acceder a él y administrarlo. Debe compartirlo con otros usuarios para que puedan colaborar con usted en el mismo espacio.

  Para obtener más información, vea [Uso compartido de un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md).

  Los administradores del sistema pueden gestionar todos los espacios de trabajo, incluso los que no hayan creado.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Existen límites en cuanto a la cantidad de objetos de espacio de trabajo que se pueden crear en la instancia de Workfront Planning. Para obtener más información, consulte [Información general sobre limitaciones de objetos de Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).
