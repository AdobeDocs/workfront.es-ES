---
content-type: api;faq
navigation-topic: general-api
title: Preguntas frecuentes - Suscripciones de eventos
description: Preguntas frecuentes - Suscripciones de eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# Preguntas frecuentes - Suscripciones de eventos

<!--
{{highlighted-preview}}
-->

Las siguientes son las preguntas más frecuentes acerca de las suscripciones a eventos:

## ¿Qué es una suscripción?

Una suscripción es un conjunto de datos que se utiliza para hacer coincidir y entregar eventos de Adobe Workfront al extremo HTTP de un cliente. Este recurso consta de 4 atributos principales:

* customer_id
* obj_code
* obj_id
* url

Una suscripción también puede tener otros atributos, como su propio ID único y la fecha en que se creó, pero los atributos enumerados arriba se utilizan principalmente para hacer coincidir eventos y enviarlos a clientes.

## ¿Puedo seleccionar qué eventos se envían a un extremo en función de determinados criterios dentro de una carga útil de evento?

Los filtros de suscripción de eventos permiten ordenar los subgrupos de eventos según criterios específicos. Se recomienda aplicar filtros a las suscripciones de evento, ya que puede reducir significativamente el número de mensajes que debe consumir un extremo. Para obtener más información, consulte [Filtrado de suscripción de eventos](../../wf-api/general/event-subs-api.md#event).

## ¿Por qué la API devuelve un código de respuesta en conflicto 409?

Si intenta crear una suscripción de evento y recibe un conflicto de código de respuesta: 409, la suscripción que intentó crear es un duplicado. Workfront no permite la creación de suscripciones duplicadas.

## ¿Qué debo hacer si mis mensajes no se entregan a mi punto final?

Busque las siguientes situaciones y utilice la solución recomendada:

* Asegúrese de que el punto final de suscripción definido por la variable **url** field: devuelve un código de respuesta HTTP 2XX. Si no es así, póngase en contacto con el Soporte técnico de Workfront o consulte [Requisitos de envío de suscripción a evento](../../wf-api/general/setup-event-sub-endpoint.md).

* Es posible que la solicitud de envío de evento se agote antes de completarse. Asegúrese de que el punto final responda de forma coherente en 5 segundos. Este es el tiempo de espera predeterminado establecido para que la solicitud HTTP envíe un mensaje de suscripción de evento. Si el punto de conexión no responde en 5 segundos, póngase en contacto con el Soporte técnico de Workfront o consulte [Requisitos de envío de suscripción a evento](../../wf-api/general/setup-event-sub-endpoint.md).
* Puede que los eventos no generen lo que piensa. Asegúrese de no estar suponiendo cómo y cuándo deben activarse los eventos y de hecho se activan. Por ejemplo, puede pensar que actualizar un documento en una tarea genera un evento de actualización de tarea, pero en su lugar, genera un evento de creación o actualización de documento.
* Es posible que su suscripción no esté configurada como espera. Puede crear suscripciones a eventos en diferentes entornos y esperar que se transfieran como lo hacen los demás datos de Workfront. Sin embargo, los datos de suscripción de evento no están configurados para copiarse o promocionarse a otros entornos. Asegúrese de emitir solicitudes de API al entorno correcto y de que las suscripciones de ese entorno estén configuradas según lo esperado.
* No se recibió la carga útil porque no se ha agregado la dirección IP de Workfront necesaria a la lista de permitidos del cortafuegos. Los eventos de suscripción a eventos se envían desde unas pocas direcciones IP. Asegúrese de que la red de destino tenga todas las excepciones de IP necesarias para recibir cargas útiles de suscripciones a eventos de Workfront.

## ¿Por qué se tarda demasiado tiempo en que mis mensajes lleguen a mi punto final?

Algunos de los siguientes escenarios podrían ser responsables:

* Una operación de gran tamaño (como una actualización masiva) en el sistema puede hacer que se ponga en cola un gran volumen de mensajes de una sola vez, lo que puede tardar algún tiempo en procesarse.
* Los cálculos de larga duración o los cálculos de escala de tiempo en proyectos grandes podrían estar causando un retraso en la publicación de mensajes a Suscripciones de eventos para que se consuman.
* Es posible que la suscripción se haya deshabilitado.

   * Tras un periodo de gracia de 100 mensajes, si una URL determinada (que podría asociarse con una o más suscripciones) falla más del 70 % de las veces o si la URL no se entrega después de 2000 intentos consecutivos, no se intenta enviar todos los mensajes que coincidan con suscripciones con la misma URL. En su lugar, esos mensajes se ponen inmediatamente en cola para volver a intentarlo.

     Cada 10 minutos después de deshabilitar una dirección URL, intentamos entregar el siguiente mensaje que pasa a través para su procesamiento. Si ese mensaje se envía correctamente, volvemos a habilitar esa dirección URL y, posteriormente, todas las suscripciones coincidentes. Si ese mensaje no se envía, ese temporizador de 10 minutos se restablece y lo intentamos de nuevo una vez caducado.

     Este comportamiento puede percibirse como incoherente o con retraso en las entregas, pero simplemente sigue nuestras políticas sobre cómo se gestionan los mensajes de suscripción de evento.

   * Una URL de suscripción a evento se desactivará si se cumple cualquiera de las siguientes condiciones:

      * La URL de suscripción no se ha podido entregar durante 7 días y ha fallado al menos 2000 intentos de entrega consecutivos en las últimas 72 horas.
      * La URL de suscripción no ha podido entregar 50 000 intentos consecutivos.

## ¿Qué debo hacer si recibo un estado de respuesta 500 al intentar llamar a la API de suscripción a evento?

Póngase en contacto con el Soporte técnico de Workfront. Para obtener información sobre cómo ponerse en contacto con el servicio de asistencia, consulte [Contactar con Atención al cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## ¿Qué diferentes tipos de autenticación puedo utilizar con las suscripciones a eventos de Workfront?

Puede utilizar cualquier autenticación que utilice un token de portador. El **authToken** de una suscripción es una cadena que representa un token de portador de OAuth2 utilizado para autenticarse con la URL especificada en la **url** field. En teoría, este valor de token podría ser cualquier cosa siempre y cuando el extremo de destino sepa cómo gestionar su codificación, que es **utf-8**.

## ¿Cuánto tiempo debe transcurrir antes de recibir la carga útil de evento de las suscripciones a eventos de Workfront?

En general, puede esperar recibir solicitudes de envío de eventos de suscripción de eventos en menos de 5 segundos desde que se registró el cambio de datos. En promedio, las notificaciones de los ganchos web se reciben en menos de 1 segundo desde el momento en que se realiza el cambio de datos. Sin embargo, el servicio puede recibir mensajes en cantidades tan grandes que también pueden tardar más tiempo.

## Recursos adicionales

* **Documentación de API**: [API de suscripción de evento](../../wf-api/general/event-subs-api.md)

* **Prácticas recomendadas**: [Prácticas recomendadas de suscripción de eventos](../../wf-api/general/event-sub-best-practice.md)

* **Campos que almacenan en déclencheur las cargas de suscripción de eventos**: [Campos de recurso de suscripción de evento](../../wf-api/api/event-sub-resource-fields.md)

* **Explicación de los reintentos de suscripción a evento**: [Reintentos de suscripción de evento](../../wf-api/api/event-sub-retries.md)

* **Configuración del cortafuegos para Workfront**: [Configuración de la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
