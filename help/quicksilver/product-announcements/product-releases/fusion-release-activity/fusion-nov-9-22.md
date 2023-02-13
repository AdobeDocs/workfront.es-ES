---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Actividad de la versión de Workfront Fusion: Semana del 7 de noviembre de 2022'
description: En esta página se describen todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 7 de noviembre de 2022.
author: Luke
feature: Product Announcements, Workfront Fusion
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 9aaba3062bc5d1166c37821a6a3216f7f1d965b1
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: Semana del 7 de noviembre de 2022

**Optimización de la cola de enlace web**

La cola de enlaces web de Fusion se ha optimizado con esta versión. El servicio que acepta webhooks ahora está separado de la cola y otros procesos. Este cambio permite que Fusion procese las colas de weblock a una velocidad más rápida y coherente.

Durante la implementación de este cambio, pudimos comprender mejor el tiempo esperado de procesamiento de registros para los eventos de weblock en cola. Se espera que la página del visor de enlaces web de Fusion no tenga más de 1 minuto.

Para ver los eventos de enlace web en cola, vaya a Webhooks, en la navegación izquierda. Los iconos del camión con un número en el numerador indican eventos de cola para ese enlace web. Haga clic en el icono del camión para ver los eventos en cola.

![](assets/fusion-webhook-queue-1866x567.png)


**Los enlaces web no utilizados ahora se desactivarán o eliminarán**

Hemos realizado algunos cambios en la forma en que Workfront Fusion gestiona los enlaces web no utilizados. Ahora, los Webhooks se desactivan automáticamente si se aplica cualquiera de las siguientes opciones:

* El enlace web no ha estado conectado a ningún escenario durante más de 5 días.
* El enlace web solo se utiliza en escenarios inactivos, que han estado inactivos durante más de 30 días.

Los enlaces web desactivados se eliminan y no se registran automáticamente si no están conectados a ningún escenario y han estado en estado desactivado durante más de 30 días.
