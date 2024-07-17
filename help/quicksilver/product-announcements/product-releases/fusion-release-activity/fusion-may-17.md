---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Actividad de la versión de Workfront Fusion: Semana del 17 de mayo de 2021"
description: Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 17 de mayo de 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 930c335e-2c88-41af-983f-82be790c1a4b
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: Semana del 17 de mayo de 2021

Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 17 de mayo de 2021.

Para obtener una lista de todos los cambios recientes, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obtener una lista de las correcciones de errores recientes en Workfront Fusion, consulte la página [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) y busque cualquier actualización denominada Actualización de mantenimiento de Workfront Fusion.

## Copia de módulos en escenarios de Workfront Fusion

Para facilitar el trabajo con sus escenarios de Workfront Fusion, hemos hecho posible copiar y pegar módulos. Ahora puede copiar un módulo o un grupo de módulos y pegarlos en el mismo escenario o en uno diferente. Al copiar módulos, se conservan los valores de campo de ese módulo.

Para obtener más información, consulte [Copiar módulos o escenarios en Adobe Workfront Fusion](../../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

## Selección de varios módulos en un escenario de Workfront Fusion

Ahora, al editar un escenario, puede seleccionar varios módulos a la vez. A continuación, puede realizar acciones masivas en los módulos seleccionados.

* Copiar
* Mover
* Eliminar

Al copiar y mover módulos, se conservan los valores de los módulos y las líneas que los conectan.

Para obtener más información sobre la edición de escenarios, consulte [Crear un escenario en Adobe Workfront Fusion](../../../workfront-fusion/scenarios/create-a-scenario.md).

## Los módulos ahora conservan la información no guardada

Para facilitar la creación de escenarios, hemos hecho posible que los módulos conserven los valores de campo cuando no están enfocados. Ahora, cuando hace clic fuera de un módulo sin guardarlo y vuelve a él, los campos muestran los valores introducidos anteriormente. Cuando el módulo está cerrado, muestra un indicador de que hay campos sin guardar.

## El conector de Azure AD ahora administra registros nuevos y actualizados por separado

Los nuevos registros y las actualizaciones de los registros existentes ahora se administran mediante módulos independientes.

* Para inspeccionar registros nuevos, puede utilizar el módulo de déclencheur Observar registros. Este módulo ya no inspecciona los registros actualizados.
* Para obtener registros actualizados, puede utilizar el nuevo módulo Delta de Buscar usuarios/grupos. Este módulo devuelve registros nuevos, actualizados y eliminados.

Para obtener más información, vea [Módulos de Active Directory de Azure](../../../workfront-fusion/apps-and-their-modules/azure-ad-modules.md).
