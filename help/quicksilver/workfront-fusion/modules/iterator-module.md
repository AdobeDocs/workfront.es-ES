---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo de iteración en Adobe Workfront Fusion
description: Un módulo Iterator es un tipo especial de módulo que convierte una matriz en una serie de paquetes. Cada elemento de matriz se genera como un paquete separado.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: a2060e7179f2295bfd42da84bd7bca9862ad0a17
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!UICONTROL Iterador] módulo en [!DNL Adobe Workfront Fusion]

Un [!UICONTROL Iterador] es un tipo especial de módulo que convierte una matriz en una serie de paquetes. Cada elemento de matriz se genera como un paquete separado.

Para obtener más información, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md) y [Asignación de una matriz en Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe adquirir Adobe Workfront Fusion y Adobe Workfront para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iterador] configuración del módulo

Configure una [!UICONTROL Iterador] del mismo modo que configuró cualquier otro módulo. La variable [!UICONTROL Matriz] contiene la matriz que se va a convertir o dividir en paquetes independientes.

![](assets/set-up-iterator-350x190.jpg)

Para obtener más información, consulte [Configuración de la configuración de un módulo en Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Ejemplos:**
>
>* El siguiente escenario muestra cómo recuperar correos electrónicos con archivos adjuntos y guardar los archivos adjuntos como archivos únicos en un [!DNL Dropbox] carpeta.
   >
   >   Los correos electrónicos pueden contener una matriz de archivos adjuntos. La variable [!UICONTROL Iterador] insertado después del primer módulo le permitirá gestionar cada archivo adjunto por separado. La variable [!UICONTROL Iterador] divide la matriz de archivos adjuntos en paquetes únicos. Cada paquete, con un archivo adjunto, se guarda de uno en uno en un [!DNL Dropbox] carpeta. La variable [!UICONTROL Iterador] la configuración del módulo se muestra arriba: el [!UICONTROL Matriz] El campo debe contener la variable `Attachments` matriz.
   >
   >   ![](assets/attachments-array-350x154.jpg)
>
>* Para su comodidad, muchas [!DNL Workfront Fusion] apps oferta especializada [!UICONTROL Iterador] con una configuración simplificada. Por ejemplo, la variable [!UICONTROL Correo electrónico] la aplicación contiene el especial [!UICONTROL Iterador] módulo [!UICONTROL Correo electrónico] > [!UICONTROL Iteración de archivos adjuntos] que producirá los mismos resultados que el [!UICONTROL Iterador] módulo.
   >
   >   ![](assets/specialized-iterators-350x135.jpg)



## Solución de problemas: El panel de asignación no muestra elementos asignables en [!UICONTROL Iterador] módulo

Cuando una [!UICONTROL Iterador] no tiene información sobre la estructura de los elementos de la matriz, el panel de asignación en los módulos que siguen a la [!UICONTROL Iterador] el módulo de muestra solo 2 elementos en la sección [!UICONTROL Iterador] módulo :`Total number of bundles` y `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Esto se debe a que cada módulo es responsable de proporcionar información sobre los elementos que genera para que estos elementos puedan mostrarse correctamente en el panel de asignación en los módulos siguientes. Sin embargo, es posible que varios módulos no puedan proporcionar esta información en algunos casos; por ejemplo, [!UICONTROL JSON] > [!UICONTROL Analizar JSON] o [!UICONTROL Enlaces web] > [!UICONTROL Vínculo web personalizado] módulos con estructura de datos faltante.

La solución es ejecutar manualmente el escenario para que el módulo conozca los elementos que genera para que pueda proporcionar la información a los siguientes módulos.

Por ejemplo, si tiene un [!UICONTROL JSON] > [!UICONTROL Analizar JSON] sin una estructura de datos como se muestra a continuación:

![](assets/json-parse-json-350x285.png)

Y entonces si conecta un [!UICONTROL Iterador] a él, no podrá asignar la salida del módulo al campo Array en el panel de configuración del [!UICONTROL Iterador] módulo :

![](assets/connect-iterator-module-350x146.png)

Para resolver esto, inicie manualmente el escenario en el editor de escenarios. Puede desvincular los módulos después de [!UICONTROL JSON] > [!UICONTROL Analizar JSON] para evitar que el flujo continúe. O puede hacer clic con el botón derecho en la variable [!UICONTROL JSON] > [!UICONTROL Analizar JSON] módulo y elija **[!UICONTROL Ejecutar solo este módulo]** del menú contextual para ejecutar solo el [!UICONTROL JSON] > [!UICONTROL Analizar JSON] módulo.

Cuando la variable [!UICONTROL JSON] > [!UICONTROL Analizar JSON] se ejecuta, aprende sobre los elementos que genera y proporciona esta información a todos los módulos subsiguientes, incluido el módulo Iterator. El panel de asignación en la configuración del iterador muestra los elementos:

![](assets/mapping-panel-displays-items-350x131.png)

Además, el panel de asignación en los módulos que están conectados después del [!UICONTROL Iterador] muestra los elementos contenidos en los elementos de la matriz:

![](assets/items-contained-in-array-350x156.png)

Si no puede ver algunos elementos en el panel de asignación de un módulo, ejecute el escenario una vez para que todos los módulos puedan obtener información sobre los elementos que generan y proporcione esta información a los siguientes módulos.
