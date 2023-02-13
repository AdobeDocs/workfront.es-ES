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
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '603'
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

## [!UICONTROL add (array; value1; value2; ...]

Agrega valores especificados en parámetros a una matriz y devuelve esa matriz.

## [!UICONTROL contiene (matriz; value)]

Comprueba si una matriz contiene el valor .

## [!UICONTROL distinto (matriz; [key])]

Elimina los duplicados dentro de una matriz. Utilice el[!UICONTROL key]&quot; para acceder a propiedades dentro de objetos complejos. Para acceder a las propiedades anidadas, utilice la notación de puntos. El primer elemento de una matriz es el índice 1.

>[!INFO]
>
>**Ejemplo:** `distinct(Contacts[];name)`
>
>Elimina los duplicados dentro de una matriz de contactos comparando la propiedad &quot;name&quot;

## [!UICONTROL acoplado (matriz)]

Crea una nueva matriz con todos los elementos de la submatriz concatenados en ella, recursivamente, hasta la profundidad especificada.


## [!UICONTROL join (array; separador)]

Concatena todos los elementos de una matriz en una cadena, utilizando el separador especificado entre cada elemento.

## [!UICONTROL teclas (objeto)]

Devuelve una matriz de las propiedades de un objeto o matriz determinados.

## [!UICONTROL length (array)]

Devuelve el número de elementos de una matriz.

## [!UICONTROL map (matriz compleja); clave;[clave para filtrar];[posibles valores para filtrar])]

Devuelve una matriz primitiva que contiene valores de una matriz compleja. Esta función permite filtrar valores. Utilice nombres de variables sin procesar para claves.

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
>  Devuelve una matriz primitiva con correos electrónicos con una etiqueta igual al trabajo o al inicio

Para obtener más información, consulte [Asignar información de un módulo a otro en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL combinar (array1; array2; ...]

Combina una o más matrices en una matriz.

## [!UICONTROL remove (array; value1; value2; ...]

Elimina los valores especificados en los parámetros de una matriz. Esta función solo es efectiva en matrices primitivas de texto o números.

## [!UICONTROL reverso (matriz)]

El primer elemento de la matriz se convierte en el último elemento, el segundo se convierte en el siguiente al último, etc.

## [!UICONTROL fracción (matriz; start; [end])]

Devuelve una nueva matriz que contiene solo elementos seleccionados.

## [!UICONTROL sort (array; [pedido]; [key])]

Ordena los valores de una matriz. Los valores válidos de la variable `order` son:

* `asc`

   (predeterminado) - orden ascendente: 1, 2, 3, ... para el tipo Número. A, B, C, a, b, c... para el tipo Texto

* `desc`

   orden descendente: ..., 3, 2, 1 para el tipo Número. ..., c, b, a, C, B, A para el tipo Texto.

* `asc ci`

   orden ascendente sin distinción de mayúsculas y minúsculas: A, a, B, b, C, c, ... para el tipo Texto.

* `desc ci`

   orden descendente sin distinción de mayúsculas y minúsculas: ..., C, c, B, b, A, a para el tipo Texto.

Utilice la variable `key` para acceder a las propiedades dentro de objetos complejos.

Utilice nombres de variables sin procesar para claves.

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
   >    Ordena una matriz de contactos por la propiedad &quot;name&quot; en orden ascendente que no distingue entre mayúsculas y minúsculas
>
>* `sort(Emails[];sender.name)`
   >
   >    Ordena una matriz de correos electrónicos por la propiedad &quot;sender.name&quot;


## [!UICONTROL arrayDifference [array1, array2, mode]]

Devuelve la diferencia entre dos matrices.

Introduzca uno de los siguientes valores para la variable `mode` parámetro.

* `classic`: Devuelve una nueva matriz que contiene todos los elementos de `array1` que no existen en `array2`.

* `symmetric`: Devuelve una matriz de elementos que no son comunes a ambas matrices.

   En otras palabras, la función devuelve una matriz que contiene todos los elementos de `array1` que no existen en `array2`y todos los elementos de `array2` que no existen en `array1`.

   >[!INFO]
   >
   >**Ejemplos:**
   >
   >Dadas las siguientes matrices:
   >
   >
   ```
   >myArray = [1,2,3,4,5]
   >```
   >
   >
   ```
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

