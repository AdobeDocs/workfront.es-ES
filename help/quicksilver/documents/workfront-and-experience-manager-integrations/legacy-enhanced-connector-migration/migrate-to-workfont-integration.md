---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migración desde el conector heredado o mejorado a la integración de Workfront para Adobe Experience Manager as a Cloud Service
description: En la información de esta página se explican las prácticas recomendadas para pasar de los conectores mejorados o heredados de Workfront for Experience Cloud a la última integración nativa que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 100%

---

# Migración desde el conector heredado o mejorado a la integración de Workfront para Adobe Experience Manager as a Cloud Service

En la información de esta página se explican las prácticas recomendadas para pasar de los conectores mejorados o heredados de Workfront for Experience Cloud a la última integración nativa que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Esta información no se aplica a los clientes que utilizan entornos On-Premise o Managed Services de Adobe Experience Manager Assets.

## Migración de la instancia de Workfront a Admin Console

Los clientes que tengan la intención de utilizar la nueva integración nativa entre Workfront y Adobe Experience Manager Assets as a Cloud Service deben asegurarse de que su entorno de Workfront esté vinculado a Adobe Admin Console. En el caso de los entornos de Workfront existentes, esto probablemente requiera una migración del entorno a un Adobe Admin Console conectado. Para obtener más información sobre esta migración y la lista de comprobación asociada, consulte [Prepárese para incorporar su organización a Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe debe ayudar a realizar esta migración. Para solicitar ayuda, siga uno de estos procedimientos:

* Si tiene acceso a Workfront Hub, envíe su solicitud a [Migración de Workfront a Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* Si no tiene acceso a Workfront Hub, puede enviar la solicitud a [Workfront a la cola de solicitudes de migración anticipada de Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Configuración de la nueva integración de Workfront for Adobe Experience Manager Assets as a Cloud Service

Una vez que el entorno de Workfront se haya migrado a Adobe Admin Console, los administradores de Workfront podrán configurar la nueva integración nativa. Para obtener ayuda sobre la configuración, consulte [Configuración de la integración de Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Mover los recursos existentes a la integración de Workfront for Adobe Experience Manager Assets as a Cloud Service

Después de configurar el entorno, puede mover los recursos y las carpetas vinculados existentes a Adobe Experience Manager. Este paso es opcional, pero garantizará que las carpetas y los recursos vinculados anteriormente a través del conector heredado o mejorado sigan siendo accesibles una vez que se desinstalen esos conectores.

Para obtener más información sobre cómo mover los recursos, consulte [Migrar carpetas y documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos los casos de uso críticos que se van a utilizar

Será importante validar todos los casos de uso críticos que se van a utilizar a través de la integración nativa antes de desinstalar el conector heredado o mejorado.

## Desinstalar el conector heredado o mejorado

Por último, debe desinstalar el conector heredado o mejorado. La integración nativa no está pensada para ejecutarse en paralelo con ninguno de los conectores.

Para desinstalar, consulte

* Instrucciones de desinstalación del conector heredado: [Desinstalar el conector heredado de Workfront con Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Instrucciones de desinstalación del conector mejorado: [Desinstalar el conector mejorado de Workfront con Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
