---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Resumen del escenario de Adobe Workfront Fusion
description: Adobe Workfront Fusion requiere una licencia de Adobe Workfront Fusion además de una licencia de Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] información general del escenario

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere un [!DNL Adobe Workfront Fusion] además de una [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] los escenarios no deben confundirse con [!DNL Workfront Scenario Planner] escenarios. Para obtener información sobre [!DNL Workfront Scenario Planner] escenarios, consulte [La variable [!DNL Scenario Planner] información general](../../scenario-planner/scenario-planner-overview.md).

El papel de [!DNL Adobe Workfront Fusion] es automatizar los procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas tareas una y otra vez. Funciona vinculando acciones dentro de y entre aplicaciones y servicios para crear un escenario que transfiera y transforme sus datos automáticamente. El escenario que cree observa los datos en una aplicación o servicio y procesa esos datos para proporcionar el resultado deseado.

Un escenario consta de una serie de módulos que indican cómo se deben transformar los datos dentro de una aplicación o transferirlos entre aplicaciones y servicios web.

## Ejemplo: Automatización de procesos dentro de [!DNL Adobe Workfront]

>[!NOTE]
>
>Esta funcionalidad está disponible para las siguientes licencias:
>
>* [!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]
>* [!UICONTROL [!DNL Workfront Fusion] para la automatización e integración del trabajo]
>


[!DNL Workfront Fusion] permite automatizar flujos de trabajo simples o complejos en [!DNL Workfront], lo que ahorra tiempo y garantiza que el proceso se ejecute de forma coherente.

En este ejemplo, el escenario déclencheur cuando un campo especificado cambia en una tarea o problema en [!DNL Workfront]. Cuando se activa, el escenario obtiene información en el proyecto relacionado y crea una actualización personalizada para una persona asignada a una función específica en el proyecto.

![](assets/fusion-template-example-350x102.png)

## Ejemplo: Conexión [!DNL Workfront] a otra aplicación o servicio web

>[!NOTE]
>
>Esta funcionalidad está disponible para la siguiente licencia:
>
>* [!UICONTROL [!DNL Workfront Fusion] para la automatización e integración del trabajo]
>


[!DNL Workfront Fusion] también puede conectarse a otras aplicaciones y servicios web. Puede acceder, importar, manipular o exportar datos de otras aplicaciones, integrándolos con Workfront o entre sí. Muchas aplicaciones están dedicadas a [!DNL Workfront Fusion] conectores. Si no hay ningún conector específico para la aplicación a la que desee acceder, puede utilizar [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] o [!UICONTROL SOAP] para conectarse a la aplicación a través de su API.

En este ejemplo, el escenario déclencheur cuando se agrega un usuario a un [!DNL Excel] hoja de cálculo. El escenario comprueba si el usuario se encuentra en [!DNL Workfront]. Si no es así, el escenario crea al usuario en [!DNL Workfront] y agrega su ID de usuario de Workfront de nuevo a la hoja de cálculo.

![](assets/fusion-integration-example--350x171.png)

Para obtener una lista de conectores dedicados, consulte [Aplicaciones y sus módulos](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] puede conectarse a casi cualquier servicio web. Si la aplicación con la que desea trabajar no tiene un [!DNL Workfront Fusion] , puede utilizar los siguientes módulos para conectarse directamente al servicio web:
>
>* [[!UICONTROL HTTP] módulos](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] módulo](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] módulos](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

