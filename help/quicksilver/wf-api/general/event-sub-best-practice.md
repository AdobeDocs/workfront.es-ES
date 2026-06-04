---
content-type: api
navigation-topic: general-api
title: Prácticas recomendadas para la suscripción a eventos
description: Prácticas recomendadas para la suscripción a eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
TQID: https://experienceleague.adobe.com/uT7erlnJR5-h-KKGQiuztzZKBtwtEvWQ8U-EUgN4TG4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 86%

---

# Prácticas recomendadas para la suscripción a eventos

Los mensajes de suscripción a eventos de Adobe Workfront se envían automáticamente desde Workfront después de configurar correctamente el servicio y crear una suscripción a eventos para activar esos envíos de mensajes. Para obtener más información sobre cómo configurar correctamente las suscripciones a eventos, consulte [Requisitos para el envío de suscripciones a eventos](../../wf-api/general/setup-event-sub-endpoint.md).


A continuación se enumeran algunas prácticas recomendadas para ayudarle a crear suscripciones a eventos de forma eficaz.

## Proporcionar todos los campos obligatorios del cuerpo de la solicitud

Asegúrese de que se proporcionan a la API todos los campos del cuerpo de la solicitud obligatorios. Para obtener información sobre todos los atributos de solicitud obligatorios, consulte [API de suscripción a evento](../../wf-api/general/event-subs-api.md).

## Evitar incluir campos de cuerpo adicionales

No incluya campos de cuerpo adicionales en la solicitud, ya que esto hará que la API no cree una suscripción.

## Evitar sobrecargar suscripciones a eventos

El servicio de suscripciones a eventos está diseñado para proporcionar un envío fiable de eventos para todos los usuarios. Para garantizar esto, se han implementado protecciones para evitar una producción de eventos excesiva por parte de un solo usuario que podría causar posibles problemas de calidad del servicio para todos los usuarios. Como resultado, un usuario que genere demasiados eventos a un ritmo elevado en un breve periodo de tiempo puede experimentar interferencias y retrasos en la entrega de eventos.

## Completar las pruebas dentro del período de gracia

Intente realizar todas las pruebas de suscripción dentro del período de gracia de 100 mensajes. Para obtener más información sobre este período de gracia, consulte [Preguntas más frecuentes: suscripciones a eventos](../../wf-api/general/event-subs-faq.md).

## Cumplir los requisitos de entrega de mensajes de suscripción a eventos estándar

Asegúrese de que el punto final de suscripción se ajuste a los requisitos de entrega de mensajes de suscripción a eventos estándar. Para obtener más información sobre estos requisitos, consulte [Requisitos para el envío de suscripciones a eventos](../../wf-api/general/setup-event-sub-endpoint.md).

## Lista de permitidos de direcciones IP por región global

Para recibir cargas útiles de suscripciones de eventos a través del cortafuegos, debe añadir las direcciones IP a la lista de permitidos por región global. Para obtener más información, consulte [API de suscripción a evento](../../wf-api/general/event-subs-api.md).

## Tener el nivel de acceso y la autenticación adecuados

Para crear, consultar o eliminar una suscripción a un evento, el usuario de Workfront necesita lo siguiente:

* Un nivel de acceso de **Administrador del sistema**
Para obtener más información, consulte [Conceder acceso administrativo completo a un usuario](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) o [Conceder acceso administrativo a usuarios de ciertas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Si su organización utiliza Adobe IMS (Identity Management System), incluya un token de usuario de IMS pasado en el encabezado `X-User-Token`.
