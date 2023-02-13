---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemas de velocidad en [!DNL Workfront Proof]
description: Esta página de ayuda puede ayudarle a determinar si existen problemas de velocidad que pueda tener al usar [!DNL Workfront Proof] están relacionados con su ISP o [!DNL Workfront Proof]de la red de entrega de contenido de .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# Problemas de velocidad en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Esta página de ayuda puede ayudarle a determinar si existen problemas de velocidad que pueda tener al usar [!DNL Workfront Proof] están relacionados con su ISP o [!DNL Workfront Proof]de la red de entrega de contenido de .

Los problemas de velocidad se deben generalmente a la conexión ISP local o a la configuración de acceso a Internet local (por ejemplo, cuando se utiliza un servidor proxy), por lo que lamentablemente están fuera del control de [!DNL Workfront Proof].

Dicho esto, puede seguir algunos pasos para comprobar la velocidad de conexión, lo que permitirá determinar la causa raíz de los problemas que experimenta. Todos estos pasos son igualmente importantes para el proceso de resolución de problemas y le recomendamos que dedique tiempo a recopilar información sobre todos los pasos indicados para garantizar el diagnóstico más preciso del problema.

Una vez recopilados todos los detalles, le recomendamos que consulte con su departamento de TI local para identificar cualquier problema local. Si necesita más ayuda en el asunto, póngase en contacto con nuestro [Equipo de asistencia](https://support.workfront.com/hc/en-us/requests/new).

## Establecer qué parte del sistema es lenta

Cuando utilice [!DNL Workfront Proof], es posible que esté trabajando con el panel de control, por ejemplo, para administrar el contenido de las carpetas y los usuarios o con el [!DNL Workfront Proof] Visor: realizar una revisión de la prueba, comprobar los comentarios ya realizados, etc.

Determinar qué parte exacta del sistema es lenta es el primer paso para solucionar problemas de velocidad. Al realizar el informe [!DNL Workfront Proof] siendo lento, asegúrese de describir lo siguiente:

* ¿Está experimentando lentitud en otras páginas web?
* ¿Se produce el problema en el panel de control o [!DNL Workfront Proof] ¿Visualizador?
* ¿Qué parte exacta del sistema es lenta? (p. ej., procesar una nueva prueba o abrir un comentario en [!DNL Workfront Proof] Visor)

## Ejecute pruebas de traceroute y ping

Cuando experimenta problemas de rendimiento, es importante ejecutar el comando traceroute para verificar la conexión. Para ello, abra el símbolo del sistema en su sistema (terminal en Mac/Linux) y realice los siguientes pasos:

1. Escriba una de las siguientes opciones y luego espere a que se complete la extracción:

   * Windows: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. Tipo (solo Windows) **ping app.proofhq.com**.
1. Cuando finalice el ping, haga clic con el botón derecho en el símbolo del sistema y seleccione Todo.
1. Copie y pegue los resultados en la respuesta a su correo electrónico.
Asegúrese de permitir que el ping y el traceroute terminen antes de enviar los resultados al equipo de asistencia.

## Probar la velocidad de conexión con Speedtest.net

1. Haga clic en [here](http://www.speedtest.net/) para acceder a Speedtest.net.
1. Siga las instrucciones de la base de conocimientos de la prueba de velocidad para probar la velocidad de su conexión a Internet.
1. Copie y pegue los resultados en un correo electrónico de nuestro equipo de asistencia.

## Compruebe la pestaña red en la consola del explorador

La consola web disponible en los navegadores modernos recopila información útil sobre cualquier latencia de red, lo que nos ayudará a determinar la causa raíz de los problemas de velocidad que experimenta.

Para comprobar los tiempos de carga de una página web:

1. Abra la consola del explorador y la pestaña Red .
1. Vuelva a cargar la página.
1. Tome capturas de pantalla o registre una proyección de los resultados.
1. Comparta los resultados con el equipo de asistencia.

Asegúrese de que la captura de pantalla muestre todos los datos. Puede expandir la ventana de la consola al tomar una captura de pantalla o desplazarse hacia abajo en un guión.

Si no sabe cómo abrir la consola en el explorador, consulte estos pasos registrados:

* [Chrome](http://screencast.com/t/AgQU6JQQ)
* [Safari](http://screencast.com/t/f31GqQYm0w)
* [Firefox](http://screencast.com/t/Xg7SscmAi)
* [Edge](http://www.screencast.com/t/epSwBiaD)
* [Internet Explorer](http://screencast.com/t/x5Q3eHczbc)

También puede consultar la documentación de su navegador para obtener instrucciones más detalladas.

## Comprobar la conexión en una red y equipo diferentes

La comprobación de si experimenta el mismo problema con la velocidad de conexión mediante un dispositivo o red diferentes es un paso crucial en el proceso de resolución de problemas. Intente cambiar a otro equipo o dispositivo móvil, e intente utilizar una red alternativa (por ejemplo, datos móviles).

Compare la conexión en diferentes combinaciones: usando un equipo diferente en la misma red, usando el mismo equipo en una red diferente y usando la máquina alternativa y la red, y luego compartir los resultados con el equipo de soporte.
