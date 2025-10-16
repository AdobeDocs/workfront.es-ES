---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Corregir el día de inicio de la semana laboral para las hojas de horas
description: El día de inicio de semana en mi hoja de horas no coincide con el día de inicio semanal esperado.
author: Lisa
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 5%

---

# Corregir el día de inicio de la semana laboral para las plantillas de horas

<!--Audited: 5/2025-->

## Problema

El día de inicio de semana en mi hoja de horas no coincide con el día de inicio semanal esperado.

Esto suele ocurrir cuando no se le asigna un perfil de hoja de horas y la hoja de horas se ha creado manualmente.


## Solución

El administrador de Workfront debe crear perfiles de hojas de horas y asignar a todos a un perfil, tal como se describe en [Crear, editar y asignar perfiles de hojas de horas](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). El administrador de Workfront puede definir la fecha de inicio de una plantilla de horas en un día distinto a la fecha de inicio semanal prevista. Hable con ellos para averiguar cuál es la fecha de inicio de un perfil de hoja de horas para su hoja de horas.

Si la hoja de horas se creó manualmente, el día de inicio de la semana en la hoja de horas usa la configuración Configuración regional de correo electrónico del perfil del usuario, tal como se describe en el artículo [Configurar mi configuración](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Por ejemplo, con la Configuración regional de correo electrónico establecida en Inglés (Estados Unidos), la semana en la plantilla de horas comienza el domingo. Como alternativa, con la Configuración regional de correo electrónico establecida en Inglés (Reino Unido), la semana en la plantilla de horas comienza en lunes.


<!--This is the old content for this article but I found this was not working this way at all, so I changed it to what it is today: 

## Problem

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solution

The start day of the week of a timesheet in Adobe Workfront uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser. 

For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.

This setting also affects the start day of the week in the pop-up calendars across the system.

The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always starts on Sunday.

Following are the directions for changing language and locale settings for various browsers that are supported with Workfront.

* **Chrome:** Copy and paste the following link into your Chrome browser: `chrome://settings/languages` then go to Languages.
* **Firefox:**Copy and paste the following link into your Firefox browser: `about:preferences#content` then go to Languages.
* **IE 11:** Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.

-->


