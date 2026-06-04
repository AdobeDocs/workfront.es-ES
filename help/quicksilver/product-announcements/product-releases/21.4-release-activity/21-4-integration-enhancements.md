---
title: Mejoras de integración en la versión 21.4
description: Mejoras de integración en la versión 21.4
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
TQID: https://experienceleague.adobe.com/dCRr9YQiXiX82Jw7wyeT786T8oJ74-u6kOuevYy-SWY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 367
ht-degree: 100%

---

# Mejoras de integración en la versión 21.4

En esta página se describen todas las mejoras de integración realizadas en la versión 21.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 4 de octubre de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.4, consulte [Descripción general de la versión 21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Enlazar documentos desde Dropbox Business

Se añadió Dropbox Business como integración de documentos disponible. Ya es posible acceder a los documentos almacenados en Dropbox Business directamente desde Workfront.

Dropbox Business permite vincular documentos compartidos y cargar documentos en carpetas compartidas. Dropbox (no Dropbox Business) permite que solo el propietario de los documentos pueda ver el documento en Workfront.

El administrador de Workfront puede habilitar esta integración para su organización.

Para obtener más información, consulte [Vincular documentos desde aplicaciones externas](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Para obtener información sobre cómo los administradores de Workfront pueden habilitar esta opción, consulte [Configuración de integraciones de documentos](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Actualizaciones en Workfront para Slack

Las siguientes actualizaciones ya están visibles en la integración de Workfront para Slack:

* Workfront para Slack tiene una nueva apariencia.
* Las notificaciones de Workfront para Slack ya se reciben en tiempo real.

  Por ejemplo, si se le asignase una tarea, recibirá esa notificación en cuanto se le asigne. Anteriormente, podía haber un retraso antes de que la notificación apareciera en Slack.

Esta actualización requiere que se vuelva a autorizar la integración de Workfront para Slack. Para obtener información sobre cómo autorizar la integración, consulte [Configuración de Adobe Workfront para Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Para obtener más información sobre las notificaciones de Workfront para Slack, consulte [Recibir notificaciones de Adobe Workfront en Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Visualización más clara de los detalles de acceso a la cuenta al dar el consentimiento para las integraciones de Adobe Workfront

Ya se actualizaron las pantallas de consentimiento de las integraciones de Adobe Workfront. Ya es posible ver las acciones y áreas específicas a las que tienen acceso las integraciones para comprender mejor a qué integración o aplicación se está permitiendo acceso.

Esta nueva pantalla de consentimiento se aplica a cualquier integración de Adobe Workfront que utilice OAuth 2.0.

Para obtener más información sobre integraciones específicas, consulte la documentación de esa integración.

## Ya no es necesaria la autenticación de claves API para las integraciones

Las integraciones de Workfront comenzaron recientemente a utilizar OAuth2 para una mayor seguridad y facilidad de uso. Como parte de este movimiento, Workfront ya no requiere claves API para la autenticación de integraciones.
