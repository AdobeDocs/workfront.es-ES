---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Acerca de la asignación de archivos en [!DNL Adobe Workfront Fusion]
description: Algunos módulos tienen la capacidad de procesar archivos. Estos módulos pueden devolver un archivo de salida para enviarlo para un procesamiento posterior o requerir que se les pase un archivo para su procesamiento. Antes de que estos módulos puedan trabajar juntos para procesar archivos, deben asignarse entre sí.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Acerca de la asignación de archivos en [!DNL Adobe Workfront Fusion]

Algunos módulos tienen la capacidad de procesar archivos. Estos módulos pueden devolver un archivo de salida para enviarlo para un procesamiento posterior o requerir que se les pase un archivo para su procesamiento. Antes de que estos módulos puedan trabajar juntos para procesar archivos, deben asignarse entre sí.

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
  </tr>  </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Asignación de archivos

Los módulos que tienen la capacidad de trabajar con archivos requieren dos fragmentos de información:

* Nombre del archivo
* Contenido del archivo (datos)

Al asignar un archivo, se eligen los módulos del escenario desde los que se desea obtener los datos. El nombre del archivo y el contenido del archivo se asignan automáticamente tal cual.

>[!NOTE]
>
>Si necesita procesar un archivo desde una dirección URL, le recomendamos que use el complemento `HTTP > Get a File` para descargar el archivo desde la dirección URL y, a continuación, asignar el archivo desde el `HTTP > Get a File` al campo del módulo deseado en su escenario.

>[!INFO]
>
>**Ejemplo:** Este ejemplo muestra cómo descargar documentos de [!DNL Adobe Workfront] a [!DNL Google Drive]. La variable [!DNL Workfront] déclencheur [!UICONTROL Registro de Watch] devuelve información detallada sobre cada documento, incluido su nombre y su ID.
>
>El siguiente módulo, [!UICONTROL Descargar documento], descarga los datos reales para que se puedan cargar en Google Drive.
>
>Para asignar esta información a [!DNL Google Drive] para que se pueda cargar, debe especificar el archivo de origen desde el que se asignará la información. Si selecciona la opción [!DNL Workfront] > [!UICONTROL Descargar documento] en el archivo de origen, [!DNL Workfront Fusion] asigna el nombre del archivo y el contenido del archivo para que el documento [!DNL Workfront] se carga en la carpeta Google especificada.
>
>![](assets/wf-download-document-350x605.png)
>
>Sin embargo, si desea cambiar el nombre del archivo, pero conservar los datos tal cual, puede usar la variable [!UICONTROL Mapa] para asignar el nombre del archivo y el contenido del archivo por separado. Debe introducir el nombre completo del archivo, incluida la extensión. Se admiten formatos de texto y formatos binarios, como fotos, vídeos y PDF.
>
>![](assets/use-the-map-option-350x358.png)
