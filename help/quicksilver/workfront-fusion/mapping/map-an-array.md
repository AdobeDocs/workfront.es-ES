---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Asignación de una matriz en [!DNL Adobe] Workfront Fusion
description: Puede asignar una matriz a un campo de módulo en Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Asignación de una matriz en [!DNL Adobe Workfront Fusion]

Una matriz es un tipo especial de elemento que puede contener lo siguiente:

* Uno o más valores de texto (matriz simple)
* Una o más colecciones del mismo tipo (matriz compleja)

>[!INFO]
>
>**Ejemplo:** La variable [!UICONTROL Ver correos electrónicos] devuelve una matriz de archivos adjuntos para cada correo electrónico. Cada archivo adjunto representa una colección que puede contener un nombre, contenido, tamaño, etc.

Para obtener más información, consulte [Tipos de datos de elementos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Asignación de una matriz

1. Haga clic en el botón situado en el campo de destino.

   >[!INFO]
   >
   >  **Ejemplo:** Para el ejemplo anterior, debe hacer clic en el [!UICONTROL Añadir un archivo adjunto] para un correo electrónico.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. En el cuadro que aparece, introduzca el elemento.

   El panel le permite asignar campos del mismo modo que con cualquier otro tipo de elemento. Si no desea rellenar cada elemento por separado, pero desea asignar otra matriz al campo de destino, utilice la variable [!UICONTROL Mapa] botón. En este caso, asegúrese de que ambas matrices (la matriz de origen y la matriz de destino) tengan la misma estructura.

   Puede agregar cualquier número de elementos a una matriz.

Puede dividir una matriz en paquetes individuales utilizando un iterador. Para obtener más información, consulte [[!UICONTROL Iterador] módulo en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
