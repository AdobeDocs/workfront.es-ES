---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo iterador en Adobe Workfront Fusion
description: Un módulo Iterator es un tipo especial de módulo que convierte una matriz en una serie de paquetes. Cada elemento de matriz se presenta como un paquete independiente.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# [!UICONTROL Iterador] módulo en [!DNL Adobe Workfront Fusion]

Un [!UICONTROL Iterador] module es un tipo especial de módulo que convierte una matriz en una serie de paquetes. Cada elemento de matriz se presenta como un paquete independiente.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe adquirir Adobe Workfront Fusion y Adobe Workfront para utilizar la funcionalidad que se describe en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iterador] configuración del módulo

Ha configurado un [!UICONTROL Iterador] módulo igual que se configura cualquier otro módulo. El [!UICONTROL Matriz] Este campo contiene la matriz que se va a convertir o dividir en paquetes independientes.

![](assets/set-up-iterator-350x190.jpg)

Para obtener más información, consulte [Configuración de los ajustes de un módulo en Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Ejemplos:**
>
>* El siguiente escenario muestra cómo recuperar correos electrónicos con archivos adjuntos y guardarlos como archivos únicos en una carpeta seleccionada [!DNL Dropbox] carpeta.
>
>   Los correos electrónicos pueden contener una matriz de archivos adjuntos. El [!UICONTROL Iterador] El módulo insertado después del primer módulo le permitirá gestionar cada archivo adjunto por separado. El [!UICONTROL Iterador] : divide la matriz de archivos adjuntos en paquetes únicos. Cada paquete, con un archivo adjunto, se guarda de uno en uno en una carpeta seleccionada [!DNL Dropbox] carpeta. El [!UICONTROL Iterador] la configuración del módulo se muestra arriba: [!UICONTROL Matriz] el campo debe contener la variable `Attachments` matriz.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Para su comodidad, muchas [!DNL Workfront Fusion] Las aplicaciones ofrecen servicios especializados [!UICONTROL Iterador] módulos con una configuración simplificada. Por ejemplo, la variable [!UICONTROL Correo electrónico] La aplicación contiene el especial [!UICONTROL Iterador] módulo [!UICONTROL Correo electrónico] > [!UICONTROL Repetir archivos adjuntos] que producirá los mismos resultados que el general [!UICONTROL Iterador] módulo.
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Solución de problemas: el panel Asignación no muestra los elementos asignables en [!UICONTROL Iterador] módulo

Cuando un [!UICONTROL Iterador] El módulo no tiene información sobre la estructura de los elementos de la matriz, el panel de asignación en los módulos que siguen a [!UICONTROL Iterador] visualización del módulo solo 2 elementos bajo el [!UICONTROL Iterador] módulo :`Total number of bundles` y `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Esto se debe a que cada módulo es responsable de proporcionar información sobre los elementos que genera para que estos elementos se puedan mostrar correctamente en el panel de asignación en los módulos posteriores. Sin embargo, es posible que varios módulos no puedan proporcionar esta información en algunos casos; por ejemplo, [!UICONTROL JSON] > [!UICONTROL Analizar JSON] o [!UICONTROL Webhooks] > [!UICONTROL Webhook personalizado] módulos con estructura de datos faltante.

La solución es ejecutar manualmente el escenario para que el módulo obtenga información sobre los elementos que genera y pueda proporcionar la información a los siguientes módulos.

Por ejemplo, si tiene un [!UICONTROL JSON] > [!UICONTROL Analizar JSON] sin una estructura de datos como se muestra a continuación:

![](assets/json-parse-json-350x285.png)

Y luego, si conectas un [!UICONTROL Iterador] módulo, no podrá asignar la salida del módulo al campo Array en el panel de configuración del [!UICONTROL Iterador] módulo :

![](assets/connect-iterator-module-350x146.png)

Para resolver esto, inicie manualmente el escenario en el editor de escenarios. Puede desvincular los módulos después de la variable [!UICONTROL JSON] > [!UICONTROL Analizar JSON] para evitar que el flujo continúe. O puede hacer clic con el botón derecho en [!UICONTROL JSON] > [!UICONTROL Analizar JSON] y elija **[!UICONTROL Ejecutar solo este módulo]** en el menú contextual para ejecutar solo la variable [!UICONTROL JSON] > [!UICONTROL Analizar JSON] módulo.

Si la variable [!UICONTROL JSON] > [!UICONTROL Analizar JSON] se ejecuta, obtiene información sobre los elementos que genera y proporciona esta información a todos los módulos posteriores, incluido el módulo Iterator. A continuación, el panel de asignación de la configuración del iterador muestra los elementos:

![](assets/mapping-panel-displays-items-350x131.png)

Además, el panel de asignación en los módulos conectados después de [!UICONTROL Iterador] muestra los elementos contenidos en los elementos de la matriz:

![](assets/items-contained-in-array-350x156.png)

Si no puede ver algunos elementos en el panel de asignación de un módulo, ejecute el escenario una vez para que todos los módulos puedan obtener información sobre los elementos que generan y proporcionar esta información a los siguientes módulos.
