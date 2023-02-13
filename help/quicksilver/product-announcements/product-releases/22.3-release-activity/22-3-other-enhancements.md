---
title: otras actualizaciones durante el intervalo de tiempo de la versión 2.3
description: otras actualizaciones durante el intervalo de tiempo de la versión 2.3
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 22.3 Otras mejoras

En esta página se describen todas las demás mejoras realizadas con la versión 2.3 del entorno de vista previa. Estas mejoras estaban disponibles en el entorno Producción durante la semana del 11 de julio de 2022. Para obtener una lista de todos los cambios disponibles con la versión 2.3, consulte [Información general sobre la versión 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Hojas de horas actualizadas

Seguimos mejorando y actualizando su experiencia al trabajar con partes de horas. Las siguientes son algunas de las funciones incluidas en esta actualización:

* Un nuevo aspecto que se adapta a la nueva experiencia de Workfront.

* Funcionalidad de guardado automático para guardar automáticamente las horas y comentarios de hora registrados en el momento en que los agregue.

* Un diseño de página más intuitivo que coincida con otras páginas de objeto. Por ejemplo, hemos agregado un panel izquierdo al parte de horas. Las actualizaciones del parte de horas ahora se muestran en la sección Actualizaciones del panel izquierdo. También puede eliminar un parte de horas de la página parte de horas, así como agregar el parte de horas a la lista Favoritos.

* Una mejor experiencia al buscar y agregar proyectos, tareas o problemas al parte de horas. Esto coincide con la experiencia de todas las demás listas de Workfront.

* El panel Resumen está disponible para tareas y problemas para agregar comentarios o actualizar información directamente desde el parte de horas.


Con la actualización actual, también se han desaprobado las siguientes funciones:

* Se ha eliminado la creación de una tarea a partir de una actualización. Esta función se ha eliminado desde la versión 2018.2 de las áreas Actualizaciones de todos los demás objetos, pero aún estaba disponible en la secuencia de actualización de hojas de horas.

* El &quot;Añadir gastos de un parte de horas&quot;. &quot;se ha eliminado la preferencia del área Preferencias de horario y parte de horas de Configuración y ya no puede registrar gastos desde el parte de horas. Aún puede registrar los gastos desde las páginas de tarea y proyecto.


Para obtener más información, consulte los siguientes artículos:

* [Comprender el diseño de la hoja de horas](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Configuración de las preferencias de horas y horas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Mejoras en el panel de navegación izquierdo

Se han realizado varias mejoras en el panel de navegación izquierdo de Adobe Workfront.

* El aspecto del panel de navegación izquierdo se actualizó a los estándares de diseño de Adobe, incluyendo colores y fuentes.

* Se ha cambiado el nombre del vínculo &quot;Agregar sección personalizada&quot; en la parte inferior del panel a &quot;Agregar tablero&quot; para explicar mejor su función.

## Habilitar la rotación automática del token de actualización en sus aplicaciones OAuth2 personalizadas

Para permitirle controlar mejor la seguridad de sus aplicaciones OAuth2 personalizadas, hemos agregado la opción a para habilitar la rotación de tokens de actualización. Cuando esta opción está habilitada, cada vez que se utiliza un token de actualización, la aplicación crea y envía automáticamente un nuevo token de actualización y deshabilita el antiguo.

La aplicación debe almacenar el nuevo token de actualización después de cada actualización. Workfront no almacena este token de actualización.

Anteriormente, los tokens de actualización caducaban después de una cantidad de tiempo establecida configurada en la configuración personalizada de la aplicación OAuth2.

Para obtener más información, consulte [Creación de aplicaciones OAuth2 para integraciones de Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Utilice PKCE en sus integraciones personalizadas de OAuth2 para aplicaciones web de una sola página

Ahora puede crear aplicaciones web de una sola página en sus integraciones personalizadas con PKCE. PKCE es un flujo de autorización seguro que funciona bien con aplicaciones que se actualizan dinámicamente, como aplicaciones móviles, pero que es valioso en todos los clientes de OAuth2. En lugar de un secreto de cliente estático, PKCE utiliza una cadena generada dinámicamente, eliminando el riesgo de que se filtre un secreto de cliente.

Anteriormente, las opciones disponibles para aplicaciones OAuth2 personalizadas utilizaban el nombre y la contraseña de un usuario o un secreto de cliente.

Para obtener más información, consulte [Creación de aplicaciones OAuth2 para integraciones de Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
