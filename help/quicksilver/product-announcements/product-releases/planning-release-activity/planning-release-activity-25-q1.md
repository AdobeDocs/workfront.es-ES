---
content-type: release-notes
title: Actividad de la versión de Adobe Workfront Planning para la versión 25.1
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el primer trimestre de 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: a6104204cae2a2d8fb021da254437008d55a43b6
workflow-type: tm+mt
source-wordcount: '2112'
ht-degree: 4%

---

# Actividad de la versión del primer trimestre de 2025 para Adobe Workfront Planning

Este artículo describe las funciones que se lanzarán para Workfront Planning durante la versión del primer trimestre de 2025.

<!--keep the sentence below for all future quarterly release pages-->

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Los campos de conexión con recursos de Adobe Experience Manager ahora se admiten en los formularios de solicitud

>[!NOTE]
>
>Versión preliminar: sábado, 20 de diciembre de 2024; versión de producción para todos los clientes: viernes, 16 de enero de 2025

AEM Ahora puede agregar campos de conexión con recursos de la a un formulario de solicitud de tipo de registro en Workfront Planning.

Antes de esta mejora, estos tipos de campos no se podían agregar a los formularios de solicitud.

Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Configuración de aprobaciones para solicitudes de Workfront Planning

>[!NOTE]
>
>Versión preliminar: martes, 16 de diciembre de 2024; versión de producción para todos los clientes: viernes, 16 de enero de 2025

Ahora puede asociar una aprobación a un formulario de solicitud de Workfront Planning. Solo puede agregar usuarios como aprobadores de una solicitud. Una vez enviada la solicitud, se envía primero a todos los aprobadores para aprobarla antes de crear un registro.

Para obtener más información, consulte [Agregar una aprobación a un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).


## Notificaciones para el envío de solicitudes, aprobaciones y cambios de estado

>[!NOTE]
>
>Versión preliminar: martes, 16 de diciembre de 2024; versión de producción para todos los clientes: viernes, 16 de enero de 2025

Ahora recibirá una notificación en la aplicación y por correo electrónico de las siguientes acciones después de enviar una solicitud en Workfront Planning:

* Un solicitante recibe una notificación de que una solicitud se ha enviado correctamente

* Un solicitante recibe una notificación de que una solicitud se ha aprobado o rechazado

* Un aprobador recibe una notificación que le informa de que se le ha enviado una solicitud para su aprobación.

>[!NOTE]
>
>La instancia de Workfront de su organización debe incorporarse a la experiencia unificada de Adobe para que los usuarios puedan recibir notificaciones por correo electrónico y en la aplicación.

Para obtener información sobre el envío o la aprobación de solicitudes, consulte los siguientes artículos:

* [Envío de solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md)

* [Aprobar una solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md).

## Búsqueda inteligente al buscar un tipo de campo

>[!NOTE]
>
>Versión preliminar: viernes, 05 de diciembre de 2024; versión de producción para todos los clientes: viernes, 05 de diciembre de 2024

Se ha añadido la funcionalidad de búsqueda inteligente al buscar un tipo de campo en Workfront Planning. Ahora puede encontrar tipos de campo al escribir una palabra clave. Por ejemplo, si escribe &quot;Precio&quot;, encontrará los tipos de campo Número y Moneda. Antes de esta mejora, solo se podía buscar el nombre real del tipo de campo.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## Selector de color personalizado para opciones con códigos de color de campos de selección única o múltiple

>[!NOTE]
>
>Versión de vista previa: 5 de diciembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Ahora puede realizar opciones de color personalizadas al crear o editar un campo de selección única o múltiple. Cuando crea o edita campos con opciones con códigos de color, al hacer clic en el icono de color se abre un cuadro selector de color. Puede elegir entre colores predefinidos o crear colores personalizados mediante códigos hexadecimales o un espectro de colores.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## Importar campos de Workfront existentes a tipos de registros de Workfront Planning

>[!NOTE]
>
>Versión de vista previa: 27 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Ahora, al agregar campos a un tipo de registro, tiene la opción de importar los campos personalizados o nativos de Workfront existentes y asociarlos al tipo de registro seleccionado. La importación de campos existentes crea una copia de los campos de Workfront en Workfront Planning. Los campos copiados son independientes de sus versiones originales.

Antes de esta mejora, tenía que crear manualmente todos los campos y asociarlos a tipos de registros.

