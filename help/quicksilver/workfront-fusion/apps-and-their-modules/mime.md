---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos MIME
description: Puede utilizar tipos MIME en Adobe Workfront Fusion. Los tipos MIME (Extensión multipropósito de correo de Internet) son etiquetas que permiten al software identificar diferentes tipos de datos compartidos en Internet. Los servidores y exploradores web utilizan el tipo MIME para determinar qué se debe hacer con un archivo. Por ejemplo, un archivo con el tipo MIME text/html se procesará en un explorador de forma diferente a un archivo con el tipo MIME image/jpeg. Los tipos MIME funcionan independientemente del sistema operativo y del hardware.
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# [!UICONTROL MIME] módulos

Puede utilizar tipos MIME en Adobe Workfront Fusion. Los tipos MIME (Extensión multipropósito de correo de Internet) son etiquetas que permiten al software identificar diferentes tipos de datos compartidos en Internet. Los servidores y exploradores web utilizan el tipo MIME para determinar qué se debe hacer con un archivo. Por ejemplo, un archivo con el tipo MIME `text/html` se procesarán en un explorador de forma diferente a un archivo con tipo MIME `image/jpeg`. Los tipos MIME funcionan independientemente del sistema operativo y del hardware.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
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

## [!UICONTROL MIME] módulos y sus campos

### [!UICONTROL Obtener un tipo MIME]

Este módulo transformador devuelve el tipo MIME asociado con un nombre, ruta o extensión determinados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo]</td> 
   <td> <p>Introduzca o asigne el archivo para el que desea determinar el tipo MIME. </p> <p>Puede introducir el archivo mediante:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ruta de archivo]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Nombre de archivo]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Extensión de archivo]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtener una extensión de archivo]

Este módulo transformador devuelve la extensión de archivo original para un tipo MIME determinado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL tipo MIME]</td> 
   <td> <p>Introduzca o asigne el tipo MIME para el que desea determinar la extensión de archivo. </p> </td> 
  </tr> 
 </tbody> 
</table>
