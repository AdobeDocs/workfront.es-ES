---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Módulos de imagen
description: Los módulos de imagen de Adobe Workfront Fusion le permiten obtener información sobre una imagen específica (dimensiones, tipo, etc.), convertir una imagen a otro formato de archivo y cambiar directamente el tamaño de la imagen.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Módulos de imagen

[!DNL Adobe Workfront Fusion] [!UICONTROL Imagen] Los módulos de permiten obtener información sobre una imagen específica (dimensiones, tipo, etc.), convertir una imagen a otro formato de archivo y cambiar directamente el tamaño de la imagen.

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

## [!UICONTROL Imagen] módulos y sus campos

Al configurar este módulo, se muestran los campos siguientes. Un título en negrita en un módulo indica un campo obligatorio.

* [[!UICONTROL Redimensionar]](#resize)
* [[!UICONTROL Convertir un formato]](#convert-a-format)
* [[!UICONTROL Extraer metadatos]](#extract-metadata)

### [!UICONTROL Redimensionar]

Este módulo transformador cambia la altura y anchura de una imagen según los criterios especificados.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione el origen de la imagen que desea convertir. Puede seleccionar la salida de un módulo anterior o asignar el archivo de datos y el nombre de archivo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datos]</td> 
   <td>Asigne el archivo que desea convertir. Este campo está disponible si ha seleccionado [!UICONTROL Map] en el campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de archivo]</td> 
   <td>Introduzca un nombre para el archivo convertido. Este campo está disponible si ha seleccionado [!UICONTROL Map] en el campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Deseo]</td> 
   <td>Seleccione si desea mantener la relación altura-anchura o cambiar las dimensiones a una altura y anchura especificadas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Según]</td> 
   <td> <p>Seleccione cómo desea que el módulo determine el nuevo tamaño de la imagen. Este campo aparece si ha seleccionado mantener la relación altura-anchura en el campo Deseo. Aparecerán otros campos en función de la selección de este campo.</p> 
    <ul> 
     <li> <p>[!UICONTROL Anchura máxima]</p> <p>Reduce una imagen al ancho especificado. La altura se calcula automáticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura máxima]</p> <p>Reduce una imagen a la altura especificada. La anchura se calcula automáticamente.</p> </li> 
     <li> <p>[!UICONTROL Alto o ancho máximo]</p> <p>Reduce una imagen de forma que su altura y anchura no superen los valores especificados. Debido a que esta opción mantiene la relación altura-anchura, una de las dimensiones puede ser más pequeña de lo especificado. Por ejemplo, si la altura y la anchura se especifican como 40, una imagen de 400 x 300 se reducirá a 40 x 30.</p> </li> 
     <li> <p>[!UICONTROL Anchura mínima]</p> <p>Amplía una imagen a la anchura especificada. La altura se calcula automáticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura mínima]</p> <p>Aumenta el tamaño de una imagen hasta la altura especificada. La anchura se calcula automáticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura o anchura mínima]</p> <p>Amplía una imagen de forma que su altura y anchura no sean menores que los valores especificados. Debido a que esta opción mantiene la relación altura-anchura, una de las dimensiones puede ser más grande de lo especificado. Por ejemplo, si la altura y la anchura se especifican como 300, una imagen de 40x30 se ampliará a 400X300.</p> </li> 
     <li> <p>[!UICONTROL Porcentaje]</p> <p>Cambia el tamaño de la imagen en un porcentaje basado en el valor especificado. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anchura]</td> 
   <td>Introduzca o asigne la anchura deseada de la imagen cuyo tamaño se ha cambiado en píxeles.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altura]</td> 
   <td>Introduzca o asigne la altura deseada de la imagen cuyo tamaño se ha cambiado en píxeles.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir un formato]

Este módulo transformador cambia el formato de un archivo de imagen. Este módulo es compatible con los siguientes formatos:

* PNG
* JPG
* GIF
* BMP

Tanto el archivo de origen como la salida deben tener uno de estos formatos. Por ejemplo, la variable [!UICONTROL Imagen] >[!UICONTROL Convertir un formato] Este módulo puede transformar un archivo PNG en un archivo BMP o un BMP en un JPG.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione el origen de la imagen que desea convertir. Puede seleccionar la salida de un módulo anterior o asignar el archivo de datos y el nombre de archivo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datos]</td> 
   <td>Asigne el archivo que desea convertir. Este campo está disponible si ha seleccionado [!UICONTROL Map] en el campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de archivo]</td> 
   <td>Introduzca un nombre para el archivo convertido. Este campo está disponible si ha seleccionado [!UICONTROL Map] en el campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de salida]</td> 
   <td>Seleccione el formato en el que desea que el módulo convierta el archivo de origen. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extraer metadatos]

Este módulo transformador devuelve información básica sobre un módulo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione el origen de la imagen que desea convertir. Puede seleccionar la salida de un módulo anterior o asignar el archivo de datos y el nombre de archivo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datos]</td> 
   <td>Asigne el archivo que desea convertir. Este campo está disponible si ha seleccionado Asignar en el campo [!UICONTROL Archivo de origen].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de archivo]</td> 
   <td>Introduzca un nombre para el archivo convertido. Este campo está disponible si ha seleccionado Asignar en el campo [!UICONTROL Archivo de origen].</td> 
  </tr> 
 </tbody> 
</table>

## Posibles problemas

### La acción ha finalizado con un error

Existen tres casos en los que una acción puede finalizar con un error:

* Los datos recibidos no tenían el formato JPG/GIF/PNG/BMP
* Se ha superado el límite máximo de anchura y altura al cambiar las dimensiones de la imagen. El tamaño de la imagen no debe superar los 3840 píxeles de anchura y los 2160 píxeles de altura
* Se ha superado el tamaño máximo permitido de una imagen al cambiar las dimensiones o el formato de la imagen.
