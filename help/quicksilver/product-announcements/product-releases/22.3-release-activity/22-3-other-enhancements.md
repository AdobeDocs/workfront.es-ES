---
title: otras actualizaciones durante el período de tiempo de la versión 22.3
description: otras actualizaciones durante el período de tiempo de la versión 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
TQID: https://experienceleague.adobe.com/mwNNzDV919eY8L3M7Be5cPyDB1IjetL-YSJETJ1bIGE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 577
ht-degree: 100%

---

# Otras mejoras de la versión 22.3

En esta página se describen todas las demás mejoras realizadas con la versión 22.3 en el entorno de Vista previa. Estas mejoras se incorporaron en el entorno de producción la semana del 11 de julio de 2022. Para obtener una lista de todos los cambios disponibles con la versión 22.3, consulte [Información general sobre la versión 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Plantillas de horas actualizadas

Seguimos mejorando y actualizando su experiencia al trabajar con plantillas de horas. Estas son algunas de las características incluidas en esta actualización:

* Una nueva apariencia que se adapta a la nueva experiencia de Workfront.

* Funcionalidad de guardado automático para guardar automáticamente las horas registradas y los comentarios de horas en el momento en que los añada.

* Un diseño de página más intuitivo para que coincida con otras páginas de objetos. Por ejemplo, hemos añadido un panel izquierdo a la plantilla de horas. Las actualizaciones de la plantilla de horas ahora se muestran en la sección Actualizaciones del panel izquierdo. También se puede eliminar una plantilla de horas de la página de plantilla de horas y añadirla a la lista Favoritos.

* Una mejor experiencia al buscar y añadir proyectos, tareas o problemas a la plantilla de horas. Esto coincide con la experiencia en todas las demás listas de Workfront.

* El panel Resumen está disponible para que las tareas y los problemas añadan comentarios o actualicen la información directamente desde la plantilla de horas.


Con la actualización actual, también han quedado obsoletas las siguientes funciones:

* Se ha eliminado la creación de una tarea a partir de una actualización. Esta función se ha eliminado desde la versión 2018.2 de las áreas de Actualizaciones de todos los demás objetos, pero aún estaba disponible en el flujo de actualización de la plantilla de horas.

* La preferencia &quot;Añadir gastos desde una plantilla de horas&quot; se ha eliminado de las áreas de plantilla de horas y preferencias de horas en Configuración, y ya no se pueden registrar gastos desde la plantilla de horas. Puede seguir registrando gastos desde las páginas de tareas y proyectos.


Para obtener más información, consulte los siguientes artículos:

* [Comprender el diseño de la plantilla de horas](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Configurar preferencias de plantilla de horas y de horas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Mejoras en el panel de navegación izquierdo

Hemos realizado varias mejoras en el panel de navegación izquierdo de Adobe Workfront.

* La apariencia del panel de navegación izquierdo se ha actualizado a los estándares de diseño de Adobe, incluidos los colores y las fuentes.

* Se ha cambiado el nombre del vínculo &quot;Agregar sección personalizada&quot; en la parte inferior del panel a &quot;Agregar panel de control&quot; para explicar mejor su función.

## Habilitar la rotación automática de tokens de actualización en las aplicaciones OAuth2 personalizadas

Para permitirle un mayor control sobre la seguridad de sus aplicaciones OAuth2 personalizadas, hemos agregado a la opción para habilitar la rotación de tokens de actualización. Cuando esta opción está habilitada, cada vez que se utiliza un token de actualización, la aplicación crea y envía automáticamente un nuevo token de actualización y deshabilita el anterior.

La aplicación debe almacenar el nuevo token después de cada actualización. Workfront no almacena este token de actualización.

Anteriormente, los tokens de actualización caducaban después de una cantidad de tiempo establecida en la configuración personalizada de la aplicación OAuth2.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Uso de PKCE en las integraciones personalizadas de OAuth2 para aplicaciones web de una sola página

Ahora puede crear aplicaciones web de una sola página en sus integraciones personalizadas mediante PKCE. PKCE es un flujo de autorización seguro que funciona bien con aplicaciones que se actualizan dinámicamente, como las aplicaciones móviles, pero que resulta útil en todos los clientes OAuth2. En lugar de un secreto de cliente estático, PKCE utiliza una cadena generada dinámicamente, lo que elimina el riesgo de que se filtre un secreto de cliente.

Anteriormente, las opciones disponibles para las aplicaciones OAuth2 personalizadas usaban el nombre y la contraseña de un usuario o un secreto de cliente.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
