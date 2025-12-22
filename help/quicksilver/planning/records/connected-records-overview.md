---
title: Información general de registros conectados
description: Después de crear conexiones entre tipos de registros, puede conectar registros individuales entre sí. En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 24%

---

# Resumen de registros conectados

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>  -->

{{planning-important-intro}}

Puede conectar registros de Adobe Workfront Planning entre sí o a objetos de otras aplicaciones.

En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Adobe Workfront Planning.

Para obtener información sobre cómo conectar registros entre sí o con otro objeto, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).


## Consideraciones sobre la conexión de registros

* Después de conectar los tipos de registros, los tipos de registros conectados se muestran como campos de registro vinculados en la tabla de los tipos de registro desde los que están vinculados y en las páginas de los registros.
* Puede examinar y añadir registros y objetos de los tipos de registro y objeto vinculados desde los campos de registro vinculados.
* Puede añadir campos (campos de búsqueda) de los tipos de registro vinculados en la tabla del tipo de registro desde el que está vinculando.

  Además, puede agregar campos (campos de búsqueda) de los tipos de registro desde los que está vinculando en la tabla del tipo de registro al que está vinculando.

  Por ejemplo, si vincula el tipo de registro de Producto desde el tipo de registro de Campaña, puede mostrar campos de producto para campañas, así como campos de campaña para productos.
* No puede actualizar manualmente los valores de los campos de búsqueda en los registros desde los que está vinculando.

  Los valores de los campos de búsqueda rellenan el registro de Workfront Planning desde el que está vinculando automáticamente después de que se hayan actualizado en el registro u objeto original.

* Todas las personas con acceso a Workfront Planning y View o permisos superiores en el espacio de trabajo y un tipo de registro pueden ver las conexiones que se realizan entre registros o entre registros y objetos de otras aplicaciones. Pueden ver los registros y objetos conectados independientemente de sus permisos en las aplicaciones a las que se conecta.
* Puede ver y editar las conexiones de todos los demás, si tiene permisos de Administración en el espacio de trabajo y el tipo de registro donde se encuentran los registros conectados.
* Se puede conectar un registro a uno o varios objetos desde otra aplicación, según el tipo de conexión seleccionado al conectar los tipos de registro. Para obtener más información, consulte la sección &quot;Tipos de conexiones&quot; en el artículo [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
  <!--* <span class="preview">If connected record types are part of hierarchies, you can access any object type within the hierarchy from the records' pages. For information, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md). </span>-->

## Áreas donde se pueden conectar registros

Puede conectar registros a otros registros o a objetos de otra aplicación en las áreas siguientes:

* Puede conectar registros de Workfront Planning a objetos de Workfront, objetos de Experience Manager Assets o marcas de GenStudio en las siguientes áreas de un registro de Planning:

   * Los campos de registro conectados en la vista de tabla de un tipo de registro en Planning.
   * La vista previa o la página de detalles del registro en los campos de registro conectados de la pestaña Detalles.
   * La página de vista previa o de detalles del registro en la ficha Conexiones.
   * La página del registro en la ficha Página de registros conectados de un registro conectado.

* Puede conectar objetos de Workfront a registros de Workfront Planning en las siguientes áreas de Workfront:

   * La sección Planificación de un objeto de Workfront.
   * Campo de conexión de Planning en el formulario personalizado de un objeto Workfront.

  Para obtener más información, consulte [Administrar conexiones de registro desde objetos de Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
