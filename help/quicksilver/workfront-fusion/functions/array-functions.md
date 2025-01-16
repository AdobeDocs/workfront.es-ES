---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funciones de matriz en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 89%

---

# Funciones de matriz en Adobe Workfront Fusion

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Funciones de matriz](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/array-functions.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

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

Para obtener información sobre licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Funciones 

* [join](#join-array-separator)
* [length](#length-array)
* [keys](#keys-object)
* [slice](#slice-array-start-end)
* [merge](#merge-array1-array2)
* [contiene](#contains-array-value)
* [remove](#remove-array-value1-value2)
* [add](#add-array-value1-value2)
* [map](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [shuffle]
* [sort](#sort-array-order-key)
* [reverse](#reverse-array)
* [flatten](#flatten-array)
* [distinct](#distinct-array-key)
* [toCollection]
* [toArray](#toarray)
* [arrayDifference](#arraydifference-array1-array2-mode)
* [deduplicate]

### [!UICONTROL join (array; separator)]

Concatena todos los elementos de una matriz en una cadena, utilizando el separador especificado entre cada elemento.

### [!UICONTROL length (array)]

Devuelve el número de elementos de una matriz.

### [!UICONTROL keys (object)]

Devuelve una matriz de las propiedades de un objeto o matriz determinados.

### [!UICONTROL slice (array; start; [end])]

Devuelve una nueva matriz que contiene solo los elementos seleccionados.

### [!UICONTROL merge (array1; array2; ...)]

Combina una o más matrices en una matriz.

### [!UICONTROL contains (array; value)]

Comprueba si una matriz contiene el valor.

### [!UICONTROL remove (array; value1; value2; ...)]

Quita los valores especificados en los parámetros de una matriz. Esta función sólo es efectiva en matrices primitivas de texto o números.

### [!UICONTROL add (array; value1; value2; ...)]

Añade los valores especificados en parámetros a una matriz y devuelve esa matriz.

### [!UICONTROL map (complex array; key;[key for filtering];[possible values for filtering])]

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

Para obtener más información, consulte [Asignar información de un módulo a otro en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)

### shuffle

### [!UICONTROL sort (array; [order]; [key])]

Ordena los valores de una matriz. Los valores válidos del parámetro `order` son los siguientes:

* `asc`

  (predeterminado): orden ascendente: 1, 2, 3, ... para el tipo Número. A, B, C, a, b, c, ... para el tipo Texto

* `desc`

  orden descendente: ..., 3, 2, 1 para el tipo Número. ..., c, b, a, C, B, A para el tipo Texto.

* `asc ci`

  orden ascendente sin distinción de mayúsculas y minúsculas: A, a, B, b, C, c, ... para el tipo Texto.

* `desc ci`

  orden descendente sin distinción de mayúsculas y minúsculas: ..., C, c, B, b, A, a para el tipo Texto.

Utilice el parámetro `key` para tener acceso a las propiedades de objetos complejos.

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
>    Ordena una matriz de contactos por la propiedad “name” en orden ascendente sin distinción de mayúsculas y minúsculas
>
>* `sort(Emails[];sender.name)`
>
>    Ordena una matriz de correos electrónicos por la propiedad “sender.name”

### [!UICONTROL reverse (array)]

El primer elemento de la matriz se convierte en el último elemento, el segundo en el último, etc.

### [!UICONTROL flatten (array)]

Crea una nueva matriz con todos los elementos de submatriz concatenados en ella, de forma recursiva, hasta la profundidad especificada.

### [!UICONTROL distinct (array; [key])]

Elimina los duplicados dentro de una matriz. Utilice el argumento &quot;[!UICONTROL key]&quot; para tener acceso a las propiedades de objetos complejos. Para acceder a las propiedades anidadas, utilice la notación de puntos. El primer elemento de una matriz es el índice 1.

>[!INFO]
>
>**Ejemplo:**`distinct(Contacts[];name)`
>
>Elimina los duplicados dentro de una matriz de contactos comparando la propiedad “name”

### toCollection

### toArray

Esta función convierte una colección en una matriz de pares clave-valor.

>[!INFO]
>
>**Ejemplos:**
>
>Dada la colección
>
>`{ key1: "value1", key2: "value2:}`
>
>La función
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>Devuelve la matriz de pares clave-valor
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [array1, array2, mode]]

Devuelve la diferencia entre dos matrices.

Introduzca uno de los siguientes valores para el parámetro `mode`.

* `classic`: devuelve una nueva matriz que contiene todos los elementos de `array1` que no existen en `array2`.

* `symmetric`: devuelve una matriz de elementos que no son comunes a ambas matrices.

  En otras palabras, la función devuelve una matriz que contiene todos los elementos de `array1` que no existen en `array2` y todos los elementos de `array2` que no existen en `array1`.

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

### deDuplicate

## Keywords

### emptyarray
