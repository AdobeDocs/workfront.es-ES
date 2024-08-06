---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Corregir el día de inicio de la semana laboral para hojas de horas
description: El día de inicio de la semana en mi hoja de horas no coincide con el día de inicio de la semana configurado en mi perfil de hoja de horas.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Corregir el día de inicio de la semana laboral para hojas de horas

## Problema

El día de inicio de la semana en mi hoja de horas no coincide con el día de inicio de la semana configurado en mi perfil de hoja de horas (como se describe en [Crear, editar y asignar perfiles de hoja de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)).

## Solución

El día de inicio de la semana de una plantilla de horas en Adobe Workfront utiliza la configuración de idioma y configuración regional del explorador para determinar el día de la semana. Debido a esto, debe actualizar la configuración de idioma y configuración regional de su explorador.

Por ejemplo, con el idioma del explorador establecido en inglés y la configuración regional establecida en Estados Unidos, la semana comienza el domingo. Como alternativa, el idioma del explorador configurado en inglés y la configuración regional configurada en Reino Unido, el día de inicio es lunes.

Esta configuración también afecta al día de inicio de la semana en los calendarios emergentes de todo el sistema.

El cambio de configuración regional no afecta al día de inicio de la semana en la cuadrícula de recursos (o vista de cuadrícula de recursos). La semana siempre empieza el domingo.

A continuación se indican las instrucciones para cambiar la configuración regional y de idioma de varios exploradores compatibles con Workfront.

* **Chrome:** Copie y pegue el siguiente vínculo en el explorador Chrome: `chrome://settings/languages` y, a continuación, vaya a Idiomas.
* **Firefox:**Copie y pegue el siguiente vínculo en el explorador Firefox: `about:preferences#content` y, a continuación, vaya a Idiomas.
* **IE 11:** Herramientas -> Opciones de Internet -> General -> Idiomas
* **Safari:** Lamentablemente, Safari no permite cambiar los idiomas de exploración web sin cambiar también todo el idioma del sistema operativo. Probablemente sea más fácil simplemente instalar otro navegador como Chrome o Firefox.


