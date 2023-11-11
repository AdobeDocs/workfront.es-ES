---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Solución de problemas - [!DNL Workfront Proof] visualizador de pruebas
description: Si el contenido de la prueba no se carga y solo puede ver un visor de pruebas vacío, lo más probable es que algo esté bloqueando esta acción localmente. Pruebe las posibles soluciones siguientes.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 0%

---

# Solución de problemas - [!DNL Workfront Proof] visualizador de pruebas

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Si el contenido de la prueba no se carga y solo puede ver un visor de pruebas vacío, lo más probable es que algo esté bloqueando esta acción localmente. Pruebe las posibles soluciones siguientes.

## Asegúrese de que su explorador y [!DNL Flash Player] Las versiones están actualizadas

Todos los desarrolladores trabajan constantemente en sus aplicaciones y lanzan regularmente nuevas funciones y correcciones para sus productos. Esto sirve para mejorar la experiencia del usuario y mantener el nivel de seguridad, por lo que se recomienda utilizar solo las versiones más recientes. Esto también ayuda a evitar conflictos entre las aplicaciones.

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### Versión del navegador

Hoy en día la mayoría de los navegadores se actualizan automáticamente, pero si estás experimentando algún problema vale la pena comprobar qué versión estás utilizando y realizar la actualización, si es necesario.

En el navegador, vaya a [!UICONTROL Menú] y busque el [!UICONTROL Acerca de] opción (en algunos casos, esto puede ser visible en [!UICONTROL Ayuda] menú). En el [!UICONTROL Acerca de] En esta ventana emergente encontrarás información sobre la versión actual del navegador y también una opción para actualizar o buscar actualizaciones.

Consulte en Chrome:

![ProofView_3.png](assets/proofview-3-350x206.png)

Una vez que tenga las últimas [!DNL Flash Player] el complemento y la versión del explorador instalados intentan volver a abrir la prueba y ver si se ha resuelto el problema.

## Asegúrese de que su [!DNL Flash] Almacenamiento disponible

Nuestro [!DNL Workfront Proof] El visor se basa en el Flash y almacenamos algunos datos sobre las pruebas (es decir, comentarios, mosaicos de prueba, etc.). [!DNL Workfront Proof] Configuración del visor) en el equipo mediante [!DNL Flash Player]. Si la variable [!DNL Workfront Proof] Se abre el visor, pero no hay contenido dentro. Debe asegurarse de que el almacenamiento de Flash esté disponible en su equipo y de que [!DNL Workfront Proof] tiene permiso para usarlo.

Si hay algo de almacenamiento asignado, pero está trabajando con pruebas más grandes con varias páginas y comentarios, intente aumentar la [!DNL Flash] Almacene y vuelva a cargar la prueba.

Consulte nuestro [Problemas Con La Visualización De Pruebas - [!DNL Flash] Objetos compartidos explicados](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) para obtener instrucciones detalladas.

## Identificar dónde está el problema

* ¿Las pruebas se abren en un explorador diferente?
* Si utiliza un navegador diariamente y tiene problemas para ver las pruebas, intente abrir la misma prueba en un navegador diferente de su ordenador. Para ello, simplemente copie el vínculo de prueba de la barra URL del explorador principal y péguelo en un explorador diferente. Si la prueba se abre correctamente, revise la configuración principal del explorador, los complementos y las extensiones, ya que pueden interferir.
* No tenemos ningún navegador preferible, pero si tiene problemas de rendimiento en su navegador actual, le recomendamos cambiar a uno diferente.
* ¿Las pruebas se abren en un equipo diferente de su ubicación?
Si la revisión no se abre en ningún explorador del equipo, intente abrirla en un equipo diferente de su ubicación o fuera de ella. Esto le permitirá determinar si un problema se debe a su equipo en particular o si es algo de su red local.
Si su nivel de seguridad es mayor, sus conexiones a [!DNL Workfront Proof] puede ser bloqueado por:

   * Su software AV local
   * Su solución de seguridad de red
   * Configuración de DNS, cortafuegos o proxy
   * Estos son los ajustes que están fuera de nuestro control. Hay varias soluciones de seguridad disponibles y no podemos saber cuáles están implementadas en su red y cuáles pueden estar bloqueando las conexiones a [!DNL Workfront Proof]. Tampoco depende de [!DNL Workfront Proof] para decidir la configuración de seguridad interna. Si tiene problemas para abrir las pruebas en varios equipos de su ubicación o red, le recomendamos que se ponga en contacto con su equipo de TI para que pueda comprobar la configuración de la red y autorizar o agregar el [!DNL Workfront Proof] a la lista de permitidos, si es necesario.

* Son las conexiones a [!DNL Workfront Proof] ¿está permitido en su red?
Dentro del visualizador de pruebas cargamos los mosaicos: fragmentos de las páginas. Si este contenido no se carga correctamente, es posible que algunas conexiones a [!DNL Workfront Proof] están bloqueados en su red. Debe asegurarse de que todas las conexiones y todo el contenido de *.proofhq.com se añada a la lista de permitidos. Su equipo de TI debe poder ayudarle a verificar esto.

## Revisar complementos

Si su explorador y [!DNL Flash Player] está actualizado y la red no está bloqueando las conexiones a. [!DNL Workfront Proof] es posible que haya algo en el explorador que esté afectando la visualización de las pruebas. Hoy en día hay varios plugins y extensiones disponibles en su navegador y algunos de ellos interfieren o entran en conflicto con los demás.

La práctica recomendada es eliminar todos los complementos desconocidos y conservar solo los que utilice y en los que confíe. Cada navegador debe ofrecerle opciones para comprobar, modificar o eliminar los complementos y las extensiones. Nuestro [!DNL Workfront Proof] El visor se basa en [!DNL Flash] y utilizamos JavaScript para cargar el visor, por lo que querrá revisar especialmente los complementos que podrían afectar a estos.

Si algún complemento en particular interfiere con la carga de las pruebas, puede intentar comprobar los detalles en la consola del explorador.

![ProofView_4.png](assets/proofview-4-350x57.png)

En la mayoría de los exploradores más recientes hay algunas herramientas adicionales disponibles para desarrolladores que se pueden utilizar para una solución de problemas más avanzada.

Si tiene problemas para ver las pruebas:

* Abra la consola del explorador y vuelva a cargar la prueba.
* Compruebe si hay alertas o mensajes en la consola. Estos detalles pueden ayudar a identificar cuál es la causa principal de los problemas.
* Pida a su equipo de TI que analice los resultados. Deben ser capaces de asesorar y ayudar a resolver el problema local.
* Comparta los resultados con nuestro equipo de asistencia. Estaremos encantados de ayudarle.


## Comprobar configuración de contenido mixto

Todas las conexiones a [!DNL Workfront Proof] son a través de HTTPS. Sin embargo, en el [!DNL Workfront Proof] Al visualizar, cargamos los mosaicos a través de HTTP y los datos se aseguran con los tokens. Esto crea contenido mixto que algunos exploradores o soluciones de seguridad pueden estar bloqueando (de forma predeterminada o según la configuración manual).

Si este es el motivo por el que las pruebas no se abren en el equipo (debería poder ver las alertas relevantes en la consola del explorador), autorice estas conexiones para [!DNL Workfront Proof] o modifique la configuración para permitir contenido mixto pasivo en el equipo. El contenido mixto puede ser bloqueado por su navegador, software AV, configuración de red, etc - para determinar la causa exacta, póngase en contacto con su equipo de TI / administradores de red. También deben poder ayudar a habilitar el contenido mixto en el equipo.


