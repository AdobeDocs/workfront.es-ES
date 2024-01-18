---
title: 20.4 Otras mejoras
description: 20.4 Otras mejoras
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 20.4 Otras mejoras

Esta página describe todas las demás mejoras realizadas con la versión 20.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 9 de noviembre de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.4, consulte [Información general de la versión 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nuevo para administradores: Cambiar la opción de entorno de Workfront disponible

Para obtener una experiencia más eficiente y práctica, los administradores de grupo y de Workfront ahora pueden cambiar rápidamente entre diferentes entornos de Workfront desde cualquier página de Workfront sin tener que cerrar la sesión.

En la nueva experiencia de Workfront, la opción Cambiar a clásico aparece en el menú principal.

En Workfront Classic, la opción Cambiar a la nueva experiencia aparece en el menú que se muestra al hacer clic en la imagen de perfil en la esquina superior derecha de la barra de navegación global.

Esta función ahora se incluye en la [Aspectos básicos del administrador, parte 1, ruta de aprendizaje](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Cifrado mejorado para Workfront Proof

Estamos realizando algunos cambios para mejorar la seguridad del cifrado de datos en movimiento de la aplicación de corrección de Workfront. Los cifrados TLS débiles quedarán obsoletos el 11 de noviembre de 2020.

Asegúrese de utilizar un explorador compatible al acceder a Workfront. Para obtener más información sobre los exploradores compatibles, consulte [Requisitos del explorador Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).

## Nueva apariencia para 3 plantillas de correo electrónico

Para mejorar la legibilidad y la experiencia general, las siguientes plantillas de correo electrónico tienen una nueva apariencia:

* Nueva solicitud de trabajo
* Una tarea dependiente a la que está asignado ya está lista para iniciarse
* Notificación de correo electrónico del equipo con predecesora completa

Para habilitar el correo electrónico para fines de prueba en el entorno de vista previa, consulte la sección Administración de correos electrónicos en vista previa en [Modificar sus propias notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Nuevas notificaciones por correo electrónico para equipos

Hemos añadido la siguiente notificación por correo electrónico para los equipos:

* Se ha finalizado una tarea predecesora de una tarea asignada a mi equipo: el equipo asignado recibe una notificación por correo electrónico cuando una tarea predecesora de una de sus tareas se marca como completada.
* Se han finalizado todas las tareas predecesoras de una tarea asignada a mi equipo: el equipo asignado recibe una notificación por correo electrónico de cada predecesora que se marca como finalizada.

Para obtener más información, consulte [Notificaciones: Información sobre el trabajo asignado a mí](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Nuevo para administradores: mejoras en las notificaciones por correo electrónico

Ahora, con un solo clic, puede habilitar o deshabilitar una notificación de correo electrónico de evento en Configuración. Simplemente haga clic en el interruptor On/Off junto al nombre de la notificación.

Además, observe que nuestro estilo moderno ahora mejora la experiencia de configuración de notificaciones de eventos en el área de notificaciones por correo electrónico.

Para obtener información sobre la configuración de notificaciones por correo electrónico, consulte [Configurar notificaciones de eventos para todos los usuarios del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Esta función ahora se incluye en la [Ruta de aprendizaje de las notificaciones por correo electrónico y en la aplicación](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) en Workfront One.

## Nuevos objetos de API que almacenan en déclencheur las actualizaciones de suscripción de eventos

Se crearon dos nuevos objetos de API, documentVersion y proofApproval, y se configuran para almacenar en déclencheur las actualizaciones de suscripción de eventos cuando se crea una versión o se aprueba un documento.

Para obtener una lista completa de los campos asociados a cada objeto, consulte [Campos de recurso de suscripción de evento](../../../wf-api/api/event-sub-resource-fields.md).
