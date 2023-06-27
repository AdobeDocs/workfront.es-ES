---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Control de flujo en Adobe Workfront Fusion
description: Al crear o editar un escenario, puede configurar opciones para controlar el modo en que los datos fluyen por él.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 1%

---

# Control de flujo en Adobe Workfront Fusion

Al crear o editar un escenario, puede configurar opciones para controlar el modo en que los datos fluyen por él.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Repetidor

Puede usar un [!UICONTROL Repetidor] para repetir una tarea un número determinado de veces. A [!UICONTROL Repetidor] Este módulo genera paquetes, uno tras otro.

Por ejemplo, puede utilizar un [!UICONTROL Repetidor] para enviar cinco correos electrónicos con los temas &quot;Hola 1&quot;, &quot;Hola 2&quot;, etc., conectando el **[!UICONTROL Correo electrónico] >[!UICONTROL Enviarme un correo electrónico]** al módulo de [!UICONTROL Repetidor] módulo.

Para utilizar un [!UICONTROL Repetidor] módulo:

1. Haga clic en [!UICONTROL Control de flujo] icono ![](assets/flow-control-icon.gif) en la parte inferior de la pantalla, haga clic en **[!UICONTROL Repetidor]** en el menú que se muestra.
1. Haga clic en [!UICONTROL Repetidor] paquete y haga clic en **[!UICONTROL Conectar automáticamente]** en el cuadro que se muestra.
1. En el [!UICONTROL Control de flujo] que aparece, escriba el número de repeticiones (paquetes generados) que desee en la **[!UICONTROL Repeticiones]** cuadro.

   En nuestro ejemplo de correo electrónico, debe escribir 5.

   ![](assets/repeater-2-350x207.png)

   El valor del elemento aumenta en cada repetición según este valor especificado en la variable **[!UICONTROL Etapa]** , que puede ver seleccionando **[!UICONTROL Mostrar configuración avanzada]**. Este número es 1 de forma predeterminada.

1. Clic **[!UICONTROL OK]** para cerrar el **[!UICONTROL Control de flujo]** cuadro.

1. Haga clic en la aplicación o el módulo de servicio conectado al [!UICONTROL Repetidor] módulo.
1. En el cuadro que aparece, escriba la información que desea repetir.

   En nuestro ejemplo de correo electrónico, escribiría Hello en la [!UICONTROL Asunto] cuadro y, a continuación, asignar `i` del módulo del repetidor.

   ![](assets/repeater-3-350x207.png)

| Elemento | Descripción |
|---|---|
| [!UICONTROL Valor inicial] | Introduzca o asigne el número que desea que establezca el módulo como `i` en la primera iteración. El valor predeterminado es 1. |
| [!UICONTROL Se repite] | Introduzca o asigne el número de veces que desea que el módulo se repita. Este número debe ser igual o bueno a 0 y menor o igual a 10 000. |
| [!UICONTROL Etapa] | Es el número en el que el módulo aumenta el valor de `i`. El valor predeterminado es 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>El número de repeticiones no está determinado por el valor de `i`, como sería en un bucle en la programación. El módulo repetirá la cantidad de veces indicada en la [!UICONTROL Repeticiones] field. El valor `i` cambia con cada iteración de [!DNL repeater] y se pueden asignar a módulos posteriores. El ejemplo anterior asigna el valor de `i` en el mensaje Hola, que genera mensajes que dicen &quot;Hola 1&quot;, &quot;Hola 2&quot;, etc.

## [!UICONTROL Iterador]

Un [!UICONTROL Iterador] es un tipo especial de módulo que convierte una matriz en una serie de paquetes. Cada elemento de matriz será un paquete independiente en el [!UICONTROL Iterador] salida del módulo. Para obtener más información, consulte [[!UICONTROL Iterador] módulo en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Agregador de matrices

Un agregador de matrices es un tipo especial de módulo que permite combinar varios paquetes en uno solo. Para obtener más información, consulte [[!UICONTROL Agregador] en Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Enrutador]

El [!UICONTROL Enrutador] Este módulo le permite ramificar el flujo en varias rutas y procesar los datos de cada una de ellas de forma diferente. Una vez al [!UICONTROL Enrutador] recibe un paquete, lo reenvía a cada ruta conectada en el orden en que se adjuntaron las rutas al [!UICONTROL Enrutador] módulo. Para obtener más información, consulte [Módulo de enrutador en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
