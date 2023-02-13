---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]
description: Al configurar una llamada de API en un módulo, debe rellenar el campo para el método de solicitud HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]

Al configurar una llamada de API en un módulo, debe rellenar el campo para el método de solicitud HTTP.

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
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Métodos HTTP

Utilice uno de los siguientes métodos HTTP.

* **[!UICONTROL GET]**: Recupera datos de un servidor web en función de sus parámetros. [!UICONTROL GET] solicita una representación del recurso especificado y recibe un [!UICONTROL 200 OK] mensaje de respuesta con el contenido solicitado si se realiza correctamente.
* **[!UICONTROL POST]**: Envía datos a un servidor web en función de sus parámetros. [!UICONTROL POST] las solicitudes incluyen acciones como cargar un archivo. Múltiple [!UICONTROL POST]puede tener como resultado un resultado diferente a un único [!UICONTROL POST], así que tenga cuidado de enviar varios de forma no intencionada [!UICONTROL POST]s. Si [!UICONTROL POST] si tiene éxito, recibirá un [!UICONTROL 200 OK] mensaje de respuesta.
* **[!UICONTROL PUT]**: Envía datos a una ubicación del servidor web en función de sus parámetros. [!UICONTROL PUT] las solicitudes incluyen acciones como cargar un archivo. La diferencia entre un [!UICONTROL PUT] y [!UICONTROL POST] es que el PUT es idempotente, lo que significa que el resultado de un solo éxito [!UICONTROL PUT] es igual que muchos idénticos [!UICONTROL PUT]s. Si un PUT se realiza correctamente, recibirá un mensaje de respuesta de 200 (normalmente 201 o 204).
* **[!UICONTROL PATCH]**: (No disponible para algunos módulos de llamadas de API) Aplica modificaciones parciales a un recurso en un servidor web en función de sus parámetros. [!UICONTROL PATCH] no es idempotente, lo que significa que el resultado de [!UICONTROL PATCH]Podría tener consecuencias no deseadas. Si [!UICONTROL PATCH] Si la respuesta es correcta, recibirá un mensaje de 200 respuestas (normalmente 204).
* **[!UICONTROL DELETE]**: Elimina el recurso especificado del servidor web en función de sus parámetros (si el recurso existe). Si [!UICONTROL DELETE] se ha realizado correctamente, recibirá un mensaje de respuesta de 200 OK.
