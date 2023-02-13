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
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 2%

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

## [!UICONTROL get (objeto o matriz; path)]

Devuelve la ruta del valor de un objeto o matriz. Para acceder a los objetos anidados, utilice la notación de puntos. El primer elemento de una matriz es el índice 1.

>[!INFO]
>
>**Ejemplos:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`


## [!UICONTROL if (expresión; value1; value2)]

Devuelve la variable `value1` si la expresión se evalúa como verdadera; de lo contrario, devuelve la variable `value2`.

>[!INFO]
>
>**Ejemplos:**
>
>* `if( 1 = 1 ; A ; B )`
   >
   >    Devuelve A
>
>* `if( = 2 ; A ; B )`
   >
   >   Devuelve B


## [!UICONTROL ifempty (value1; value2)]

Devuelve la variable `value1` si este valor no está vacío, de lo contrario, devuelve la variable `value2`.

>[!INFO]
>
>**Ejemplos:**
>
>* `ifempty(` `A` `;` `B` )
   >
   >   Devuelve A
>
>* `ifempty(` `unknown` `;` `B` )
   >
   >   Devuelve B
>
>* `ifempty(` `""` `;` `B` )
   >
   >   Devuelve B


## [!UICONTROL switch (expresión; value1; result1; [value2; result2; ...]; [else])]

Evalúa un valor (denominado expresión) frente a una lista de valores; devuelve el resultado correspondiente al primer valor coincidente.

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
>  Devuelve 4

## [!UICONTROL omit(object; key1; [key2; ...])]

Omite las claves dadas del objeto y devuelve el resto.

>[!INFO]
>
>**Ejemplo:**
>
>`omit(` Usuario `;` password `)`
>
>Devuelve una colección de la información del usuario, excluyendo >la contraseña.

## [!UICONTROL pick(object; key1; [key2; ...])]

Solo selecciona las claves dadas del objeto.

>[!INFO]
>
>**Ejemplo:**
>
>`pick(` Usuario `;` password `;` email `)`
>
>Devuelve una colección de solamente la contraseña y la dirección de correo electrónico del usuario.
