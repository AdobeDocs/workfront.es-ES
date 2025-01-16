---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Métodos de petición HTTP en  [!DNL Adobe Workfront Fusion]
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 83%

---

# Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Métodos de solicitud HTTP](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/http-request-methods.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Al configurar una llamada de API en un módulo, debe rellenarse el campo del método de petición HTTP.

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

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Métodos HTTP

Utilice uno de los siguientes métodos HTTP.

* **[!UICONTROL GET]**: recupera datos de un servidor web en función de sus parámetros. [!UICONTROL GET] solicita una representación del recurso especificado y recibe un mensaje de respuesta [!UICONTROL 200 OK] con el contenido solicitado si se ejecuta correctamente.
* **[!UICONTROL POST]**: envía datos a un servidor web en función de sus parámetros. Las peticiones [!UICONTROL POST] incluyen acciones como cargar un archivo. Si hay varios [!UICONTROL POST], el resultado puede ser diferente del de un solo [!UICONTROL POST], por lo que debe tener cuidado si envía varios [!UICONTROL POST] de forma involuntaria. Si un [!UICONTROL POST] se ejecuta correctamente, se recibe un mensaje de respuesta [!UICONTROL 200 OK].
* **[!UICONTROL PUT]**: envía datos a una ubicación del servidor web en función de sus parámetros. Las peticiones [!UICONTROL PUT] incluyen acciones como cargar un archivo. La diferencia entre [!UICONTROL PUT] y [!UICONTROL POST] es que el PUT es idempotente, lo que significa que el resultado de un único [!UICONTROL PUT] correcto es el mismo que el de muchos [!UICONTROL PUT] idénticos. Si un PUT se ejecuta correctamente, se recibe un mensaje de respuesta 200 (normalmente 201 o 204).
* **[!UICONTROL PATCH]**: (no disponible para algunos módulos de llamadas de API) Aplica modificaciones parciales a un recurso en un servidor web en función de sus parámetros. [!UICONTROL PATCH] no es idempotente, lo que significa que el resultado de varios [!UICONTROL PATCH] podría tener consecuencias no deseadas. Si un [!UICONTROL PATCH] se ejecuta correctamente, se recibe un mensaje de respuesta 200 (normalmente 204).
* **[!UICONTROL DELETE]**: elimina el recurso especificado del servidor web en función de sus parámetros (si el recurso existe). Si un [!UICONTROL DELETE] se ejecuta correctamente, se recibe un mensaje de respuesta 200 OK.
