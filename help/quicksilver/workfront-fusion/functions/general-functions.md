---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funciones generales en Adobe Workfront Fusion
description: Las siguientes funciones generales están disponibles en el panel de asignación de Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 5cd1cbd1976d5574668098be53daee780a9cc1fb
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Funciones generales en [!DNL Adobe Workfront Fusion]

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
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL get (objeto o matriz; ruta de acceso)]

Devuelve la ruta de valor de un objeto o matriz. Para acceder a objetos anidados, utilice la notación de puntos. El primer elemento de una matriz es el índice 1.

>[!INFO]
>
>**Ejemplos:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if (expresión; valor1; valor2)]

Devuelve `value1` si la expresión se evalúa como verdadera; en caso contrario, devuelve `value2`.

Para crear una instrucción if que devuelva un valor sólo si dos o más expresiones se evalúan como true, utilice la palabra clave `and`.

Para combinar instrucciones `if`, use los operadores `and` y `or`.

![y operador](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**Ejemplos:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Devuelve un
>
>* `if( 1 = 2 ; A ; B )`
>
>   Devuelve B
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    Devuelve B
>   

## [!UICONTROL ifempty (value1; value2)]

Devuelve `value1` si este valor no está vacío; en caso contrario, devuelve `value2`.

>[!INFO]
>
>**Ejemplos:**
>
>* `ifempty(` `A` `;` `B` )
>
>   Devuelve un
>
>* `ifempty(` `unknown` `;` `B` )
>
>   Devuelve B
>
>* `ifempty(` `""` `;` `B` )
>
>   Devuelve B

## [!UICONTROL modificador (expresión; valor1; resultado1; [valor2; resultado2; ...]; [Else])]

Evalúa un valor (denominado expresión) frente a una lista de valores; devuelve el resultado correspondiente al primer valor coincidente. Para incluir un valor `else`, agréguelo después de la expresión o valor final.

>[!INFO]
>
>**Ejemplos:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Devuelve 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Devuelve 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>   Devuelve 4
>   
>   En esta función, 4 es el valor que se devuelve si no se aplica ninguna expresión (el valor `else`).

## [!UICONTROL omitir(objeto; clave1; [clave2; ...])]

Omite las claves dadas del objeto y devuelve el resto.

>[!INFO]
>
>**Ejemplo:**
>
>`omit(` Usuario `;` contraseña `)`
>
>Devuelve una colección de información del usuario, excluida la contraseña.

## [!UICONTROL pick(object; key1; [key2; ...])]

Selecciona solo las claves dadas del objeto.

>[!INFO]
>
>**Ejemplo:**
>
>`pick(` Usuario `;` contraseña `;` correo electrónico `)`
>
>Devuelve una colección que incluye únicamente la contraseña y la dirección de correo electrónico del usuario.

## mergeCollections(colección1 ; colección2)

Combina dos colecciones combinando sus pares clave-valor. Si ambas colecciones contienen la misma clave, el valor de la segunda colección sobrescribe ese valor de la primera colección.

