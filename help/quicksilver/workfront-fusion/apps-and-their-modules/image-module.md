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
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Módulos de imagen

[!DNL Adobe Workfront Fusion] [!UICONTROL Imagen] los módulos permiten obtener información sobre una imagen específica (dimensiones, tipo, etc.), convertir una imagen a otro formato de archivo y cambiar directamente el tamaño de la imagen.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Imagen] módulos y sus campos

Al configurar este módulo, se muestran los campos siguientes: Un título en negrita en un módulo indica un campo obligatorio.

* [[!UICONTROL Cambiar tamaño]](#resize)
* [[!UICONTROL Convertir un formato]](#convert-a-format)
* [[!UICONTROL Extraer metadatos]](#extract-metadata)

### [!UICONTROL Cambiar tamaño]

Este módulo de transformador cambia la altura y la anchura de una imagen según los criterios especificados.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione el origen de la imagen que desea convertir. Puede seleccionar la salida de un módulo anterior o asignar el archivo de datos y el nombre de archivo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Asigne el archivo que desea convertir. Este campo está disponible si ha seleccionado [!UICONTROL Map] en el campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Introduzca un nombre para el archivo convertido. Este campo está disponible si ha seleccionado [!UICONTROL Map] en el campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL que quiero]</td> 
   <td>Seleccione si desea mantener la relación alto-ancho o cambiar las dimensiones a una altura y anchura especificadas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Según]</td> 
   <td> <p>Seleccione cómo desea que el módulo determine el nuevo tamaño de la imagen. Este campo aparece si ha seleccionado mantener la relación alto-ancho en el campo I want to . Aparecen otros campos basados en la selección de este campo.</p> 
    <ul> 
     <li> <p>[!UICONTROL Ancho máximo]</p> <p>Reduce la anchura especificada de una imagen. La altura se calcula automáticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura máxima]</p> <p>Reduce una imagen a la altura especificada. La anchura se calcula automáticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura o anchura máximas]</p> <p>Reduce una imagen de forma que su altura y anchura no excedan los valores especificados. Debido a que esta opción mantiene la relación alto-ancho, una de las dimensiones puede ser menor que la especificada. Por ejemplo, si la altura y la anchura se especifican como 40, una imagen de 400 x 300 se reducirá a 40 x 30.</p> </li> 
     <li> <p>[!UICONTROL Ancho mínimo]</p> <p>Aumenta la imagen a un ancho especificado. La altura se calcula automáticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura mínima]</p> <p>Aumenta una imagen a una altura especificada. La anchura se calcula automáticamente.</p> </li> 
     <li> <p>[!UICONTROL Altura o anchura mínimas]</p> <p>Aumenta una imagen de forma que su altura y anchura no sean menores que los valores especificados. Debido a que esta opción mantiene la relación alto-ancho, una de las dimensiones puede ser mayor de lo especificado. Por ejemplo, si la altura y la anchura se especifican como 300, una imagen de 40 x 30 se ampliará a 400 x 300.</p> </li> 
     <li> <p>[!UICONTROL Porcentaje]</p> <p>Cambia el tamaño de la imagen en un porcentaje según el valor que especifique. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ancho]</td> 
   <td>Introduzca o asigne el ancho deseado de la imagen cuyo tamaño se ha cambiado de tamaño en píxeles.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altura]</td> 
   <td>Introduzca o asigne la altura deseada de la imagen redimensionada en píxeles.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir un formato]

Este módulo de transformador cambia el formato de un archivo de imagen. Este módulo es compatible con los siguientes formatos:

* PNG
* JPG
* GIF
* BMP

Tanto el archivo de origen como la salida deben estar en uno de estos formatos. Por ejemplo, la variable [!UICONTROL Imagen] >[!UICONTROL Convertir un formato] puede transformar un archivo PNG en un archivo BMP o BMP en un JPG.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione el origen de la imagen que desea convertir. Puede seleccionar la salida de un módulo anterior o asignar el archivo de datos y el nombre de archivo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Asigne el archivo que desea convertir. Este campo está disponible si ha seleccionado [!UICONTROL Map] en el campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Introduzca un nombre para el archivo convertido. Este campo está disponible si ha seleccionado [!UICONTROL Map] en el campo [!UICONTROL Source file].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de salida]</td> 
   <td>Seleccione el formato al que desea que el módulo convierta el archivo de origen. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extraer metadatos]

Este módulo de transformador devuelve información básica sobre un módulo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione el origen de la imagen que desea convertir. Puede seleccionar la salida de un módulo anterior o asignar el archivo de datos y el nombre de archivo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Asigne el archivo que desea convertir. Este campo está disponible si ha seleccionado Map en el campo [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Introduzca un nombre para el archivo convertido. Este campo está disponible si ha seleccionado Map en el campo [!UICONTROL Source file] .</td> 
  </tr> 
 </tbody> 
</table>

## Posibles problemas

### Acción terminada con un error

Hay tres casos en los que una acción puede finalizar con un error:

* Los datos recibidos no estaban en formato JPG/GIF/PNG/BMP
* Se ha superado el límite máximo de anchura y altura al cambiar las dimensiones de la imagen. El tamaño de la imagen no debe superar la anchura de 3840 píxeles y la altura de 2160 píxeles
* Se ha superado el tamaño máximo permitido de una imagen al cambiar las dimensiones o el formato de la imagen.
