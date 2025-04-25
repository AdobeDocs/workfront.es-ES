---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migración del conector heredado al conector mejorado
description: El siguiente proceso describe las prácticas recomendadas para pasar del conector heredado de Adobe Experience Manager al conector mejorado para integrar Adobe Workfront con AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 99%

---

# Migración del conector heredado al conector mejorado

El siguiente proceso describe las prácticas recomendadas para pasar del conector heredado de Adobe Experience Manager al conector mejorado para integrar Adobe Workfront con AEM Assets.

>[!IMPORTANT]
>
>Esta documentación solo se aplica a los clientes que utilizan entornos Adobe Experience Manager Assets On-Premise o Managed Services.


Para los clientes con Adobe Experience Manager Assets as a Cloud Service, la ruta de migración desde el conector heredado será a la nueva integración nativa dentro de Workfront. Para obtener más información sobre este proceso de migración, consulte [Migrar del conector heredado o mejorado a Workfront para la integración con Adobe Experience Manager as a Cloud Service](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementación del conector mejorado

>[!IMPORTANT]
>
>Se necesita un partner certificado o servicios de Adobe Consulting para implementar el conector mejorado.
>
> Para los partners que deseen certificar el conector mejorado, consulte el siguiente artículo: [Workfront para Experience Manager con conector mejorado Expert Series](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview).

Para implementar el conector mejorado, consulte [Configuración de Workfront para el conector mejorado de Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/integrations/workfront-connector-configure).


## Mover recursos existentes

Después de configurar el entorno, puede mover los recursos y las carpetas vinculados existentes a Adobe Experience Manager. Este es un paso opcional, pero garantizará que las carpetas y los recursos vinculados anteriormente a través del conector heredado seguirán siendo accesibles una vez que se desinstale el conector heredado.

Para obtener más información sobre cómo mover los recursos, consulte [Migrar carpetas y documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos los casos de uso críticos que se van a utilizar

Es importante validar todos los casos de uso críticos que se van a utilizar a través del conector mejorado antes de desinstalar el conector heredado.

## Desinstalar el conector heredado

Por último, debe desinstalar el conector heredado. El conector heredado no está diseñado para ejecutarse en paralelo con el conector mejorado.

Para desinstalarlo, consulte [Desinstalar Workfront con el conector heredado de Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
