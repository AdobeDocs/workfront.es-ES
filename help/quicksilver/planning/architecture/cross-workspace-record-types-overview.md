---
title: Información general del tipo de registro entre espacios de trabajo
description: Puede habilitar los tipos de registro para que sean globales o conectables. Los tipos de registros globales se pueden agregar a varios espacios de trabajo desde un espacio de trabajo central o principal en Adobe Workfront Planning, mientras que los tipos de registros conectables se pueden conectar a desde otros espacios de trabajo que no sean los suyos propios.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: 0c890cc535c61c5402a334e43ed45b3ec3f9f748
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 2%

---


# Información general sobre el tipo de registro entre espacios de trabajo

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información acerca de las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Puede habilitar las funciones entre espacios de trabajo para un tipo de registro en Adobe Workfront Planning. Se puede hacer referencia a un tipo de registro entre espacios de trabajo o se puede acceder a él desde más de un espacio de trabajo.

>[!IMPORTANT]
>
>Se han mejorado los requisitos de paquetes de Workfront para poder habilitar las funciones entre espacios de trabajo para los tipos de registros del sistema. Para obtener más información, consulte [Información general sobre el acceso a Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).


Las siguientes son funciones de varios espacios de trabajo de los tipos de registro:

* <span class="preview">**Tipos de registros globales**: los usuarios pueden agregar tipos de registros globales a otros espacios de trabajo que administren.</span>

* **Tipos de registros conectables**: los usuarios pueden conectarse a este tipo de registro desde otros espacios de trabajo.

