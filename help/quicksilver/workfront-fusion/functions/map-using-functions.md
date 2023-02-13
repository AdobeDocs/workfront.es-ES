---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Asignación de elementos mediante funciones en [!DNL Adobe Workfront Fusion]
description: Al asignar elementos, se pueden utilizar funciones para crear fórmulas simples o complejas.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Asignación de elementos mediante funciones en [!DNL Adobe Workfront Fusion]

Al asignar elementos, se pueden utilizar funciones para crear fórmulas simples o complejas.

Las funciones disponibles en [!DNL Adobe Workfront Fusion] son similares a las funciones de Excel y de algunos lenguajes de programación. Evaluan lógica general, matemáticas, texto, fechas y matrices. Permiten realizar lógicas condicionales y transformaciones de valores de elementos, como convertir un texto en mayúsculas, recortar texto, convertir una fecha en un formato diferente, etc. Para obtener más información, consulte [Asignación de información de un módulo a otro en Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Insertar funciones en campos

Si hace clic en un campo, la variable [!UICONTROL asignación] en el panel. El panel de asignación contiene varias pestañas:

![](assets/functions-toolbar-350x189.png)

La primera pestaña ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (se muestra al abrir el panel) muestra los elementos que se pueden asignar desde otros módulos.

Las otras pestañas contienen los siguientes tipos de funciones:

* **Funciones generales** ![](assets/toolbar-icon-general-function.png) - Consulte [Funciones generales en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) para obtener más información.

* **Funciones matemáticas** ![](assets/toolbar-icon-math-functions.png) - Consulte [Funciones matemáticas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) para obtener más información.

* **Funciones de texto y binarias** ![](assets/toolbar-icon-text&binary-functions.png) - Consulte [Funciones de cadena en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) para obtener más información.

* **Fecha y hora** ![](assets/toolbar-icon-date&time-functions.png) - Consulte [Funciones de fecha y hora en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) y los artículos siguientes para obtener más información.

   * [Tokens para el formato de fecha y hora en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Tokens para el análisis de fecha y hora en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funciones para trabajar con matrices** ![](assets/toolbar-icon-functions-for-arrays.png) - Consulte [Funciones de matriz en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) para obtener más información.

Inserción de una función en un campo:

1. Haga clic en el nombre de la función.

   O

   Arrastre la función al campo .

>[!INFO]
>
>**Ejemplo:** Algunos tipos de datos impiden que los usuarios introduzcan más de un determinado número de caracteres. Puede utilizar la función de subcadena para limitar un valor a un determinado número de caracteres.
>
>En este ejemplo, la función de subcadena limita el nombre del proyecto a 50 caracteres.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Funciones de anidación

Puede anidar funciones entre sí.

## Uso [!DNL Google Sheets] funciones

If [!DNL Workfront Fusion] no incluye una función que desee usar, pero la incluye [!DNL Google Sheets], puede usarlo siguiendo estos pasos:

1. En [!DNL Google Sheets], cree una nueva hoja de cálculo vacía.
1. En [!DNL Workfront Fusion], abra el escenario.
1. Agregue la variable **[!DNL Google Sheets]** >**[!UICONTROL Actualizar una celda]** al escenario.

   Para obtener instrucciones sobre cómo agregar un módulo, consulte [Añadir un módulo en un escenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) en el artículo [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configure el módulo:

   1. Elija la hoja de cálculo recién creada en la **[!UICONTROL Hoja de cálculo]** campo .
   1. Inserte la fórmula que contiene el [!DNL Google Sheets] en el **[!UICONTROL Valor]** campo .

      Puede utilizar la salida de los módulos anteriores como de costumbre.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Inserte el **[!UICONTROL Hojas de Google] >[!UICONTROL Obtener una celda]** para obtener el resultado calculado.
1. Configure el módulo con el mismo ID de celda utilizado en el paso 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
