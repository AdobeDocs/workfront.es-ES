---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funciones matemáticas en Adobe Workfront Fusion
description: Las siguientes funciones matemáticas están disponibles en el panel de asignación de Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Funciones matemáticas en [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL average ([matriz de valores]) average(value1; [value2], ...)]

Devuelve el valor medio de los valores numéricos de una matriz específica o el valor medio de los valores numéricos introducidos individualmente.

## [!UICONTROL ceil (número)]

Devuelve el menor entero bueno o igual que un número especificado.

>[!INFO]
>
>**Ejemplos:**
>
>* `ceil(` `1.2` `)`
   >
   >   Devuelve 2
>
>* `ceil(` `4` `)`
   >
   >   Devuelve 4


## [!UICONTROL suelo (número)]

Devuelve el mayor entero que sea menor o igual que un número especificado.

>[!INFO]
>
>**Ejemplos:**
>
>* `floor(` `1.2` `)`
   >
   >   Devuelve 1
>
>* `floor(` `1.9` `)`
   >
   >   Devuelve 1
>
>* `floor(` `4` `)`
   >
   >   Devuelve 4


## [!UICONTROL formatNumber (número; decimalPOINTS; [decimalSeparator]; [milesSeparator])]

Devuelve un número en el formato solicitado. De forma predeterminada, el punto decimal es una coma (,) y el separador de miles es un punto (.).

>[!INFO]
>
>**Ejemplo:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Devuelve 123.456.789.000

## [!UICONTROL max ([matriz de valores]), max(value1;value2; ...]

Devuelve el número mayor de una matriz especificada o el número mayor entre los números introducidos individualmente.

## [!UICONTROL min ([matriz de valores]), min(value1; value2; ...]

Devuelve el número más pequeño de una matriz especificada o el número más pequeño entre los números introducidos individualmente.

## [!UICONTROL parseNumber (número; separador decimal)]

Analiza una cadena con un número y devuelve el número. Por ejemplo, parseNumber(1 756,456;,)

## [!UICONTROL round (número)]

Redondea un valor numérico al entero más cercano.

>[!INFO]
>
>**Ejemplos:**
>
>* `round(` `1.2` `)`
   >
   >   Devuelve 1
>
>* `round(` `1.5` `)`
   >
   >   Devuelve 2
>
>* `round(` `1.7` `)`
   >
   >   Devuelve 2
> 
>* `round(` `2` `)`
   >
   >   Devuelve 2


## [!UICONTROL sum ([matriz de valores]), sum(value1; value2; ...]

Devuelve la suma de los valores de una matriz especificada o la suma de números introducidos individualmente.
