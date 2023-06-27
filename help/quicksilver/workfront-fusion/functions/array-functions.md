---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funciones de matriz en Adobe Workfront Fusion
description: Las siguientes funciones de matriz están disponibles en el panel de asignación de Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Funciones de matriz en Adobe Workfront Fusion

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

## [!UICONTROL add (matriz; valor1; valor2; ...)]

Agrega los valores especificados en parámetros a una matriz y devuelve esa matriz.

## [!UICONTROL contiene (matriz; valor)]

Comprueba si una matriz contiene el valor.

## [!UICONTROL distinct (matriz; [key])]

Elimina los duplicados dentro de una matriz. Utilice el &quot;[!UICONTROL key]&quot; para acceder a las propiedades dentro de objetos complejos. Para acceder a las propiedades anidadas, utilice la notación de puntos. El primer elemento de una matriz es el índice 1.

>[!INFO]
>
>**Ejemplo:** `distinct(Contacts[];name)`
>
>Elimina los duplicados dentro de una matriz de contactos comparando la propiedad &quot;name&quot;

## [!UICONTROL acoplar (matriz)]

Crea una nueva matriz con todos los elementos de submatriz concatenados en ella, de forma recursiva, hasta la profundidad especificada.


## [!UICONTROL unir (matriz; separador)]

Concatena todos los elementos de una matriz en una cadena, utilizando el separador especificado entre cada elemento.

## [!UICONTROL keys, objeto]

Devuelve una matriz de las propiedades de un objeto o matriz determinados.

## [!UICONTROL longitud (matriz)]

Devuelve el número de elementos de una matriz.

## [!UICONTROL map (matriz compleja; clave;[clave de filtrado];[valores posibles de filtrado])]

Devuelve una matriz primitiva que contiene los valores de una matriz compleja. Esta función permite filtrar valores. Utilice nombres de variables sin procesar para las claves.

>[!INFO]
>
>**Ejemplos:**
>
>* `map(Emails[];email)`
>
>  Devuelve una matriz primitiva con correos electrónicos
>
>* `map(Emails[];email;label;work;home)`
>
>  Devuelve una matriz primitiva con correos electrónicos que tienen una etiqueta igual a trabajo o inicio

Para obtener más información, consulte [Asignación de información de un módulo a otro en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL combinar (matriz1; matriz2; ...)]

Combina una o más matrices en una matriz.

## [!UICONTROL remove (matriz; valor1; valor2; ...)]

Quita los valores especificados en los parámetros de una matriz. Esta función sólo es efectiva en matrices primitivas de texto o números.

## [!UICONTROL inverso (matriz)]

El primer elemento de la matriz se convierte en el último elemento, el segundo en el último, etc.

## [!UICONTROL segmento (matriz; inicio; [fin])]

Devuelve una nueva matriz que contiene solo los elementos seleccionados.

## [!UICONTROL sort (matriz; [pedido]; [key])]

Ordena los valores de una matriz. Los valores válidos del `order` Los parámetros son:

* `asc`

  (predeterminado): orden ascendente: 1, 2, 3, ... para el tipo Número. A, B, C, a, b, c, ... para el tipo Texto

* `desc`

  orden descendente: ..., 3, 2, 1 para el tipo Número. ..., c, b, a, C, B, A para el tipo Texto.

* `asc ci`

  orden ascendente sin distinción de mayúsculas y minúsculas: A, a, B, b, C, c, ... para el tipo Texto.

* `desc ci`

  orden descendente sin distinción de mayúsculas y minúsculas: ..., C, c, B, b, A, a para el tipo Texto.

Utilice el `key` para acceder a propiedades dentro de objetos complejos.

Utilice nombres de variables sin procesar para las claves.

Para acceder a las propiedades anidadas, utilice la notación de puntos.

El primer elemento de una matriz es el índice 1.

>[!INFO]
>
>**Ejemplos:**
>
>* `sort(Contacts[];name)`
>
>    Ordena una matriz de contactos por la propiedad &quot;name&quot; en orden ascendente predeterminado
>
>* `sort(Contacts[];desc;name)`
>
>   Ordena una matriz de contactos por la propiedad &quot;name&quot; en orden descendente
>
>* `sort(Contacts[];asc ci;name)`
>
>    Ordena una matriz de contactos por la propiedad &quot;name&quot; en orden ascendente sin distinción de mayúsculas y minúsculas
>
>* `sort(Emails[];sender.name)`
>
>    Ordena una matriz de correos electrónicos por la propiedad &quot;sender.name&quot;

## [!UICONTROL arrayDifference [matriz1, matriz2, modo]]

Devuelve la diferencia entre dos matrices.

Introduzca uno de los siguientes valores para `mode` parámetro.

* `classic`: devuelve una nueva matriz que contiene todos los elementos de `array1` que no existen en `array2`.

* `symmetric`: Devuelve una matriz de elementos que no son comunes a ambas matrices.

  En otras palabras, la función devuelve una matriz que contiene todos los elementos de `array1` que no existen en `array2`y todos los elementos de `array2` que no existen en `array1`.

  >[!INFO]
  >
  >**Ejemplos:**
  >
  >Dadas las siguientes matrices:
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    Devuelve `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    Devuelve `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    Devuelve `[1,2,6,7]`
