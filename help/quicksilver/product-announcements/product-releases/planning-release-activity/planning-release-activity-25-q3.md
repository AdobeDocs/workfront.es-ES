---
content-type: release-notes
title: Actividad de la versión del tercer trimestre de 2025 para Adobe Workfront Planning
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el tercer trimestre de 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 6761f5af-2501-4487-8114-2751f1e4fe69
source-git-commit: 686db6004d1a64279080ab3ba311c172a6a24d1f
workflow-type: tm+mt
source-wordcount: '1308'
ht-degree: 3%

---

# Actividad de la versión del tercer trimestre de 2025 para Adobe Workfront Planning

Este artículo describe las funciones que se lanzarán para Workfront Planning durante la versión del tercer trimestre de 2025.

<!--keep the sentence below for all future quarterly release pages-->

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Filtros, columnas y campos adicionales añadidos a la pestaña Planificación en el área Solicitudes

>[!NOTE]
>
>* Vista previa: viernes, 29 de mayo de 2025
>* Versión rápida de producción: 12 de junio de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Hemos agregado la siguiente funcionalidad a una lista de solicitudes en la pestaña Planificación del área Solicitudes:

* Introducido por columna para indicar la persona que agregó una solicitud
* Filtra para limitar el número de solicitudes que ve en la pestaña Planificación. Puede filtrar la lista por los siguientes elementos:

   * la Workspace desde la que se originó el formulario de solicitud
   * el tipo de registro asociado al formulario de solicitud
   * la fecha de entrada de la solicitud
   * el nombre del formulario de solicitud
   * el estado de las solicitudes
   * el nombre de la persona que introdujo la solicitud.

* Control Columns para ver u ocultar campos (o columnas) en la lista de solicitudes de Planning.

Para obtener más información, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Nueva experiencia al desglosar registros en modo compacto en la vista de cronología

>[!NOTE]
>
>* Vista previa: viernes, 22 de mayo de 2025
>* Versión rápida de producción: 12 de junio de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Hemos cambiado la experiencia al desglosar registros en la vista de cronología y se le ha aplicado la vista Compacta.
Con la nueva actualización, cuando se definen los objetos de desglose mientras se muestra la línea de tiempo en el modo Compacto, se le pedirá que cambie la vista a Estándar una vez que haya terminado de configurar las condiciones de desglose.

Antes de esta mejora, no era posible definir las condiciones de desglose al mostrar la vista de la línea de tiempo en el modo compacto.

Con esta actualización, la opción Estándar es la predeterminada. Antes de esto, el modo compacto era el predeterminado.

