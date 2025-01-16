---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funciones matemáticas en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 80%

---

# Funciones matemáticas en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Funciones matemáticas](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/math-functions.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

<!--Audited: 4/2024-->

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td role="rowheader">Producto</td>  
   <td> 
   <p>Nuevo:</p> <ul><li>Plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: su organización debe comprar [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] está incluido.</li></ul> 
   <p>O</p> 
   <p>Actual: su organización debe comprar [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL average ([array of values]) average(value1; [value2], ...)]

Devuelve el valor promedio de los valores numéricos en una matriz específica o el valor promedio de los valores numéricos introducidos individualmente.

## [!UICONTROL ceil (number)]

Devuelve el valor entero menor que sea mayor o igual que un número especificado.

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

## [!UICONTROL floor (number)]

Devuelve el valor entero más alto que sea menor o igual que un número especificado.

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

## [!UICONTROL max ([array of values]), max(value1;value2; ...)]

Devuelve el número mayor de una matriz especificada o el número mayor entre los números introducidos individualmente.

## [!UICONTROL min ([array of values]), min(value1; value2; ...)]

Devuelve el número menor dentro de una matriz especificada o el número menor entre los números introducidos individualmente.

## [!UICONTROL round (number)]

Redondea al valor numérico entero más cercano

>[!INFO]
>
>**Ejemplos**
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

## [!UICONTROL sum ([array of values]), sum(value1; value2; ...)]

Devuelve la suma de los valores en una matriz especificada o la suma de los números introducidos individualmente.

## [!UICONTROL parseNumber (number; decimal separator)]

Analiza una cadena con un número y devuelve el número. Por ejemplo, parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (number; decimalPOINTS; [decimalSeparator]; [thousandsSeparator])]

Devuelve un número en el formato solicitado. De forma predeterminada, el punto decimal es una coma (,) y el separador de miles es un punto (.).

>[!INFO]
>
>**Ejemplo:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Devuelve 123 456 789 000
