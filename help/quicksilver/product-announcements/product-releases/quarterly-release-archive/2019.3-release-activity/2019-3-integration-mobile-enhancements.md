---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 Integración y mejoras móviles
description: Esta página describe todos los cambios realizados en la integración y las mejoras móviles realizadas con la versión 2019.3. Estaba disponible en el entorno de producción la semana del 19 de agosto de 2019.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 2019.3 Integración y mejoras móviles

Esta página describe todos los cambios realizados en la integración y las mejoras móviles realizadas con la versión 2019.3. Estaba disponible en el entorno de producción la semana del 19 de agosto de 2019.

Para obtener una lista de todos los cambios realizados en 2019.3, consulte [Resumen de la actividad de la versión 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Compatibilidad con elementos compartidos en la integración de MS OneDrive

Ahora puede vincular los archivos y carpetas compartidos de OneDrive a objetos de Workfront. Por el contrario, puede cargar archivos en Workfront en carpetas compartidas de OneDrive.

Para obtener más información, consulte las secciones [Vincular un documento externo a Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Vincular una o más carpetas externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder) y [Actualizar y vincular un documento de Workfront a un proveedor de nube externo](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) en el artículo [Vincular documentos de aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Para obtener más información, consulte la sección [Vincular un documento externo a Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) en el artículo [Vincular documentos de aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Especificación de dominio necesaria para todos los inicios de sesión de Workfront

Ahora, todos los inicios de sesión de Workfront requieren que el usuario especifique el dominio si este no se ha especificado ya en la URL de Workfront. Si necesita esta información, la instancia de Workfront será más segura. Además, si la implementación de Workfront tiene varias instancias, esta mejora le permite agregar el mismo usuario a cada instancia de Workfront dentro de la implementación.

Este cambio puede afectar tanto a los inicios de sesión del usuario como a las integraciones de API:

* **Inicios de sesión de usuario**

  Si el dominio de su empresa no se incluye en la dirección URL de Workfront, ahora verá un nuevo campo Dominio en la pantalla de inicio de sesión, además de los campos Nombre de usuario y Contraseña.

  Para la mayoría de los clientes, no se requiere ningún cambio porque la información del dominio ya está incluida en la dirección URL de Workfront. Por ejemplo, &quot;*dominio*.my.workfront.com.&quot;

* **integraciones de API**

  Si tiene algún código API que va a una dirección que no incluye su nombre de dominio, ese código API ya no funcionará.

Para obtener más información, consulte [Iniciar sesión en Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Conversión de tareas y problemas en proyectos mediante la aplicación móvil en iOS

Ahora puede convertir tareas y problemas individuales en proyectos en la aplicación móvil de Workfront en iOS.

## Inicie sesión en la aplicación móvil con la huella digital o el identificador de rostro

Según el dispositivo, puede elegir iniciar sesión en la aplicación móvil de Workfront con la tecnología de huella digital o ID de rostro. Al iniciar sesión en la aplicación móvil, se le preguntará si desea iniciar sesión con el método de autenticación que admita el teléfono.

Para obtener más información sobre cómo administrar esta característica, consulte [Adobe Workfront para iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) o [Adobe Workfront para Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## Nueva configuración para cerrar la sesión de los usuarios automáticamente en dispositivos móviles

Para que la aplicación móvil de Workfront sea más segura para usted y para su empresa, la sesión de los usuarios se cerrará automáticamente tras 15 días de inactividad. Los administradores de Workfront pueden personalizar este límite de tiempo en la aplicación web, en Configuración > Sistema > Preferencias.

Para obtener más información, consulte [Configurar las preferencias de seguridad del sistema](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## La Aplicación Móvil Requiere Un Dominio Al Iniciar Sesión

Como mejora de seguridad, la aplicación móvil de Workfront ahora requiere que proporcione su dominio si no inicia sesión con credenciales de inicio de sesión único.

>[!NOTE]
>
>Disponibilidad de iOS: 12 de junio de 2019
>
>Disponibilidad de producción: 17 de junio de 2019

## Eliminación de objetos mediante la aplicación móvil en iOS

>[!NOTE]
>
>Esta función estuvo disponible en las tiendas de aplicaciones para iOS la semana del 19 de agosto de 2019.

Ahora puede eliminar objetos como tareas, problemas y plantillas de horas en la aplicación móvil de iOS. Debe tener los permisos correctos en el objeto para eliminarlo.

## Filtrar por proyectos inactivados en la aplicación móvil

>[!NOTE]
>
>Esta función estará disponible en las tiendas de aplicaciones tanto para iOS como para Android la semana del 19 de agosto de 2019.

Hemos añadido Proyectos inactivados como opción de filtro en la pestaña Proyectos de la aplicación móvil.

## Restablecer la contraseña con la aplicación móvil

Puede usar la aplicación de Workfront Mobile para restablecer la contraseña si la ha olvidado. Pulse ¿Olvidó su contraseña? y siga las indicaciones de la pantalla. No puede restablecer su contraseña de SSO en la aplicación móvil.

## Nueva apariencia para dispositivos móviles

Hemos añadido las siguientes mejoras de aspecto para mejorar su experiencia en la aplicación móvil de Workfront.

* Se han movido los siguientes elementos de la barra superior de la página Detalles a áreas más destacadas de la pantalla:

   * El icono &quot;+&quot; se encuentra ahora en la esquina inferior izquierda de la pantalla
   * La marca de verificación para comenzar a trabajar en un elemento ahora es un botón Trabajar en ello en la parte superior central de la pantalla

* Ahora puede ver los formularios personalizados adjuntos tocando Mostrar más en la parte inferior de la página Detalles.
* Se ha cambiado el aspecto de las páginas que usa para enviar tareas, problemas y solicitudes.

