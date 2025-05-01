---
title: Información general sobre registros conectados
description: Después de crear conexiones entre tipos de registros, puede conectar registros individuales entre sí. En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Adobe Systems Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 6e2e337969fccba88ea7089fe9a6d9db605343f7
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 26%

---

# Información general sobre registros conectados

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en la entorno de Vista previa para todos los clientes. Después de los lanzamientos mensuales para Producción, las mismas características también están disponibles en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información acerca de las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Puede conectar registros de Adobe Workfront Planning entre sí o a objetos de otras aplicaciones.

En este artículo se describen las consideraciones que debe tener en cuenta al conectar registros en Adobe Systems Workfront Planning.

Para obtener información acerca de cómo puede conectar registros entre sí o con otro objeto, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).


## Consideraciones sobre la conexión de registros

* Después de conectar los tipos de registros, los tipos de registros conectados se muestran como campos de registro vinculados en la tabla de los tipos de registro desde los que están vinculados y en las páginas de los registros.
* Puede examinar y añadir registros y objetos de los tipos de registro y objeto vinculados desde los campos de registro vinculados.
* Puede añadir campos (campos de búsqueda) de los tipos de registro vinculados en la tabla del tipo de registro desde el que está vinculando.

  Además, puede agregar campos (campos de búsqueda) de los tipos de registro desde los que está vinculando en la tabla del tipo de registro al que está vinculando.

  Por ejemplo, si vincular el tipo de registro de Producto del tipo de registro de Campaign, puede mostrar los campos de producto para las campañas, así como campaña campos para los productos.
* No puede actualizar manualmente los valores de los campos de búsqueda en los registros desde los que está vinculando.

  Los valores de los campos de búsqueda rellenan automáticamente el registro de Workfront Planning desde el que se vincula después de actualizarse en el registro u objeto original.

* Todas las personas con acceso a Workfront Planning and Ver o permisos superiores para el espacio de trabajo <span class="preview">y un tipo</span>  de registro pueden ver las conexiones que realiza entre registros o entre registros y objetos de otras aplicaciones. Pueden ver los registros y objetos conectados independientemente de sus permisos en las aplicaciones a las que se conecta.
* Puede vista y editar las conexiones de todos los demás, si tiene permisos de administración para el espacio de trabajo <span class="preview">y el tipo</span>  de registro donde están los registros conectados.
* Puede conectar un registro a uno o varios objetos de otro aplicación., dependiendo del tipo de conexión que seleccionó al conectar los tipos de registro. Para obtener más información, consulte la sección &quot;Tipos de conexiones&quot; en el artículo [Información general](/help/quicksilver/planning/architecture/connect-record-types-overview.md) sobre los tipos de registros conectados.

## Áreas donde puede conectar registros

Puede conectar registros a otros registros o a objetos de otra aplicación en las siguientes áreas:

* Puede conectar registros de planificación de Workfront a objetos de Workfront o Experience Manager objetos de Assets en las siguientes áreas de un registro de planificación:

   * Los campos de registro conectados en la tabla vista de un tipo de registro en Planificación.
   * El registro se previsualización o Página en los campos de registro conectados del pestaña Detalles.
   * El registro se previsualización o Página en el pestaña de conexiones.
   * El Página del registro en un <span class="preview">registro conectado Página</span> pestaña de un registro conectado.

* Puede conectar objetos de Workfront a registros de planificación de Workfront en las siguientes áreas de Workfront:

   * Sección Planificación de un objeto Workfront.
   * Campo de conexión de planificación en un formulario personalizado de un objeto Workfront.

  Para obtener información, consulte [Administrar conexiones de registro desde objetos](/help/quicksilver/planning/records/manage-records-in-planning-section.md) de Workfront.
