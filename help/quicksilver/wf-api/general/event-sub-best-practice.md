---
content-type: api
navigation-topic: general-api
title: Prácticas recomendadas para la suscripción de eventos
description: Prácticas recomendadas para la suscripción de eventos
author: John
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Prácticas recomendadas para la suscripción de eventos

Los mensajes de suscripción a eventos de Adobe Workfront se envían automáticamente desde Workfront después de haber configurado correctamente el servicio y de crear una suscripción a eventos para almacenar en déclencheur esos envíos de mensajes. Para obtener más información sobre la configuración correcta de las Suscripciones de eventos, consulte [Requisitos de entrega de suscripción de evento](../../wf-api/general/setup-event-sub-endpoint.md).


A continuación se enumeran algunas prácticas recomendadas para ayudarle a crear suscripciones de eventos de forma eficaz.

## Proporcione todos los campos del cuerpo de solicitud necesarios

Asegúrese de que todos los campos obligatorios del cuerpo de la solicitud se proporcionan a la API. Para obtener información sobre todos los atributos de solicitud necesarios, consulte [API de suscripción de evento](../../wf-api/general/event-subs-api.md).

## Evite incluir campos de cuerpo adicionales

No incluya campos de cuerpo adicionales en la solicitud, ya que esto provocará que la API no cree una suscripción.

## Pruebas completas dentro del período de gracia

Intente realizar todas las pruebas de suscripción dentro del período de gracia de 100 mensajes. Para obtener más información sobre este período de gracia, consulte [Preguntas más frecuentes: Suscripciones a eventos](../../wf-api/general/event-subs-faq.md).

## Cumplir los requisitos de entrega de mensajes de suscripción a eventos estándar

Asegúrese de que el extremo de suscripción cumpla los requisitos de entrega de mensajes de suscripción a eventos estándar. Para obtener más información sobre estos requisitos, consulte [Requisitos de entrega de suscripción de evento](../../wf-api/general/setup-event-sub-endpoint.md).

## Lista de permitidos de direcciones IP por región global

Para recibir cargas de suscripciones de eventos a través del cortafuegos, debe añadir las direcciones IP a la lista de permitidos por región global. Para obtener más información, consulte [API de suscripción de evento](../../wf-api/general/event-subs-api.md).

## Tener el nivel de acceso correcto y una clave de API

Para crear, consultar o eliminar una suscripción de evento, el usuario de Workfront debe:

* Un nivel de acceso de **Administrador del sistema**
Para obtener más información, consulte [Conceder a un usuario acceso administrativo completo](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) o [Conceder a los usuarios acceso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Una clave de API

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
