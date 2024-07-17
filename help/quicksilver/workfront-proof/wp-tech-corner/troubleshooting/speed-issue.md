---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemas de velocidad en  [!DNL Workfront Proof]
description: Esta página de ayuda puede ayudarle a determinar si algún problema de velocidad que podría estar experimentando al usar [!DNL Workfront Proof] está relacionado con su ISP o con la red de entrega de contenido de [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Problemas de velocidad en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Esta página de ayuda puede ayudarle a determinar si algún problema de velocidad que podría estar experimentando al usar [!DNL Workfront Proof] está relacionado con su ISP o con la red de entrega de contenido de [!DNL Workfront Proof].

Los problemas de velocidad suelen deberse a la conexión del ISP local o a la configuración del acceso local a Internet (por ejemplo, cuando se utiliza un servidor proxy), por lo que lamentablemente están fuera del control de [!DNL Workfront Proof].

Dicho esto, hay algunos pasos que puede seguir para comprobar la velocidad de conexión, lo que permitirá determinar la causa raíz de los problemas que está experimentando. Todos estos pasos son igualmente importantes para el proceso de resolución de problemas y le recomendamos que se tome el tiempo de recopilar información sobre todos los pasos enumerados para garantizar el diagnóstico más preciso del problema.

Una vez que recopile todos los detalles, le recomendamos que consulte con su departamento de TI local para identificar cualquier problema local.

## Establecer qué parte del sistema es lenta

Al usar [!DNL Workfront Proof], es posible que esté trabajando con el panel, por ejemplo, administrando el contenido de la carpeta y los usuarios, o con el visor [!DNL Workfront Proof]: realizando una revisión de revisión, comprobando los comentarios ya realizados, etc.

Determinar qué parte exacta del sistema es lenta es el primer paso para solucionar los problemas de velocidad. Cuando informe de la lentitud de [!DNL Workfront Proof], asegúrese de describir lo siguiente:

* ¿Está experimentando lentitud en alguna otra página web?
* ¿Ocurre el problema en el panel o en el visor [!DNL Workfront Proof]?
* ¿Qué parte exacta del sistema es lenta? (por ejemplo, procesar una nueva prueba o abrir un comentario en el visor [!DNL Workfront Proof])

## Ejecutar pruebas de traceroute y ping

Cuando tenga problemas de rendimiento, es importante ejecutar el comando traceroute para comprobar la conexión. Para ello, abra el Símbolo del sistema en su sistema (Terminal en Mac/Linux) y realice los siguientes pasos:

1. Escriba una de las siguientes opciones y espere a que se complete el tracerout:

   * Windows: **tracert.app.proofhq.com**
   * Mac/Linux: **traceroute.app.proofhq.com**

1. (Solo Windows) Escriba **ping app.proofhq.com**.
1. Cuando finalice el ping, haga clic con el botón secundario en el símbolo del sistema y seleccione Todo.
1. Copie y pegue los resultados en la respuesta a su correo electrónico.
Asegúrese de permitir que traceroute y ping finalicen antes de enviar los resultados al equipo de asistencia.

## Prueba de la velocidad de conexión mediante Speedtest.net

1. Abra un explorador y vaya a Speedtest.net.
1. Siga las instrucciones de la base de conocimiento de Speedtest para probar la velocidad de su conexión a Internet.
1. Copie y pegue los resultados en un correo electrónico con nuestro Equipo de soporte.

## Compruebe la pestaña de red en la consola del explorador

La consola web disponible en los navegadores modernos recopila información útil sobre cualquier latencia de red, lo que nos resultará útil para determinar la causa raíz de los problemas de velocidad que está experimentando.

Para comprobar los tiempos de carga de una página web:

1. Abra la consola del explorador y la pestaña Red (Network).
1. Vuelva a cargar la página.
1. Tome capturas de pantalla o grabe una proyección de los resultados.
1. Comparta los resultados con el equipo de asistencia.

Asegúrese de que la captura de pantalla muestre todos los datos; puede expandir la ventana de la consola al realizar una captura de pantalla o desplazarse hacia abajo en una proyección.

También puede consultar la documentación del explorador para obtener instrucciones más detalladas.

## Compruebe la conexión en una red y un equipo diferentes

Comprobar si experimenta el mismo problema con la velocidad de conexión mediante un dispositivo o una red diferentes es un paso crucial en el proceso de resolución de problemas. Intente cambiar a otro equipo o dispositivo móvil, así como intentar utilizar una red alternativa (por ejemplo, datos móviles).

Compare la conexión en diferentes combinaciones: usando un equipo diferente en la misma red, usando el mismo equipo en una red diferente y usando tanto un equipo alternativo como una red, y luego comparta los resultados con el Equipo de soporte.
