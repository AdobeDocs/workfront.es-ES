---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo del iterador en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 89%

---

# Módulo [!UICONTROL del iterador] en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulo iterador](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/iterator-module.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Un módulo [!UICONTROL de iterador] es un tipo especial de módulo que convierte una matriz en una serie de paquetes. Cada elemento de matriz se presenta como un paquete independiente.

Para obtener más información, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md) y [Asignar una matriz en Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>Su organización debe adquirir Adobe Workfront Fusion y Adobe Workfront para utilizar la funcionalidad que se describe en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte Licencias de [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Configuración del módulo [!UICONTROL del iterador]

Configuró un módulo [!UICONTROL del iterador] igual que cualquier otro módulo. El campo [!UICONTROL Array] contiene la matriz que se va a convertir o dividir en paquetes separados.

![](assets/set-up-iterator-350x190.jpg)

Para obtener más información, consulte [Configuración de los valores de un módulo en Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Ejemplos**
>
>* El siguiente escenario muestra cómo recuperar correos electrónicos con archivos adjuntos y guardarlos como archivos únicos en una carpeta [!DNL Dropbox] seleccionada.
>
>   Los correos electrónicos pueden contener una matriz de archivos adjuntos. El módulo [!UICONTROL del iterador] insertado después del primer módulo le permitirá gestionar cada archivo adjunto por separado. El módulo [!UICONTROL del iterador] divide la matriz de archivos adjuntos en paquetes únicos. Cada paquete, con un archivo adjunto, se guarda de uno en uno en una carpeta [!DNL Dropbox] seleccionada. La configuración del módulo [!UICONTROL del iterador] se muestra arriba: el campo [!UICONTROL Array] debe contener la matriz `Attachments`.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Para su comodidad, muchas aplicaciones de [!DNL Workfront Fusion] ofrecen módulos [!UICONTROL del iterador] especializados con una configuración simplificada. Por ejemplo, la aplicación [!UICONTROL Email] contiene el módulo especial [!UICONTROL del iterador] [!UICONTROL Email] > [!UICONTROL Iterate attachments] que producirá los mismos resultados que el módulo general [!UICONTROL del iterador].
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Solución de problemas: el panel Asignación no muestra elementos asignables en el módulo [!UICONTROL Iterator]

Cuando un módulo [!UICONTROL Iterator] no tiene información sobre la estructura de los elementos de la matriz, el panel de asignación de los módulos que siguen al módulo [!UICONTROL Iterator] muestra solo 2 elementos bajo el módulo [!UICONTROL Iterator] :`Total number of bundles` y `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Esto se debe a que cada módulo es responsable de proporcionar información sobre los elementos que genera para que estos elementos se puedan mostrar correctamente en el panel de asignación de los módulos posteriores. Sin embargo, es posible que varios módulos no puedan proporcionar esta información en algunos casos; por ejemplo, módulos [!UICONTROL JSON] > [!UICONTROL Parse JSON] o [!UICONTROL Webhooks] > [!UICONTROL Custom Webhook] a los que les falta una estructura de datos.

La solución es ejecutar manualmente el escenario para que el módulo obtenga información sobre los elementos que genera y pueda proporcionar la información a los siguientes módulos.

Por ejemplo, si tiene un módulo [!UICONTROL JSON] > [!UICONTROL Parse JSON] sin una estructura de datos como la que se muestra a continuación:

![](assets/json-parse-json-350x285.png)

Y entonces, si se le conecta un módulo [!UICONTROL Iterator], no podrá asignar la salida del módulo al campo Array en el panel de configuración del módulo [!UICONTROL Iterator]:

![](assets/connect-iterator-module-350x146.png)

Para resolver esto, inicie manualmente el escenario en el editor de escenarios. Puede desenlazar los módulos después del módulo [!UICONTROL JSON] > [!UICONTROL Parse JSON] para evitar que el flujo continúe. O puede hacer clic con el botón derecho en el módulo [!UICONTROL JSON] > [!UICONTROL Parse JSON] y elegir **[!UICONTROL Run this module only]** del menú contextual para ejecutar solo el módulo [!UICONTROL JSON] > [!UICONTROL Parse JSON].

Cuando se ejecuta [!UICONTROL JSON] > [!UICONTROL Parse JSON], obtiene información sobre los elementos que genera y proporciona esta información a todos los módulos subsiguientes, incluido el módulo Iterator. A continuación, el panel de asignación de la configuración del iterador muestra los elementos siguientes:

![](assets/mapping-panel-displays-items-350x131.png)

Además, el panel de asignación de los módulos conectados después del módulo [!UICONTROL Iterator] muestra los elementos contenidos en los elementos de la matriz:

![](assets/items-contained-in-array-350x156.png)

Si no puede ver algunos elementos en el panel de asignación del módulo, ejecute el escenario una vez para que todos los módulos puedan obtener información sobre los elementos que generan y proporcionar esta información a los siguientes módulos.
