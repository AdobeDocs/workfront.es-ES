---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Acerca de la asignación de archivos en [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 84%

---

# Acerca de la asignación de archivos en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Asignar un archivo entre módulos](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-files.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Algunos módulos tienen la capacidad de procesar archivos. Estos módulos pueden devolver un archivo de salida para enviarlo a un procesamiento posterior o requerir que se les pase un archivo para procesarlo. Para que estos módulos puedan trabajar juntos para procesar archivos, deben asignarse entre sí.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr>  </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Asignación de archivos

Los módulos con la capacidad de trabajar con archivos requieren dos fragmentos de información:

* Nombre del archivo
* Contenido de archivo (datos)

Al asignar un archivo, elige los módulos del escenario desde los que desea obtener los datos. A continuación, el nombre y el contenido del archivo se asignan automáticamente tal cual.

>[!NOTE]
>
>Si necesita procesar un archivo desde una dirección URL, le recomendamos que utilice el módulo `HTTP > Get a File` para descargar el archivo desde la dirección URL; a continuación, asigne el archivo desde el módulo `HTTP > Get a File` al campo del módulo deseado en su escenario.

>[!INFO]
>
>**Ejemplo:** Este ejemplo muestra cómo descargar documentos de [!DNL Adobe Workfront] a [!DNL Google Drive]. El activador [!UICONTROL Observar registro] de [!DNL Workfront] devuelve información detallada sobre cada documento, incluidos su nombre e ID.
>
>El módulo siguiente, [!UICONTROL Descargar documento], descarga los datos en sí para que se puedan cargar en Google Drive.
>
>Para asignar esta información a [!DNL Google Drive] para que se pueda cargar, debe especificar el archivo de origen desde el que se asignará la información. Si selecciona la opción [!DNL Workfront] > [!UICONTROL Descargar documento] en el archivo de origen, [!DNL Workfront Fusion] asigna el nombre de archivo y el contenido de archivo para que el documento de [!DNL Workfront] se cargue en la carpeta de Google especificada.
>
>![](assets/wf-download-document-350x605.png)
>
>Sin embargo, si desea cambiar el nombre del archivo pero mantener los datos tal cual, puede usar la opción [!UICONTROL Asignar] para asignar el nombre y el contenido del archivo por separado. Debe introducir el nombre completo del archivo, incluida la extensión. Se admiten formatos de texto y formatos binarios, como fotos, vídeos y PDF.
>
>![](assets/use-the-map-option-350x358.png)
