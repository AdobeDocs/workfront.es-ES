---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Corrija el día de inicio de la semana laboral para hojas de hora
description: El día de inicio de la semana en mi parte de horas no coincide con el día de inicio de la semana que está configurado en mi perfil de parte de horas.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Corrija el día de inicio de la semana laboral para hojas de hora

## Problema

El día de inicio de la semana en mi parte de horas no coincide con el día de inicio de la semana que está configurado en mi perfil de parte de horas (como se describe en [Crear, editar y asignar perfiles de parte de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solución

El día de inicio de la semana de un parte de horas en Adobe Workfront usa la configuración de idioma y configuración regional del explorador para determinar el día de la semana. Debido a esto, debe actualizar la configuración de idioma y configuración regional de su navegador. 

Por ejemplo, con el idioma del explorador configurado en inglés y la configuración regional establecida en Estados Unidos, la semana comienza el domingo. Alternativamente, el idioma del navegador establecido en inglés y la configuración regional establecida en Reino Unido, el día de inicio es lunes.

Esta configuración también afecta al día de inicio de la semana en los calendarios emergentes de todo el sistema.

El cambio de configuración regional no afecta al día de inicio de la semana en la cuadrícula de recursos (o vista de cuadrícula de recursos). La semana siempre comienza el domingo.

A continuación se indican las instrucciones para cambiar la configuración de idioma y configuración regional de varios navegadores compatibles con Workfront.

* **Chrome:** Copie y pegue el siguiente vínculo en el explorador Chrome: `chrome://settings/languages` a continuación, vaya a Idiomas.
* **Firefox:**Copie y pegue el siguiente vínculo en el navegador Firefox: `about:preferences#content` a continuación, vaya a Idiomas.
* **IE 11:** Herramientas -> Opciones de Internet -> General -> Idiomas
* **Safari:** Lamentablemente, Safari no permite cambiar los idiomas de navegación sin cambiar también el idioma completo del sistema operativo. Probablemente sea más fácil simplemente instalar otro navegador como Chrome o Firefox.

 