Este artículo le ofrece una descripción general de los tipos de registros de espacio de trabajo cruzado. Para obtener información acerca de cómo definir las capacidades entre espacios de trabajo de un tipo de registro, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registros](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

<div class="preview">

## Información general sobre los tipos de registros globales

Los tipos de registros globales se pueden agregar a varios espacios de trabajo desde un espacio de trabajo central o principal en Workfront Planning.

Al implementar Workfront Planning para una organización de varios equipos con flujos de trabajo comunes, es posible que necesite definir una estructura y metadatos coherentes para los tipos de registro clave (como Campañas o Entregables) que se pueden agregar a los espacios de trabajo de cada equipo para capturar y administrar su trabajo.

Además, es posible que necesite el trabajo de cada equipo para llegar a un nivel central.

En un flujo de trabajo de este tipo, puede asegurarse de que los equipos capturan su trabajo de forma coherente y, al mismo tiempo, desbloquean la visibilidad entre equipos, sin necesidad de agregar todo a un espacio de trabajo o a todos los miembros de la organización en cada uno de ellos. Puede utilizar tipos de registros globales para conseguirlo.

Para utilizar tipos de registros globales, haga lo siguiente:

1. Desde un espacio de trabajo que administre, configure un tipo de registro para que sea global.

   Un administrador de espacio de trabajo puede otorgar permisos a usuarios con una licencia Standard o a equipos, grupos, funciones y empresas para agregar un tipo de registro elegido a un espacio de trabajo que administren.

   El tipo de registro original existirá en su espacio de trabajo original, pero será visible en otros espacios de trabajo.

   Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Agregue un tipo de registro a un espacio de trabajo secundario desde uno existente que se haya configurado como tipo de registro global.

   El tipo de registro existe en los siguientes espacios de trabajo:

   * Su espacio de trabajo original donde se designó como tipo de registro global.
   * Un espacio de trabajo secundario.

   Para obtener más información, vea [Agregar tipos de registros existentes desde otro área de trabajo](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   En las secciones siguientes se describen consideraciones acerca de los tipos de registros globales y cómo funcionan en sus espacios de trabajo originales o secundarios.

### Consideraciones sobre los tipos de registros globales en su espacio de trabajo original

El tipo de registro configurado para ser global tiene las siguientes propiedades:

* Toda su información (aspecto, campos originales) solo se puede editar en el espacio de trabajo original.

* Puede realizar las siguientes acciones en el tipo de registro global desde su espacio de trabajo original:

   * Edítela

     La edición de un tipo de registro global incluye la edición de su aspecto, las funciones entre espacios de trabajo y todos los campos creados en el espacio de trabajo original.
   * Creación y administración de formularios de solicitud
   * Creación y administración de automatizaciones

* Sólo se puede eliminar un tipo de registro global si no se ha agregado a un espacio de trabajo secundario. Primero debe eliminarlo (eliminándolo) de los espacios de trabajo secundarios para poder eliminarlo del espacio de trabajo original.

  Para obtener más información, vea [Eliminar tipos de registros](/help/quicksilver/planning/architecture/delete-record-types.md).
* Los registros que agregue a un tipo de registro global sólo son visibles para los usuarios que tienen permisos de Vista en el área de trabajo donde se agregaron.
* Los registros que agregue desde un espacio de trabajo secundario se acumulan y se muestran en el espacio de trabajo original. Todos los miembros del espacio de trabajo original obtienen permisos de visualización para ellos.
* Cuando se agrega el tipo de registro global original a varios espacios de trabajo secundarios, se presentan los siguientes escenarios:

   * Los miembros del espacio de trabajo original obtienen automáticamente permisos de Vista para todos los registros agregados desde cualquier espacio de trabajo, incluso si no son miembros de dichos espacios de trabajo.
   * Los miembros del área de trabajo secundaria sólo pueden ver registros de áreas de trabajo en las que son miembros.
* Los tipos de registro conectados de un tipo de registro global estarán disponibles para la conexión desde los espacios de trabajo donde se agregue este tipo de registro.

  Por ejemplo, si tiene un tipo de registro global de campaña que tiene una conexión con un tipo de registro de regiones y agrega el tipo de registro de campaña a un espacio de trabajo secundario, las regiones se podrán conectar entre espacios de trabajo desde el espacio de trabajo secundario. Los miembros del espacio de trabajo secundario ahora pueden crear campañas y vincularlas a regiones.

* Los campos creados para un tipo de registro global desde el espacio de trabajo original son visibles desde todos los espacios de trabajo donde se agrega el tipo de registro. Solo se puede editar la configuración de campo desde el espacio de trabajo original. La configuración de los campos creados en el espacio de trabajo original es de sólo lectura en los espacios de trabajo secundarios para todos los miembros, independientemente de sus permisos en el espacio de trabajo secundario. Los administradores del espacio de trabajo secundario no pueden modificar la configuración de campos de los campos configurados en el espacio de trabajo original. Sólo los administradores del espacio de trabajo original pueden modificar la configuración de campos del espacio de trabajo original.

### Consideraciones sobre los tipos de registros globales en un espacio de trabajo secundario

* Los colaboradores secundarios del espacio de trabajo obtienen permiso de contribución para el tipo de registro global en el espacio de trabajo de su equipo. Pueden agregar y administrar registros desde el espacio de trabajo secundario.

* Los visualizadores de espacio de trabajo secundario obtienen permiso de visualización para el tipo de registro global en el espacio de trabajo de su equipo. No pueden agregar ni administrar registros en él.

* Los gestores de espacio de trabajo secundario pueden realizar las siguientes acciones adicionales en el tipo de registro añadido desde un tipo de registro global en un espacio de trabajo secundario:

   * Elimínelo.

     Al eliminar el tipo de registro de un espacio de trabajo secundario, solo se elimina de este. También se eliminan los registros y campos que se le hayan agregado desde el espacio de trabajo secundario. Esto no elimina el tipo de registro de su espacio de trabajo original ni de ningún otro espacio de trabajo secundario donde se haya agregado.

     Para obtener más información, vea [Eliminar tipos de registros](/help/quicksilver/planning/architecture/delete-record-types.md).
   * Comparta las vistas de los tipos de registros.

     No se puede compartir una vista públicamente desde un tipo de registro global en un espacio de trabajo secundario. Solo puede compartir vistas internamente desde un espacio de trabajo secundario. Puede compartir una vista interna y públicamente para un tipo de registro global en su espacio de trabajo original.

     Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).


     <!-- when they will be able to add fields to the secondary space, this bullet will need this extra information: 
         After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added. -->

  <!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
    * Add new fields
        Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
    * Share it
    * Add request forms to it
    * Add automations to it-->

* Ningún usuario puede realizar las siguientes acciones en un tipo de registro global en un espacio de trabajo secundario:

   * Edítela

     No se puede editar su aspecto, sus funciones entre espacios de trabajo ni los campos añadidos desde el espacio de trabajo original.
   * Compartirlo
   * Creación y administración de formularios de solicitud
   * Creación y administración de automatizaciones

* Los registros añadidos en un espacio de trabajo secundario son visibles desde los siguientes espacios de trabajo, solo si tiene permisos de Vista o superiores en estos espacios de trabajo:

   * Espacio de trabajo secundario donde se agregan.
   * Espacio de trabajo original del tipo de registro global.
   * Todos los demás espacios de trabajo en los que se agrega el espacio de trabajo global.

* Los siguientes escenarios existen para registros creados en espacios de trabajo secundarios:

   * Si tiene permisos de Administración en el espacio de trabajo original y no tiene permisos en espacios de trabajo secundarios, puede ver los registros agregados desde los espacios de trabajo secundarios en el espacio de trabajo original, pero no puede administrarlos desde el espacio de trabajo original.
   * Si tiene permisos de Administración en el espacio de trabajo secundario, puede administrar los registros tanto del espacio de trabajo original del tipo de registro global como del espacio de trabajo secundario donde se agregaron.
   * Puede ver los registros en espacios de trabajo secundarios adicionales en los que el tipo de registro global se agrega sólo si tiene permisos de visualización en dichos espacios de trabajo.

### Acceso a las conexiones de un tipo de registro global

Los tipos de registro conectados al tipo de registro global en el espacio de trabajo original se hacen visibles desde otros espacios de trabajo donde se agrega el tipo de registro global y están disponibles para conexiones desde los espacios de trabajo secundarios donde se agrega el tipo de registro global.

### Acceso a la API de un tipo de registro global

Al agregar registros a un tipo de registro global desde un espacio de trabajo secundario mediante la API de Workfront Planning, el sistema comprueba si el usuario tiene acceso para crear registros en el espacio de trabajo original del tipo de registro global.

Se dan los siguientes casos:

* Si el usuario tiene acceso, el registro se crea en el espacio de trabajo original de los tipos de registro global.

* Si el usuario no tiene acceso, recibe el error de que no tiene acceso al espacio de trabajo original del tipo de registro global y debe proporcionar el ID del espacio de trabajo donde tenga acceso para crear registros.

</div>

## Información general sobre los tipos de registros conectables

Puede conectarse a un tipo de registro que se haya definido como conectable desde cualquier espacio de trabajo que administre.

Es posible que sus equipos necesiten registros vinculados a tipos de registros de otros espacios de trabajo o ver información capturada en registros que pertenecen a registros de otros espacios de trabajo. Puede conseguir esta configuración designando un tipo de registro como conectable.

Para utilizar tipos de registros conectables, haga lo siguiente:

1. Configure un tipo de registro para que se pueda conectar en un espacio de trabajo específico.

   Un gestor de espacio de trabajo puede seleccionar a qué espacios de trabajo está disponible un tipo de registro designado para conectarse.

   El tipo de registro original existirá en su espacio de trabajo original y se puede acceder a él desde otro espacio de trabajo.

   Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Conéctese a un tipo de registro designado como conectable desde otro espacio de trabajo que administre.

   Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
