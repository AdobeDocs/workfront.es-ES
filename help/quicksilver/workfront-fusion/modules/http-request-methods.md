---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]
description: Cuando configure una llamada de API en un módulo, debe rellenar el campo del método de solicitud HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]

Cuando configure una llamada de API en un módulo, debe rellenar el campo del método de solicitud HTTP.

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

## Métodos HTTP

Utilice uno de los siguientes métodos HTTP.

* **[!UICONTROL GET]**: recupera datos de un servidor web en función de sus parámetros. [!UICONTROL GET] solicita una representación del recurso especificado y recibe un [!UICONTROL 200 OK] mensaje de respuesta con el contenido solicitado si se realiza correctamente.
* **[!UICONTROL POST]**: envía datos a un servidor web en función de sus parámetros. [!UICONTROL POST] Las solicitudes de incluyen acciones como cargar un archivo. Múltiple [!UICONTROL POST]s puede dar como resultado un resultado diferente a uno solo [!UICONTROL POST], por lo que debe tener cuidado al enviar varios de forma involuntaria [!UICONTROL POST]s. Si a [!UICONTROL POST] se ha realizado correctamente, recibe un [!UICONTROL 200 OK] mensaje de respuesta.
* **[!UICONTROL PUT]**: envía datos a una ubicación del servidor web en función de sus parámetros. [!UICONTROL PUT] Las solicitudes de incluyen acciones como cargar un archivo. La diferencia entre una [!UICONTROL PUT] y [!UICONTROL POST] es que el PUT es idempotente, lo que significa que el resultado de un único [!UICONTROL PUT] es el mismo que muchos idénticos [!UICONTROL PUT]s. Si un PUT tiene éxito, recibe un mensaje de respuesta de 200 (normalmente 201 o 204).
* **[!UICONTROL PATCH]**: (no disponible para algunos módulos de llamada de API) aplica modificaciones parciales a un recurso en un servidor web en función de sus parámetros. [!UICONTROL PATCH] no es idempotente, lo que significa que el resultado de múltiples [!UICONTROL PATCH]La de podría tener consecuencias no deseadas. Si un [!UICONTROL PATCH] tiene éxito, recibirá un mensaje de respuesta de 200 (normalmente 204).
* **[!UICONTROL DELETE]**: elimina el recurso especificado del servidor web en función de sus parámetros (si existe el recurso). Si un [!UICONTROL DELETE] se ha realizado correctamente, recibe un mensaje de respuesta 200 OK.
