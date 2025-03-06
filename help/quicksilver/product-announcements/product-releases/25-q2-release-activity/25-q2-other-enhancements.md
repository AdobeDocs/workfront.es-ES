---
title: Otras mejoras durante el segundo trimestre de 2025
description: Otras mejoras durante el periodo de tiempo de lanzamiento del segundo trimestre de 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
source-git-commit: d603edee0099b6ce3e4f8d3414d1b31f94209196
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 10%

---

# Otras mejoras durante el segundo trimestre de 2025

Esta página describe las mejoras realizadas con la versión del segundo trimestre de 2025 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del segundo trimestre de 2025, consulte [Información general de la versión del segundo trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md).

## Actualización a la nueva versión de suscripción de evento con puntos finales de actualización de versión

>[!NOTE]
>
>Producción para todos los clientes: 6 de marzo de 2025

Workfront ahora tiene versiones de suscripciones a eventos. La nueva versión no es un cambio en la API de Workfront, sino un cambio en la funcionalidad de suscripción de evento.

La capacidad de actualizar o reducir las suscripciones a eventos garantiza que, cuando se realicen cambios en la estructura de los eventos, las suscripciones existentes no se rompan, lo que le permite probar y actualizar a la nueva versión sin interrupciones en la suscripción de evento.

Para obtener más información sobre las diferencias entre las dos versiones, consulte el artículo [Versiones de suscripción de evento](/help/quicksilver/wf-api/general/event-subs-versioning.md).

Para obtener información sobre los extremos utilizados para actualizar o reducir una suscripción de evento entre versiones, consulte la sección [Versiones de suscripción de evento](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) en el artículo API de suscripción de evento.

## Representar los cambios del usuario de Adobe Admin Console como &quot;Sistema&quot; en la fuente de actualización de Workfront

>[!NOTE]
>
>Versión de vista previa: 23 de enero de 2025; producción para versión rápida: con la versión 25.2 (13 de febrero de 2025); producción para versión trimestral: con la versión 25.4 (abril de 2025)

Ahora, cuando el administrador de Adobe Admin Console realiza un cambio en la información de usuario de un usuario de Workfront, Workfront registra este cambio en la pestaña de actividad del sistema del área de Actualizaciones del usuario como perteneciente al &quot;Sistema&quot;. Hace referencia al administrador de Adobe Admin Console.

Antes de esta actualización, los cambios de usuario realizados por el administrador de Admin Console se registraban como realizados por el administrador principal del sistema de Workfront.

Para obtener información sobre cómo administrar usuarios en Adobe Admin Console, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
