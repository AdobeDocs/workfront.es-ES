---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Asignación de elementos mediante funciones en [!DNL Adobe Workfront Fusion]
description: Al asignar elementos, puede utilizar funciones para crear fórmulas simples o complejas.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Asignación de elementos mediante funciones en [!DNL Adobe Workfront Fusion]

Al asignar elementos, puede utilizar funciones para crear fórmulas simples o complejas.

Las funciones disponibles en [!DNL Adobe Workfront Fusion] son similares a las funciones de Excel y de algunos lenguajes de programación. Evalúan la lógica general, las matemáticas, el texto, las fechas y las matrices. Permiten realizar lógica condicional y transformaciones de los valores de los elementos, como convertir un texto a mayúsculas, recortar texto, convertir una fecha a un formato diferente y mucho más. Para obtener más información, consulte [Asignación de información de un módulo a otro en Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

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

## Inserción de funciones en campos

Si hace clic en un campo, la variable [!UICONTROL asignación] se muestra el panel. El panel Asignación contiene varias pestañas:

![](assets/functions-toolbar-350x189.png)

La primera pestaña ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (que se muestra al abrir el panel) muestra los elementos que puede asignar desde otros módulos.

Las otras pestañas contienen los siguientes tipos de funciones:

* **Funciones generales** ![](assets/toolbar-icon-general-function.png) - Consulte [Funciones generales en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) para obtener más información.

* **Funciones matemáticas** ![](assets/toolbar-icon-math-functions.png) - Consulte [Funciones matemáticas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) para obtener más información.

* **Funciones de texto y binarias** ![](assets/toolbar-icon-text&binary-functions.png) - Consulte [Funciones de cadena en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) para obtener más información.

* **Fecha y hora** ![](assets/toolbar-icon-date&time-functions.png) - Consulte [Funciones de fecha y hora en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) y los artículos siguientes para obtener más información.

   * [Tokens para el formato de fecha y hora en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Tokens para el análisis de fecha y hora en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funciones para trabajar con matrices** ![](assets/toolbar-icon-functions-for-arrays.png) - Consulte [Funciones de matriz en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) para obtener más información.

Para insertar una función en un campo:

1. Haga clic en el nombre de la función.

   O

   Arrastre la función al campo.

>[!INFO]
>
>**Ejemplo:** Algunos tipos de datos impiden que los usuarios introduzcan más de un determinado número de caracteres. Puede utilizar la función subcadena para limitar un valor a un determinado número de caracteres.
>
>En este ejemplo, la función de subcadena limita el nombre del proyecto a 50 caracteres.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Anidado de funciones

Puede anidar funciones entre sí.

## Uso [!DNL Google Sheets] Funciones

If [!DNL Workfront Fusion] no incluye una función que desee utilizar, pero la presenta [!DNL Google Sheets], puede usarlo siguiendo estos pasos:

1. Entrada [!DNL Google Sheets], cree una nueva hoja de cálculo vacía.
1. Entrada [!DNL Workfront Fusion], abra su escenario.
1. Añada el **[!DNL Google Sheets]** >**[!UICONTROL Actualizar una celda]** al escenario.

   Para obtener instrucciones sobre cómo añadir un módulo, consulte [Adición de un módulo en un escenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) en el artículo [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configure el módulo:

   1. Seleccione la hoja de cálculo recién creada en la **[!UICONTROL Hoja de cálculo]** field.
   1. Inserte la fórmula que contiene el [!DNL Google Sheets] función(es) en el **[!UICONTROL Valor]** field.

      Puede utilizar la salida de los módulos anteriores como de costumbre.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Inserte el **[!UICONTROL Hojas de Google] >[!UICONTROL Consigue una celda]** para obtener el resultado calculado.
1. Configure el módulo con el mismo ID de celda utilizado en el paso 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
