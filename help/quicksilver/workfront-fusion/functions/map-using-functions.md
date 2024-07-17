---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Asignar elementos usando funciones en  [!DNL Adobe Workfront Fusion]
description: Al asignar elementos, puede utilizar funciones para crear fórmulas simples o complejas.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: d175a3d43f13338661d8b7e1cb79038a36522ff9
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Asignar elementos usando funciones en [!DNL Adobe Workfront Fusion]

Al asignar elementos, puede utilizar funciones para crear fórmulas simples o complejas. Las funciones disponibles en [!DNL Adobe Workfront Fusion] son similares a las funciones de Excel y de algunos lenguajes de programación:

* Evalúan la lógica general, las matemáticas, el texto, las fechas y las matrices.
* Permiten realizar lógica condicional y transformaciones de los valores de los elementos, como convertir un texto a mayúsculas, recortar texto, convertir una fecha a un formato diferente y mucho más.

Para obtener más información, consulte [Asignar información de un módulo a otro en Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).


## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">

<col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Cualquiera</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td>  
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Work] o superior</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td>  
   <td> 
   <p>Actual: no se requiere licencia para [!DNL Workfront Fusion].</p> 
   <p>O</p> 
   <p>Heredado: cualquiera </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Product</td>  
   <td> 
   <p>Nuevo:</p> <ul><li>Plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: su organización debe adquirir [!DNL Adobe Workfront Fusion].</li><li>Se incluye el plan [!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion].</li></ul> 
   <p>O</p> 
   <p>Actual: su organización debe comprar [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## Información general de la pestaña Asignación

Para abrir el panel [!UICONTROL mapping] para un campo:

1. Haga clic en **Escenarios** en el panel izquierdo.
1. Elija un escenario.

![](assets/open-functions-bar.png)


### Pestañas del panel Asignación

Las siguientes son pestañas del panel de asignación:

* **Funciones generales** ![](assets/toolbar-icon-general-function.png) - Vea [Funciones generales en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) para obtener más información.

* **Funciones matemáticas** ![](assets/toolbar-icon-math-functions.png) - Vea [Funciones matemáticas en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) para obtener más información.

* **Funciones binarias y de texto** ![](assets/toolbar-icon-text&binary-functions.png) - Vea [Funciones de cadena en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) para obtener más información.

* **Fecha y hora** ![](assets/toolbar-icon-date&time-functions.png) - Consulte [Funciones de fecha y hora en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) y los artículos siguientes para obtener más información:

   * [Tokens para el formato de fecha y hora en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Tokens para el análisis de fecha y hora en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funciones para trabajar con matrices** ![](assets/toolbar-icon-functions-for-arrays.png) - Vea [Funciones de matriz en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) para obtener más información.

* **Asignar otras funciones** ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) muestra los elementos que puede asignar desde otros módulos. Esta pestaña no siempre está disponible.

![](assets/functions-toolbar-350x189.png)

## Inserción de funciones en campos

Para insertar una función en un campo:

1. Haga clic en el nombre de la función.

   O

   Arrastre la función al campo.


>[!BEGINSHADEBOX]

**Ejemplo:** Algunos tipos de datos impiden que los usuarios introduzcan más de un determinado número de caracteres. Puede utilizar la función subcadena para limitar un valor a un determinado número de caracteres.

En este ejemplo, la función de subcadena limita el nombre del proyecto a 50 caracteres.

![](assets/example-meet-length-restriction-350x184.png)

>[!ENDSHADEBOX]

## Anidado de funciones

Puede anidar funciones entre sí.

## Usar funciones de [!DNL Google Sheets]

Si [!DNL Workfront Fusion] no incluye una función que desee usar, pero la incluye [!DNL Google Sheets], puede usarla siguiendo estos pasos:

1. En [!DNL Google Sheets], cree una nueva hoja de cálculo vacía.
1. En [!DNL Workfront Fusion], abra su escenario.
1. Agregue el módulo **[!DNL Google Sheets]** >**[!UICONTROL Actualizar una celda]** al escenario.

   Para obtener instrucciones sobre cómo agregar un módulo, consulte [Agregar un módulo en un escenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) en el artículo [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configure el módulo:

   1. Elija la hoja de cálculo recién creada en el campo **[!UICONTROL Hoja de cálculo]**.
   1. Inserte la fórmula que contiene las funciones [!DNL Google Sheets] en el campo **[!UICONTROL Valor]**.

      Puede utilizar la salida de los módulos anteriores como de costumbre.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Inserte el módulo **[!UICONTROL Hojas de cálculo de Google] >[!UICONTROL Obtenga un módulo de celda]** para obtener el resultado calculado.
1. Configure el módulo con el mismo ID de celda utilizado en el paso 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
