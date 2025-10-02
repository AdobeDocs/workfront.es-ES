---
title: Información general sobre tipos de registros entre espacios de trabajo
description: Los tipos de registros centralizados se pueden agregar a varios espacios de trabajo desde un espacio de trabajo central o principal en Adobe Workfront Planning.
hidefromtoc: true
hide: true
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '1349'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Información general sobre tipos de registros entre espacios de trabajo

En Adobe Workfront Planning, puede habilitar las funciones entre espacios de trabajo para un tipo de registro que le permita hacer referencia a un tipo de registro en más de un espacio de trabajo.

Las siguientes son funciones de varios espacios de trabajo de los tipos de registro:

* Puede designar un tipo de registro como centralizado. Los usuarios pueden agregar tipos de registros centralizados a otros espacios de trabajo que administran.

  >[!IMPORTANT]
  >
  >Debe tener un paquete Workfront Planning Plus, además de un paquete Workfront para utilizar tipos de registros centralizados.
  >
  >Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront.

* Puede designar un tipo de registro como conectable. Los usuarios pueden conectarse a este tipo de registro desde otros espacios de trabajo.

Este artículo le ofrece una descripción general de los tipos de registros de espacio de trabajo cruzado. Para obtener información acerca de cómo definir las capacidades entre espacios de trabajo de un tipo de registro, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registros](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


## Descripción general de los tipos de registros centralizados

Los tipos de registros centralizados se pueden agregar a varios espacios de trabajo desde un espacio de trabajo central o principal en Workfront Planning.

Al implementar Workfront Planning para una organización de varios equipos con flujos de trabajo comunes, es posible que necesite definir una estructura y metadatos coherentes para los tipos de registro clave (como Campañas o Entregables) que se pueden agregar a los espacios de trabajo de cada equipo para capturar y administrar su trabajo.

Además, es posible que necesite el trabajo de cada equipo para llegar a un nivel central.

En un flujo de trabajo de este tipo, puede asegurarse de que los equipos capturan su trabajo de forma coherente y, al mismo tiempo, desbloquean la visibilidad entre equipos, sin necesidad de agregar todo a un espacio de trabajo o a todos los miembros de la organización en cada uno de ellos. Puede utilizar tipos de registros centralizados para conseguirlo.

Para utilizar tipos de registros centralizados, haga lo siguiente:

1. Configure un tipo de registro para que esté centralizado en un espacio de trabajo específico.

   Un administrador de espacio de trabajo puede otorgar permisos a usuarios con una licencia Standard o a equipos, grupos, funciones y empresas para agregar un tipo de registro elegido a un espacio de trabajo que administren.

   El tipo de registro original existirá en su espacio de trabajo original, pero será visible en otros espacios de trabajo.

   Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Agregue un tipo de registro a un espacio de trabajo secundario desde uno existente que se haya configurado como tipo de registro centralizado.

   El tipo de registro existe en los siguientes espacios de trabajo:

   * Su espacio de trabajo original, donde se designó como tipo de registro centralizado.
   * Un espacio de trabajo secundario.

   Para obtener más información, vea [Agregar tipos de registros existentes desde otro área de trabajo](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   Las secciones siguientes describen consideraciones sobre los tipos de registros centralizados y cómo funcionan en sus espacios de trabajo originales o secundarios.

### Consideraciones sobre los tipos de registros centralizados en su espacio de trabajo original

El tipo de registro configurado para ser centralizado tiene las siguientes propiedades:

* Toda su información (aspecto, campos originales) solo se puede editar en el espacio de trabajo original.

* Puede realizar las siguientes acciones en el tipo de registro centralizado desde el espacio de trabajo original de un tipo de registro centralizado:

   * Edítela

     La edición de un tipo de registro centralizado incluye la edición de su aspecto, las funciones entre espacios de trabajo y todos los campos creados en el espacio de trabajo original.
   * Creación de formularios de solicitud
   * Administrar formularios de solicitud

* Sólo se puede eliminar un tipo de registro centralizado si no se ha agregado a un espacio de trabajo secundario. Una vez añadido a otro espacio de trabajo, al intentar eliminarlo del espacio de trabajo original se genera un error.

  Esto se hace para que el tipo de registro centralizado pueda permanecer en los espacios de trabajo donde ya se ha agregado.
* Los registros que agregue a un tipo de registro centralizado solo serán visibles para los usuarios que tengan permisos de visualización en el espacio de trabajo en el que se agregaron.
* Los registros que agregue desde un espacio de trabajo secundario se acumulan y se muestran en el espacio de trabajo original. Todos los miembros del espacio de trabajo original obtienen permisos de visualización para ellos.

* Los tipos de registro conectados de un tipo de registro centralizado estarán disponibles para la conexión desde los espacios de trabajo en los que se agregue este tipo de registro.

  Por ejemplo, si tiene un tipo de registro de campaña que tiene una conexión con el tipo de registro Regiones y agrega el tipo de registro Campaña a un espacio de trabajo secundario, las Regiones se podrán conectar entre espacios de trabajo para el espacio de trabajo secundario. Los miembros del espacio de trabajo secundario ahora pueden crear campañas y vincularlas a regiones.

* Los campos creados para un tipo de registro centralizado desde el espacio de trabajo original son visibles desde todos los espacios de trabajo en los que se ha añadido el tipo de registro. La configuración de campo de un espacio de trabajo original es de sólo lectura en los espacios de trabajo secundarios.

### Consideraciones sobre los tipos de registros centralizados después de agregarlos a un espacio de trabajo secundario

* Los colaboradores secundarios del espacio de trabajo obtienen permiso de contribución para el tipo de registro centralizado en el espacio de trabajo de su equipo. Pueden agregar y administrar registros desde el espacio de trabajo secundario.

* Los visualizadores de espacio de trabajo secundario obtienen permiso de visualización para el tipo de registro centralizado en el espacio de trabajo de su equipo. No pueden agregar ni administrar registros en él.

* Los gestores de espacio de trabajo secundario pueden realizar las siguientes acciones adicionales en el tipo de registro añadido desde un tipo de registro centralizado en un espacio de trabajo secundario:

   * Elimínelo.

     Al eliminar el tipo de registro de un espacio de trabajo secundario, solo se elimina de este. Los registros que se le agregan del espacio de trabajo secundario también se eliminan. Esto no elimina el tipo de registro de su espacio de trabajo original ni de ningún otro espacio de trabajo secundario donde se haya agregado.

  <!--These two capabilities will come later:
    * Add new fields
        Fields added to a centralized record from a secondary workspace are visible only from the secondary workspace. 
    * Share it-->

* Ningún usuario puede realizar las siguientes acciones en el tipo de registro añadido desde un tipo de registro centralizado en un espacio de trabajo secundario:

   * Edítela

     No se puede editar su aspecto, sus funciones entre espacios de trabajo ni los campos añadidos desde el espacio de trabajo original.
   * Creación y administración de formularios de solicitud
   * Creación y administración de automatizaciones

* Los registros añadidos en espacios de trabajo secundarios son visibles desde los siguientes espacios de trabajo, solo si tiene permisos de Vista o superiores en estos espacios de trabajo:

   * Espacio de trabajo secundario donde se agregan.
   * Espacio de trabajo original del tipo de registro centralizado.
   * Todos los demás espacios de trabajo en los que se haya añadido el espacio de trabajo centralizado.

* Los siguientes escenarios existen para registros creados en espacios de trabajo secundarios:

   * Si tiene permisos de Administración en el espacio de trabajo original y no tiene permisos en espacios de trabajo secundarios, puede ver los registros agregados desde los espacios de trabajo secundarios en el espacio de trabajo original, pero no puede administrarlos desde el espacio de trabajo original.
   * Si tiene permisos de Administración en el espacio de trabajo secundario, puede administrar los registros en el espacio de trabajo original del tipo de registro centralizado o desde el espacio de trabajo en el que se agregaron.
   * Puede ver los registros en espacios de trabajo secundarios adicionales en los que el tipo de registro centralizado se agrega solo si tiene permisos de vista en dichos espacios de trabajo.

### Acceso a las conexiones de un tipo de registro centralizado

Los tipos de registro conectados al tipo de registro centralizado en el espacio de trabajo original se hacen visibles desde otros espacios de trabajo donde se agrega el tipo de registro centralizado.

### Acceso a la API de un tipo de registro centralizado

Al agregar registros a un tipo de registro centralizado desde un espacio de trabajo secundario mediante la API de Workfront Planning, el sistema comprueba si el usuario tiene acceso para crear registros en el espacio de trabajo original del tipo de registro centralizado.

Se dan los siguientes casos:

* Si el usuario tiene acceso, el registro se crea en el espacio de trabajo original de los tipos de registro centralizados.

* Si el usuario no tiene acceso, recibe el error de que no tiene acceso al espacio de trabajo original del tipo de registro centralizado y debe proporcionar el ID del espacio de trabajo donde tiene acceso para crear registros.

## Información general sobre los tipos de registros conectables

Puede conectarse a un tipo de registro que se haya definido como conectable desde cualquier espacio de trabajo que administre.

Es posible que sus equipos necesiten registros vinculados a tipos de registros de otros espacios de trabajo o ver información capturada en registros que pertenecen a registros de otros espacios de trabajo. Puede conseguir esta configuración designando un tipo de registro como conectable.

Para utilizar tipos de registros conectables, haga lo siguiente:

1. Configure un tipo de registro para que se pueda conectar en un espacio de trabajo específico.

   Un gestor de espacio de trabajo puede seleccionar los espacios de trabajo a los que está disponible un tipo de registro designado para conectarse desde otros espacios de trabajo.

   El tipo de registro original existirá en su espacio de trabajo original y se agregará como un tipo de registro conectado a otro espacio de trabajo.

   Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Conéctese a un tipo de registro designado como conectable desde otro espacio de trabajo que administre.

   Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
