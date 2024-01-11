---
title: Resumen de campo
description: Puede agregar nuevos campos en Adobe Maestro que reflejen el ciclo de vida de su organización. Los campos son atributos de tipos de registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

---

# Resumen de campo

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Debe ser cliente de Workfront para utilizar las funciones de Maestro.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede agregar nuevos campos en Adobe Maestro que reflejen el ciclo de vida de su organización. Los campos son atributos de tipos de registro.


## Consideraciones sobre los campos de Maestro

* Sólo puede crear campos desde la vista de tabla de una página de tipo de registro. Los campos se muestran como columnas en la vista de tabla. Todos los campos asociados a un tipo de registro también se muestran en la página Detalles de cada registro de ese tipo.

  Para obtener información sobre la administración de columnas de tabla (o campos de registro), consulte [Administrar la vista de tabla](../views/manage-the-table-view.md).

  Para obtener información sobre la administración de campos, consulte los siguientes artículos:

   * [Editar campos](../fields/edit-fields.md)
   * [Eliminar campos](../fields/delete-fields.md)

* Los campos asociados a un tipo de registro están disponibles para asociarse a todos los registros de ese tipo. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Los campos asociados a un tipo de registro no se pueden agregar a otro tipo de registro. <!-- this will change when they open the Field library tab when creating a field-->

* Puede crear campos manual o automáticamente de las siguientes maneras:

   * Manualmente:

      * Agregando columnas en la vista de tabla de una página de tipo de registro. Las columnas de la tabla son los campos asociados al tipo de registro. Son los mismos campos que se muestran en la página Detalles de un registro.

        No se pueden crear campos desde la página Detalles de un registro.

        Este artículo describe cómo crear campos manualmente.

      * Conectando tipos de registros. Puede crear campos de registro vinculados cuando agregue una nueva conexión entre dos tipos de registro Maestro o un tipo de registro y un tipo de objeto de otras aplicaciones.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Para obtener más información acerca de cómo conectar tipos de registros de Maestro, vea [Conectar tipos de registros](../architecture/connect-record-types.md).

      * Mediante la importación de tipos de registros mediante un archivo CSV o de Excel. Para obtener más información, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

   * Automáticamente:

      * De forma predeterminada, cada vez que crea un tipo de registro.

        Los siguientes son campos estándar creados por defecto para cada nuevo tipo de registro operativo:

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

           Puede agregar más valores o cambiar el nombre de los existentes.

        A continuación se muestran los campos estándar creados de forma predeterminada para cada nuevo tipo de registro de taxonomía:

         * Nombre <!--will more be added? If not, consider rephrasing this bullet-->

      * Cuando se crea un espacio de trabajo a partir de una plantilla. Maestro crea campos para tipos de registros operativos y taxonomías cuando se crea un espacio de trabajo a partir de una plantilla. Para obtener más información, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).

* No se puede acceder a los campos Maestro desde Workfront.

* Los campos de Workfront sólo son accesibles desde Maestro cuando conecta los tipos de registro de Maestro con los tipos de objetos de Workfront y agrega campos vinculados o de búsqueda desde objetos de Workfront. Para obtener más información, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).

* Puede ver y actualizar la configuración de los campos que ha creado usted o cualquier otro usuario si tiene permisos de administración en el espacio de trabajo al que pertenece el campo.

* Puede tener hasta 500 campos para un tipo de registro.

* Los nombres de campo pueden tener hasta 250 caracteres.

* Al eliminar un tipo de registro operativo, taxonomía o espacio de trabajo, todos los campos asociados a ellos y los valores de los campos también se eliminan y no se pueden recuperar. <!-- this might change with a possible recycle bin solution?!-->
