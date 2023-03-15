---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Control de flujo en Adobe Workfront Fusion
description: Cuando crea o edita un escenario, puede configurar opciones para controlar el modo en que los datos fluyen a través de él.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# Control de flujo en Adobe Workfront Fusion

Cuando crea o edita un escenario, puede configurar opciones para controlar el modo en que los datos fluyen a través de él.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Repetidor

Puede usar un [!UICONTROL Repetidor] para repetir una tarea un número determinado de veces. A [!UICONTROL Repetidor] genera paquetes, uno tras otro.

Por ejemplo, puede usar un [!UICONTROL Repetidor] para enviar cinco correos electrónicos con los temas &quot;Hello 1,&quot; &quot;Hello 2,&quot;, etc., conectando el **[!UICONTROL Correo electrónico] >[!UICONTROL Enviarme un correo electrónico]** al [!UICONTROL Repetidor] módulo.

Para usar un [!UICONTROL Repetidor] módulo:

1. Haga clic en el [!UICONTROL Control de flujo] icono ![](assets/flow-control-icon.gif) en la parte inferior de la pantalla, haga clic en **[!UICONTROL Repetidor]** en el menú que se muestra.
1. Haga clic en el [!UICONTROL Repetidor] paquete y haga clic en **[!UICONTROL Conectar automáticamente]** en el cuadro que aparece.
1. En el [!UICONTROL Control de flujo] que aparece, escriba el número de repeticiones (paquetes de salida) que desee en la **[!UICONTROL Repetidas]** en la ventana

   En nuestro ejemplo de correo electrónico, escribiría 5.

   ![](assets/repeater-2-350x207.png)

   El valor del elemento aumenta en cada repetición por este valor especificado en la variable **[!UICONTROL Paso]** , que puede ver seleccionando **[!UICONTROL Mostrar configuración avanzada]**. Este número es 1 de forma predeterminada.

1. Haga clic en **[!UICONTROL OK]** para cerrar el **[!UICONTROL Control de flujo]** en la ventana

1. Haga clic en el módulo de aplicación o servicio conectado al [!UICONTROL Repetidor] módulo.
1. En el cuadro que aparece, escriba la información que desee repetir.

   En nuestro ejemplo de correo electrónico, escribiría Hello en la [!UICONTROL Asunto] cuadro, luego mapa `i` del módulo repetidor.

   ![](assets/repeater-3-350x207.png)

| Elemento | Descripción |
|---|---|
| [!UICONTROL Valor inicial] | Introduzca o asigne el número que desea que establezca el módulo como `i` en la primera iteración. El valor predeterminado es 1. |
| [!UICONTROL Se repite] | Introduzca o asigne el número de veces que desea que se repita el módulo. Este número debe ser bueno o igual a 0 y menor o igual que 10 000. |
| [!UICONTROL Etapa] | Este es el número por el cual el módulo aumenta el valor de `i`. El valor predeterminado es 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>El número de repeticiones no está determinado por el valor de `i`, ya que estaría en un bucle en la programación. El módulo repetirá el número de veces indicado en la variable [!UICONTROL Repetidas] campo . El valor `i` cambia con cada iteración del [!DNL repeater] y se pueden asignar a módulos posteriores. El ejemplo anterior asigna el valor de `i` en el mensaje Hello, lo que da como resultado mensajes que dicen &quot;Hello 1,&quot; Hello 2,&quot;, etc.

## [!UICONTROL Iterador]

Un [!UICONTROL Iterador] es un tipo especial de módulo que convierte una matriz en una serie de paquetes. Cada elemento de matriz será un paquete separado en la variable [!UICONTROL Iterador] salida del módulo. Para obtener más información, consulte [[!UICONTROL Iterador] módulo en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Agrupador de matrices

Un agregador de matrices es un tipo especial de módulo que permite combinar varios paquetes en un único paquete. Para obtener más información, consulte [[!UICONTROL Acumulador] módulo en Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Enrutador]

La variable [!UICONTROL Enrutador] permite ramificar el flujo en varias rutas y procesar los datos dentro de cada ruta de forma diferente. Una vez [!UICONTROL Enrutador] recibe un paquete, lo reenvía a cada ruta conectada en el orden en que se adjuntaron las rutas al [!UICONTROL Enrutador] módulo. Para obtener más información, consulte [Módulo Router en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
