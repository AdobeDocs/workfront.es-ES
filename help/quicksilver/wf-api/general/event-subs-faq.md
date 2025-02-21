---
content-type: api;faq
navigation-topic: general-api
title: 'Preguntas frecuentes: suscripciones a eventos'
description: 'Preguntas frecuentes: suscripciones a eventos'
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: 074f78e27d2ab1cb1d1b8216f14557b91d9afd00
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 94%

---

# Preguntas frecuentes: suscripciones a eventos

<!--
{{highlighted-preview}}
-->

A continuación se muestran las preguntas frecuentes acerca de las suscripciones a eventos:

## ¿Qué es una suscripción?

Una suscripción es un conjunto de datos que se utiliza para hacer coincidir y entregar eventos de Adobe Workfront al punto final HTTP de un cliente. Este recurso consta de 4 atributos principales:

* customer_id
* obj_code
* obj_id
* Dirección URL

Una suscripción también puede tener otros atributos, como su propio ID único y la fecha en que se creó, pero los atributos enumerados aquí arriba se utilizan principalmente para hacer coincidir eventos y enviarlos a clientes.

## ¿Puedo seleccionar qué eventos se envían a un punto final en función de determinados criterios dentro de una carga útil del evento?

Los filtros de suscripción a eventos permiten ordenar los subgrupos de eventos según criterios específicos. Se recomienda aplicar filtros a las suscripciones a eventos, ya que ello que puede reducir significativamente el número de mensajes que debe consumir un punto final. Para obtener más información, consulte [Filtrado de suscripciones a eventos](../../wf-api/general/event-subs-api.md#event).

## ¿Por qué la API devuelve un código de respuesta de conflicto 409?

Si intenta crear una suscripción a eventos y recibe el código de respuesta: conflicto 409, significa que la suscripción que intentó crear es un duplicado. Workfront no permite la creación de suscripciones duplicadas.

## ¿Qué debo hacer si mis mensajes no se entregan a mi punto final?

Busque las siguientes situaciones y utilice la solución recomendada:

* Asegúrese de que el punto final de la suscripción (definido por el campo **url**) devuelva un código de respuesta HTTP 2XX. Si no es así, póngase en contacto con el servicio de soporte de Workfront o consulte [Requisitos de entrega de suscripción a eventos](../../wf-api/general/setup-event-sub-endpoint.md).

* Es posible que la solicitud de envío de eventos se agote antes de completarse. Asegúrese de que el punto final responda de forma constante en 5 segundos. Este es el tiempo de espera predeterminado establecido para que la solicitud HTTP envíe un mensaje de suscripción a un evento. Si el punto final no responde en 5 segundos, póngase en contacto con el servicio de soporte de Workfront o consulte [Requisitos de entrega de suscripciones a eventos](../../wf-api/general/setup-event-sub-endpoint.md).
* Puede que los eventos no generen lo que piensa. Asegúrese de no hacer suposiciones sobre cómo y cuándo deben activarse los eventos y de cuándo de hecho se activan. Por ejemplo, es posible que piense que actualizar un documento en una tarea genera un evento de actualización de la tarea, pero en lugar de ello, se genera un evento de creación o actualización de documento.
* Es posible que su suscripción no esté configurada como cree. Se pueden crear suscripciones a eventos en diferentes entornos y creer que se van a transferir igual que lo hacen los demás datos de Workfront. Sin embargo, los datos de suscripción a eventos no están configurados para copiarse o promocionarse a otros entornos. Asegúrese de emitir solicitudes de API al entorno correcto y de que las suscripciones de ese entorno estén configuradas según lo que necesite.
* No se recibió la carga útil porque no se ha añadido la dirección IP de Workfront necesaria a la lista de permitidos del cortafuegos. Los eventos de suscripción a eventos se envían desde unas pocas direcciones IP. Asegúrese de que la red de destino tenga todas las excepciones de IP necesarias para recibir cargas útiles de suscripciones a eventos de Workfront.
* No se recibió la carga útil porque era superior a 1 MB. El objeto o los mensajes de suscripción de evento no pueden superar 1 MB.

## ¿Por qué se tarda demasiado tiempo en que mis mensajes lleguen a mi punto final?

Algunos de los siguientes escenarios podrían ser responsables:

* Una operación de gran tamaño (como una actualización masiva) en el sistema puede hacer que se ponga en cola un gran volumen de mensajes de una sola vez, lo que puede tardar algún tiempo en procesarse.
* Los cálculos de larga duración o los cálculos de cronología en grandes proyectos podrían estar causando un retraso en la publicación de mensajes para que los consuman las Suscripciones a eventos.
* Es posible que la suscripción se haya deshabilitado.

   * Tras un periodo de gracia de 100 mensajes, si una URL determinada (que podría estar asociada a una o más suscripciones) falla más del 70 % de las veces o si la URL falla en la entrega después de 2000 intentos consecutivos, no se intentará la entrega de todos los mensajes que coincidan con suscripciones con esa misma URL. En lugar de ello, esos mensajes se ponen inmediatamente en cola para un nuevo intento.

     Cada 10 minutos después de deshabilitar una URL, intentamos entregar el siguiente mensaje que llega para su procesamiento. Si ese mensaje se envía correctamente, volvemos a habilitar esa dirección URL y, posteriormente, todas las suscripciones coincidentes. Si ese mensaje no se envía, el temporizador de 10 minutos se restablece y lo intentamos de nuevo una vez caducado.

     Este comportamiento puede percibirse como incoherente o de retraso en las entregas, pero solo sigue nuestras políticas concernientes a la gestión de los mensajes de suscripción a eventos.

   * Una URL de suscripción a eventos se desactivará si se cumple cualquiera de las siguientes condiciones:

      * La URL de suscripción no se ha podido entregar durante 7 días y ha fallado al menos 2000 intentos de entrega consecutivos en las últimas 72 horas.
      * La URL de suscripción no ha podido ofrecer 50 000 intentos consecutivos.

## ¿Qué debo hacer si recibo un estado de respuesta 500 al intentar llamar a la API de suscripción a evento?

Póngase en contacto con asistencia de Workfront. Para obtener información sobre cómo ponerse en contacto con atención al cliente, consulte [Contactar con el servicio de atención al cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## ¿Qué diferentes tipos de autenticación puedo utilizar con las suscripciones a eventos de Workfront?

Puede utilizar cualquier autenticación que utilice un token de portador. El campo **authToken** de una suscripción es una cadena que representa un token portador de OAuth2 que se usó para autenticarse con la dirección URL especificada en el campo **url**. En teoría, este valor de token podría tener menos de 255 caracteres siempre y cuando el extremo de destino sepa cómo manejar su codificación, que es **utf-8**.

## ¿Cuánto tiempo debe transcurrir antes de recibir la carga útil de evento de las suscripciones a eventos de Workfront?

En general, puede esperar recibir solicitudes de envío de eventos de suscripción de eventos en menos de 5 segundos desde que se registró el cambio de datos. En promedio, las notificaciones de los webhook se reciben en menos de 1 segundo desde el momento en que se realiza el cambio de datos. Sin embargo, el servicio puede recibir mensajes en cantidades tan grandes que también pueden tardar más tiempo.

## Recursos adicionales

* **Documentación de API**: [API de suscripción a evento](../../wf-api/general/event-subs-api.md)

* **Prácticas recomendadas**: [Prácticas recomendadas de suscripción a eventos](../../wf-api/general/event-sub-best-practice.md)

* **Campos que activan cargas útiles de suscripción a eventos**: [Campos de recursos de suscripción a eventos](../../wf-api/api/event-sub-resource-fields.md).

* **Explicación de los reintentos de suscripción a eventos**: [Reintentos de suscripción a eventos](../../wf-api/api/event-sub-retries.md)

* **Configuración del firewall para Workfront**: [Configuración de la lista de permitidos del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
