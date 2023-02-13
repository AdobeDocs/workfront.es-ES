---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Resolución de problemas - [!DNL Workfront Proof] visor de pruebas
description: Si el contenido de la prueba no se carga y solo puede ver un visor de pruebas vacío, lo más probable es que algo esté bloqueando esta acción localmente. Pruebe las posibles soluciones a continuación.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# Resolución de problemas - [!DNL Workfront Proof] visor de pruebas

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Si el contenido de la prueba no se carga y solo puede ver un visor de pruebas vacío, lo más probable es que algo esté bloqueando esta acción localmente. Pruebe las posibles soluciones a continuación.

## Asegúrese de que su explorador y [!DNL Flash Player] Las versiones están actualizadas

Todos los desarrolladores trabajan constantemente en sus aplicaciones y publican regularmente nuevas funciones y correcciones para sus productos. Esto sirve para mejorar la experiencia del usuario y mantener el nivel de seguridad, por lo que se recomienda utilizar solo las versiones más recientes. Esto también ayuda a evitar conflictos entre las aplicaciones.

### [!DNL Flash Player] Versión del complemento

Para comprobar su actual [!DNL Flash Player] visita la versión [[!DNL Adobe] sitio web](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

Si su número de versión difiere del que se indica para su plataforma, vaya a la [[!DNL Flash Player] descargar página](http://get.adobe.com/flashplayer/otherversions/) y obtenga la versión más reciente.

Tenga en cuenta: recomendamos usar el original [!DNL Adobe] , así que si su navegador utiliza una solución integrada, desactívelo e instale la [!DNL Adobe] solución.

### Versión del explorador

En la actualidad, la mayoría de los exploradores se actualizan automáticamente, pero si tiene algún problema, vale la pena comprobar qué versión utiliza y realizar la actualización, si es necesario.

En el navegador, vaya a [!UICONTROL Menú] y busque la variable [!UICONTROL Acerca de] (en algunos casos, esto puede ser visible en [!UICONTROL Ayuda] ). En el [!UICONTROL Acerca de] ventana emergente encontrará información sobre la versión actual del explorador y también una opción para actualizar o buscar actualizaciones.

Consulte en Chrome:

![ProofView_3.png](assets/proofview-3-350x206.png)

Una vez que tenga la última [!DNL Flash Player] plugin y versión de navegador instalados intente volver a abrir la prueba y ver si el problema se ha resuelto.

## Asegúrese de que su [!DNL Flash] Almacenamiento disponible

Nuestra [!DNL Workfront Proof] El visor se basa en el Flash y almacenamos algunos datos sobre las pruebas (es decir, comentarios, mosaicos de prueba, [!DNL Workfront Proof] Configuración del visor) en el equipo mediante [!DNL Flash Player]. Si la variable [!DNL Workfront Proof] El visor se abre, pero no hay contenido dentro del que desee asegurarse de que el Almacenamiento en Flash esté disponible en su equipo y que [!DNL Workfront Proof] puede utilizarlo.

Si hay algún almacenamiento asignado, pero está trabajando con las pruebas más grandes con varias páginas y los comentarios intentan aumentar el [!DNL Flash] Almacenamiento y vuelva a cargar la prueba.

Consulte nuestra [Problemas Con La Visualización De Pruebas: [!DNL Flash] Objetos compartidos explicados](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) para obtener instrucciones detalladas.

## Identificar dónde está el problema

* ¿Se abren las pruebas en un explorador diferente?
* Si utiliza un explorador a diario y tiene problemas para ver las pruebas, intente abrir la misma prueba en un explorador diferente del equipo. Para ello, simplemente copie el vínculo de prueba de la barra URL del navegador principal y péguelo en un navegador diferente. Si la prueba se abre correctamente, revise la configuración, los complementos y las extensiones del explorador principal, ya que pueden estar interfiriendo.
* No tenemos ningún navegador preferible, pero si tiene algún problema de rendimiento en su navegador actual, le recomendamos que cambie a otro.
* ¿Las pruebas se abren en una máquina diferente en su ubicación?
Si la prueba no se abre en ningún explorador del equipo, intente abrirla en otro equipo de la ubicación o fuera de la ubicación. Esto le permitirá determinar si un problema se debe a su equipo en particular o si es algo de su red local.
Si el nivel de seguridad es mayor, las conexiones a [!DNL Workfront Proof] puede ser bloqueado por:

   * Su software AV local
   * Su solución de seguridad de red
   * Configuración de DNS, firewall o proxy
   * Estos son los ajustes que están fuera de nuestro control. Hay varias soluciones de seguridad disponibles y no podemos saber cuáles están implementadas en su red y cuáles pueden estar bloqueando las conexiones a [!DNL Workfront Proof]. Tampoco depende de [!DNL Workfront Proof] para decidir la configuración de seguridad interna. Si tiene problemas para abrir las pruebas en los múltiples equipos de su ubicación/red, le recomendamos que se ponga en contacto con su equipo de TI para que puedan comprobar la configuración de la red y autorizar o agregar la [!DNL Workfront Proof] a la lista de permitidos, si es necesario.

* ¿Son las conexiones a [!DNL Workfront Proof] ¿está permitido en su red?
Dentro del Visor de pruebas cargamos los mosaicos - fragmentos de las páginas. Si este contenido no se carga bien al final, puede ser que algunas conexiones a [!DNL Workfront Proof] están bloqueados en la red. Asegúrese de que todas las conexiones y todo el contenido de *.proofhq.com se añada a la lista de permitidos. Su equipo de TI debería poder ayudarle a verificarlo.

## Revisar complementos

Si su navegador y [!DNL Flash Player] está actualizado y su red no bloquea las conexiones a [!DNL Workfront Proof] puede haber algo en el navegador que esté afectando a la visualización de las pruebas. Actualmente hay varios complementos y extensiones disponibles en su explorador y algunos de ellos interfieren o están en conflicto con los demás.

La práctica recomendada es eliminar todos los complementos desconocidos y mantener solo los que usa y en los que confía. Cada explorador debe darle opciones para comprobar, modificar o eliminar los complementos y las extensiones. Nuestra [!DNL Workfront Proof] El visor se basa en [!DNL Flash] y utilizamos JavaScript para cargar el visor, de modo que querrá revisar especialmente los complementos que podrían afectar a estos.

Visite las páginas enumeradas a continuación para obtener instrucciones más detalladas de los desarrolladores sobre cómo deshabilitar los complementos del explorador:

* Chrome: [plugins](https://support.google.com/chrome/answer/142064?hl=en-GB) / [extensiones](https://support.google.com/chrome/answer/113907?hl=en-GB)
* Firefox: [complementos](https://support.mozilla.org/en-US/kb/disable-or-remove-add-ons)
* Internet Explorer: [complementos](http://windows.microsoft.com/en-GB/internet-explorer/manage-add-ons#ie=ie-11)
* Safari: [complementos](http://support.apple.com/en-gb/HT203353)

Si hay algún complemento en particular que interfiera con la carga de las pruebas, puede intentar comprobar los detalles en la consola del explorador.

![ProofView_4.png](assets/proofview-4-350x57.png)

En la mayoría de los exploradores más recientes, hay algunas herramientas de desarrollador adicionales disponibles que se pueden utilizar para solucionar problemas más avanzados.

Si tiene problemas para ver las pruebas:

* Abra la consola del explorador y vuelva a cargar la prueba.
* Compruebe si hay alertas o mensajes en la consola. Estos detalles pueden ayudar a identificar cuál es la causa principal de los problemas.
* Pida a su equipo de TI que analice los resultados. Deben ser capaces de asesorar y ayudar a resolver el problema local.
* Comparta los resultados con nuestra [Equipo de asistencia](https://support.workfront.com/hc/en-us/requests/new). Estaremos encantados de ayudar.

Si no sabe cómo abrir la consola en el explorador, consulte los pasos registrados:

* [Firefox](http://screencast.com/t/eP6FRtk4vxWS)
* [Internet Explorer](http://screencast.com/t/bYzq1iQv)
* [Google Chrome](http://screencast.com/t/2anpeAzOOyj)
* [Safari](http://screencast.com/t/rnOvgl3GidjL)

También puede consultar la documentación del desarrollador del explorador para obtener instrucciones más detalladas.

## Comprobar la configuración de contenido mixto

Todas las conexiones a [!DNL Workfront Proof] se encuentran en HTTPS. Sin embargo, en la variable [!DNL Workfront Proof] El visor carga los mosaicos a través de HTTP y los datos se protegen con los tokens. Esto crea contenido mixto que algunos de los navegadores o soluciones de seguridad pueden estar bloqueando (de forma predeterminada o según la configuración manual).

Si esta es la razón por la que las pruebas no se abren en el equipo (debería poder ver las alertas relevantes en la consola del explorador) autorice estas conexiones para [!DNL Workfront Proof] o modifique la configuración para permitir contenido mixto pasivo en su equipo. El contenido mixto puede ser bloqueado por su navegador, software AV, configuración de red, etc. - para determinar la causa exacta, póngase en contacto con su equipo de TI/administradores de red. También deberían poder ayudarle a habilitar el contenido mixto en su equipo.

Póngase en contacto con [Equipo de asistencia](https://support.workfront.com/hc/en-us/requests/new) si necesita ayuda desde nuestro final.
