---
content-type: api
navigation-topic: general-api
title: Requisitos de envío de suscripción a evento
description: Requisitos de envío de suscripción a evento
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Requisitos de envío de suscripción a evento

Los mensajes de suscripción de eventos son notificaciones que se pueden configurar para notificar a los usuarios cuando se producen determinados eventos. Para obtener más información sobre las suscripciones a eventos, consulte [Preguntas frecuentes - Suscripciones de eventos](../../wf-api/general/event-subs-faq.md).

## Estándares para la entrega de mensajes de suscripción de evento

Los extremos de servicio que consumen mensajes de suscripción de evento de Adobe Workfront deben cumplir los siguientes requisitos básicos, para garantizar que los mensajes se envíen y reciban correctamente:

* El extremo de servicio debe aceptar solicitudes de POST HTTP. El POST HTTP es el método de solicitud utilizado en todas las entregas de mensajes de suscripción de evento, incluidos los mensajes de validación.

* Para que el sistema de entrega de suscripción de evento reconozca que el mensaje se recibió correctamente, el punto de conexión debe devolver un estado HTTP de 200 niveles (por ejemplo, 200 OK o 202) para todos los mensajes entrantes.

* Si no se devuelve un estado de 200 niveles, el sistema de suscripción de eventos supone que el mensaje no se entregó correctamente y comienza a aplicar la directiva de reintentos adecuada. Para obtener más información acerca de la directiva de reintentos de Workfront, consulte [Reintentos de suscripción de evento](../../wf-api/api/event-sub-retries.md).

* Junto con devolver un estado de 200 niveles como estado de respuesta, la respuesta HTTP debe recibirse en un plazo de cinco segundos después de iniciarse el intento de envío. Esta restricción garantiza que los procesos empresariales del consumidor o las limitaciones de infraestructura no retrasen el envío de otros mensajes pendientes de envío.

* Si un proceso empresarial de larga duración déclencheur a partir de un mensaje de suscripción de evento, Workfront recomienda lo siguiente

   1. el punto de conexión guarda la información del mensaje al recibirlo y responde inmediatamente con un estado de 200 niveles.
   1. Una vez que un extremo ha respondido a una solicitud de envío de suscripción de evento, se pueden procesar los mensajes guardados.
