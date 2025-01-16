---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Estructuras de datos en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 78%

---

# Estructuras de datos en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Crear y administrar almacenes de datos](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/data-stores.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Una estructura de datos es un documento que describe en detalle el formato de los datos que se transfieren a [!DNL Adobe Workfront Fusion]. En función de este documento, el editor de escenarios es capaz de averiguar qué módulo devuelve o recibe qué tipo de datos. Los documentos de estructura de datos suelen utilizarse para serializar o analizar formatos de datos como JSON, XML, CSV y otros.

Puede crear una estructura de datos haciendo clic en el botón [!UICONTROL Crear una nueva estructura de datos] de la sección [!UICONTROL Información general sobre la estructura de datos] o en la configuración del módulo que requiera la especificación de la estructura de datos.

Los tipos de datos admitidos se describen en el artículo [[!UICONTROL Tipos de módulos]](../../workfront-fusion/modules/module-types.md).

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
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte Licencias de [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Generador de estructuras de datos

No siempre es necesario crear estructuras de datos. Puede hacerlo más fácil utilizando una plantilla de nuestro generador integrado. Al proporcionar una muestra de datos, el generador creará de forma automática una estructura de datos basada en la muestra de datos introducida. La estructura de datos creada se puede modificar a mano.

![](assets/data-structure-generator-350x341.jpg)
