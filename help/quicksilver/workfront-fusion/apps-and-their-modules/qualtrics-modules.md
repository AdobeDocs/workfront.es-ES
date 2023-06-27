---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Qualtrics
description: En un [!DNL Adobe Workfront Fusion] En este escenario, se pueden automatizar los flujos de trabajo que utilizan Qualtrics y conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Módulos de Qualtrics

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Qualtrics], así como conectarlo a múltiples aplicaciones y servicios de terceros.

Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Requisitos previos

Para usar [!DNL Qualtrics] módulos, debe tener un [!UICONTROL Qualtrics] cuenta.

## Conectando [!DNL Qualtrics] hasta [!DNL Workfront Fusion]

Puede crear una conexión con su [!DNL Qualtrics] cuenta directamente desde dentro de un [!UICONTROL Qualtrics] módulo.

1. En cualquier [!UICONTROL Qualtrics] , haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. Introduzca la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nombre de conexión]</p> </td> 
      <td> <p>Introduzca un nombre para la nueva conexión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID del centro de datos] </td> 
      <td>Usar el formato <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clave de API [!UICONTROL]</td> 
      <td>Para localizar la clave de API, consulte la [!DNL Qualtrics] documentación.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!DNL Qualtrics] módulos y sus campos

Los siguientes módulos están disponibles para [!DNL Qualtrics] conector:

* [!UICONTROL Ver nueva respuesta de encuesta]
* [!UICONTROL Crear un contacto de directorio]
* [!UICONTROL Eliminar un contacto de directorio]
* [!UICONTROL Obtener un contacto de directorio]
* [!UICONTROL Actualizar un contacto de directorio]
* [!UICONTROL Creación de una nueva distribución de encuesta mediante SMS]
* [!UICONTROL Distribuir una encuesta por correo electrónico]
* [!UICONTROL Realizar una llamada de API]
* [!UICONTROL Enumerar contactos de directorio]
