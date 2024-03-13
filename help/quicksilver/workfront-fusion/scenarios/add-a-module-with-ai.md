---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generación de un módulo mediante IA
description: Puede introducir un mensaje de texto para crear un módulo HTTP configurado para el mensaje.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: 5623ca255478757c58605d05f2f24e56b21a5d78
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 1%

---

# Generación de un módulo mediante IA

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Debido a que esta función aún se encuentra en las primeras etapas de desarrollo, solo está disponible para usuarios internos de Workfront.

Puede utilizar IA para escribir un mensaje de texto que describa lo que necesita que haga un módulo. Fusion generará entonces un módulo HTTP que se conectará al punto final correcto de la API deseada.

Al igual que con cualquier elemento generado a partir de IA, le recomendamos que compruebe y pruebe el módulo generado para asegurarse de que funciona según lo previsto.

## Aplicaciones de módulo de IA admitidas actualmente

Fusion AI puede generar actualmente módulos que se conectan a las siguientes aplicaciones:

* Adobe Maestro
* Adobe Analytics
* Servicios de Adobe PDF
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

## Generar un módulo

1. Añada un módulo y seleccione **Generar con IA** de la lista de aplicaciones.

   O

   Haga clic con el botón derecho en un área en blanco del editor de escenarios y seleccione **Generar con IA**.
1. Escriba un mensaje de texto en el cuadro.

   Para obtener sugerencias sobre los mensajes, consulte [Sugerencias para crear mensajes de texto](#tips-for-creating-text-prompts) en este artículo.
1. Añada el token de API para la aplicación en el módulo.
1. Compruebe el módulo para asegurarse de que parece estar configurado para la aplicación y la acción adecuadas.
1. (Condicional) Si el módulo no está adjunto a su escenario, arrástrelo a su lugar.

Se recomienda probar el módulo para garantizar que el módulo generado funcione según lo previsto.

## Sugerencias para crear mensajes de texto

Los mensajes de texto deben incluir la siguiente información como mínimo:

* La aplicación a la que se está conectando
* La acción que desea realizar

>[!INFO]
>
>**Ejemplos**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   Esto incluye la aplicación `Google Calendar` y la acción `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   Esto incluye la aplicación `Spotify` y la acción `Retrieve popular songs`.

Tenga en cuenta lo siguiente al crear mensajes de texto:

* Dado que cada módulo Fusion realiza una única acción, el mensaje de texto debe describir una acción específica.
* Utilice un lenguaje directo y sencillo.
* Compruebe y pruebe su módulo. Si no funciona como se espera, perfeccione el mensaje e inténtelo de nuevo.



