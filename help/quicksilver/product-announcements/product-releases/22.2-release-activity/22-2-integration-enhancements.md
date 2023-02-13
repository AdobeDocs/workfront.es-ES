---
title: 22.2 Mejoras en la integración
description: 22.2 Mejoras en la integración
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 22.2 Mejoras en la integración

En esta página se describen todas las mejoras de integración realizadas con la versión 2.2 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno Producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 4 de abril de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 2.2, consulte [Resumen de la versión 2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Ya está disponible la integración de Adobe Workfront con Anaplan

Para ofrecerle una mayor flexibilidad y comprensión de los aspectos financieros de sus proyectos de Workfront, Workfront ahora puede integrarse con su cuenta de Anaplan. Al vincular objetos de Workfront a objetos de Anaplan, se puede actualizar la información entre las dos cuentas automáticamente, asegurándose de que la información de ambos sea actualizada e idéntica. También puede almacenar en déclencheur los procesos automatizados en Anaplan según las acciones de Workfront (o viceversa).

Por ejemplo, puede crear una campaña en Anaplan y luego crear un proyecto o programa de Workfront vinculado a la campaña. A continuación, cualquier coste rastreado en Workfront se puede volver a cargar en Anaplan para revisar el rendimiento de la campaña.

Otros flujos de trabajo que puede considerar utilizar la integración de Workfront con Anaplan para incluyen:

* Creación de solicitudes de presupuesto de Anaplan a partir de nuevos proyectos de Workfront
* Creación de proyectos de Workfront a partir de nuevos elementos de lista de Anaplan
* Inicio de solicitudes de proveedores de Anaplan desde proyectos de Workfront

Para obtener más información, consulte [Adobe Workfront con Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront para actualizaciones de conector mejoradas del Experience Manager

El conector mejorado de Workfront para Experience Manager ahora incluye las siguientes actualizaciones:

* Ahora puede crear carpetas vinculadas entre Adobe Workfront y Adobe Experience Manager Assets as a Cloud Service incluso si hay varias configuraciones de carpeta vinculadas al proyecto.
* Se ha agregado compatibilidad con la paginación de suscripción de eventos
* Se ha agregado compatibilidad con AEM 6.4.x
* Se ha agregado compatibilidad con entornos de proxy
* Varias correcciones de errores basadas en los comentarios de socios y clientes

Para obtener más información, consulte [Descripción general del conector mejorado de Workfront para Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>La implementación y configuración de este conector requiere un socio certificado. Consulte [Instalación de Workfront para conector mejorado del Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) para obtener más información.

## Las integraciones de Adobe Creative Cloud ahora utilizan OAuth2

Para lograr una seguridad buena y una experiencia más coherente en todas las integraciones, hemos actualizado las integraciones de Adobe Creative Cloud para utilizar la autenticación OAuth2, una forma estándar del sector de autenticar a los usuarios. Ahora, cuando los usuarios inician sesión, pueden ver las acciones y áreas específicas a las que las integraciones tienen acceso y permiten el acceso. Después de esto, no necesitan iniciar sesión con tanta frecuencia.

Para obtener más información, consulte [Usar la extensión de Workfront para Illustrator y InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Consulte los detalles del Secreto del cliente para integraciones personalizadas de OAuth2 o JWT

Para proporcionar transparencia en el uso de sus integraciones personalizadas de OAuth2 y JWT, le hemos hecho posible ver los detalles de los secretos del cliente que utilizan sus integraciones. Ahora, puede ver las fechas en las que se creó y utilizó por última vez el Secreto del cliente. También puede agregar y ver sus propias notas sobre el Secreto del cliente.

Anteriormente, estos detalles no estaban disponibles.

Para obtener más información sobre los secretos del cliente en las integraciones personalizadas de OAuth2 o JWT, consulte [Creación de aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Consulte el tipo de autenticación en la lista de aplicaciones OAuth2 personalizadas

Ahora, cuando ve la lista de aplicaciones OAuth2 personalizadas en su organización, puede ver si cada aplicación utiliza autenticación de usuario o autenticación de servidor.

Anteriormente, esta información solo se podía ver si entraba en las opciones de edición de cada aplicación.

Para obtener más información, consulte [Creación de aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Establezca la caducidad de los tokens de actualización en sus integraciones personalizadas de OAuth2

Para controlar mejor el acceso y la seguridad para sus integraciones personalizadas de OAuth2, ahora puede personalizar la duración de los tokens de actualización. Una vez que caduque el token de actualización de un usuario, deberá iniciar sesión de nuevo en la integración.

Para obtener más información, consulte [Creación de aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Utilice claves públicas y privadas en sus integraciones personalizadas de OAuth2 para aplicaciones servidor a servidor

Ahora puede configurar aplicaciones OAuth2 de servidor a servidor en sus integraciones personalizadas. Al configurar claves públicas y privadas, puede permitir que Workfront se comunique con otra aplicación sin usar credenciales de inicio de sesión.

Anteriormente, toda la autenticación en las aplicaciones OAuth2 personalizadas utilizaba las credenciales de inicio de sesión del usuario.

Para obtener más información, consulte [Creación de aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## La integración de Google G Suite ahora utiliza OAuth2

Para lograr una seguridad buena y una experiencia más coherente en todas las integraciones, hemos actualizado la integración de Google G Suite para utilizar la autenticación OAuth2, una forma estándar del sector de autenticar a los usuarios. Ahora, cuando los usuarios inician sesión, pueden ver las acciones y áreas específicas a las que las integraciones tienen acceso y permiten el acceso. Después de esto, no necesitan iniciar sesión con tanta frecuencia.

Para obtener más información, consulte [Inicio y cierre de sesión de Adobe Workfront para G Suite](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
