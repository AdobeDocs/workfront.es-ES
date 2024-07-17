---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Desinstalar el conector heredado
description: texto
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Desinstalar Workfront con el conector heredado de Adobe Experience Manager

Debe desinstalar Workfront con el conector heredado de Adobe Experience Manager a la última integración nativa que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.

## Cancelar suscripción a Workfront

1. Abra Adobe Experience Manager.
1. En Experience Manager, vaya a **Herramientas** > **Cloud Service** > **Configuración de integración de Workfront**.
1. Seleccione su configuración (global-workfront de manera predeterminada) y haga clic en **Propiedades**.
   ![cancelar la suscripción a workfront](assets/unsubscribe-from-workfront.png)
1. Deshabilitar sincronización de documentos, comentarios y metadatos. La etiqueta debe estar deshabilitada durante el día.
Esto eliminará las suscripciones en Workfront y permitirá al usuario crear una nueva suscripción con la misma URL definida en Day CQ Link Externalizer.

## Eliminar la configuración de integración de Workfront

Después de eliminar la suscripción, ahora es seguro eliminar la Configuración de integración de Workfront.

1. Abra la configuración y seleccione **Eliminar**.
   ![eliminar configuración](assets/delete-wf-configuration.png)

## Quitar asignación

A continuación, debe eliminar Workfront Property Mapping.

1. En Experience Manager, vaya a **Herramientas** > **Assets** > **Asignación de propiedades de Workfront**.

1. Seleccione todas las asignaciones y haga clic en **Eliminar**.

## Permisos de usuario

AEM A todos los usuarios que accedieron a Dam desde Workfront se les otorgaron permisos de lectura para `/content/dam`. Si un usuario ya no lo necesita, puede eliminar los permisos otorgados a dichos usuarios.

El conector funciona mediante el usuario del sistema workfront-service. Esto se desinstala al desinstalar el conector.

>[!NOTE]
>
>Si usa la versión 2.0.3 del conector y agregó el grupo `workfront-aem-connector-group`, también debe eliminarlo yendo a **Herramientas** > **Seguridad** > **Grupos**.

## Externalizador de vínculos CQ de día

Si no necesita el Day CQ Link Externalizer, puede revertirlo a `localhost:4502` yendo a `/system/console/configMgr` y buscando &quot;Day CQ Link Externalizer&quot;.

>[!NOTE]
>
>Si usa Adobe Experience Manager as a Cloud Service, puede cambiar esto si busca en su proyecto y busca el archivo _com.day.cq.commons.impl.ExternalizerImpl.xml_ en _ui.apps/src/main/content/jcr_root/apps/mysite/config_.

![Externalizador de vínculos CQ por día](assets/Day-CQ-Link-Externalizer.png)

## Desinstalar paquete de conector

Los pasos necesarios para desinstalar el paquete del conector difieren según la versión de Adobe Experience Manager que tenga.

### Adobe Experience Manager local

Si usa Adobe Experience Manager local, vaya a _crx/packmgr/index.jsp_ y busque `workfront-aem-connector.all-<version>.zip`, haga clic en **Más** y, a continuación, en **Desinstalar**.

Compruebe en `/conf` que se hayan eliminado todos los archivos creados por Workfront.

### Adobe Experience Manager as a Cloud Service

En Adobe Experience Manager as a Cloud Service, puede eliminar las dependencias del conector desde los archivos pom.js del proyecto.

## Firewall y Dispatcher

No olvide eliminar las URL de Workfront de la lista blanca si ya no necesita comunicarse. Además, el conector utiliza los encabezados apiKey y el nombre de usuario que se configuraron en Dispatcher. Estas también se pueden eliminar.
