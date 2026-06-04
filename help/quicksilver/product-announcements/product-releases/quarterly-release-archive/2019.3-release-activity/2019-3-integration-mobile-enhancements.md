---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 Integración y mejoras en la aplicación móvil
description: En esta página se describen todos los cambios realizados en la integración y las mejoras en la aplicación móvil realizadas con la versión 2019.3. Estaba disponible en el entorno de producción la semana del 19 de agosto de 2019.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
TQID: https://experienceleague.adobe.com/6l1X-py3VV1LysiT-WtBvW4zJjGseRKfAL6C6ysdhUI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 790
ht-degree: 100%

---

# 2019.3 Integración y mejoras en la aplicación móvil

En esta página se describen todos los cambios realizados en la integración y las mejoras en la aplicación móvil realizadas con la versión 2019.3. Estaba disponible en el entorno de producción la semana del 19 de agosto de 2019.

Para obtener una lista de todos los cambios realizados en 2019.3, consulte [Información general de la actividad de la versión 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Compatibilidad con elementos compartidos en la integración de MS OneDrive

Ahora puede vincular los archivos y carpetas compartidos de OneDrive a objetos de Workfront. Y a la inversa, puede cargar archivos en Workfront en carpetas compartidas de OneDrive.

Para obtener más información, consulte las secciones [Vincular un documento externo a Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Vincular una o más carpetas externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder) y [Actualizar y vincular un documento de Workfront a un proveedor externo de servicios en la nube](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) en el artículo [Vincular documentos de aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Para obtener más información, consulte la sección [Vincular un documento externo a Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) en el artículo [Vincular documentos de aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Especificación de dominio necesaria para todos los inicios de sesión en Workfront

Ahora, todos los inicios de sesión de Workfront requieren que el usuario especifique el dominio si este no se ha especificado ya en la URL de Workfront. Si necesita esta información, la instancia de Workfront será más segura. Además, si la implementación de Workfront tiene varias instancias, esta mejora le permite añadir el mismo usuario a cada instancia de Workfront dentro de la implementación.

Este cambio puede afectar tanto a los inicios de sesión del usuario como a las integraciones de API:

* **Inicios de sesión del usuario**

  Si el dominio de su compañía no se incluye en la dirección URL de Workfront, ahora verá un nuevo campo Dominio en la pantalla de inicio de sesión, además de los campos Nombre de usuario y Contraseña.

  Para la mayoría de los clientes no se requiere ningún cambio, porque la información del dominio ya está incluida en la dirección URL de Workfront. Por ejemplo, “*dominio*.my.workfront.com”.

* **Integraciones de API**

  Si tiene algún código API que va a una dirección que no incluye su nombre de dominio, dicho código API ya no funcionará.

Para obtener más información, consulte [Iniciar sesión en Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Conversión de tareas y problemas en proyectos mediante la aplicación móvil en iOS

Ahora puede convertir tareas y problemas individuales en proyectos en la aplicación móvil de Workfront en iOS.

## Inicie sesión en la aplicación móvil con la huella digital o el identificador de rostro

Según el dispositivo, puede elegir iniciar sesión en la aplicación móvil de Workfront con la tecnología de huella digital o ID de rostro. Al iniciar sesión en la aplicación móvil, se preguntará al usuario si desea iniciar sesión con el método de autenticación que admite el teléfono.

Para obtener más información sobre cómo administrar esta característica, consulte [Adobe Workfront para iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) o [Adobe Workfront para Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## Nueva configuración para cerrar la sesión de los usuarios automáticamente en dispositivos móviles

Para que la aplicación móvil de Workfront sea más segura para los usuarios y para su compañía, la sesión de los usuarios se cerrará automáticamente tras 15 días de inactividad. Los administradores de Workfront pueden personalizar este límite de tiempo en la aplicación web, en Configuración > Sistema > Preferencias.

Para obtener más información, consulte [Configurar las preferencias de seguridad del sistema](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## La aplicación móvil requiere un dominio al iniciar sesión

Como mejora de seguridad, la aplicación móvil de Workfront ahora requiere que proporcione su dominio si no inicia sesión con credenciales de inicio de sesión único.

>[!NOTE]
>
>Disponibilidad de iOS: 12 de junio de 2019
>
>Disponibilidad de producción: 17 de junio de 2019

## Eliminar objetos mediante la aplicación móvil en iOS

>[!NOTE]
>
>Esta función estuvo disponible en las tiendas de aplicaciones para iOS la semana del 19 de agosto de 2019.

Ahora puede eliminar objetos como tareas, problemas y plantillas de horas en la aplicación móvil de iOS. Debe tener los permisos correctos sobre el objeto para eliminarlo.

## Filtrar por proyectos inactivos en la aplicación móvil

>[!NOTE]
>
>Esta función estará disponible en las tiendas de aplicaciones tanto para iOS como para Android la semana del 19 de agosto de 2019.

Hemos añadido Proyectos inactivos como opción de filtro en la pestaña Proyectos de la aplicación móvil.

## Restablecer la contraseña con la aplicación móvil

Puede usar la aplicación de Workfront Mobile para restablecer la contraseña si la ha olvidado. Pulse ¿Olvidó su contraseña? y siga las indicaciones de la pantalla. No puede restablecer su contraseña de SSO en la aplicación móvil.

## Nueva apariencia y experiencia para móviles

Hemos añadido las siguientes mejoras de Aspecto y presentación de las mejoras, su experiencia en la aplicación móvil de Workfront.

* Se han movido los siguientes elementos de la barra superior de la página Detalles a áreas más destacadas de la pantalla:

   * El icono &quot;+&quot; se encuentra ahora en la esquina inferior izquierda de la pantalla
   * La marca de verificación para comenzar a trabajar en un elemento ahora es un botón Trabajar en ello en la parte superior central de la pantalla

* Ahora puede ver los formularios personalizados adjuntos tocando Mostrar más en la parte inferior de la página Detalles.
* Se ha cambiado el aspecto de las páginas que usa para enviar tareas, problemas y solicitudes.

