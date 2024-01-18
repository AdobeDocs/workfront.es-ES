---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Actividad de la versión de Workfront Fusion: Semana del 7 de noviembre de 2022"
description: Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 7 de noviembre de 2022.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: Semana del 7 de noviembre de 2022

**Optimización de cola de webhook**

La cola de ganchos web de Fusion se ha optimizado con esta versión. El servicio que acepta webhooks ahora está separado de la cola y otros procesos. Este cambio hace posible que Fusion procese las colas de los ganchos web a una velocidad más rápida y coherente.

Durante la implementación de este cambio, pudimos comprender mejor el tiempo de procesamiento de registros esperado para los eventos de ganchos web en cola. Se espera que la página del visor de ganchos web de Fusion no tenga más de 1 minuto.

Para ver los eventos de webhook en cola, vaya a Webhooks, en la navegación de la izquierda. Los iconos de los camiones con un número en el numerador indican eventos de cola para ese webhook. Haga clic en el icono del camión para ver los eventos en cola.

![](assets/fusion-webhook-queue-1866x567.png)


**Los webhooks que no se usen ahora se desactivarán o eliminarán**

Hemos realizado algunos cambios en la forma en que Workfront Fusion gestiona los webhooks que no se utilizan. Ahora, los webhooks se desactivan automáticamente si se aplica cualquiera de las siguientes opciones:

* El webhook no ha estado conectado a ningún escenario durante más de 5 días.
* El webhook solo se utiliza en escenarios inactivos, que han estado inactivos durante más de 30 días.

Los webhooks desactivados se borran y no se registran automáticamente si no están conectados a ningún escenario y han estado en estado desactivado durante más de 30 días.
