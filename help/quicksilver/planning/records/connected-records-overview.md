---
title: Información general de registros conectados
description: Después de crear conexiones entre tipos de registros, puede conectar registros individuales entre sí. En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Resumen de registros conectados

<!--for the Planning connection field, see commented out below; also add preview tags-->

{{planning-important-intro}}

Puede conectar registros de Adobe Workfront Planning entre sí o a objetos de otras aplicaciones.

En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Adobe Workfront Planning.

Para obtener información sobre cómo conectar registros entre sí o con otro objeto, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).


## Consideraciones sobre la conexión de registros

* Después de conectar los tipos de registros, los tipos de registros conectados se muestran como campos de registro vinculados en la tabla de los tipos de registros desde los que están vinculados y en las páginas de los registros.
* Puede examinar y agregar registros y objetos de los tipos de registro y objeto vinculados desde los campos de registro vinculados.
* Puede agregar campos (campos de búsqueda) de los tipos de registro vinculados en la tabla del tipo de registro desde el que está vinculando.

  Además, puede agregar campos (campos de búsqueda) de los tipos de registro desde los que está vinculando en la tabla del tipo de registro al que está vinculando.

  Por ejemplo, si vincula el tipo de registro de Producto desde el tipo de registro de Campaña, puede mostrar campos de producto para campañas, así como campos de campaña para productos.
* No puede actualizar manualmente los valores de los campos de búsqueda en los registros desde los que está vinculando.

  Los valores de los campos de búsqueda rellenan el registro de Workfront Planning desde el que está vinculando automáticamente después de que se hayan actualizado en el registro u objeto original.

* Todas las personas con acceso a Workfront Planning y View o permisos superiores en el espacio de trabajo pueden ver las conexiones que se realizan entre registros o entre registros y objetos de otras aplicaciones. Pueden ver los registros y objetos conectados independientemente de sus permisos en las aplicaciones a las que se conecta.
* Puede ver y editar las conexiones de todos los demás, si tiene permisos de Administración en el espacio de trabajo donde se encuentran los registros conectados.
* Puede conectar un registro a uno o varios objetos desde otra aplicación. Para obtener más información, consulte la sección &quot;Tipos de conexiones&quot; en el artículo [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Áreas donde se pueden conectar registros

Puede conectar registros a otros registros o a objetos de otra aplicación en las áreas siguientes:

* Puede conectar registros de Workfront Planning a objetos de Workfront u objetos de Experience Manager Assets en las siguientes áreas de un registro de Planning:

   * Los campos de registro conectados en la vista de tabla de un tipo de registro en Planning.
   * Vista previa o página del registro en los campos de registro conectados de la pestaña Detalles.
   * La página o vista previa del registro en la ficha Conexiones.

* Puede conectar objetos de Workfront a registros de Workfront Planning en las siguientes áreas:

   * Desde la sección Planificación de un objeto de Workfront.
  <!--* From a Planning connection field on a Workfront object's custom form. -->

  Para obtener más información, consulte [Administrar conexiones de registro desde objetos de Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md)