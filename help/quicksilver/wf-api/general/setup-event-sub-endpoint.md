---
content-type: api
navigation-topic: general-api
title: Requisitos para el envío de suscripciones a eventos
description: Requisitos para el envío de suscripciones a eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 77c07c7c7104d37360cc7630a89dd72836da477c
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 96%

---


# Requisitos para el envío de suscripciones a eventos

Los mensajes de suscripción de eventos son notificaciones que se pueden configurar para notificar a los usuarios cuando se producen determinados eventos. Para obtener más información sobre las suscripciones a eventos, consulte [Preguntas frecuentes - Suscripciones a eventos](../../wf-api/general/event-subs-faq.md).

## Estándares para el envío de mensajes de suscripciones a eventos

Los puntos finales de servicio que consumen mensajes de suscripción de evento de Adobe Workfront deben cumplir los siguientes requisitos básicos para garantizar que los mensajes se envíen y reciban correctamente:

* El punto final de servicio debe aceptar solicitudes de HTTP POST. El HTTP POST es el método de solicitud utilizado en todas las entregas de mensajes de suscripción de evento, incluidos los mensajes de validación.

* Para que el sistema de envío de suscripciones a eventos reconozca que el mensaje se recibió correctamente, el punto final debe devolver un estado HTTP de nivel 200 (por ejemplo, 200 OK o 202) para todos los mensajes entrantes.

* Si no se devuelve un estado de nivel 200, el sistema de suscripción de eventos supone que el mensaje no se entregó correctamente y comienza a aplicar la directiva de reintentos adecuada. Para obtener más información sobre la directiva de reintentos de Workfront, consulte [Reintentos de suscripción a eventos](../../wf-api/api/event-sub-retries.md).

* Junto con devolver un estado de nivel 200 como estado de respuesta, la respuesta HTTP debe recibirse en un plazo de cinco segundos después de iniciarse el intento de envío. Esta restricción garantiza que los procesos empresariales del consumidor o las limitaciones de infraestructura no retrasen el envío de otros mensajes pendientes de envío.

* Si un proceso empresarial de larga duración se desencadena desde un mensaje de suscripción de evento, Workfront recomienda que

   1. el punto final guarde la información del mensaje al recibirlo y responda inmediatamente con un estado de nivel 200.
   1. Una vez que un puto final ha respondido a una solicitud de envío de suscripción de evento, se pueden procesar los mensajes guardados.

* Los mensajes u objetos de suscripción de evento no pueden superar 1 MB.