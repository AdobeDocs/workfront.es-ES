---
content-type: release-notes
keywords: notas, trimestral, actualizar, versión
navigation-topic: 2021-2-release-activity
title: 21.2 Otras mejoras
description: Esta página describe todas las otras mejoras realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte Información general de la versión 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# 21.2 Otras mejoras

Esta página describe todas las otras mejoras realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte [Información general sobre la versión 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Ahora somos oficialmente Adobe Workfront

Workfront ha cambiado a Adobe Workfront.

Ahora se actualizan las áreas más destacadas de la aplicación de Adobe Workfront y de nuestros sitios web orientados al cliente. Otras áreas se actualizarán pronto.

**Áreas actualizadas**

* Pantalla de inicio de sesión, navegación superior, corrección
* IU de plantillas de diseño, menú principal, exportación personalizada de Forms (solo disponible en la nueva experiencia de Adobe Workfront)
* Aplicación móvil de Workfront (iOS y Android)

Áreas que se actualizarán pronto

* Aplicaciones de corrección para equipos de escritorio y móviles
* Exportaciones de PDF para listas e informes
* Icono de Favicon en la pestaña del navegador

**Áreas actualizándose más tarde**

* Notificaciones por correo electrónico

## Validación de lista de permitidos de correo electrónico

>[!NOTE]
>
>Disponible solo en la nueva experiencia de Adobe Workfront.

Si utiliza la lista de permitidos de correo electrónico, las direcciones de correo electrónico de los usuarios nuevas y actualizadas ahora se validan con la lista de permitidos. Cuando agrega un usuario nuevo o edita un usuario existente e introduce un dominio de correo electrónico que no está en la lista de permitidos, un mensaje le notifica que el usuario no recibirá mensajes de correo electrónico. Puede seguir guardando el perfil de usuario, pero debe agregar el dominio a la lista de permitidos para que el usuario reciba correos electrónicos.

Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Nueva apariencia para los encabezados de objeto

>[!NOTE]
>
>Esta función se publicó en el entorno de producción el 10 de marzo de 2020.
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para reforzar aún más la jerarquía de la información y ayudar a los usuarios a comprender mejor en qué página se encuentran, cada encabezado de objeto ahora tiene:

* Coloridos iconos más modernos para cada tipo de objeto
* El tipo de objeto mostrado encima del nombre del objeto
* Estilo de fuente y tamaño de texto actualizados
* Otros cambios de estilo menores

Anteriormente, no había ningún icono y aparecía un distintivo con el nombre del objeto a la derecha del título del objeto.

Los encabezados de página de las áreas de la nueva experiencia de Workfront, como Análisis mejorado, Administración de recursos y otras, también tienen este aspecto actualizado.

Para obtener más información sobre los nuevos encabezados de objeto en la nueva experiencia de Workfront, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## Actualizaciones a respuestas de búsqueda de estado de objeto

Workfront ahora almacena los estados de objetos de una nueva manera.

Estos cambios no afectan a la forma en que se realizan las solicitudes de búsqueda de estado. Sin embargo, las solicitudes de API que contengan una búsqueda de estado de objeto devolverán una lista incompleta de estados de grupo.

Para obtener más información, consulte [Cambios principales en la API: respuestas de búsqueda de estado](../../../wf-api/api/api-changes-search.md) .

## Las cargas de suscripción de evento se han actualizado para incluir todos los campos que terminan en ID

Todas las cargas útiles de suscripción de eventos ahora contienen todos los campos que terminan en &quot;ID&quot;.

Es importante tener en cuenta que cada objeto tiene su propio conjunto único de campos asociados, que incluye un conjunto único de campos asociados que terminan en ID. Esto significa que, aunque cada carga útil contiene todos los campos asociados de ese objeto que terminan en ID, cada objeto tiene un conjunto diferente de campos que terminan en ID.

## La versión beta de modelos ya está disponible en Previsualización

>[!NOTE]
>
>Esta funcionalidad no estará disponible en general en el entorno de producción hasta la versión 21.3, más adelante este año. Disponible solo en la nueva experiencia de Adobe Workfront.

Blueprints proporciona bloques de construcción básicos para ayudarle a crear un sistema de administración de trabajo que crezca con usted. Los administradores del sistema pueden examinar el catálogo de modelos e instalar plantillas de proyecto listas para usar.

Para obtener más información, vea [Modelos](../../../administration-and-setup/blueprints/blueprints.md).
