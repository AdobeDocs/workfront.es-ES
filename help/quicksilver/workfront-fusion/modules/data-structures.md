---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Estructuras de datos en  [!DNL Adobe Workfront Fusion]
description: Una estructura de datos es un documento que describe en detalle el formato de los datos que se transfieren a Adobe Workfront Fusion. En función de este documento, el editor de escenarios es capaz de averiguar qué módulo devuelve o recibe qué tipo de datos. Los documentos de estructura de datos se utilizan principalmente para serializar y analizar formatos de datos como JSON, XML, CSV y otros.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Estructuras de datos en [!DNL Adobe Workfront Fusion]

Una estructura de datos es un documento que describe en detalle el formato de los datos que se están transfiriendo a [!DNL Adobe Workfront Fusion]. En función de este documento, el editor de escenarios es capaz de averiguar qué módulo devuelve o recibe qué tipo de datos. Los documentos de estructura de datos se utilizan principalmente para serializar y analizar formatos de datos como JSON, XML, CSV y otros.

Puede crear una estructura de datos haciendo clic en el botón [!UICONTROL Crear una nueva estructura de datos] de la sección [!UICONTROL Descripción general de la estructura de datos] o en la configuración del módulo que requiera la especificación de la estructura de datos.

Los tipos de datos admitidos se describen en el artículo [[!UICONTROL Tipos de módulos]](../../workfront-fusion/modules/module-types.md).

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
   <td role="rowheader">Product</td> 
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

## Generador de estructura de datos

No siempre es necesario crear estructuras de datos. Puede hacerlo más fácil utilizando una plantilla de nuestro generador integrado. Al proporcionar una muestra de datos, el generador creará automáticamente una estructura de datos basada en la muestra de datos introducida. La estructura de datos creada se puede modificar manualmente.

![](assets/data-structure-generator-350x341.jpg)
