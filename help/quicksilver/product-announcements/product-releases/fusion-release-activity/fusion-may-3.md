---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Actividad de la versión de Workfront Fusion: Semana del 3 de mayo de 2021'
description: En esta página se describen todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 3 de mayo de 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 9c2321794c5ba773bfda1d6e9dfda6b8de1a1449
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: semana del 3 de mayo de 2021

En esta página se describen todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 3 de mayo de 2021.

Para obtener una lista de todos los cambios recientes, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obtener una lista de las correcciones de errores recientes en Workfront Fusion, consulte la [Actualizaciones de mantenimiento de Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) y compruebe si hay actualizaciones etiquetadas como Actualización de mantenimiento de Workfront Fusion.

## El conector Salesforce ahora puede buscar utilizando SOQL

El módulo Salesforce > Buscar registros ahora tiene la opción de buscar mediante SOQL (Salesforce Object Query Language). También puede buscar utilizando las opciones disponibles anteriormente (SOSL y búsquedas simples).

Para obtener más información, consulte [Módulos de Salesforce](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## El nuevo tipo de conexión en el conector DevOps de Azure requiere menos ámbitos

Para mejorar la seguridad, se ha agregado un nuevo tipo de conector al conector DevOps de Workfront Fusion Azure. Ahora, al crear una conexión en un módulo de DevOps de Azure, puede seleccionar entre dos tipos de conexiones:

* Operaciones de desarrollo de Azure

   Este nuevo tipo de conexión limita los ámbitos a los que Workfront Fusion necesita específicamente.

* Operaciones de desarrollo de Azure (Solicitar todos los ámbitos)

   Este es el tipo de conexión heredado, que solicita todos los ámbitos disponibles en una conexión con Azure DevOps.

Le recomendamos que utilice el tipo de conexión de DevOps de Azure en todos los casos nuevos que usen las operaciones de desarrollo de Azure. También le recomendamos que cambie cualquier módulo de Azure DevOps en sus escenarios existentes para usar el nuevo tipo de conexión. El tipo de conexión de Azure DevOps (solicitud de todos los ámbitos) heredado quedará obsoleto en un futuro próximo.

Para obtener más información, consulte [Módulos de DevOps de Azure](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
