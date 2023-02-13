---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migración del conector heredado al conector mejorado
description: El siguiente proceso describe las prácticas recomendadas para trasladar el conector heredado de Adobe Experience Manager al conector mejorado para integrar Adobe Workfront con AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Migración del conector heredado al conector mejorado

El siguiente proceso describe las prácticas recomendadas para trasladar el conector heredado de Adobe Experience Manager al conector mejorado para integrar Adobe Workfront con AEM Assets.

>[!IMPORTANT]
>
>Esta documentación se aplica solo a clientes que utilizan entornos On-Premise o Managed Services de Adobe Experience Manager Assets.


Para los clientes con recursos as a Cloud Service de Adobe Experience Manager Assets, la ruta de migración desde el conector heredado se dirigirá a la nueva integración nativa dentro de Workfront. Para obtener más información sobre este proceso de migración, consulte [Migración del conector heredado o mejorado a Workfront para la integración con Adobe Experience Manager as a Cloud Service](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementación del conector mejorado

>[!IMPORTANT]
>
>Se requiere un socio certificado o servicios de consultoría de Adobe para la implementación del conector mejorado.
>
> Para los socios que deseen certificar en el conector mejorado, revise el siguiente artículo: [Workfront para conector mejorado de Experience Manager Serie de expertos](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

Para implementar el conector mejorado, consulte [Configuración de Workfront para conector mejorado de Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## Mover recursos existentes

Después de configurar el entorno, puede mover los recursos y carpetas vinculados existentes a Adobe Experience Manager. Este es un paso opcional, pero garantiza que las carpetas y recursos previamente vinculados a través del conector heredado seguirán siendo accesibles una vez que se desinstale el conector heredado.

Para obtener más información sobre cómo mover recursos, consulte [Migración de carpetas y documentos vinculados](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validar todos los casos de uso críticos que se vayan a usar

Es importante validar todos los casos de uso críticos que se pretenden utilizar mediante el conector mejorado antes de desinstalar el conector heredado.

## Desinstalación del conector heredado

Por último, debe desinstalar el conector heredado. El conector heredado no está diseñado para ejecutarse en paralelo con el conector mejorado.

Para desinstalar, consulte [Desinstalación de Workfront con el conector heredado de Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
