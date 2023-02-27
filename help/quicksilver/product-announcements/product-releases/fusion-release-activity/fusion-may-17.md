---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Actividad de la versión de Workfront Fusion: Semana del 17 de mayo de 2021'
description: En esta página se describen todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 17 de mayo de 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 930c335e-2c88-41af-983f-82be790c1a4b
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: semana del 17 de mayo de 2021

En esta página se describen todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 17 de mayo de 2021.

Para obtener una lista de todos los cambios recientes, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obtener una lista de las correcciones de errores recientes en Workfront Fusion, consulte la [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) y compruebe si hay actualizaciones etiquetadas como Actualización de mantenimiento de Workfront Fusion.

## Copiar módulos en situaciones de Workfront Fusion

Para facilitar el trabajo con los escenarios de fusión de Workfront, hemos hecho posible copiar y pegar módulos. Ahora, puede copiar un módulo o un grupo de módulos y pegarlos en el mismo escenario o en otro. Al copiar módulos, se conservan los valores de campo de ese módulo.

Para obtener más información, consulte [Copiar módulos o escenarios en Adobe Workfront Fusion](../../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

## Seleccionar varios módulos en un escenario de Workfront Fusion

Ahora, al editar un escenario, puede seleccionar varios módulos a la vez. A continuación, puede realizar acciones masivas en los módulos seleccionados.

* Copiar
* Mover
* Eliminar

Al copiar y mover módulos, se conservan los valores del módulo y cualquier línea que conecte los módulos.

Para obtener más información sobre los escenarios de edición, consulte [Crear un escenario en Adobe Workfront Fusion](../../../workfront-fusion/scenarios/create-a-scenario.md).

## Los módulos ahora conservan la información no guardada

Para facilitar la creación de escenarios, hemos hecho posible que los módulos conserven los valores de campo cuando no están enfocados. Ahora, cuando hace clic fuera de un módulo sin guardarlo y vuelve a él, los campos muestran los valores introducidos anteriormente. Cuando se cierra el módulo, se muestra un indicador de que hay campos no guardados.

## El conector de Azure AD ahora gestiona los registros nuevos y actualizados por separado

Los nuevos registros y actualizaciones de registros existentes ahora se gestionan mediante módulos independientes.

* Para buscar registros nuevos, puede utilizar el módulo déclencheur Registros de observación . Este módulo ya no ve registros actualizados.
* Para obtener registros actualizados, puede utilizar el nuevo módulo Buscar usuarios/Grupos Delta. Este módulo devuelve registros nuevos, actualizados y eliminados.

Para obtener más información, consulte [Módulos de Azure Active Directory](../../../workfront-fusion/apps-and-their-modules/azure-ad-modules.md).
