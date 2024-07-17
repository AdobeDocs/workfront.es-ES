---
content-type: release-notes
keywords: notas,trimestral,actualizar
navigation-topic: product-releases
title: 21.1 Otras mejoras
description: Esta página describe todas las demás mejoras realizadas con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 15 de febrero de 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 21.1 Otras mejoras

Esta página describe todas las demás mejoras realizadas con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 15 de febrero de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.1, consulte [Información general sobre la versión 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Actualizaciones de los requisitos de error de suscripción de evento

Estamos actualizando los requisitos de deshabilitación de software de los errores de suscripción de evento. Además de los requisitos existentes, las suscripciones a eventos ahora estarán desactivadas si no se consigue un envío correcto en un plazo de 2000 intentos. Esto sirve para reforzar la regla de fallo del 70 % existente, que puede llevar a cantidades excesivas de fallos, en algunas condiciones.

Además, añadiremos los requisitos de deshabilitación de hardware a partir de febrero de 2021.

Para obtener información adicional sobre los nuevos requisitos de deshabilitación de software y deshabilitación de hardware, consulte [Preguntas frecuentes - Suscripciones de eventos](../../../wf-api/general/event-subs-faq.md).

## Nuevos campos de equipo disponibles para el resumen diario

Hemos agregado los campos de Aprobación del equipo y Asignaciones al correo electrónico de resumen diario de la acción necesaria.

Para obtener más información, consulte [Notificaciones: Acción necesaria](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Sustituir opción de correo electrónico POP en colas de solicitudes

Estamos reemplazando la opción de correo electrónico POP para las colas de solicitud con un nuevo sistema administrado por Workfront. Todavía podrá enviar solicitudes por correo electrónico, pero en su lugar deberá configurar una nueva dirección de correo electrónico administrada por Adobe Workfront en el área de Cola de solicitudes.

Estos cambios están disponibles para probarlos en la vista previa.

El correo electrónico se desactiva automáticamente en todos los entornos de vista previa. Para habilitar el correo electrónico con fines de prueba, consulte [Habilitar el envío de correos electrónicos desde el entorno de vista previa de espacio aislado](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Para obtener más información, consulte [Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitudes](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Para obtener más información sobre el motivo por el que realizamos este cambio, consulte [Nuevo sistema administrado de Adobe Workfront para reemplazar el correo electrónico POP en las colas de solicitudes con 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Esta característica ahora se incluye en [Administración de colas en la nueva ruta de aprendizaje de la experiencia Workfront](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) en Workfront One.

## Restringir la edición de horas en hojas de horas

Para proporcionar más control sobre las plantillas de horas y la edición de horas, hemos agregado una configuración que le permite restringir la edición de horas a los propietarios de plantillas de horas y a los administradores del sistema.

Anteriormente, los usuarios con la opción Plantillas de horas y Horas habilitada en su nivel de acceso podían editar las horas en cualquier plantilla de horas.

Para obtener más información, consulte [Configurar la hoja de horas y las preferencias de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Filtros y vistas mejorados en el área de Plantillas de horas

Se han agregado las siguientes mejoras al agregar un proyecto, tarea o problema a una hoja de horas:

* Filtros: se han agregado filtros para Proyectos y Problemas. Haga clic en Más opciones para ver estos filtros. Anteriormente, solo el filtrado de Tareas estaba disponible.
* Vistas: se han añadido las opciones Ver y Agrupar a la página Buscar.

Para obtener más información, consulte [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ocultar el cuadro de horas extra en Plantillas de horas

Ahora puede ocultar el cuadro de horas extra para facilitar la confusión del usuario si no rastrea las horas extra en Workfront. Puede ocultar el cuadro de horas extra de una plantilla de horas de un solo uso o en el Perfil de plantilla de horas:

* Hoja de horas de un solo uso: cuando opta por ocultar la casilla de horas extra en una hoja de horas individual, solo está oculta para esa hoja de horas. Para obtener más información, consulte [Crear una hoja de horas de un solo uso](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Perfil de hoja de horas: cuando opta por ocultar la casilla de horas extra del perfil de hoja de horas, todas las hojas de horas futuras creadas para los usuarios asignados a ese perfil no verán la casilla de horas extra. Para obtener más información, consulte [Crear, editar y asignar perfiles de hojas de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Anteriormente, no se podía ocultar la casilla de horas extra en las plantillas de horas.

## Expandir o contraer elementos en la navegación de la ruta de exploración

Para facilitar la visualización de la ruta de exploración completa, se ha agregado la funcionalidad de expandir y contraer.

Ahora, todos los elementos truncados se agrupan antes del proyecto con el texto &quot;más&quot;. Por ejemplo, &quot;3 más&quot; indica que hay 3 objetos que no se muestran.

Anteriormente, se tenía que hacer clic en los puntos suspensivos para mostrar los objetos truncados en un menú desplegable.

Para ver todos los elementos de la ruta de exploración, haga clic en &quot;más&quot; al principio de la ruta de exploración para expandir los elementos. Una vez expandido, puede hacer clic en &quot;Menos&quot; para contraer los elementos de nuevo.

## Nueva apariencia para la navegación por rutas de exploración

Para ayudar a los usuarios a identificar mejor dónde se encuentran en Workfront y navegar más fácilmente entre objetos, hemos mejorado la navegación por la ruta de exploración de la siguiente manera:

* Cada elemento de la ruta de exploración ahora incluye una etiqueta de objeto.
* La página actual ahora se incluye en la ruta de exploración y está en cursiva.
* La navegación mediante el teclado y el lector de pantalla ya están disponibles para las rutas de exploración.
* Cambios menores de estilo adicionales

