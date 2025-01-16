---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Información general sobre los escenarios de Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 54%

---

# Información general sobre los escenarios de [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Descripción general del escenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere una licencia de [!DNL Adobe Workfront Fusion] además de [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>Los escenarios de [!DNL Workfront Fusion] no deben confundirse con escenarios de [!DNL Workfront Scenario Planner]. Para obtener información sobre los escenarios de [!DNL Workfront Scenario Planner], consulte [Información general sobre [!DNL Scenario Planner] ](../../scenario-planner/scenario-planner-overview.md).

La función de [!DNL Adobe Workfront Fusion] es automatizar sus procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas tareas una y otra vez. Funciona vinculando acciones dentro de las aplicaciones y servicios y entre ellos para crear un escenario que transfiera y transforme los datos automáticamente. El escenario que crea ve los datos de una aplicación o servicio y los procesa para proporcionar el resultado deseado.

Un escenario se compone de una serie de módulos que indican cómo se deben transformar los datos dentro de una aplicación o transferirse entre aplicaciones y servicios web.

## Información general sobre elementos de escenario

Se crea un escenario de diferentes elementos. Entender la terminología de estos elementos facilita el uso de la documentación.

### Escenario

Un **escenario** es una serie de pasos automatizados creados por el usuario para mover y manipular datos. El término &quot;escenario&quot; hace referencia a todo el grupo de pasos conectados.

![Escenario](assets/entire-scenario-scenario.png)

### Activador

Un escenario comienza con un **déclencheur**. El déclencheur inspecciona la existencia de datos nuevos y actualizados e inicia el escenario cuando se aplican determinadas condiciones configuradas en el módulo. Los déclencheur se pueden configurar para que inicien un escenario según una programación (sondeo) o siempre que se produzcan cambios en los datos (instantáneo).

![Déclencheur](assets/scenario-trigger.png)

### Módulo

El déclencheur va seguido de **módulos**. Un módulo representa un solo paso en un escenario que realiza una acción específica. Los módulos se configuran y encadenan para crear escenarios.

![Módulo](assets/scenario-module.png)

### Ruta

Un escenario se puede dividir en **rutas**. Una ruta es una sección del escenario que puede utilizarse o no para un conjunto determinado de datos. Las rutas se configuran mediante un módulo de enrutador y filtros.

![Ruta](assets/scenario-route.png)

### Segmento de escenario

Un segmento de escenario es una sección de un escenario que consta de una serie de módulos contiguos que se conectan a la misma aplicación. Los segmentos de escenario suelen representar un flujo de trabajo corto en la aplicación.

![Segmento de escenario](assets/scenario-segment.png)

### Conector

Un conector es el conjunto de módulos de una aplicación determinada. Workfront Fusion ofrece conectores a muchas aplicaciones de trabajo comunes, como Workfront, Salesforce y Jira, así como conectores genéricos que pueden utilizarse para cualquier servicio web.

![Conectores](assets/scenario-connectors.png)



## Ejemplo: automatización de procesos en [!DNL Adobe Workfront]

>[!NOTE]
>
>Esta funcionalidad está disponible para las siguientes licencias:
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation]
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]

[!DNL Workfront Fusion] le permite automatizar flujos de trabajo simples o complejos en [!DNL Workfront], lo que ahorra tiempo y garantiza que el proceso se ejecute de manera coherente.

En este ejemplo, el escenario se activa cuando un campo especificado cambia en una tarea o problema en [!DNL Workfront]. Cuando se activa, el escenario obtiene información del proyecto relacionado y crea una actualización adaptada para una persona asignada a una función específica en el proyecto.

![](assets/fusion-template-example-350x102.png)

## Ejemplo: conectar [!DNL Workfront] a otra aplicación o servicio web

>[!NOTE]
>
>Esta funcionalidad está disponible para la siguiente licencia:
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]
>

[!DNL Workfront Fusion] también puede conectarse a otras aplicaciones y servicios web. Puede acceder, importar, manipular o exportar datos de otras aplicaciones, integrándolos con Workfront o entre sí. Muchas aplicaciones tienen conectores de [!DNL Workfront Fusion] dedicados. Si no hay ningún conector dedicado para la aplicación a la que desee acceder, puede usar los módulos [!UICONTROL HTTP] o [!UICONTROL SOAP] de [!DNL Workfront Fusion] para conectarse a la aplicación a través de su API.

En este ejemplo, el escenario se activa cuando se añade un usuario a una hoja de cálculo de [!DNL Excel]. El escenario comprueba si el usuario está en [!DNL Workfront]. Si no es así, el escenario creará el usuario en [!DNL Workfront] y volverá a añadir su ID de usuario de Workfront a la hoja de cálculo.

![](assets/fusion-integration-example--350x171.png)

Para obtener una lista de conectores dedicados, consulte [Aplicaciones y sus módulos](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] puede conectarse a casi cualquier servicio web. Si la aplicación con la que desea trabajar no tiene un conector de [!DNL Workfront Fusion] dedicado, puede utilizar los siguientes módulos para conectarse directamente al servicio web:
>
>* Módulos [[!UICONTROL HTTP]](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* ](../../workfront-fusion/apps-and-their-modules/soap-module.md)Módulo [[!UICONTROL SOAP]
>* Módulos [[!UICONTROL JSON]](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
