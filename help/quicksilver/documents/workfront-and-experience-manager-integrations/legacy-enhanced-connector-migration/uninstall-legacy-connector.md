---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Desinstalación del conector heredado
description: text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Desinstalación de Workfront con el conector heredado de Adobe Experience Manager

Debe desinstalar el conector heredado de Workfront con Adobe Experience Manager a la integración nativa más reciente que conecta Workfront y Adobe Experience Manager Assets as a Cloud Service.

## Cancelación de suscripción a Workfront

1. Abra Adobe Experience Manager.
1. En el Experience Manager, vaya a **Herramientas** > **Cloud Services** > **Configuración de integración de Workfront**.
1. Seleccione la configuración (frente a trabajo global de forma predeterminada) y haga clic en **Propiedades**.
   ![cancelar suscripción a workfront](assets/unsubscribe-from-workfront.png)
1. Desactive la sincronización de documentos, comentarios y metadatos. La etiqueta debe ser el día Deshabilitado.
Esto eliminará las suscripciones en Workfront y permitirá al usuario crear una nueva suscripción utilizando la misma url definida en Day CQ Link Externalizer.

## Eliminar la configuración de integración de Workfront

Después de quitar la suscripción, ahora es seguro eliminar la Configuración de integración de Workfront.

1. Abra la configuración y seleccione **Eliminar**.
   ![eliminar configuración](assets/delete-wf-configuration.png)

## Eliminar asignación

A continuación, debe eliminar la asignación de propiedades de Workfront.

1. En el Experience Manager, vaya a **Herramientas** > **Recursos** > **Asignación de propiedades de Workfront**.

1. Seleccione todas las asignaciones y haga clic en **Eliminar**.

## Permisos de usuario

Todos los usuarios que acceden AEM Dam desde Workfront recibieron permisos de lectura para `/content/dam`. Si un usuario ya no lo necesita, puede eliminar los permisos otorgados a dichos usuarios.

El conector funciona utilizando el servicio de interfaz de trabajo del usuario del sistema. Esto se desinstala al desinstalar el conector.

>[!NOTE]
>
>Si utiliza la versión 2.0.3 del conector y ha añadido el grupo `workfront-aem-connector-group`, esto también debe eliminarse. Para ello, vaya a **Herramientas** > **Seguridad** > **Grupos**.

## Externalizador de vínculos de CQ de día

Si no necesita el externalizador de vínculos de CQ de día, puede volver a convertirlo en `localhost:4502` yendo a `/system/console/configMgr` y buscando &quot;Day CQ Link Externalizer&quot;.

>[!NOTE]
>
>Si utiliza Adobe Experience Manager as a Cloud Service, puede cambiar esto mirando el proyecto y localizando el archivo _com.day.cq.commons.impl.ExternalizerImpl.xml_ interior _ui.apps/src/main/content/jcr_root/apps/mysite/config_.

![Externalizador de vínculos de CQ de día](assets/Day-CQ-Link-Externalizer.png)

## Desinstalar paquete de conector

Los pasos necesarios para desinstalar el paquete del conector difieren según la versión de Adobe Experience Manager que tenga.

### Adobe Experience Manager local

Si utiliza Adobe Experience Manager de forma local, vaya a _crx/packmgr/index.jsp_ y busque `workfront-aem-connector.all-<version>.zip`, haga clic en **Más** y luego **Desinstalar**.

Compruebe en `/conf` para asegurarse de que se han eliminado todos los archivos creados por Workfront.

### Adobe Experience Manager as a Cloud Service

Para Adobe Experience Manager as a Cloud Service, puede eliminar las dependencias del conector de los archivos pom.files del proyecto.

## Firewall y Dispatcher

No olvide eliminar las direcciones URL de Workfront en la lista blanca si la comunicación ya no es necesaria. Además, el conector utiliza los encabezados apiKey y el nombre de usuario que se establecieron en Dispatcher. También se pueden eliminar.
