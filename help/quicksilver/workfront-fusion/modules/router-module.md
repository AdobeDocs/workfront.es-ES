---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo de enrutador en Adobe Workfront Fusion
description: El módulo Router le permite bifurcar el flujo en varias rutas y procesar los datos de cada ruta de forma diferente. Una vez que un módulo Enrutador recibe un paquete, lo reenvía a cada ruta conectada en el orden en que se adjuntaron las rutas al módulo Enrutador.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Módulo [!UICONTROL Router] en [!DNL Adobe Workfront Fusion]

El módulo [!UICONTROL Router] le permite bifurcar el flujo en varias rutas y procesar los datos de cada ruta de forma diferente. Una vez que un módulo [!UICONTROL Router] recibe un paquete, lo reenvía a cada ruta conectada en el orden en que se adjuntaron las rutas al módulo [!UICONTROL Router].

>[!NOTE]
>
>* Para comprobar el orden de las rutas, puede hacer clic en el icono [!UICONTROL Alinear automáticamente], que organizará las rutas según el orden de arriba a abajo.
>
>  Para cambiar el orden, quite el módulo [!UICONTROL Router] y vuelva a conectar las rutas en el orden deseado.
>
>* Las rutas se procesan secuencialmente, no en paralelo. Un paquete no se envía a la siguiente ruta hasta que la ruta anterior lo haya procesado completamente.
>



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
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Agregando un módulo [!UICONTROL Router] a un escenario

Se puede agregar un [!UICONTROL enrutador] a un escenario de una de las siguientes maneras:

* Si desea conectar el módulo [!UICONTROL Router] después de un módulo, haga clic en el identificador derecho del módulo, empiece a escribir **[!UICONTROL router]** para buscarlo y, a continuación, elija **[!UICONTROL Flow Control]** > **[!UICONTROL Router]** en la lista de módulos que se muestra.

  ![](assets/connect-the-router-350x108.png)

* Si desea insertar el módulo [!UICONTROL Router] entre dos módulos, haga clic en el icono de la llave inglesa debajo de la ruta que conecta los dos módulos (o haga clic con el botón derecho en la ruta) y elija **[!UICONTROL Agregar un enrutador]** en el menú.

  ![](assets/insert-router-350x191.png)

* Puede insertar un módulo [!UICONTROL Enrutador] automáticamente. Por ejemplo, en la siguiente imagen, para conectar el módulo de la esquina inferior derecha al de la esquina superior izquierda (que ya está conectado al de la esquina superior derecha), arrastre el controlador izquierdo del módulo inferior derecho y suéltelo en el módulo superior izquierdo.

  ![](assets/insert-router-automatically-350x379.png)

## Filtros

Puede colocar un filtro en una ruta después del módulo [!UICONTROL Router] para filtrar paquetes como en cualquier otra ruta:

1. Haga clic en uno de los puntos de la ruta.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. En el cuadro **[!UICONTROL Configurar un filtro]** que se muestra, agregue condiciones y, a continuación, haga clic en **[!UICONTROL Aceptar]** para guardar la configuración del filtro.

   ![](assets/set-up-a-filter-2-350x242.png)

Para obtener más información, vea [Agregar un filtro a un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## La ruta de reserva

La configuración del filtro en una ruta después de un módulo [!UICONTROL Router] contiene una opción especial: La ruta de reserva:

![](assets/fallback-route-350x260.png)

Cuando está habilitada, esta ruta se usa en el caso de que un paquete no pueda continuar desde el módulo [!UICONTROL Router] a través de ninguna otra ruta porque los filtros de las otras rutas lo filtraron.

La ruta de reserva se distingue con un signo de flecha diferente dentro del módulo [!UICONTROL Enrutador]:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Un caso de uso típico de la ruta de reserva es continuar el flujo con una ruta si se cumple la condición y con otra ruta si no, como en los pasos siguientes:

1. Inserte un módulo [!UICONTROL Router] en su escenario.
1. Conecte ambas rutas al módulo [!UICONTROL Router]
1. Haga clic en la primera ruta y especifique una condición:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Haga clic en la segunda ruta y habilite la opción [!UICONTROL ruta de reserva]:

   ![](assets/enable-fallback-route-option-350x238.png)
