---
title: Otras mejoras en la versión 20.4
description: Otras mejoras en la versión 20.4
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 99%

---

# Otras mejoras en la versión 20.4

Esta página describe todas las demás mejoras realizadas con la versión 20.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 9 de noviembre de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.4, consulte [Información general de la versión 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nuevo para administradores: disponibilidad de la opción Cambiar entorno de Workfront

Para obtener una experiencia más eficiente y práctica, los administradores de grupo y de Workfront ahora pueden cambiar rápidamente entre diferentes entornos de Workfront desde cualquier página de Workfront sin tener que cerrar la sesión.

En la nueva experiencia de Workfront, la opción Cambiar a Classic aparece en el menú principal.

En Workfront Classic, la opción Cambiar a la nueva experiencia aparece en el menú que se muestra al hacer clic en la imagen de perfil de la esquina superior derecha de la barra de navegación global.

Esta característica ahora se incluye en la [ruta de aprendizaje Aspectos básicos del administrador, parte 1](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/home) en Workfront One.

## Cifrado mejorado para Workfront Proof

Estamos realizando algunos cambios para mejorar la seguridad del cifrado de datos en movimiento de la aplicación de corrección de Workfront. Los cifrados TLS débiles quedarán obsoletos el 11 de noviembre de 2020.

Asegúrese de utilizar un explorador compatible al acceder a Workfront. Para obtener más información sobre los exploradores admitidos, consulte [Requisitos del explorador Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).

## Nueva apariencia para 3 plantillas de correo electrónico

Para mejorar la legibilidad y la experiencia general, las siguientes plantillas de correo electrónico tienen una nueva apariencia:

* Nueva solicitud de trabajo
* Una tarea dependiente a la que se le ha asignado ya está lista para iniciarse
* Notificación por correo electrónico del equipo con predecesora completada

Para habilitar el correo electrónico con fines de prueba en su entorno de vista previa, consulte la sección Administración de correos electrónicos en vista previa en [Modificar sus propias notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Nuevas notificaciones por correo electrónico para los equipos

Hemos añadido la siguiente notificación por correo electrónico para los equipos:

* Se ha completado una predecesora de una tarea asignada a mi equipo: el equipo asignado recibe una notificación por correo electrónico cuando una predecesora de una de sus tareas se marca como completada.
* Se han completado todas las predecesoras de una tarea asignada a mi equipo: el equipo asignado recibe una notificación por correo electrónico de cada predecesora que se marca como completada.

Para obtener más información, consulte [Notificaciones: información sobre el trabajo asignado a mí](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Nuevo para administradores: mejoras en las notificaciones por correo electrónico

Ahora, con un solo clic, puede habilitar o deshabilitar una notificación de evento por correo electrónico en Configuración. Simplemente, haga clic en el interruptor Activado/Desactivado junto al nombre de la notificación.

Además, observe que con nuestro moderno estilo ahora ha mejorado la experiencia de configuración de notificaciones de eventos en el área Notificaciones por correo electrónico.

Para obtener información sobre la configuración de notificaciones por correo electrónico, consulte [Configurar notificaciones de los eventos para todos los usuarios del sistema](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Esta característica ahora se incluye en la [ruta de aprendizaje Notificaciones por correo electrónico y en la aplicación](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/home) en Workfront One.

## Nuevos objetos de API que activan actualizaciones de suscripción a eventos

Se han creado dos nuevos objetos de API, documentVersion y proofApproval, que se configuran para activar actualizaciones de suscripción a eventos cuando se crea una versión de un documento o se aprueba uno.

Para obtener una lista completa de los campos asociados a cada objeto, consulte [Campos de recurso de suscripción de eventos](../../../wf-api/api/event-sub-resource-fields.md).
