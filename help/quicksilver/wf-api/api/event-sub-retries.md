---
content-type: api
navigation-topic: api-navigation-topic
title: Reintentos de suscripción de eventos
description: Reintentos de suscripción de eventos
author: John
feature: Workfront API
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Reintentos de suscripción de eventos

Al implementar un sistema de entrega de mensajes, hay que tener en cuenta algunas advertencias para garantizar la estabilidad, la coherencia y la buena experiencia del usuario. Una de las deficiencias de un sistema de envío de mensajes es garantizar que los mensajes lleguen a su destino correctamente y saber qué hacer cuando no llegan los mensajes.

Algunas integraciones pueden aceptar errores de entrega y luego dejar el mensaje y pasar al siguiente mensaje.  En otras integraciones, no se puede ignorar el error al enviar un mensaje. Por ejemplo, una integración financiera podría intentar enviar un mensaje, pero en su lugar recibe un código de estado HTTP de 404, que indica que el servidor no pudo encontrar el punto final al que se enviaría el mensaje. En tales casos, un mensaje que falta podría significar que alguien no recibe su tiempo o que una organización que excede el presupuesto en recursos contratados.

## Estrategia de Adobe Workfront para reintentos de suscripción de eventos

Dado que los clientes aprovechan la plataforma de Workfront como parte central de su trabajo diario de conocimientos, el marco de suscripción a eventos de Workfront proporciona un mecanismo para garantizar que se intente realizar el envío de cada mensaje en la mayor medida posible.

Los mensajes salientes activados por evento que no se puedan entregar a los puntos finales del cliente se reenvían hasta que el envío se realice correctamente durante un periodo de 48 horas. Durante este tiempo, los reintentos se producen con una frecuencia reducida incrementalmente hasta que el envío se realiza correctamente o hasta que hayan transcurrido 48 horas.

Los clientes deben asegurarse de que todos los extremos que consuman mensajes salientes desde Suscripciones de eventos de Workfront estén configurados para devolver un mensaje de respuesta de 200 niveles a Workfront cuando la entrega se realice correctamente.

## Gestión de mensajes salientes activados por eventos fallidos

El siguiente diagrama de flujo muestra la estrategia para volver a tentar los envíos de mensajes con suscripciones de eventos de Workfront:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

Las siguientes explicaciones se corresponden con los pasos descritos en el diagrama de flujo:

1. El mensaje no se puede entregar.
1. Se registra la información del error en la entrega de mensajes.

   Todos los intentos fallidos para enviar un mensaje se registran de modo que la depuración se pueda realizar para determinar la causa raíz de un error determinado o de una serie de errores.

1. Los errores de URL se incrementaron.
1. El recuento de intentos de mensajes se incrementa.
1. Calcule el retraso hasta que se intente de nuevo la entrega de este mensaje.
1. El mensaje se coloca en la cola de reintentos del mensaje.

   Como se muestra en el diagrama de flujo anterior, la cola de mensajes utilizada para procesar los reintentos de entrega de mensajes es una cola separada de la que procesa el intento de envío inicial para cada mensaje. Esto permite que el flujo de mensajes casi en tiempo real continúe sin impedimentos por el fallo de cualquier subconjunto de mensajes.

1. Se evalúa el estado del circuito de URL. Se produce una de las siguientes situaciones:

   * Si el circuito está abierto y no permite entregas en este momento, reinicie el proceso en el paso 5.
   * Si el circuito está semiabierto, esto implica que nuestro circuito está abierto actualmente, pero ha pasado tiempo suficiente para permitir la prueba de la URL para ver si el problema con la entrega a él se ha resuelto.
   * Si se han alcanzado los límites del intento de envío de mensajes (48 horas después de volver a intentarlo), se descarta el mensaje

1. Si el circuito URL está cerrado y permite entregas, intente enviar el mensaje. Si este envío falla, el mensaje se reiniciará en el paso 1

1. Si el circuito URL está cerrado y permite entregas, intente enviar el mensaje. Si este envío falla, el mensaje se reiniciará en el paso 1.

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
