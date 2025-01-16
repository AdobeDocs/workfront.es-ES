---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generación de un segmento de escenario mediante IA
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 24%

---

# Generación de un segmento de escenario mediante IA

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Generar un segmento de escenario mediante IA](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-module-with-ai.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Como esta función se encuentra en Beta, solo está disponible para algunos usuarios de Workfront.

Puede utilizar IA para escribir un mensaje de texto que describa lo que necesita que haga una sección del escenario. Fusion generará módulos que realizarán esas acciones, que puede utilizar en su escenario.

Al igual que con cualquier elemento generado a partir de IA, le recomendamos que compruebe y pruebe los módulos generados para asegurarse de que funcionan según lo previsto.

## Aplicaciones de módulo de IA admitidas actualmente

Fusion AI puede generar actualmente módulos que se conectan a las siguientes aplicaciones:

* Adobe Firefly
* Azure OpenAI
* Microsoft Graph
* Planificación de Adobe Workfront
* Adobe Analytics
* Servicios Adobe PDF
* Adobe Marketo
* Adobe Frame.io
* Dropbox
* NetSuite
* Google Calendar
* Atlassian Jira
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## Generar módulos

1. Empiece a agregar un módulo y seleccione **Generar con IA** de la lista de aplicaciones.

   O

   Haga clic en el icono Generar con IA ![Generar con IA](assets/generate-with-ai-icon-beta.png) cerca de la parte inferior de la página del editor de escenarios.

   Se abrirá el panel Ayudante de IA.
1. Escriba un mensaje de texto en el cuadro.

   Para obtener sugerencias para crear mensajes de texto, consulte [Sugerencias para crear solicitudes de texto](#tips-for-creating-text-prompts) en este artículo.

   El asistente de IA genera el módulo o conjunto de módulos.
1. (Condicional) Si es necesario, agregue el token de API para la aplicación en los módulos.
1. Compruebe los módulos para asegurarse de que están configurados para la aplicación y la acción adecuadas.
1. (Condicional) Si la sección de escenario generado no está adjunta al escenario, arrástrela a su lugar.

Se recomienda probar los módulos para asegurarse de que funcionan según lo previsto.

## Sugerencias para crear mensajes de texto

Los mensajes de texto deben incluir la siguiente información como mínimo:

* La aplicación a la que se está conectando
* La acción o acciones que desea realizar

>[!IMPORTANT]
>
>Puede generar más de un módulo a la vez, pero solo puede generar módulos para una aplicación a la vez.

>[!INFO]
>
>**Ejemplos**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>Esto incluye la aplicación `Workfront Planning` y la acción `delete records`. Este mensaje crea tres módulos, uno para cada registro que se eliminará.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>Esto incluye la aplicación `Workfront Planning` y la acción `change campaign summary`.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>Esto incluye la aplicación `Workfront Planning` y la acción `get field details`.
>
>El siguiente ejemplo NO es correcto:
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    Este ejemplo es incorrecto porque incluye varias aplicaciones

Tenga en cuenta lo siguiente al crear mensajes de texto:

* Utilice un lenguaje directo y sencillo.
* Compruebe y pruebe sus módulos. Si no funciona como se espera, perfeccione el mensaje e inténtelo de nuevo.
