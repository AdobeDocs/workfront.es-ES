---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Configuración de suscripciones a eventos en Workfront
description: Como administrador de Adobe Workfront, puede crear, ver y eliminar suscripciones de eventos desde el área de Configuración para enviar eventos de Workfront a un extremo externo.
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: 5a44679115dcfda871e2fe40c0c8443649fc43cf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 11%
---

# Configuración de suscripciones a eventos en Workfront

{{highlighted-preview-article-level}}

Como administrador de Adobe Workfront, puede crear, ver y eliminar suscripciones de evento desde el área de Configuración. Las suscripciones a eventos envían información de eventos de Workfront a un extremo externo cuando se producen eventos especificados.

Puede crear y eliminar suscripciones de evento en Workfront, pero no puede editar una suscripción existente. Si necesita cambiar una suscripción, elimínela y cree una nueva.

Para obtener más información acerca de las suscripciones a eventos, vea los artículos en [Suscripciones a eventos](/help/quicksilver/wf-api/api/event-subscriptions.md).

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
   <td>Debe ser administrador de Workfront.</td>
  </tr>
 </tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una suscripción de evento

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Sistema** y, a continuación, haga clic en **Suscripciones de eventos**.
1. Haga clic en **Nueva suscripción a evento**.
1. En el campo **Objeto**, seleccione el objeto Workfront que desee supervisar.
1. En el campo **Tipo de evento**, seleccione si desea que la suscripción de evento se déclencheur cuando se cree, actualice, elimine o comparta el objeto.
1. En el campo **URL de webhook**, introduzca el extremo que debería recibir la carga útil de evento.
1. En el campo **Token de autenticación**, ingrese el token usado para autenticar la solicitud en su extremo.
1. Si desea que Workfront codifique la carga útil antes de enviarla, habilite la opción para enviar la carga útil como Base64.
1. Si es necesario, añada uno o más filtros para limitar los eventos que almacenan en déclencheur la suscripción. Los filtros disponibles se basan en el objeto seleccionado.
1. Haga clic en **Crear**.

Para obtener información acerca de los requisitos de extremo, consulte [Requisitos de envío de suscripción a eventos](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md).

## Ver suscripciones a eventos

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Sistema** y, a continuación, haga clic en **Suscripciones de eventos**.

Desde la página Suscripciones de eventos puede revisar las suscripciones configuradas para su entorno. También puede ver cuántas suscripciones totales tiene su organización y cuántas de ellas están activas, deshabilitadas o congeladas.

* **Suscripciones deshabilitadas**: estas suscripciones se han deshabilitado automáticamente debido a errores repetidos de entrega.
* **Suscripciones inmovilizadas**: estas suscripciones están inmovilizadas temporalmente debido a problemas de entrega.

## Eliminación de una suscripción de evento

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Sistema** y, a continuación, haga clic en **Suscripciones de eventos**.
1. Seleccione la suscripción de evento que desee eliminar.
1. Haga clic **eliminar**.
