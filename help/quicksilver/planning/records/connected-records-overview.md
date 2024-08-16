---
title: Información general de registros conectados
description: Después de crear conexiones entre tipos de registros, puede conectar registros individuales entre sí. En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d56a4721353f8b7db856eab5a3ae3b53396bd079
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


<!--update metadata at GA-->

# Resumen de registros conectados

{{planning-important-intro}}

Puede conectar registros de Adobe Workfront Planning entre sí o a objetos de otras aplicaciones.

En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Adobe Workfront Planning.

Para obtener información sobre cómo conectar registros entre sí o con otro objeto, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).


## Consideraciones sobre la conexión de registros

* Después de conectar los tipos de registros, los tipos de registros conectados se muestran como campos de registro vinculados en la tabla de los tipos de registros desde los que están vinculados y en las páginas de los registros.
* Puede examinar y agregar registros y objetos de los tipos de registro y objeto vinculados desde los campos de registro vinculados.
* Puede agregar campos (campos de búsqueda) de los tipos de registro vinculados en la tabla del tipo de registro desde el que está vinculando.

  Puede agregar campos (campos de búsqueda) de los tipos de registro desde los que está vinculando en la tabla del tipo de registro al que está vinculando.

  Por ejemplo, si vincula el tipo de registro de Producto desde el tipo de registro de Campaña, puede mostrar campos de Producto para campañas, así como campos de Campaña para Productos.
* No puede actualizar manualmente los valores de los campos de búsqueda en los registros desde los que está vinculando.

  Los valores de los campos de búsqueda rellenan el registro de Workfront Planning desde el que está vinculando automáticamente después de que se hayan actualizado en el registro u objeto original.

* Todas las personas con acceso a Workfront Planning y View o permisos superiores en el espacio de trabajo pueden ver las conexiones que se realizan entre registros o entre registros y objetos de otras aplicaciones. Pueden ver los registros y objetos conectados independientemente de sus permisos en las aplicaciones a las que se conecta.
* Puede ver y editar las conexiones de todos los demás, si tiene permisos de Administración en el espacio de trabajo donde se encuentran los registros conectados.
* Puede conectar un registro a uno o varios objetos desde otra aplicación. <!--For more information, see the "Connections types" section in the article [Connected record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md). -->

## Áreas donde se pueden conectar registros

Puede conectar registros a otros registros o a objetos de otra aplicación en las áreas siguientes:

* Puede conectar registros de Workfront Planning a objetos de Workfront en las siguientes áreas:
   * Desde un registro de Planning en Workfront Planning en los campos conectados en la vista de tabla.
   * Desde un registro de Planning en Workfront Planning en la vista previa del registro o página en los campos de registro conectados.
  <!--
  * From a Planning record in Workfront Planning in the record preview or page in the connected record fields on the Details tab.
  * From a Planning record in the record's preview or page on the Connections tab.  -->

* Puede conectar los registros de Workfront Planning a Experience Manager Assets en las siguientes áreas:

   * Desde un registro de Planning en Workfront Planning en la vista de tabla.
  <!--* From a Planning record in the Connections tab on the record's preview or page.  -->

* Puede conectar objetos de Workfront a registros de Workfront Planning en las siguientes áreas:

   * Desde la sección Planificación de un objeto de Workfront.