Para obtener más información, consulte [Administrar la vista de línea de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Actualice la configuración de la vista de escala de tiempo para definir el aspecto de las barras de los registros conectados al utilizar la opción Desglose

>[!NOTE]
>
>* Vista previa: viernes, 15 de mayo de 2025
>* Versión rápida de producción: 12 de junio de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Ahora puede dar formato al aspecto de las barras de registro en la vista de escala de tiempo para los registros del desglose. Puede actualizar la siguiente configuración para las barras de estos registros:

* Estilo de barra
* Color

Antes de esta mejora, sólo se podía dar formato a las barras de los registros principales tal como se mostraban en la vista de escala de tiempo, y no se podía dar formato a las barras de los registros conectados.\
 
Para obtener más información, vea [Administrar la vista de escala de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).  

## Exportar la vista de tabla a un archivo CSV o de Excel 

>[!NOTE]
>
>* Vista previa: viernes, 15 de mayo de 2025
>* Versión rápida de producción: 12 de junio de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Se ha añadido una nueva funcionalidad a Workfront Planning, donde puede exportar información visible en la vista de tabla a un archivo CSV o de Excel.  

Tenga en cuenta lo siguiente al exportar información desde la vista de tabla:  

* La información exportada tiene en cuenta los filtros, agrupaciones y ordenaciones aplicados a la vista de tabla en Workfront Planning.
* El archivo exportado no admite miniaturas ni colores de fila personalizados.  
* Solo se exportan los campos que se hacen visibles en la interfaz de Workfront. Los campos ocultos no se exportan.  

Para obtener más información, vea [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md). 

## Los campos conectados de Workfront Planning ahora se admiten al importar registros mediante un archivo CSV o de Excel

>[!NOTE]
>
>* Vista previa: viernes, 15 de mayo de 2025
>* Versión rápida de producción: 12 de junio de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Ahora puede rellenar los valores de los campos conectados al agregar registros a un tipo de registro mediante un archivo CSV o de Excel.  Solo se admiten los campos de registro de Planning conectados. No se admiten campos que muestren conexiones con otras aplicaciones.

Este cambio se admite al importar un archivo CSV y de Excel para crear un tipo de registro y registros para un tipo de registro existente.

Antes de esta mejora, los campos de conexión no se podían rellenar al importar registros.

Para obtener más información, consulte los siguientes artículos:

* [Cree registros importando información desde un archivo CSV o de Excel](/help/quicksilver/planning/records/import-file-to-create-records.md).

* [Cree tipos de registros importando información desde un archivo CSV o de Excel](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

## Edición en línea en la página Registros conectados de un registro

>[!NOTE]
>
>* Vista previa: 30 de abril de 2025
>* Versión rápida de producción: 15 de mayo de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Ahora puede editar registros en la página Registros conectados de un registro. Con esta actualización, hemos introducido lo siguiente:

* El nombre de la página se ha cambiado de &quot;Vista de conexión&quot; a &quot;Página de registros conectados&quot;.
* Los registros conectados que se muestran en esta página se pueden editar en línea en la vista de tabla. Los objetos de Workfront conectados siguen apareciendo en una tabla de solo lectura.

Antes de esta mejora, la tabla de la página Vista de conexión era de solo lectura para las conexiones de registro.

Para obtener más información, vea [Administrar el diseño de la página de registros](/help/quicksilver/planning/records/manage-the-record-page.md).

## Área de planificación visible de forma predeterminada en el menú principal para usuarios con licencia estándar

>[!NOTE]
>
>* Vista previa: 30 de abril de 2025
>* Versión rápida de producción: 15 de mayo de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Los usuarios de Standard y System Administrator ahora pueden encontrar el área de Planning en el menú principal de forma predeterminada, sin que se les asigne una plantilla de diseño que la incluya. Todos los demás usuarios deben tener una plantilla de diseño que incluya el área de Planning asignada para acceder a ella.

Antes de esta mejora, los usuarios con todos los niveles de licencia debían asignarse a una plantilla de diseño modificada para incluir el área de planificación en el menú principal para acceder a esta área.

>[!NOTE]
>
>Este cambio será visible para todos los usuarios nuevos y existentes con una licencia de administrador del sistema y estándar.
>&#x200B;>Los usuarios existentes asignados a una plantilla de diseño seguirán viendo todo según la configuración definida en la plantilla.

Para obtener más información, consulte [Descripción general de Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

## Formato de color de nivel de fila en la vista de tabla

>[!NOTE]
>
>* Vista previa: 30 de abril de 2025
>* Versión rápida de producción: 15 de mayo de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Para obtener una mejor visibilidad de la información importante de sus registros, hemos introducido el formato de color de nivel de fila para la vista de tabla. Ahora puede elegir un color para cada fila después de definir las condiciones para cada opción.  Esta es una nueva capacidad que no existía antes de esta actualización.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

## Nueva configuración para truncar los nombres de registros largos en la vista de escala de tiempo estándar

>[!NOTE]
>
>* Vista previa: 23 de abril de 2025
>* Versión rápida de producción: 15 de mayo de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Ahora puede habilitar una configuración en la ficha Estilo de barra del cuadro Configuración de una vista de escala de tiempo para truncar nombres de registro más largos al mostrarlos en la vista Estándar. La configuración está deshabilitada de forma predeterminada y solo se puede habilitar cuando se muestra la vista de cronología en el modo Estándar. Como esta opción está deshabilitada, la información de las barras de registros se muestra expandida de forma predeterminada. Antes de esta mejora, la información de las barras de registro se truncaba de forma predeterminada.

Para obtener más información, consulte [Administrar la vista de línea de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Permisos de uso compartido para tipos de registros


>[!NOTE]
>
>* Vista previa: 17 de abril de 2025
>* Versión rápida de producción: 12 de junio de 2025
>* Producción para todos los clientes: viernes, 17 de julio de 2025

Para controlar mejor quién puede ver o administrar registros en cada tipo de registro y garantizar que solo las personas autorizadas puedan administrar la información de cada tipo de registro en función de sus funciones y responsabilidades, hemos introducido permisos en el nivel de tipo de registro.

Antes de esta mejora, sólo se podían compartir espacios de trabajo con otros usuarios y el permiso que se les otorgaba se podía aplicar a todos los tipos de registros del espacio de trabajo.

Hemos introducido las siguientes actualizaciones:

* Los permisos de Workspace se comparten automáticamente con todos los tipos de registros del espacio de trabajo.
* El nivel de permisos otorgados para el espacio de trabajo se muestra como Permisos heredados para el tipo de registro.
* No se puede compartir un tipo de registro con un nivel de permisos superior al que tienen los usuarios en el espacio de trabajo.
* Puede deshabilitar los permisos heredados en el tipo de registro para que sea de solo lectura para todas las personas del espacio de trabajo. A continuación, puede agregar personas, equipos, grupos, empresas o roles individuales y concederles permiso para contribuir al tipo de registro.

Para obtener más información, vea [Compartir tipos de registros](/help/quicksilver/planning/access/share-record-types.md).


