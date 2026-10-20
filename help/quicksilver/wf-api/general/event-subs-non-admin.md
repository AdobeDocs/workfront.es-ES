---
content-type: api
navigation-topic: general-api
title: Administración de suscripciones a eventos como usuario no administrador
description: Si el acceso a Workfront lo permite, puede crear, ver y eliminar suscripciones de evento que se encuentren dentro del ámbito permitido por los permisos y la configuración del sistema.
author: Courtney
feature: Workfront API
role: Developer
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 10%
---

# Administración de suscripciones a eventos como usuario no administrador

Si el acceso a Workfront lo permite, puede crear, ver y eliminar suscripciones de evento desde el área de Configuración. Sin embargo, su acceso se limita a las suscripciones y acciones autorizadas para su función y a la configuración del sistema de su organización.

Esta función no está disponible para todos los usuarios del mismo modo que lo está para los administradores de Workfront. Los usuarios con el acceso necesario solo pueden administrar suscripciones de evento dentro del ámbito que se les ha concedido.

Por ejemplo, los permisos pueden permitirle administrar únicamente ciertos tipos de objetos, tipos de eventos o suscripciones para un conjunto de trabajos definido. No puede administrar suscripciones de evento fuera del ámbito permitido por su acceso y configuración.

Para la configuración administrada por el administrador, consulte [Configuración de suscripciones a eventos en Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md).

Para obtener información sobre la API de suscripciones a eventos, consulte [API de suscripción a eventos](/help/quicksilver/wf-api/general/event-subs-api.md).

>[!NOTE]
>
>Los usuarios solo pueden administrar suscripciones de eventos dentro del ámbito permitido por sus permisos y la configuración del sistema de la organización. El acceso no equivale automáticamente al acceso de administrador.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Paquete de Adobe Workfront</td>
   <td>Cualquiera</td>
  </tr>
  <tr>
   <td role="rowheader">Licencia de Adobe Workfront</td>
   <td>
    <p>Estándar</p>
    <p>Plan</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Configuraciones de nivel de acceso</td>
   <td>
    <p>Debe tener el acceso adecuado para administrar suscripciones a eventos.</p>
    <p>Su acceso se limita a las suscripciones y acciones permitidas por los permisos y la configuración del sistema de su organización.</p>
   </td>
  </tr>
 </tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Trabajo con suscripciones a eventos

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Sistema** y, a continuación, haga clic en **Suscripciones de eventos**.
1. Revise las suscripciones disponibles.
1. Crear, ver o eliminar solo las suscripciones que se incluyan en el ámbito autorizado.

Si no ve las opciones que espera, o si no puede crear o administrar una suscripción, póngase en contacto con el administrador de Workfront para confirmar si el acceso está limitado por la función, los permisos o la configuración del sistema.

## Artículos relacionados

* [Configuración de suscripciones a eventos en Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [API de suscripción a eventos](/help/quicksilver/wf-api/general/event-subs-api.md)
