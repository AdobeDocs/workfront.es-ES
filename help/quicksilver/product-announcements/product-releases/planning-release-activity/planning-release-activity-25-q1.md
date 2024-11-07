---
content-type: release-notes
title: Actividad de la versión de Adobe Workfront Planning para la versión 25.1
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el primer trimestre de 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 0022892cabb9a44fb21e33d88148b098c937f388
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Actividad de la versión del primer trimestre de 2025 para Adobe Workfront Planning

<!--remove this important intro after the 25.1 release-->

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Workfront Planning, una nueva oferta de Adobe Workfront.
>
>Debe adquirir un plan de Workfront Planning, además de un plan de Workfront, para poder acceder y utilizar las funcionalidades de Workfront Planning.
>
>Para obtener una lista completa de los requisitos para acceder a Workfront Planning, consulte [Descripción general del acceso](/help/quicksilver/planning/access/access-overview.md).
>Para obtener una descripción general de Workfront Planning, consulte [Descripción general de Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Este artículo describe las funciones que se lanzarán para Workfront Planning durante la versión del primer trimestre de 2025.

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning después de la publicación de disponibilidad general del 28 de agosto de 2024, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Nuevos tipos de visualización para campos de tipo porcentual en la vista de tabla

>[!NOTE]
>
>Versión de vista previa: 7 de noviembre de 2024; producción para versión rápida: con la versión 24.12 (diciembre de 2024); producción para versión trimestral: con la versión 25.1 (enero de 2025)

Para facilitar la lectura de los números en la vista de tabla, ahora puede seleccionar entre las siguientes opciones para cambiar el modo en que se muestra un campo de tipo Porcentaje en la vista de tabla:

* Número
* Barra
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
