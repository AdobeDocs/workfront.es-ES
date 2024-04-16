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
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# Funciones matemáticas en [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

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
   <p>Actual: No [!DNL Workfront Fusion] requisito de licencia.</p> 
   <p>O</p> 
   <p>Heredado: cualquiera </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Product</td>  
   <td> 
   <p>Nuevo:</p> <ul><li>[!UICONTROL Seleccionar] o [!UICONTROL Prime] [!DNL Workfront] Plan: su organización debe comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] está incluido.</li></ul> 
   <p>O</p> 
   <p>Actual: Su organización debe comprar [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL media ([matriz de valores]) average(valor1; [value2], ...)]

Devuelve el valor promedio de los valores numéricos de una matriz específica o el valor promedio de los valores numéricos introducidos individualmente.

## [!UICONTROL ceil (número)]

Devuelve el menor entero que sea mayor o igual que un número especificado.

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

## [!UICONTROL floor (número)]

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

## [!UICONTROL max ([matriz de valores]), max(valor1;valor2; ...)]

Devuelve el número mayor de una matriz especificada o el número mayor entre los números introducidos individualmente.

## [!UICONTROL min ([matriz de valores]), min(valor1; valor2; ...)]

Devuelve el menor número de una matriz especificada o el menor número entre los números introducidos individualmente.

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

## [!UICONTROL sum ([matriz de valores]), sum(valor1; valor2; ...)]

Devuelve la suma de los valores de una matriz especificada o la suma de los números introducidos individualmente.

## [!UICONTROL parseNumber (número; separador decimal)]

Analiza una cadena con un número y devuelve el número. Por ejemplo, parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (número; decimalPOINTS; [decimalSeparator]; [milesSeparator])]

Devuelve un número en formato solicitado. De forma predeterminada, el punto decimal es una coma (,) y el separador de miles es un punto (.).

>[!INFO]
>
>**Ejemplo:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Devuelve 123 456 789 000
