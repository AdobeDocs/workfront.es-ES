---
content-type: api;faq
navigation-topic: general-api
title: 'Preguntas más frecuentes: Suscripciones a eventos'
description: 'Preguntas más frecuentes: Suscripciones a eventos'
author: Becky
feature: Workfront API
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# Preguntas más frecuentes: Suscripciones a eventos

<!--
{{highlighted-preview}}
-->

Las siguientes son las preguntas más frecuentes sobre las suscripciones a eventos:

## ¿Qué es una suscripción?

Una suscripción es un conjunto de datos que se utiliza para hacer coincidir y enviar eventos de Adobe Workfront al extremo HTTP de un cliente. Este recurso consta de 4 atributos principales:

* customer_id
* obj_code
* obj_id
* url

Una suscripción también puede tener otros atributos, como su propio ID único y la fecha en que se creó, pero los atributos enumerados anteriormente se utilizan principalmente para hacer coincidir eventos y enviarlos a los clientes.

## ¿Puedo seleccionar qué eventos se envían a un extremo en función de ciertos criterios dentro de una carga útil de evento?

Los filtros de suscripción de eventos son una forma de ordenar los subgrupos de eventos según criterios específicos. Se recomienda aplicar filtros a las suscripciones de eventos, ya que puede reducir significativamente la cantidad de mensajes que un extremo necesita consumir. Para obtener más información, consulte [Filtro de suscripción de evento](../../wf-api/general/event-subs-api.md#event).

## ¿Por qué la API devuelve un código de respuesta de conflicto 409?

Si intenta crear una suscripción de evento y recibir un código de respuesta: 409, entonces la suscripción que intentó crear es un duplicado. Workfront no permite la creación de suscripciones duplicadas.

## ¿Qué debo hacer si mis mensajes no se envían a mi punto final?

Busque las siguientes situaciones y use la solución recomendada:

* Asegúrese de que el punto final de suscripción (definido por la variable **url** field: devuelve un código de respuesta HTTP 2XX. Si no es así, póngase en contacto con el servicio de asistencia de Workfront o consulte [Requisitos de entrega de suscripción de evento](../../wf-api/general/setup-event-sub-endpoint.md).

* La solicitud de entrega de evento podría agotarse antes de completarse. Asegúrese de que el punto final responda de forma coherente en 5 segundos. Este es el tiempo de espera predeterminado establecido para que la solicitud HTTP envíe un mensaje de suscripción de evento. Si el punto final no responde en un plazo de 5 segundos, póngase en contacto con el servicio de asistencia de Workfront o consulte [Requisitos de entrega de suscripción de evento](../../wf-api/general/setup-event-sub-endpoint.md).
* Es posible que los eventos no generen la forma que usted piensa. Asegúrese de que no está haciendo suposiciones sobre cómo o cuándo los eventos deben activarse y deben activarse. Por ejemplo, puede pensar que la actualización de un documento en una tarea genera un evento de actualización de tarea, pero en su lugar genera un evento de creación o actualización de documento.
* Es posible que la suscripción no esté configurada como esperaba. Puede crear suscripciones de eventos en diferentes entornos y esperar que se transfieran como lo hacen sus otros datos de Workfront. Sin embargo, los datos de suscripción a eventos no están configurados para copiarse o promocionarse a otros entornos. Asegúrese de que está enviando solicitudes de API al entorno correcto y de que las suscripciones de ese entorno están configuradas según lo esperado.
* No se recibió la carga útil porque la dirección IP de Workfront necesaria no se ha agregado a la lista de permitidos del cortafuegos. Los eventos de suscripción de evento se envían desde solo unas pocas direcciones IP. Asegúrese de que la red de destino tiene todas las excepciones de IP necesarias para recibir cargas desde Suscripciones de eventos de Workfront.

## ¿Por qué se está tardando una cantidad excesiva de tiempo en que mis mensajes alcancen mi punto final?

Algunos de los siguientes escenarios pueden ser responsables:

* Una operación de gran tamaño (como una actualización masiva) en el sistema puede hacer que se ponga en cola un gran volumen de mensajes a la vez, lo que puede llevar cierto tiempo procesar.
* Los cálculos de larga duración o los cálculos de línea de tiempo en proyectos grandes podrían estar provocando un retraso en la publicación de mensajes en Suscripciones de eventos para consumir.
* Es posible que la suscripción esté deshabilitada.

   * Después de un período de gracia de 100 mensajes, si una URL concreta (que podría asociarse con una o más suscripciones) falla más del 70% de las veces o si la URL no se entrega después de 2000 intentos consecutivos, no se intenta enviar todos los mensajes que coinciden con suscripciones con esa misma URL. En su lugar, esos mensajes se ponen en cola inmediatamente para un reintento.

      Cada 10 minutos después de deshabilitar una URL, intentamos enviar el siguiente mensaje que llega para su procesamiento. Si ese mensaje se envía correctamente, se vuelve a habilitar esa dirección URL y, posteriormente, cualquier suscripción coincidente. Si ese mensaje no se envía, entonces ese temporizador de 10 minutos se restablece y lo intentamos de nuevo después de que caduque.

      Este comportamiento puede percibirse como incoherente o como envíos retrasados, pero simplemente sigue nuestras políticas para controlar cómo se gestionan los mensajes de suscripción de eventos.

   * Una URL de suscripción de evento no se podrá habilitar si se cumple una de las siguientes condiciones:

      * La URL de suscripción no se ha podido entregar durante 7 días y ha fallado al menos 2000 intentos de envío consecutivos en las últimas 72 horas.
      * La URL de suscripción no pudo entregar 50 000 intentos consecutivos.

## ¿Qué debo hacer si recibo un estado de respuesta 500 cuando intento llamar a la API de suscripción de evento?

Póngase en contacto con el servicio de asistencia técnica de Workfront. Para obtener información sobre cómo ponerse en contacto con el servicio de asistencia técnica, consulte [Contactar con el servicio de atención al cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## ¿Qué tipos diferentes de autenticación puedo utilizar con las suscripciones a eventos de Workfront?

Puede utilizar cualquier autenticación que utilice un token al portador. La variable **authToken** El campo de una suscripción es una cadena que representa un token al portador de OAuth2 utilizado para autenticarse con la dirección URL especificada en la **url** campo . En teoría, este valor de token puede ser cualquier cosa siempre y cuando el extremo de destino sepa cómo gestionar su codificación, que es **utf-8**.

## ¿Cuánto tiempo debe transcurrir antes de recibir mi carga útil de evento desde Suscripciones a eventos de Workfront?

En general, se espera recibir solicitudes de envío de eventos de suscripción de evento en menos de 5 segundos desde que se registró el cambio de datos. De media, las notificaciones de weblock se reciben en menos de 1 segundo desde que se realiza el cambio de datos. Sin embargo, el servicio puede recibir mensajes en cantidades tan grandes que también puede tardar más.

## Recursos adicionales

* **Documentación de API**: [API de suscripción de evento](../../wf-api/general/event-subs-api.md)

* **Prácticas recomendadas**: [Prácticas recomendadas para la suscripción de eventos](../../wf-api/general/event-sub-best-practice.md)

* **Campos que generan déclencheur en las cargas de suscripción de eventos**: [Campos de recurso de suscripción de evento](../../wf-api/api/event-sub-resource-fields.md)

* **Explicación de los reintentos de suscripción de eventos**: [Reintentos de suscripción de eventos](../../wf-api/api/event-sub-retries.md)

* **Configuración del cortafuegos para Workfront**: [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
