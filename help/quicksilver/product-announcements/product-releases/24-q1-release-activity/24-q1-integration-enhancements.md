---
title: Mejoras en la integración del primer trimestre de 2024
description: Mejoras en la integración del primer trimestre de 2024
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Mejoras en la integración del primer trimestre de 2024

Esta página describe todas las mejoras de integración realizadas con la versión del primer trimestre de 2024 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción con la versión del primer trimestre de 2024.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del primer trimestre de 2024, consulte [Información general de la versión del primer trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## La asignación de metadatos en Experience Manager Assets Essentials ahora utiliza `xcm:keywords` en lugar de `dc:subject`

Hemos actualizado la integración de Experience Manager Assets Essentials para que coincida con la experiencia en la integración as a Cloud Service de Experience Manager Assets. Ahora, cuando se asignan varios campos de texto de una sola línea a un único campo en Experience Manager Assets, ambos servicios utilizan el campo `xcm:keywords`.

Anteriormente, estos campos se asignaban al campo `dc:subject` en Experience Manager Assets Essentials. La funcionalidad as a Cloud Service de Experience Manager Assets no se ha modificado.

Cualquier metadato de Experience Manager Assets Essentials asignado actualmente a `dc:subject` debe reasignarse a `xcm:keywords`.

Para obtener información sobre la asignación de metadatos a Experience Manager Assets AEM Essentials, consulte [Palabra clave de](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Los campos de escritura anticipada ahora están disponibles en la integración de Adobe Experience Manager

Para facilitar el vínculo de campos entre Workfront y Adobe Experience Manager, se ha añadido la compatibilidad con los campos de escritura anticipada en la asignación de metadatos. Ahora puede asignar campos de escritura anticipada a los campos correspondientes en Adobe Experience Manager.

Si un usuario selecciona un valor diferente para un campo en Workfront, este cambio se refleja inmediatamente en Adobe Experience Manager. Además, si cambia una opción de valor de campo (como un equipo que cambia su nombre a un nuevo nombre), este cambio también se refleja en Adobe Experience Manager.

Para obtener información e instrucciones sobre la asignación de metadatos en la integración de Adobe Experience Manager, consulte [Configurar metadatos](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Publicar recursos automáticamente en Adobe Experience Manager

Se ha añadido otro flujo de trabajo a la integración de Adobe Experience Manager. Ahora puede configurar los recursos para que se publiquen automáticamente cuando se envíen a Adobe Experience Manager. La integración se puede configurar para que publique en el servicio de publicación de Adobe Experience Manager o en un portal de marca de Adobe Experience Manager.

El flujo de trabajo Automatic Publish se puede habilitar y configurar en la integración de Adobe Experience Manager. Cuando se habilita, el flujo de trabajo se puede editar en el nivel de plantilla o proyecto.

Para obtener más información, consulte [Publicar recursos](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) en [Usar flujos de trabajo en la integración de Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
