---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Información general sobre Adobe Workfront Fusion
description: Adobe Workfront Fusion requiere una licencia Adobe Workfront Fusion además de una licencia Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 27158301e491d4ff45ce7987a81f841fb4525b2a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Resumen del escenario [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere una licencia de [!DNL Adobe Workfront Fusion] además de [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] escenarios no deben confundirse con [!DNL Workfront Scenario Planner] escenarios. Para obtener información sobre [!DNL Workfront Scenario Planner] escenarios, consulte [La [!DNL Scenario Planner] descripción general](../../scenario-planner/scenario-planner-overview.md).

La función de [!DNL Adobe Workfront Fusion] es automatizar sus procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas tareas una y otra vez. Funciona vinculando acciones dentro de las aplicaciones y servicios y entre ellos para crear un escenario que transfiera y transforme los datos automáticamente. El escenario que cree inspecciona los datos de una aplicación o servicio y procesa esos datos para proporcionar el resultado deseado.

Un escenario se compone de una serie de módulos que indican cómo se deben transformar los datos dentro de una aplicación o transferirlos entre aplicaciones y servicios web.

## Ejemplo: Automatización de procesos en [!DNL Adobe Workfront]

>[!NOTE]
>
>Esta funcionalidad está disponible para las siguientes licencias:
>
>* [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]
>* [!UICONTROL [!DNL Workfront Fusion] para la automatización e integración de trabajo]

[!DNL Workfront Fusion] le permite automatizar flujos de trabajo simples o complejos en [!DNL Workfront], lo que ahorra tiempo y garantiza que el proceso se ejecute de manera consistente.

En este ejemplo, el escenario entra en déclencheur cuando un campo especificado cambia en una tarea o problema en [!DNL Workfront]. Cuando se activa, el escenario obtiene información en el proyecto relacionado y crea una actualización adaptada para una persona asignada a una función específica en el proyecto.

![](assets/fusion-template-example-350x102.png)

## Ejemplo: conectar [!DNL Workfront] a otra aplicación o servicio web

>[!NOTE]
>
>Esta funcionalidad está disponible para la siguiente licencia:
>
>* [!UICONTROL [!DNL Workfront Fusion] para la automatización e integración de trabajo]
>

[!DNL Workfront Fusion] también puede conectarse a otras aplicaciones y servicios web. Puede acceder, importar, manipular o exportar datos de otras aplicaciones, integrándolos con Workfront o entre sí. Muchas aplicaciones tienen conectores [!DNL Workfront Fusion] dedicados. SOAP Si no hay ningún conector dedicado para la aplicación a la que desee tener acceso, puede usar los módulos [!UICONTROL HTTP] o  de [!DNL Workfront Fusion] para conectarse a la aplicación a través de su API.

En este ejemplo, el escenario entra en déclencheur cuando se agrega un usuario a una hoja de cálculo de [!DNL Excel]. El escenario comprueba si el usuario está en [!DNL Workfront]. Si no es así, el escenario creará el usuario en [!DNL Workfront] y volverá a agregar su ID de usuario de Workfront a la hoja de cálculo.

![](assets/fusion-integration-example--350x171.png)

Para obtener una lista de conectores dedicados, consulte [Aplicaciones y sus módulos](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] puede conectarse a casi cualquier servicio web. Si la aplicación con la que desea trabajar no tiene un conector [!DNL Workfront Fusion] dedicado, puede utilizar los siguientes módulos para conectarse directamente al servicio web:
>
>* [[!UICONTROL módulos HTTP]](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* SOAP [[!UICONTROL módulo ] {20000000001000000000000000000000000000000000000000000000000000000 00000000000000000000000000000000000000000000000000000000000000000000000000000000](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL módulos JSON]](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
