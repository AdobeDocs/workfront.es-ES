---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Control de flujo en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 85%

---

# Control de flujo en Adobe Workfront Fusion

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Control de flujo](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/flow-control.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Al crear o editar un escenario, es posible configurar opciones para controlar el modo en que los datos fluirán a través de el.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte Licencias de [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Repetidor

Use un módulo [!UICONTROL Repetidor] para repetir una tarea un número determinado de veces. Un módulo [!UICONTROL Repetidor] genera paquetes uno tras otro.

Por ejemplo, podría usarse un módulo [!UICONTROL Repetidor] para enviar cinco correos electrónicos con los temas “Hola 1”, “Hola 2”, etc., conectando el módulo **[!UICONTROL Correo electrónico] >[!UICONTROL Enviarme un correo electrónico]** al módulo [!UICONTROL Repetidor].

Para usar un módulo [!UICONTROL Repetidor]:

1. Haga clic en el icono [!UICONTROL Control de flujo] ![](assets/flow-control-icon.gif) de la parte inferior de la pantalla y, a continuación, haga clic en **[!UICONTROL Repetidor]** en el menú que se muestra.
1. Haga clic en el paquete [!UICONTROL Repetidor] y, a continuación, haga clic en **[!UICONTROL Conectarse automáticamente]** en el cuadro que aparecerá.
1. En el cuadro [!UICONTROL Control de flujo] que aparezca, escriba el número de repeticiones (paquetes de salida) que quiera en el cuadro **[!UICONTROL Repeticiones]**.

   En el ejemplo de correo electrónico, debe escribir 5.

   ![](assets/repeater-2-350x207.png)

   El valor del elemento aumenta en cada repetición según este valor especificado en el campo **[!UICONTROL Paso]**, que se puede ver seleccionando **[!UICONTROL Mostrar ajustes avanzados]**. Este número se establece en 1 de forma predeterminada.

1. Haga clic en **[!UICONTROL Aceptar]** para cerrar el cuadro **[!UICONTROL Control de flujo]**.

1. Haga clic en la aplicación o el módulo de servicio conectado al módulo [!UICONTROL Repetidor].
1. En el cuadro que aparecerá, escriba la información que quiera repetir.

   En el ejemplo de correo electrónico, escribiría Hola en el cuadro [!UICONTROL Asunto] y, a continuación, asignaría `i` desde el módulo del repetidor.

   ![](assets/repeater-3-350x207.png)

| Elemento | Descripción |
|---|---|
| [!UICONTROL Valor inicial] | Escriba o asigne el número que quiera que el módulo establezca como `i` en la primera iteración. El valor predeterminado es 1. |
| [!UICONTROL Repeticiones] | Introduzca o asigne el número de veces que quiera que el módulo se repita. Este número debe ser mayor o igual que 0, y menor o igual que 10 000. |
| [!UICONTROL Paso] | Es el número por el que el módulo aumenta el valor de `i`. El valor predeterminado es 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>El número de repeticiones no está determinado por el valor de `i`, ya que sería un bucle en la programación. El módulo repetirá la cantidad de veces indicada en el campo [!UICONTROL Repeticiones]. El valor de `i` cambia con cada iteración del módulo [!DNL repeater] y se puede asignar a módulos posteriores. El ejemplo anterior asigna el valor de `i` al mensaje Hola, lo que da como resultado mensajes que dicen “Hola 1”, “Hola 2”, etc.

## [!UICONTROL Iterador]

Un [!UICONTROL Iterador] es un tipo especial de módulo que convierte una matriz en una serie de paquetes. Cada elemento de matriz será un paquete independiente en la salida del módulo [!UICONTROL Iterador]. Para obtener más información, consulte el módulo [[!UICONTROL Iterador] en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Agregador de matrices

Un agregador de matrices es un tipo especial de módulo que permite combinar varios paquetes en uno solo. Para obtener más información, consulte el módulo [[!UICONTROL Agregador] en Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Enrutador]

El módulo [!UICONTROL Enrutador] permite bifurcar el flujo en varias rutas y procesar los datos de cada ruta de forma diferente. Una vez que un módulo [!UICONTROL Enrutador] recibe un paquete, lo reenvía a cada ruta conectada en el orden en que se adjuntaron las rutas al módulo [!UICONTROL Enrutador]. Para obtener más información, consulte [Módulo Enrutador en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