Los campos calculados no son compatibles en este momento.

Para obtener más información, consulte [Importar campos desde Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md)

## Crear tipos de registros, registros y campos importando un archivo CSV o de Excel

>[!NOTE]
>
>Versión de vista previa: 27 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Ahora puede importar nuevos tipos de registros importando un archivo CSV o de Excel.

Se importa la siguiente información:

* El nombre de la hoja o el archivo se importará como el nombre del tipo de registro.

* La primera fila de cada columna se importa como un nuevo campo. Puede tener hasta 500 campos en cada hoja importada.

* Cada fila se importa como un registro nuevo. Puede tener hasta 10 000 registros en cada hoja.

Para obtener más información, vea [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

## Evitar referencias circulares en fórmulas

>[!NOTE]
>
>Versión de vista previa: 27 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Hemos introducido un mensaje de advertencia al editar o crear un campo de fórmula que puede crear una referencia circular a sí mismo o a campos compartidos. No se puede guardar un campo de fórmula que haga referencia a sí mismo o a elementos a los que se hace referencia en su cálculo.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## Agregar páginas de vista Conexión a la página de un registro para mostrar los registros conectados en una vista de tabla

>[!NOTE]
>
>Versión de vista previa: 27 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Puede agregar páginas al área de detalles de un registro para mostrar los registros conectados en una vista de tabla. Puede agregar una página por cada registro conectado.

Las páginas agregadas son de solo lectura.

Para obtener más información, vea [Administrar el diseño de la página de registros](/help/quicksilver/planning/records/manage-the-record-page.md).

## Nuevas pestañas de Workfront y Planning en la sección Enviados del área de Solicitudes

>[!NOTE]
>
>Versión de vista previa: 27 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Ahora puede encontrar solicitudes de Workfront Planning en la sección Enviadas del área de Solicitudes de Workfront. La sección Enviado ahora muestra las siguientes pestañas:

* Workfront: Muestra las solicitudes enviadas en Workfront.
* Planificación: Muestra las solicitudes enviadas mediante un formulario de solicitud de Workfront Planning.

Debe utilizar un vínculo al formulario de solicitud para poder agregar solicitudes a un tipo de registro de Workfront Planning. El envío de una solicitud de planificación de Workfront desde el área de solicitudes de Workfront estará disponible en una fecha posterior.

Su organización debe adquirir un paquete de Workfront Planning antes de que la pestaña Planning esté disponible en el área Solicitudes.

Para obtener más información, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Ahora se admiten tipos de campo adicionales en los formularios de solicitud

>[!NOTE]
>
>Versión de vista previa: 27 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Ahora puede agregar los siguientes tipos de campo a un formulario de solicitud de tipo de registro en Workfront Planning:

* Personas
* Conexiones de Workfront

Antes de esta mejora, estos tipos de campos no se podían agregar a los formularios de solicitud en Workfront Planning.

Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Limitar el uso compartido público de formularios de solicitud que contienen determinados tipos de campo

>[!NOTE]
>
>Versión de vista previa: 27 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Ya no puede compartir un formulario de solicitud públicamente si el formulario contiene cualquiera de los siguientes tipos de campo:

* Fórmula
* Conexiones de Workfront y AEM Assets
* Campos de búsqueda
* Personas

Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


## Mostrar registros por semana en la vista de calendario

>[!NOTE]
>
>Versión de vista previa: 26 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Ahora puede mostrar los registros en la vista de calendario por semana. Antes de esta mejora, solo se podía mostrar la vista de calendario por mes.

Para obtener más información, vea [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Restauración de registros eliminados

>[!NOTE]
>
>Versión de vista previa: 22 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Una vez eliminados los registros, ahora se mueven temporalmente a un grupo eliminado recientemente durante 30 días. Puede acceder a la bandeja eliminada recientemente desde la página del tipo de registro y solo contiene registros de un tipo específico.

Los administradores de Workspace pueden restaurar registros de la papelera durante un máximo de 30 días después de eliminarlos. También se restauran los registros conectados y su información de campo.

Antes de esta mejora, los registros eliminados no se podían restaurar.

Para obtener más información, vea [Restaurar registros eliminados](/help/quicksilver/planning/records/records-information.md).

## Asistente de IA de Adobe disponible en las áreas de detalles de registro

>[!NOTE]
>
>Versión de vista previa: 21 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Para facilitar la realización de su trabajo, hemos agregado el Asistente de IA de Adobe a la vista previa de detalles de un registro o a la página del registro. Puede utilizar el Asistente de IA dentro de una página de registro para actualizar la información sobre el registro.

Para obtener más información, consulte [Descripción general del Asistente de IA de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

## Nueva experiencia al añadir una miniatura y una imagen de portada a una página de registro

>[!NOTE]
>
>Versión de vista previa: 20 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Cuando se abre la vista previa o la página de un registro y éste no tiene una miniatura o una imagen de portada, debe situarse sobre el área situada encima del nombre del registro en el encabezado para ver las opciones para agregar una portada y una imagen en miniatura al registro. Antes de esta mejora, las imágenes de marcador de posición vacías para la miniatura y la portada mostradas encima del nombre del registro.

Para obtener más información, consulte los siguientes artículos:

* [Añadir una imagen de portada a un registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [Añadir una imagen en miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

## Nuevos tipos de visualización para campos de tipo porcentual en la vista de tabla

>[!NOTE]
>
>Versión de vista previa: 7 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Para facilitar la lectura de los números en la vista de tabla, ahora puede seleccionar entre las siguientes opciones para cambiar el modo en que se muestra un campo de tipo Porcentaje en la vista de tabla:

* Número
* Barras
* Círculo

Este tipo de visualización solo es compatible con la vista de tabla.

Antes de esta mejora, los valores de porcentaje solo se podían mostrar como números.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## Los campos de conexión ahora son compatibles con los formularios de solicitud

>[!NOTE]
>
>Versión de vista previa: 31 de octubre de 2024; producción para versión rápida: con la versión 24.11 (14 de noviembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Ahora puede agregar campos conectados para registros de Workfront Planning a un formulario de solicitud de tipo de registro.

No se pueden agregar campos de búsqueda de conexión ni campos conectados para objetos Workfront en el formulario de solicitud.

Antes de esta mejora, estos tipos de campos no se podían agregar a los formularios de solicitud en Workfront Planning.

Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Advertencia de conexión al conectar registros que ya están vinculados a otros registros

>[!NOTE]
>
>Versión de vista previa: 31 de octubre de 2024; producción para versión rápida: con la versión 24.11 (14 de noviembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Cuando intenta conectar registros que ya están conectados en otra parte y que pertenecen a un tipo de registro conectado a través de un tipo de conexión Uno a varios o Uno a uno, ahora recibe una advertencia de que los registros ya están conectados. Si confirma que desea avanzar con la conexión, los registros seleccionados se quitan del registro original y se agregan al registro que está editando actualmente.

Para obtener información acerca de los tipos de conexión, vea [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Icono de información nueva con la descripción de los campos de la página de detalles del registro

>[!NOTE]
>
>Versión de vista previa: 30 de octubre de 2024; producción para versión rápida: con la versión 24.11 (14 de noviembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Hemos añadido un icono de información a la derecha de los nombres de campo en una página de registro. Al hacer clic en el icono de información, se muestra la descripción del campo, cuando existe una descripción. Antes de esta mejora, la descripción del campo se mostraba al pasar el ratón por encima del nombre del campo.

Para obtener más información, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

## Nuevo tipo de campo de Workfront para conexiones de Planning

>[!NOTE]
>
>Versión de vista previa: 24 de octubre de 2024; producción para versión rápida: con la versión 24.11 (14 de noviembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Para continuar vinculando objetos de Workfront a registros de Workfront Planning, se ha agregado un nuevo tipo de campo en formularios personalizados de Workfront llamado Conexión de Planning. Al agregar este tipo de campo en un formulario personalizado de Workfront y, finalmente, en un objeto de Workfront, ahora puede hacer lo siguiente:

* Muestra los registros conectados a un objeto de Workfront en el formulario personalizado.

* Conecte y desconecte los registros de Workfront Planning de un objeto Workfront.

Puede agregar el nuevo campo a los formularios para todos los tipos de objetos. Sin embargo, sólo puede editar la información del campo desde formularios adjuntos a los siguientes objetos de Workfront que se pueden conectar desde los tipos de registro de Workfront Planning: Portfolio, Programa, Proyecto, Empresa, Grupo.

Aún no está disponible la edición masiva de los campos de conexión de Planning para objetos de Workfront.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Ver una demostración en vídeo de esta característica](https://video.tv.adobe.com/v/3435633/){target=_blank}
