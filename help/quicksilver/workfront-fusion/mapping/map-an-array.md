---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Asignar una matriz en  [!DNL Adobe] Workfront Fusion
description: Puede asignar una matriz a un campo de módulo en Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: f87bc22f4ce70f266a199fcb54c5a74f9e3ba914
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# Asignar una matriz en [!DNL Adobe Workfront Fusion]

Una matriz es un tipo especial de elemento que puede contener lo siguiente:

* Uno o más valores de texto (matriz simple)
* Una o más colecciones del mismo tipo (matriz compleja)

>[!INFO]
>
>**Ejemplo:** El módulo [!UICONTROL Ver correos electrónicos] devuelve una matriz de archivos adjuntos para cada correo electrónico. Cada archivo adjunto representa una colección que puede contener un nombre, contenido, tamaño, etc.

Para obtener más información, vea [Tipos de datos de elementos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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



## Asignar una matriz completa

1. En los módulos a los que va a asignar la matriz, haga clic en el campo en el que desee asignar la matriz. Este es el campo al que está asignada la matriz.

1. En el cuadro que aparece, asigne el elemento.

   El panel le permite asignar campos del mismo modo que con cualquier otro tipo de elemento. Si no desea rellenar cada elemento por separado pero desea asignar otra matriz al campo de destino, utilice el botón [!UICONTROL Asignar]. En este caso, asegúrese de que ambas matrices (la matriz de origen y la matriz de destino) tienen la misma estructura.

   Puede agregar cualquier número de elementos a una matriz.

Puede dividir una matriz en paquetes individuales mediante un iterador. Para obtener más información, consulte el módulo [[!UICONTROL Iterator] en [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/modules/iterator-module.md).

## Asignar elementos a una nueva matriz

Algunos campos de Workfront Fusion permiten asignar elementos a una matriz. Por ejemplo, puede crear una matriz de elementos de lista de comprobación en el módulo Tableros de Workfront > Agregar elemento de lista de comprobación. Cuando se ejecuta el módulo, todos los elementos de la lista de comprobación se añaden a la tarjeta.

Cualquier campo de módulo que muestre &quot;Agregar elemento&quot; crea una matriz.

![Agregar elemento](assets/add-item.png)

Para agregar elementos a la matriz:

1. Haga clic en **Agregar elemento**
1. En el panel que se abre, escriba detalles sobre el elemento.
1. Haga clic en **Agregar**.
1. (Opcional) Repita los pasos del 1 al 3 con cada elemento que desee agregar a la matriz .

## Asignar elementos de matriz


### Asignar elementos de matriz por número

Los elementos de la matriz se muestran como un número entre corchetes después del nombre de la matriz. Puede asignar un elemento individual de una matriz a un campo utilizando este número de índice.

![](assets/map-array-1st-element.png)

>[!NOTE]
>
>La indexación de matrices en Workfront Fusion comienza desde 1.

Para asignar un elemento de matriz:

1. Haga clic en el campo donde desee asignar el elemento.

   Se abrirá el panel Asignación.

1. Busque la matriz que contiene el elemento que desea asignar.
1. Haga clic en la flecha desplegable situada junto a la matriz.
1. Haga clic en el elemento que desee asignar.

   El elemento se asigna con el índice de 1. Esto asigna el primer elemento de la matriz.

1. Para asignar un elemento diferente de la matriz, haga clic en [1] e introduzca el número de índice del elemento de matriz que desea asignar.

   ![](assets/access-another-element.png)

### Asignar un elemento de una matriz con una clave determinada

Algunas matrices contienen colecciones con elementos clave-valor como metadatos, atributos, etc. Para utilizar uno de estos valores, puede buscar un elemento por su valor clave dado y obtener el valor correspondiente del elemento de valor. Se recomienda utilizar una fórmula que emplee una combinación de las funciones `map()` y `get()`.



>[!BEGINSHADEBOX]

El siguiente ejemplo muestra el resultado de la aplicación [!DNL Jira].

![](assets/output-of-jira-app-350x100.png)

Este ejemplo obtiene un nombre de archivo de una matriz de archivos adjuntos, para el archivo adjunto específico con un ID de 10108.

Este ejemplo genera el siguiente resultado:

![](assets/output-from-jira-350x261.png)

La fórmula se puede explicar de la siguiente manera:

* `map`

   1. El primer parámetro de la función `map()` es todo el elemento de matriz.
   1. El segundo parámetro es el nombre sin procesar del elemento de valor. Para obtener el nombre sin procesar, pase el ratón sobre el elemento del panel [!UICONTROL mapping]:

      ![](assets/obtain-raw-name-350x124.png)

      >[!NOTE]
      >
      >Todos los parámetros distinguen entre mayúsculas y minúsculas. Aunque en este ejemplo concreto la etiqueta del elemento difiere de su nombre sin procesar solo en mayúsculas, es necesario utilizar el nombre sin procesar.

   1. El tercer parámetro es el nombre sin procesar del elemento clave:

      ![](assets/3rd-parameter-350x166.png)

   1. El cuarto parámetro es el valor de clave dado.

  Dado que la función `map()` devuelve una matriz (ya que podría haber más elementos con el valor de clave dado), es necesario aplicar la función `get()` para obtener su primer elemento:

* `get`

   1. El primer parámetro de la función `get()` es el resultado de la función `map()`.

   1. El segundo parámetro es el índice del elemento. En este ejemplo, el índice es `1`.

Este ejemplo genera el siguiente resultado:

![](assets/output-from-jira-350x261.png)

>[!ENDSHADEBOX]

Para obtener más información acerca de la función `map()`, vea [Funciones de matriz](/help/quicksilver/workfront-fusion/functions/array-functions.md).

Para obtener más información acerca de la función `get()`, vea [Funciones generales](/help/quicksilver/workfront-fusion/functions/general-functions.md).

## Conversión de elementos de matriz en una serie de paquetes

Las matrices se pueden convertir en una serie de paquetes mediante el módulo [!UICONTROL Iterator]. Para obtener más información, consulte [[!UICONTROL Iterator] module](/help/quicksilver/workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles.png)

