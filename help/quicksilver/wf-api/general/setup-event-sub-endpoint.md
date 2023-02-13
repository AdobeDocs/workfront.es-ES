---
content-type: api
navigation-topic: general-api
title: Requisitos de entrega de suscripción de evento
description: Requisitos de entrega de suscripción de evento
author: John
feature: Workfront API
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Requisitos de entrega de suscripción de evento

Los mensajes de suscripción de evento son notificaciones que se pueden configurar para notificar a los usuarios cuando se producen determinados eventos. Para obtener más información sobre las suscripciones de eventos, consulte [Preguntas más frecuentes: Suscripciones a eventos](../../wf-api/general/event-subs-faq.md).

## Estándares para la entrega de mensajes de suscripción a eventos

Los extremos de servicio que consumen mensajes de suscripción de eventos de Adobe Workfront deben cumplir los siguientes requisitos básicos para garantizar que los mensajes se envíen y reciban correctamente:

* El extremo de servicio debe aceptar solicitudes de POST HTTP. El POST HTTP es el método de solicitud que se utiliza en todas las entregas de mensajes de suscripción de evento, incluidos los mensajes de validación.

* Para que el sistema de entrega de suscripciones de eventos reconozca que el mensaje se recibió correctamente, el extremo debe devolver un estado HTTP de 200 niveles (por ejemplo, 200 OK o 202) para todos los mensajes entrantes.

* Si no se devuelve un estado de 200 niveles, el sistema de suscripción de eventos supone que el mensaje no se entregó correctamente y comienza a aplicar la política de reintentos adecuada. Para obtener más información sobre la directiva de reintentos de Workfront, consulte [Reintentos de suscripción de eventos](../../wf-api/api/event-sub-retries.md).

* Junto con devolver un estado de 200 niveles como estado de respuesta, la respuesta HTTP debe recibirse en los cinco segundos posteriores al inicio del intento de envío. Esta restricción garantiza que los procesos comerciales del consumidor o las limitaciones de infraestructura no retrasen el envío de otros mensajes pendientes de envío.

* Si un proceso empresarial de larga duración déclencheur de un mensaje de suscripción de evento, Workfront recomienda que

   1. el extremo guarda la información del mensaje al recibirlo y responde inmediatamente con un estado de 200 niveles.
   1. Una vez que un extremo ha respondido a una solicitud de entrega de suscripción de evento, se pueden procesar los mensajes guardados.
