---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migración del conector heredado o mejorado a la integración de Workfront para Adobe Experience Manager as a Cloud Service
description: En la información de esta página se explican las prácticas recomendadas para pasar de los conectores mejorados o heredados de Workfront for Experience Cloud a la última integración nativa que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Migración del conector heredado o mejorado a la integración de Workfront para Adobe Experience Manager as a Cloud Service

En la información de esta página se explican las prácticas recomendadas para pasar de los conectores mejorados o heredados de Workfront for Experience Cloud a la última integración nativa que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Esta información no se aplica a los clientes que utilizan entornos On-Premise o Managed Services de Adobe Experience Manager Assets.

## Mover la instancia de Workfront al Admin Console

Los clientes que tengan intención de utilizar la nueva integración nativa entre Workfront y Adobe Experience Manager Assets as a Cloud Service deben asegurarse de que su entorno de Workfront esté vinculado a un Adobe Admin Console. Para los entornos de Workfront existentes, esto probablemente requiera una migración del entorno a un Adobe Admin Console conectado. Para obtener más información sobre esta migración y la lista de comprobación asociada, consulte [Prepárese para incorporar su organización a Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

El Adobe debe ayudar a realizar esta migración. Para solicitar ayuda, siga uno de estos procedimientos:

* Si tiene acceso a Workfront Hub, envíe la solicitud al [Migración de Workfront a Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Si no tiene acceso a Workfront Hub, puede enviar la solicitud a [Cola de solicitudes de migración anticipada de Workfront a Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Configuración del nuevo Workfront para la integración as a Cloud Service de recursos de Adobe Experience Manager

Una vez que el entorno de Workfront se haya migrado a Adobe Admin Console, los administradores de Workfront podrán configurar la nueva integración nativa. Para obtener ayuda sobre la configuración, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Mueva los recursos existentes a su integración as a Cloud Service de Workfront para Adobe Experience Manager Assets

Después de configurar el entorno, puede mover los recursos y las carpetas vinculados existentes a Adobe Experience Manager. Este es un paso opcional, pero garantizará que las carpetas y los recursos vinculados anteriormente a través del conector heredado o mejorado seguirán siendo accesibles una vez que se desinstalen esos conectores.

Para obtener más información sobre cómo mover los recursos, consulte [Migración de carpetas y documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos los casos de uso críticos que se van a utilizar

Será importante validar todos los casos de uso críticos que se van a utilizar a través de la integración nativa antes de desinstalar el conector heredado o mejorado.

## Desinstalar el conector heredado o mejorado

Por último, debe desinstalar el conector heredado o mejorado. La integración nativa no está pensada para ejecutarse en paralelo con ninguno de los conectores.

Para desinstalar, consulte

* Instrucciones para desinstalar conectores heredados: [Desinstalar Workfront con el conector heredado de Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Instrucciones de desinstalación del conector mejorado: [Desinstalar Workfront con el conector mejorado de Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
