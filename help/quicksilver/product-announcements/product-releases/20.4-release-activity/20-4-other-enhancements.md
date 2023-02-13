---
title: 20.4 Otras mejoras
description: 20.4 Otras mejoras
author: Luke
draft: Probably
feature: Product Announcements
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 20.4 Otras mejoras

En esta página se describen todas las demás mejoras realizadas con la versión 20.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 9 de noviembre de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.4, consulte [Información general sobre la versión 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Novedades para los administradores: la opción Cambiar entorno de Workfront está disponible

Para obtener una experiencia más eficaz y práctica, los administradores de grupos y los administradores de Workfront ahora pueden cambiar rápidamente entre diferentes entornos de Workfront desde cualquier página de Workfront sin tener que cerrar la sesión.

En la nueva experiencia de Workfront, la opción Cambiar a clásico aparece en el menú principal.

En Workfront Classic, la opción Cambiar a la nueva experiencia aparece en el menú que aparece al hacer clic en la imagen de perfil en la esquina superior derecha de la barra de navegación global.

Esta función ahora se incluye en la función [Aspectos básicos del administrador, parte 1, ruta de aprendizaje](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) en Workfront One.

## Encriptado mejorado para Workfront Proof

Estamos realizando algunos cambios para mejorar la seguridad del cifrado de datos en movimiento de la aplicación de prueba de Workfront. Los cifrados TLS débiles quedarán obsoletos el 11 de noviembre de 2020.

Asegúrese de que utiliza un explorador compatible al acceder a Workfront. Para obtener más información sobre los navegadores compatibles, consulte [Requisitos del explorador Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).

## Nueva apariencia para 3 plantillas de correo electrónico

Para mejorar la legibilidad y la experiencia general, las siguientes plantillas de correo electrónico tienen una nueva apariencia:

* Nueva solicitud de trabajo
* Una tarea dependiente a la que está asignado está lista para iniciarse
* Notificación de correo electrónico del equipo con el predecesor completado

Para activar el correo electrónico con fines de prueba en el entorno de vista previa, consulte la sección Administración de correos electrónicos en vista previa en [Activar o desactivar sus propias notificaciones de eventos](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Nuevas notificaciones por correo electrónico para equipos

Hemos añadido la siguiente notificación por correo electrónico para equipos:

* Se completó un predecesor de una tarea asignada a mi equipo: El equipo asignado recibe una notificación por correo electrónico cuando se marca como completado un predecesor de una de sus tareas.
* Se completan todas las predecesoras de una tarea asignada a mi equipo: El equipo asignado recibe una notificación por correo electrónico para cada predecesor que se marca como completado.

Para obtener más información, consulte [Notificaciones: Información sobre el trabajo asignado a mí](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Novedades para administradores: Mejoras en las notificaciones por correo electrónico

Ahora, con un solo clic, puede habilitar o deshabilitar una notificación de correo electrónico de evento en Configuración. Haga clic en el conmutador de activación/desactivación situado junto al nombre de la notificación.

Además, observe nuestro estilo moderno que ahora mejora la experiencia de configurar notificaciones de eventos en el área Notificaciones de correo electrónico .

Para obtener información sobre la configuración de las notificaciones por correo electrónico, consulte [Configurar notificaciones de eventos para todos los miembros del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Esta función ahora se incluye en la función [Ruta de aprendizaje de las notificaciones por correo electrónico y en la aplicación](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) en Workfront One.

## Nuevos objetos de API que actualizan la suscripción de eventos de déclencheur

Se han creado dos nuevos objetos de API, documentVersion y proofApproval, que se configuran para almacenar en déclencheur las actualizaciones de suscripción de eventos cuando se crea una versión de un documento o se aprueba.

Para obtener una lista completa de los campos asociados a cada objeto, consulte [Campos de recurso de suscripción de evento](../../../wf-api/api/event-sub-resource-fields.md).
