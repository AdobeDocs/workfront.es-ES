---
title: 22.2 Mejoras en la integración
description: 22.2 Mejoras en la integración
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 99%

---

# 22.2 Mejoras en la integración

Esta página describe todas las mejoras de integración realizadas con la versión 22.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 4 de abril de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.2, consulte [Información general sobre la versión 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Ya está disponible la integración de Adobe Workfront con Anaplan

Para ofrecer una mejor flexibilidad y perspectiva de los aspectos financieros de los proyectos de Workfront, este ya se puede integrar con su cuenta de Anaplan. Al vincular objetos de Workfront a objetos de Anaplan, puede actualizar automáticamente la información entre las dos cuentas, asegurándose de que la información de ambas esté actualizada y sea idéntica. También es posible activar los procesos automatizados en Anaplan en función de las acciones realizadas en Workfront (o viceversa).

Por ejemplo, podría crear una campaña en Anaplan y, a continuación, crear un proyecto o programa de Workfront vinculado a la campaña. Cualquier coste producido en Workfront se podrá volver a cargar en Anaplan para revisar el rendimiento de la campaña.

Otros flujos de trabajo para los que puede considerar la posibilidad de utilizar la integración de Workfront con Anaplan son:

* Creación de solicitudes de presupuesto de Anaplan a partir de nuevos proyectos de Workfront
* Creación de proyectos de Workfront a partir de nuevos elementos de lista de Anaplan
* Inicio de solicitudes de proveedor de Anaplan desde proyectos Workfront

Para obtener más información, consulte [Adobe Workfront con Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Actualizaciones del conector mejorado de Workfront para Experience Manager

El conector mejorado de Workfront para Experience Manager ya incluye las siguientes actualizaciones:

* Ya es posible crear carpetas vinculadas entre Adobe Workfront y Adobe Experience Manager Assets as a Cloud Service aunque haya varias configuraciones de carpeta vinculadas a un proyecto.
* Compatibilidad añadida a la paginación de suscripción de eventos
* Se añadió compatibilidad con la versión 6.4.x de AEM
* Compatibilidad añadida con entornos proxy
* Varias correcciones de errores basadas en los comentarios de socios y clientes

Para obtener más información, consulte [Información general sobre el conector mejorado de Workfront para Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>La implementación y configuración de este conector requiere un partner certificado. Consulte [Instalar Workfront para el conector mejorado de Experience Manager](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install) para obtener más información.

## Las integraciones de Adobe Creative Cloud ahora utilizan OAuth2

Para una mayor seguridad y una experiencia más coherente en todas las integraciones, se actualizaron las integraciones de Adobe Creative Cloud para utilizar la autenticación OAuth2, una forma estándar en el sector para autenticar a los usuarios. Cuando los usuarios inicien sesión, ya podrán ver las acciones y áreas específicas a las que las integraciones tengan y permitan acceso. Después de esto, no será necesario que inicien sesión con tanta frecuencia.

Para obtener más información, consulte [Usar la extensión de Workfront para Illustrator e InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Consulta de detalles del secreto del cliente para integraciones personalizadas de OAuth2 o JWT

Para proporcionar transparencia en el uso de integraciones personalizadas de OAuth2 y JWT, se hizo posible la consulta de detalles de los secretos de cliente que usan sus integraciones. Ya es posible ver las fechas en las que se creó y utilizó por última vez el secreto de cliente. También es posible añadir y ver las propias notas acerca del secreto de cliente.

Anteriormente, estos detalles no estaban disponibles.

Para obtener más información sobre los secretos de cliente en integraciones personalizadas de OAuth2 o JWT, consulte [Crear aplicaciones de OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Consulta del tipo de autenticación en lista de aplicaciones OAuth2 personalizadas

Al ver la lista de aplicaciones OAuth2 personalizadas de la organización, ya es posible ver si cada aplicación utiliza la autenticación de usuario o la autenticación de servidor.

Anteriormente, esta información solo se podía consultar en las opciones de edición de cada aplicación.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Definir la caducidad de los tókenes de actualización en las integraciones personalizadas de OAuth2

Para controlar mejor el acceso y la seguridad de las integraciones de OAuth2 personalizadas, ahora puede personalizar la duración de los tokens de actualización. Una vez que caduca el token de actualización de un usuario, deberá volver a iniciar sesión en la integración.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Utilice claves públicas y privadas en las integraciones personalizadas de OAuth2 para aplicaciones de servidor a servidor

Ahora puede configurar aplicaciones OAuth2 de servidor a servidor en sus integraciones personalizadas. Al configurar las claves pública y privada, puede permitir que Workfront se comunique con otra aplicación sin utilizar las credenciales de inicio de sesión.

Anteriormente, toda la autenticación en las aplicaciones OAuth2 personalizadas utilizaba las credenciales de inicio de sesión del usuario.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## La integración de Google Workspace ahora utiliza OAuth2

Para lograr una mayor seguridad y una experiencia más coherente en todas las integraciones, hemos actualizado la integración de Google Workspace para utilizar la autenticación OAuth2, una forma estándar en el sector para autenticar a los usuarios. Cuando los usuarios inicien sesión, ya podrán ver las acciones y áreas específicas a las que las integraciones tengan y permitan acceso. Después de esto, no será necesario que inicien sesión con tanta frecuencia.

Para obtener más información, consulte [Iniciar y cerrar sesión en Adobe Workfront para Google Workspace](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
