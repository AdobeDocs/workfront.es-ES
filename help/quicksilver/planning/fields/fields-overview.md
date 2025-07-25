---
title: Información general de campo
description: Añada nuevos campos en Adobe Workfront Planning que reflejen el ciclo de vida de la organización. Los campos son atributos de tipos de registro.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 79%

---


# Información general sobre campos

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Añada nuevos campos en Adobe Workfront Planning que reflejen el ciclo de vida de la organización. Los campos son atributos de tipos de registro.


## Consideraciones sobre los campos de Adobe Workfront Planning

* Solo puede crear campos desde la vista de tabla de una página de tipo de registro. Los campos se muestran como columnas en la vista de tabla. Todos los campos asociados a un tipo de registro también se muestran en la página de registro.

  Para obtener más información acerca de cómo administrar columnas de tabla (o campos de registro), vea [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

  Para obtener más información sobre la administración de campos, consulte también los siguientes artículos:

   * [Editar configuración de campo](/help/quicksilver/planning/fields/edit-fields.md)
   * [Eliminación de campos](/help/quicksilver/planning/fields/delete-fields.md)

* Los campos asociados a un tipo de registro están disponibles para asociarse a todos los registros de ese tipo. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Los campos asociados a un tipo de registro no se pueden añadir a otro tipo de registro. <!-- this will change when they open the Field library tab when creating a field-->

* Puede crear campos manual o automáticamente de las siguientes maneras:

   * Manualmente:

      * Cuando se agregan columnas en la vista de tabla de una página de tipo de registro. Las columnas de la tabla son los campos asociados al tipo de registro. Son los mismos campos que se muestran en una página de registro.

        No puede crear campos desde la página del registro.

      * Al conectar tipos de registros. Puede crear campos de registro vinculados al añadir una nueva conexión entre dos tipos de registro o un tipo de registro y un tipo de objeto de otras aplicaciones.

        Para obtener más información acerca de cómo conectar tipos de registros, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

      * Al importar campos existentes desde Workfront.

        Para obtener más información, consulte [Importar campos de Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md).


   * Automáticamente:

      * Al crear un tipo de registro:

         * Nombre
         * Descripción
         * Fecha de inicio
         * Fecha de finalización
         * Estado. Los valores predeterminados para los estados de registro son:
            * Desarrollo
            * Planificados
            * Activo
            * Finalizado
            * En espera

        Puede añadir más valores o cambiar el nombre de los existentes.

      * Cuando se crea un espacio de trabajo a partir de una plantilla.

        Para obtener más información, consulte [Crear espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Al importar tipos de registros mediante un archivo CSV o de Excel.

        Para obtener más información, vea [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

* No se puede acceder a los campos de Workfront Planning desde Workfront.

* Los campos de Workfront solo son accesibles desde Workfront Planning cuando se conectan tipos de registro con tipos de objetos de Workfront y se añaden campos vinculados o de búsqueda desde objetos de Workfront. Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

* Puede ver y actualizar la configuración de los campos que ha creado usted o cualquier otro usuario, si tiene permisos de administración en el espacio de trabajo y el tipo de registro al que pertenece el campo.

* Puede tener hasta 500 campos para un tipo de registro.

* Los nombres de campo pueden tener hasta 250 caracteres.

* Al eliminar un tipo de registro o espacio de trabajo, todos los campos asociados a ellos y los valores de los campos también se eliminan y no se pueden recuperar. <!-- this might change with a possible recycle bin solution?!-->
