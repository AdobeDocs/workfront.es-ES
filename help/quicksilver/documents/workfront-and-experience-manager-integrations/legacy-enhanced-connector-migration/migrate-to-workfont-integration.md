---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migración del conector heredado o mejorado a Workfront para la integración con Adobe Experience Manager as a Cloud Service
description: La información de esta página explica las prácticas recomendadas para pasar de Workfront para conectores mejorados o heredados de Experience Cloud a la integración nativa más reciente que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Migración del conector heredado o mejorado a Workfront para la integración con Adobe Experience Manager as a Cloud Service

La información de esta página explica las prácticas recomendadas para pasar de Workfront para conectores mejorados o heredados de Experience Cloud a la integración nativa más reciente que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Esta información no se aplica a los clientes que utilizan entornos On-Premise o Managed Services de Adobe Experience Manager Assets.

## Mover la instancia de Workfront al Admin Console

Los clientes que pretendan utilizar la nueva integración nativa entre Workfront y Adobe Experience Manager Assets as a Cloud Service deben asegurarse de que su entorno de Workfront esté vinculado a un Adobe Admin Console. Para los entornos Workfront existentes, es probable que esto requiera una migración del entorno a un Adobe Admin Console conectado. Para obtener más información sobre esta migración y la lista de comprobación asociada, consulte [Preparación para incorporar su organización a Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe debe ayudar a llevar a cabo esta migración. Para solicitar ayuda, realice una de las siguientes acciones:

* Si tiene acceso a Workfront Hub, envíe su solicitud a la [Migración de Workfront a Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Si no tiene acceso a Workfront Hub, puede enviar su solicitud al [Workfront a la cola de solicitud de migración anticipada de Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Configuración de la nueva integración as a Cloud Service de Workfront para Adobe Experience Manager Assets

Una vez que el entorno de Workfront se haya migrado a un Adobe Admin Console, los administradores de Workfront pueden configurar la nueva integración nativa. Para obtener ayuda sobre la configuración, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Mover los recursos existentes a la integración as a Cloud Service de Workfront para Adobe Experience Manager Assets

Después de configurar el entorno, puede mover los recursos y carpetas vinculados existentes a Adobe Experience Manager. Este es un paso opcional, pero garantiza que las carpetas y recursos previamente vinculados a través del conector heredado o mejorado seguirán siendo accesibles una vez que esos conectores se desinstalen.

Para obtener más información sobre cómo mover recursos, consulte [Migración de carpetas y documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos los casos de uso críticos que se vayan a usar

Será importante validar todos los casos de uso críticos que se pretendan usar a través de la integración nativa antes de desinstalar el conector heredado o mejorado.

## Desinstalación del conector heredado o mejorado

Por último, debe desinstalar el conector heredado o mejorado. La integración nativa no está pensada para ejecutarse en paralelo con ninguno de los conectores.

Para desinstalar, consulte

* Instrucciones de desinstalación del conector heredado: [Desinstalación de Workfront con el conector heredado de Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Instrucciones mejoradas de desinstalación del conector: [Desinstalación de Workfront con conector mejorado de Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
