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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 3%

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

## [!UICONTROL get (objeto o matriz; ruta)]

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

Devuelve el `value1` si la expresión se evalúa como verdadera; en caso contrario, devuelve el valor `value2`.

>[!INFO]
>
>**Ejemplos:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Devuelve un
>
>* `if( = 2 ; A ; B )`
>
>   Devuelve B

## [!UICONTROL ifempty (valor1; valor2)]

Devuelve el `value1` si este valor no está vacío; en caso contrario, devuelve el valor `value2`.

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

## [!UICONTROL switch (expresión; valor1; resultado1; [value2; result2; ...]; [else])]

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

## [!UICONTROL omit(objeto; key1; [key2; ...])]

Omite las claves dadas del objeto y devuelve el resto.

>[!INFO]
>
>**Ejemplo:**
>
>`omit(` Usuario `;` contraseña `)`
>
>Devuelve una colección de información del usuario, excluyendo >la contraseña.

## [!UICONTROL pick(objeto; key1; [key2; ...])]

Selecciona solo las claves dadas del objeto.

>[!INFO]
>
>**Ejemplo:**
>
>`pick(` Usuario `;` contraseña `;` email `)`
>
>Devuelve una colección que incluye únicamente la contraseña y la dirección de correo electrónico del usuario.
