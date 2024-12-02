---
content-type: api
navigation-topic: api-navigation-topic
title: Reintentos de suscripción de evento
description: Reintentos de suscripción de evento
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 0325d305c892c23046739feff17d4b1fc11100cc
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Reintentos de suscripción de evento

Al implementar un sistema de entrega de mensajes, hay que tener en cuenta algunas advertencias para garantizar la estabilidad, la coherencia y la buena experiencia del usuario. Una de las deficiencias de un sistema de entrega de mensajes es garantizar que los mensajes lleguen a su destino correctamente y saber qué hacer cuando los mensajes no llegan.

Algunas integraciones pueden aceptar un error de envío y luego soltar el mensaje y pasar al siguiente mensaje.  En otras integraciones, no se puede ignorar el error al entregar un mensaje. Por ejemplo, una integración financiera podría intentar enviar un mensaje, pero en su lugar recibe un código de estado HTTP 404, que indica que el servidor no pudo encontrar el punto final al que se iba a enviar el mensaje. En estos casos, un mensaje que falte podría significar que alguien no recibe un pago por su tiempo o que una organización sobrepasa el presupuesto en recursos contratados.

## Estrategia de Adobe Workfront para reintentos de suscripción a eventos

Dado que los clientes aprovechan la plataforma de Workfront como parte central de su trabajo diario de conocimientos, el marco de suscripción a eventos de Workfront proporciona un mecanismo para garantizar que se intente entregar cada mensaje al máximo.

Los mensajes salientes activados por eventos que no se entregan a los extremos de los clientes se vuelven a enviar hasta que la entrega se realiza correctamente durante un período de hasta 48 horas. Durante este tiempo, los reintentos se producen con una frecuencia cada vez mayor hasta que el envío se realiza correctamente o hasta que se realizan 11 intentos.

La fórmula para estos intentos de reintento es:

`((2^attempt) - 1) * 84800ms`

El primer reintento se produce después de 1,5 minutos, el segundo, casi 5 minutos, y el undécimo es aproximadamente a las 48 horas.

Los clientes deben asegurarse de que todos los puntos finales que consuman mensajes salientes de las suscripciones de evento de Workfront estén configurados para devolver un mensaje de respuesta de 200 niveles a Workfront cuando la entrega se realice correctamente.

## Reglas de suscripción desactivadas y bloqueadas

* Una dirección URL de suscripción está **deshabilitada** si tiene una tasa de error superior al 70% con más de 100 intentos O si tiene 2000 errores consecutivos
* Una dirección URL de suscripción está **inmovilizada** si tiene más de 2.000 errores consecutivos y el último éxito fue hace más de 72 horas O si tiene 50.000 errores consecutivos en cualquier intervalo de tiempo.
* Una URL de suscripción **deshabilitada** seguirá intentando la entrega cada 10 minutos y se volverá a habilitar con una entrega correcta.
* La URL de suscripción **locked** nunca intentará la entrega a menos que se habilite manualmente mediante una solicitud de API.



<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->
