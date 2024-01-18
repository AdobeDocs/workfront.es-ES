---
title: 21.4 Mejoras de la integración
description: 21.4 Mejoras de la integración
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 21.4 Mejoras de la integración

Esta página describe todas las mejoras de integración realizadas con la versión 21.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 4 de octubre de 2021.

Para ver una lista de todos los cambios disponibles con la versión 21.4, consulte [21.4 Información general de la versión](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Enlazar documentos desde Dropbox Business

Se ha agregado Dropbox empresarial como una integración de documentos disponible. Ahora, puede acceder a los documentos que ha almacenado en Dropbox Business directamente desde Workfront.

Dropbox Business le permite vincular documentos compartidos y cargar documentos en carpetas compartidas. Dropbox (no Dropbox Empresa) permite que solo el propietario de los documentos vea el documento en Workfront.

El administrador de Workfront puede habilitar esta integración para su organización.

Para obtener más información, consulte [Vinculación de documentos desde aplicaciones externas](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Para obtener información sobre cómo un administrador de Workfront puede activar esta opción, consulte [Configurar integraciones de documentos](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Actualizaciones en Workfront para Slack

Las siguientes actualizaciones ahora están visibles en la integración de Workfront para Slack:

* Workfront para Slack tiene un nuevo aspecto.
* Ahora recibe las notificaciones de Workfront para Slack en tiempo real.

  Por ejemplo, si se le asigna una tarea, recibirá esa notificación en cuanto se le asigne. Anteriormente, podía haber un retraso antes de que la notificación apareciera en Slack.

Esta actualización requiere que vuelva a autorizar la integración de Workfront con Slack. Para obtener información sobre la autorización de la integración, consulte [Configuración de Adobe Workfront para Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Para obtener más información sobre Workfront para notificaciones de Slack, consulte [Recibir notificaciones de Adobe Workfront en Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Ver más claramente los detalles de acceso a la cuenta al dar su consentimiento para las integraciones de Adobe Workfront

Ahora se actualizan las pantallas de consentimiento para integraciones de Adobe Workfront. Ahora puede ver las acciones y áreas específicas a las que tienen acceso las integraciones, para que pueda comprender mejor a qué está permitiendo el acceso a la integración o aplicación.

Esta nueva pantalla de consentimiento se aplica a cualquier integración de Adobe Workfront que utilice OAuth 2.0.

Para obtener más información sobre integraciones específicas, consulte la documentación de esa integración.

## Ya no es necesaria la autenticación de claves API para las integraciones

Las integraciones de Workfront han comenzado recientemente a utilizar OAuth2 para una mayor seguridad y facilidad de uso. Como parte de este movimiento, Workfront ya no requiere claves API para la autenticación de integraciones.
