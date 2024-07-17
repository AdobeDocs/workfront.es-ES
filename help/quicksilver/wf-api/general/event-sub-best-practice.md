---
content-type: api
navigation-topic: general-api
title: Prácticas recomendadas de suscripción de eventos
description: Prácticas recomendadas de suscripción de eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Prácticas recomendadas de suscripción de eventos

Los mensajes de suscripción a eventos de Adobe Workfront se envían automáticamente desde Workfront después de configurar correctamente el servicio y crear una suscripción a eventos para almacenar en déclencheur los envíos de mensajes. Para obtener más información sobre cómo configurar correctamente las suscripciones a eventos, consulte [Requisitos para la entrega de suscripciones a eventos](../../wf-api/general/setup-event-sub-endpoint.md).


A continuación se enumeran algunas prácticas recomendadas para ayudarle a crear suscripciones a eventos de forma eficaz.

## Proporcione todos los campos obligatorios del cuerpo de la solicitud

Asegúrese de que todos los campos del cuerpo de la solicitud requeridos se proporcionen a la API. Para obtener información acerca de todos los atributos de solicitud requeridos, consulte [API de suscripción a evento](../../wf-api/general/event-subs-api.md).

## Evite incluir campos de cuerpo adicionales

No incluya campos de cuerpo adicionales en la solicitud, ya que esto provocará que la API no cree una suscripción.

## Completar pruebas dentro del período de gracia

Intente realizar todas las pruebas de suscripción dentro del período de gracia de 100 mensajes. Para obtener más información acerca de este período de gracia, consulte [Preguntas más frecuentes - Suscripciones a eventos](../../wf-api/general/event-subs-faq.md).

## Cumplir los requisitos de entrega de mensajes de suscripción de evento estándar

Asegúrese de que el punto final de suscripción se ajuste a los requisitos de entrega de mensajes de suscripción de evento estándar. Para obtener más información sobre estos requisitos, consulte [Requisitos de entrega de suscripción a eventos](../../wf-api/general/setup-event-sub-endpoint.md).

## Lista de permitidos de direcciones IP por región global

Para recibir cargas útiles de suscripciones de eventos a través del cortafuegos, debe añadir las direcciones IP a la lista de permitidos por región global. Para obtener más información, consulte [API de suscripción a evento](../../wf-api/general/event-subs-api.md).

## Tener el nivel de acceso adecuado y una clave de API

Para crear, consultar o eliminar una suscripción a evento, el usuario de Workfront necesita lo siguiente:

* Un nivel de acceso de **Administrador del sistema**
Para obtener más información, consulte [Conceder acceso administrativo completo a un usuario](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) o [Conceder acceso administrativo a usuarios de ciertas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Una clave de API

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
