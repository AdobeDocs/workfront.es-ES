---
content-type: release-notes
keywords: notas,trimestral,actualizar
navigation-topic: product-releases
title: 21.1 Otras mejoras
description: En esta página se describen todas las demás mejoras realizadas con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 15 de febrero de 2021.
author: Luke
feature: Product Announcements
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 21.1 Otras mejoras

En esta página se describen todas las demás mejoras realizadas con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 15 de febrero de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.1, consulte [Información general sobre la versión 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Actualizaciones de los requisitos de error de suscripción a eventos

Actualizamos los requisitos de deshabilitación de software de los errores de suscripción de eventos. Además de los requisitos existentes, las suscripciones a eventos ahora se desactivarán de forma suave si no logran una entrega correcta en un plazo de 2000 intentos. Esto es para fortalecer la regla de fallo del 70% existente que puede llevar a cantidades excesivas de fallas, bajo algunas condiciones.

Además, añadiremos requisitos de deshabilitación a partir de febrero de 2021.

Para obtener información adicional sobre los nuevos requisitos de deshabilitación y deshabilitación de software, consulte [Preguntas más frecuentes: Suscripciones a eventos](../../../wf-api/general/event-subs-faq.md).

## Nuevos campos de equipo disponibles para el compendio diario

Hemos añadido los campos Aprobación de equipo y asignaciones al correo electrónico del compendio diario de acción necesario.

Para obtener más información, consulte [Notificaciones: Acción necesaria](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Sustitución de la opción de correo electrónico POP en colas de solicitud

Estamos reemplazando la opción de correo electrónico POP para colas de solicitud con un nuevo sistema administrado por Workfront. Aún podrá enviar solicitudes por correo electrónico, pero tendrá que configurar una nueva dirección de correo electrónico administrada por Adobe Workfront en el área Cola de solicitudes .

Estos cambios están disponibles para probarlos en Vista previa.

El correo electrónico se desactiva automáticamente en todos los entornos de vista previa. Para habilitar el correo electrónico con fines de prueba, consulte [Habilitar el envío de correos electrónicos desde el entorno de Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Para obtener más información, consulte [Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitud](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Para obtener más información sobre por qué estamos realizando este cambio, consulte [Nuevo sistema administrado por Adobe Workfront para reemplazar el correo electrónico POP para colas de solicitud con 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Esta función ahora se incluye en la función [Administración de colas en la nueva experiencia de Workfront](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) ruta de aprendizaje en Workfront One.

## Restringir la edición de horas en hojas de horas

Para proporcionar más control sobre las hojas de horas y la edición de horas, hemos agregado una configuración que le permite restringir la edición de horas a los propietarios de hojas de horas y a los administradores del sistema.

Anteriormente, los usuarios con la opción Hojas de hora y horas habilitada en su nivel de acceso podían editar horas en cualquier parte de horas.

Para obtener más información, consulte [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Filtros y vistas mejorados en el área Hojas de horas

Se han añadido las siguientes mejoras al agregar un proyecto, una tarea o un problema a un parte de horas:

* Filtros: Hemos agregado filtros para Proyectos y problemas. Haga clic en Más opciones para ver estos filtros. Anteriormente, solo estaba disponible el filtro Tareas.
* Vistas: Hemos añadido las opciones Ver y Agrupar a la página Buscar.

Para obtener más información, consulte [Tiempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ocultar el cuadro de horas extra en Hojas de horas

Ahora puede ocultar el cuadro de horas extra para facilitar la confusión del usuario si no realiza el seguimiento de las horas extra en Workfront. Puede ocultar el cuadro de horas extra de un solo uso o en el Perfil de parte de horas:

* Hoja de horas de un solo uso: Cuando opta por ocultar el cuadro de horas extra en un parte de horas individual, solo se oculta para ese parte de horas. Para obtener más información, consulte [Crear un parte de horas de un solo uso](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Perfil de parte de horas: Cuando opta por ocultar el cuadro de horas extra en el Perfil de parte de horas, todas las hojas de horas futuras creadas para los usuarios asignados a ese perfil no verán el cuadro de horas extra. Para obtener más información, consulte [Crear, editar y asignar perfiles de parte de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Anteriormente, no se podía ocultar el cuadro de horas extra en las hojas de horas.

## Expandir o contraer elementos en la navegación de la ruta de exploración

Para facilitar la visualización de la ruta de exploración completa, hemos agregado la funcionalidad de expandir y contraer.

Ahora, los elementos truncados se agrupan antes del proyecto con el texto &quot;más&quot;. Por ejemplo, &quot;3 más&quot; indica que hay 3 objetos que no se están mostrando.

Anteriormente, había que hacer clic en los puntos suspensivos para mostrar cualquier objeto truncado en un menú desplegable.

Para ver todos los elementos de la ruta de exploración, haga clic en &quot;más&quot; al principio de la ruta para expandir los elementos. Una vez expandidos, puede hacer clic en &quot;Menos&quot; para contraer los elementos de nuevo.

## Nueva apariencia para la navegación por la ruta de exploración

Para ayudar a los usuarios a identificar mejor dónde están en Workfront y a navegar más fácilmente entre objetos, hemos realizado las siguientes mejoras en la navegación de la ruta de exploración:

* Cada elemento de la ruta de exploración ahora incluye una etiqueta de objeto.
* La página actual ahora está incluida en la ruta y en cursiva.
* La navegación mediante el teclado y el lector de pantalla ya están disponibles para las rutas de exploración.
* Cambios de estilo menores adicionales

