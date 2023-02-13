---
content-type: release-notes
keywords: notas,trimestral,actualizar,versión
navigation-topic: 2021-2-release-activity
title: 21.2 Otras mejoras
description: En esta página se describen todas las demás mejoras realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte Información general sobre la versión 21.2.
author: Luke
feature: Product Announcements
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 21.2 Otras mejoras

En esta página se describen todas las demás mejoras realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte [Resumen de la versión 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Ahora estamos oficialmente en Adobe Workfront

Workfront ha cambiado a Adobe Workfront.

Se han actualizado las áreas más destacadas dentro de la aplicación Adobe Workfront y nuestros sitios web orientados al cliente. Pronto se actualizarán otras áreas.

**Áreas actualizadas**

* Pantalla de inicio de sesión, navegación superior, prueba
* IU de plantillas de diseño, menú principal, exportación de Forms personalizada (solo disponible en la nueva experiencia de Adobe Workfront)
* Aplicación móvil de Workfront (iOS y Android)

Próximamente se actualizarán las áreas

* Aplicaciones de prueba para escritorio y dispositivos móviles
* Exportaciones de PDF para listas e informes
* Icono de favoritos en la ficha del navegador

**Las áreas se actualizan más tarde**

* Notificaciones por correo electrónico

## Validación de lista de permitidos de correo electrónico

>[!NOTE]
>
>Disponible solo en la nueva experiencia de Adobe Workfront.

Si utiliza la lista de permitidos de correo electrónico, las direcciones de correo electrónico de usuario nuevas y actualizadas ahora se validan para la lista de permitidos. Cuando agrega un usuario nuevo o edita un usuario existente e introduce un dominio de correo electrónico que no está en la lista de permitidos, un mensaje le notifica que el usuario no recibirá mensajes de correo electrónico. Puede seguir guardando el perfil de usuario, pero debe agregar el dominio a la lista de permitidos para que el usuario reciba correos electrónicos.

Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Nueva apariencia para encabezados de objeto

>[!NOTE]
>
>Esta función se publicó en el entorno Producción el 10 de marzo de 2020.
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para reforzar aún más la jerarquía de información y ayudar a los usuarios a comprender mejor en qué página se encuentran, ahora cada encabezado de objeto tiene:

* Iconos coloridos y más modernos para cada tipo de objeto
* El tipo de objeto que aparece encima del nombre del objeto
* Estilo de fuente y tamaño de texto actualizados
* Otros cambios de estilo menores

Anteriormente, no había ningún icono y aparecía un distintivo con el nombre del objeto a la derecha del título del objeto.

Los encabezados de página de las áreas de la nueva experiencia de Workfront (como Análisis mejorado, Gestión de recursos y otros) también tienen este aspecto actualizado.

Para obtener más información sobre los nuevos encabezados de objeto en la nueva experiencia de Workfront, consulte [Nuevos encabezados de objeto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## Actualizaciones en las respuestas de búsqueda de estado de objeto

Workfront ahora almacena los estados de los objetos de una nueva forma.

Estos cambios no afectan a cómo se realizan las solicitudes de búsqueda de estado. Sin embargo, las solicitudes de API que contengan una búsqueda de estado de objeto devolverán una lista incompleta de estados de grupo.

Para obtener más información, consulte [Cambios en las API principales: Respuestas de búsqueda de estado](../../../wf-api/api/api-changes-search.md) .

## Las cargas de suscripción de evento se actualizan para incluir todos los campos que terminan en ID

Todas las cargas de suscripción de eventos ahora contienen todos los campos que terminan en &quot;ID&quot;.

Es importante tener en cuenta que cada objeto tiene su propio conjunto único de campos asociados, que incluye un conjunto único de campos asociados que terminan en ID. Esto significa que, aunque cada carga útil contiene todos los campos asociados a ese objeto que terminan en ID, cada objeto tiene un conjunto diferente de campos que terminan en ID.

## Planes beta ahora disponibles en Vista previa

>[!NOTE]
>
>Esta funcionalidad no estará disponible para el público en general en el entorno de producción hasta la versión 21.3, que se publicará más adelante este año. Disponible solo en la nueva experiencia de Adobe Workfront.

Los modelos proporcionan componentes básicos para ayudarle a crear un sistema de gestión del trabajo que crezca con usted. Los administradores del sistema pueden examinar el catálogo de modelos e instalar plantillas de proyecto listas para usar.

Para obtener más información, consulte [Planes](../../../administration-and-setup/blueprints/blueprints.md).
