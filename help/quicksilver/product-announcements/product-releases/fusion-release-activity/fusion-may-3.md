---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Actividad de la versión de Workfront Fusion: Semana del 3 de mayo de 2021"
description: Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 3 de mayo de 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: Semana del 3 de mayo de 2021

Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 3 de mayo de 2021.

Para obtener una lista de todos los cambios recientes, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obtener una lista de las correcciones de errores recientes en Workfront Fusion, consulte la página [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) y busque cualquier actualización denominada Actualización de mantenimiento de Workfront Fusion.

## Ahora, el conector Salesforce puede buscar mediante SOQL

El módulo Salesforce > Buscar registros ahora tiene la opción de buscar usando SOQL (Lenguaje de consulta de objetos de Salesforce). También puede buscar utilizando las opciones disponibles anteriormente (SOSL y búsquedas simples).

Para obtener más información, consulte [Módulos de Salesforce](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## El nuevo tipo de conexión en el conector de Azure DevOps requiere menos ámbitos

Para mejorar la seguridad, hemos agregado un nuevo tipo de conector al conector de desarrollo de Workfront Fusion Azure. Ahora, cuando crea una conexión en un módulo de Azure DevOps, puede seleccionar entre dos tipos de conexiones:

* Azure DevOps

  Este nuevo tipo de conexión limita los ámbitos a los que necesita específicamente Workfront Fusion.

* Azure DevOps (solicitar todos los ámbitos)

  Este es el tipo de conexión heredada, que solicita todos los ámbitos disponibles en una conexión a Azure DevOps.

Le recomendamos que utilice el tipo de conexión de Azure DevOps en todos los escenarios nuevos que utilicen Azure DevOps. También le recomendamos que cambie cualquier módulo de Azure DevOps en sus escenarios existentes para utilizar el nuevo tipo de conexión. El tipo de conexión heredada de Azure DevOps (Solicitar todos los ámbitos) quedará obsoleto en un futuro próximo.

Para obtener más información, consulte [Módulos de DevOps de Azure](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
