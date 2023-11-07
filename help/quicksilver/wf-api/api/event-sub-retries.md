---
content-type: api
navigation-topic: api-navigation-topic
title: Reintentos de suscripción de evento
description: Reintentos de suscripción de evento
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Reintentos de suscripción de evento

Al implementar un sistema de entrega de mensajes, hay que tener en cuenta algunas advertencias para garantizar la estabilidad, la coherencia y la buena experiencia del usuario. Una de las deficiencias de un sistema de entrega de mensajes es garantizar que los mensajes lleguen a su destino correctamente y saber qué hacer cuando los mensajes no llegan.

Algunas integraciones pueden aceptar un error de envío y luego soltar el mensaje y pasar al siguiente mensaje.  En otras integraciones, no se puede ignorar el error al entregar un mensaje. Por ejemplo, una integración financiera podría intentar enviar un mensaje, pero en su lugar recibe un código de estado HTTP 404, que indica que el servidor no pudo encontrar el punto final al que se iba a enviar el mensaje. En estos casos, un mensaje que falte podría significar que alguien no recibe un pago por su tiempo o que una organización sobrepasa el presupuesto en recursos contratados.

## Estrategia de Adobe Workfront para reintentos de suscripción a eventos

Dado que los clientes aprovechan la plataforma de Workfront como parte central de su trabajo diario de conocimientos, el marco de suscripción a eventos de Workfront proporciona un mecanismo para garantizar que se intente entregar cada mensaje al máximo.

Los mensajes salientes activados por eventos que no se entregan a los extremos de los clientes se vuelven a enviar hasta que la entrega se realiza correctamente durante un período de hasta 48 horas. Durante este tiempo, los reintentos se producen con una frecuencia reducida gradualmente hasta que el envío se realiza correctamente o hasta que han transcurrido 48 horas.

Los clientes deben asegurarse de que todos los puntos finales que consuman mensajes salientes de las suscripciones de evento de Workfront estén configurados para devolver un mensaje de respuesta de 200 niveles a Workfront cuando la entrega se realice correctamente.

## Gestión de mensajes salientes con eventos erróneos

El siguiente diagrama de flujo muestra la estrategia para volver a probar los envíos de mensajes con suscripciones a eventos de Workfront:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

Las siguientes explicaciones se corresponden con los pasos descritos en el diagrama de flujo:

1. El mensaje no se puede entregar.
1. Se registra la información de error de entrega del mensaje.

   Todos los intentos fallidos de enviar un mensaje se registran para que se pueda realizar la depuración con el fin de determinar la causa raíz de un error determinado o de una serie de errores.

1. Errores de URL incrementados.
1. El recuento de intentos de mensajes se incrementa.
1. Calcule el retraso hasta que se vuelva a intentar enviar este mensaje.
1. El mensaje se coloca en la cola de reintentos de mensajes.

   Como se muestra en el diagrama de flujo anterior, la cola de mensajes utilizada para procesar los reintentos de entrega de mensajes es una cola independiente de la que procesa el intento de entrega inicial de cada mensaje. Esto permite que el flujo de mensajes casi en tiempo real continúe sin impedimentos por el error de cualquier subconjunto de mensajes.

1. Se evalúa el estado del circuito URL. Se produce una de las siguientes situaciones:

   * Si el circuito está abierto y no permite entregas en este momento, reinicie el proceso en el paso 5.
   * Si el circuito está medio abierto, esto implica que nuestro circuito está abierto actualmente, pero ha pasado tiempo suficiente para permitir la prueba de la URL y ver si se ha resuelto el problema con la entrega.
   * Si se han alcanzado los límites de intentos de entrega de mensajes (48 horas de reintento), se pierde el mensaje

1. Si el circuito URL está cerrado y permite envíos, intente enviar el mensaje. Si este envío falla, el mensaje se reiniciará en el paso 1

1. Si el circuito URL está cerrado y permite envíos, intente enviar el mensaje. Si este envío falla, el mensaje se reiniciará en el paso 1.

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
