---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Mejoras de revisión 2019.1
description: Esta página describe todas las mejoras de corrección incluidas en la versión 2019.1. La funcionalidad ya está disponible en el entorno de producción.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Mejoras de revisión 2019.1

Esta página describe todas las mejoras de corrección incluidas en la versión 2019.1. La funcionalidad ya está disponible en el entorno de producción.

Para obtener una lista de todos los cambios realizados en 2019.1, consulte [Resumen de la actividad de la versión 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Para administradores

* [Configuración de la función de corrección predeterminada para los no destinatarios que abren una prueba](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## Para todos los usuarios

* [Revisar contenido interactivo en el visor de revisión web](#proof-interactive-content-in-the-web-proofing-viewer)
* [El orden de clasificación predeterminado de los comentarios en el Visor de pruebas ahora es del más antiguo al más reciente](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [Revisión mejorada para comentarios en el visor de revisiones asociado a un intervalo de vídeos](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [Vínculo a los detalles del documento desde una notificación de revisión o el visor de revisión](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [Cambiar las notificaciones por correo electrónico en el Visor de pruebas](#change-your-email-notifications-in-the-proofing-viewer)
* [Cambiar el color de fondo en el visor de corrección de escritorio](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Borrar datos de explorador en caché de una prueba en el visualizador de pruebas de escritorio](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## Configuración de la función de corrección predeterminada para los no destinatarios que abren una prueba {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Los administradores de Workfront ahora pueden configurar la función de corrección predeterminada para los usuarios que no están designados como destinatarios en el flujo de trabajo de la revisión, pero que tienen acceso a la revisión a través de su objeto de Workfront (como proyecto, tarea o problema).

Anteriormente, cuando los usuarios e invitados tenían acceso a una prueba sin añadirla a su flujo de trabajo, su función de prueba predeterminada era Revisor.

Esta funcionalidad se aplica solo a las pruebas creadas en Workfront, no en Workfront Proof.

## Proof Interactive Content in the Web Proofing Viewer {#proof-interactive-content-in-the-web-proofing-viewer}

Si las políticas de seguridad de su organización no permiten el uso de la aplicación independiente Desktop Proofing Viewer, su administrador de Workfront ahora puede activar el contenido interactivo en el visor de revisión web. El contenido debe incluirse en un archivo ZIP antes de crear la prueba.

Para obtener más información, consulte en el artículo .

VÍDEO

## El orden de clasificación predeterminado de los comentarios en el Visor de pruebas ahora es del más antiguo al más reciente  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

En el Visor de pruebas, el orden de clasificación predeterminado de los comentarios en una prueba ahora es De más antiguo a más reciente, como en una conversación verbal.

Anteriormente, el orden de clasificación predeterminado era De más reciente a más antiguo.

Puede seleccionar una opción de ordenación diferente y esta se recuerda para todas las demás pruebas que abra.

Para obtener más información, consulte la sección en el artículo

## Revisión mejorada para comentarios en el visualizador de pruebas asociado a un rango de vídeos {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

Cuando revise un comentario asociado a un rango de material de archivo de vídeo en el Visor de pruebas, ahora puede hacer clic en Reproducir para ver todo el rango de material de archivo. La reproducción se pausa cuando llega al final del intervalo. El comentario permanece abierto para que no pierda la noción de dónde se encuentra.

Anteriormente, cuando se abría un comentario para una amplia gama de secuencias de vídeo, había que buscar manualmente el principio de la gama mirando los números de fotograma mostrados en el comentario antes de hacer clic en Reproducir. De lo contrario, el Visor de pruebas comenzó a reproducirse donde hiciera clic por última vez en la cronología del vídeo y no se detuvo al final del intervalo. Además, el comentario colapsó cuando hizo clic en Reproducir, por lo que ya no estaba claro qué comentario estaba revisando.

Para obtener más información sobre la revisión de pruebas de vídeo, consulte .

VÍDEO

## Vínculo a los detalles del documento desde una notificación de prueba o el visor de pruebas {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

Cuando reciba un correo electrónico que le invita a revisar una prueba o cuando esté revisándola en el Visor de pruebas, ahora puede acceder rápidamente a la página de detalles del documento para la prueba. En esta página, puede ver el objeto Workfront (como una tarea, un proyecto o un problema) asociado a la prueba. Esto proporciona contexto para ayudarle a comprender el trabajo que debe realizar en la prueba.

Es posible que esta funcionalidad solo funcione para los nuevos usuarios que agregue al sistema. Este problema es temporal.

Para obtener más información, consulte el artículo .

VÍDEO

## Cambio de las notificaciones por correo electrónico en el visualizador de pruebas {#change-your-email-notifications-in-the-proofing-viewer}

Ahora todos los revisores de revisión pueden especificar qué notificaciones de prueba desean recibir para una prueba. Esto es especialmente importante a la hora de colaborar con partes interesadas externas.

Anteriormente, solo el propietario de la prueba o el administrador de tráfico podían configurar las alertas de correo electrónico de una prueba para los revisores que agregaban a la prueba. Los colaboradores externos no podían controlar qué alertas de correo electrónico recibían sobre la revisión porque no tenían el acceso necesario a Workfront ni el nivel de permiso adecuado.

Esta configuración es independiente de la configuración de alertas de correo electrónico que se puede establecer en Workfront.

Para obtener más información, consulte [Administrar notificaciones para comentarios y decisiones sobre pruebas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

VÍDEO

## Cambiar el color de fondo en el visor de corrección de escritorio {#change-the-background-color-in-the-desktop-proofing-viewer}

Ahora puede cambiar el color de fondo del Visor de corrección de escritorio del color predeterminado casi negro al blanco. Esto facilita la visualización del contenido de revisión que tiene un fondo transparente.

Para obtener más información, consulte [Configurar ajustes del visor de revisión](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VÍDEO

## Borrar datos de explorador en caché de una prueba en el visualizador de pruebas de escritorio {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

Cuando la configuración de caché y cookies del explorador está configurada para bloquear contenido como las ventanas emergentes, este comportamiento de bloqueo también puede producirse en el Visor de corrección de escritorio, lo que impide que los revisores vean y comenten el contenido emergente de la prueba.

Ahora puede borrar los datos de caché del explorador que se pueden guardar con una prueba para que todo el contenido aparezca en el Visor de pruebas de escritorio y los revisores puedan verlo y realizar comentarios al respecto.

Para obtener más información, consulte [Configurar ajustes del visor de revisión](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VÍDEO
