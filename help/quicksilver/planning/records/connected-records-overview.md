---
title: Información general de registros conectados
description: Después de crear conexiones entre tipos de registros, puede conectar registros individuales entre sí. En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 11d856aeee3bd9edcdc1dbca3964f37bdf83bd00
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 13%

---

# Resumen de registros conectados

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

Puede conectar registros de Adobe Workfront Planning entre sí o a objetos de otras aplicaciones.

En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Workfront Planning.

Para obtener información sobre cómo conectar registros entre sí o con otro objeto, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Requisitos previos

Debe conectar lo siguiente para poder conectar registros en Workfront Planning:

* Dos tipos de registro
* Un tipo de registro con un objeto de otra aplicación

Para obtener más información, vea [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).


## Consideraciones sobre la conexión de registros

* Después de conectar tipos de registro, los tipos de registro conectados se muestran como campos de conexión en la tabla de los tipos de registro desde los que están vinculados y en las páginas de los registros.
* Puede examinar y añadir registros y objetos de los tipos de registro y objeto vinculados desde los campos de registro vinculados.
* Puede añadir campos (campos de búsqueda) de los tipos de registro vinculados en la tabla del tipo de registro desde el que está vinculando.

  Además, puede agregar campos (campos de búsqueda) de los tipos de registro desde los que está vinculando en la tabla del tipo de registro al que está vinculando.

  Por ejemplo, si vincula el tipo de registro de Producto desde el tipo de registro de Campaña, puede mostrar campos de producto para campañas, así como campos de campaña para productos.
* No puede actualizar manualmente los valores de los campos de búsqueda en los registros desde los que está vinculando.

  Los valores de los campos de búsqueda rellenan el registro de Workfront Planning desde el que está vinculando automáticamente después de que se hayan actualizado en el registro u objeto original.

* Todas las personas con acceso a Workfront Planning y View o permisos superiores en el espacio de trabajo y un tipo de registro pueden ver las conexiones que se realizan entre registros o entre registros y objetos de otras aplicaciones. Pueden ver los registros y objetos conectados independientemente de sus permisos en las aplicaciones a las que se conecta.
* Puede ver y editar las conexiones de todos los demás, si tiene permisos de Administración en el espacio de trabajo y el tipo de registro donde se encuentran los registros conectados.
* Se puede conectar un registro a uno o varios objetos desde otra aplicación, según el tipo de conexión seleccionado al conectar los tipos de registro. Para obtener más información, consulte la sección &quot;Tipos de conexiones&quot; en el artículo [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
* Cuando los tipos de registro conectados forman parte de jerarquías, se puede tener acceso a cualquier tipo de objeto dentro de la jerarquía desde las páginas de los registros. Para obtener más información, consulte [Información general sobre jerarquía y ruta de exploración](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).
* Cuando los tipos de registro conectados forman parte de jerarquías, puede conectar un registro de un tipo de registro secundario a un máximo de 10 registros de un tipo de registro principal. Para obtener más información, consulte [Información general sobre jerarquía y ruta de exploración](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Áreas donde se pueden conectar registros

Puede conectar registros manual o automáticamente en Workfront.

### Conexión manual de registros

Puede conectar manualmente registros a otros registros o a objetos de otra aplicación en las áreas siguientes:

* Puede conectar registros de Workfront Planning a objetos de Workfront, objetos de Experience Manager Assets o marcas de GenStudio en las siguientes áreas de un registro de Planning:

   * Los campos de registro conectados en la vista de tabla de un tipo de registro en Planning.
   * Los campos de registro conectados en la página de vista previa o detalles de un registro.
   * La página de vista previa o de detalles del registro en la página Registros conectados de un registro.

* Puede conectar objetos de Workfront a registros de Workfront Planning en las siguientes áreas de Workfront:

   * La sección Planificación de un objeto de Workfront.
   * Campo de conexión de Planning en el formulario personalizado de un objeto Workfront.

  Para obtener más información, consulte [Administrar conexiones de registro desde objetos de Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

### Conectar registros automáticamente

Después de conectar los tipos de registro entre sí o un tipo de registro a un tipo de objeto de otra aplicación, puede conectar automáticamente registros y objetos de las siguientes maneras:

* Uso de automatizaciones

  Puede crear registros u objetos de Workfront a partir de un registro de Planning en el que configure automatizaciones.

  Cuando se cumple una condición definida, se crea un registro o un objeto y se conecta automáticamente al registro desde el que se activa la automatización.

  Para obtener más información, consulte [Configuración de automatizaciones de Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

* Uso de formularios de solicitud para crear registros

  Puede crear registros al enviar una solicitud de Planning. La solicitud y el registro se conectan automáticamente.

  >[!NOTE]
  >
  >No se puede desconectar un registro de su solicitud original.

  Para obtener más información, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).
