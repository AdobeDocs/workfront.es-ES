---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Métodos de solicitud HTTP en  [!DNL Adobe Workfront Fusion]
description: Cuando configure una llamada de API en un módulo, debe rellenar el campo del método de solicitud HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '410'
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

## Métodos HTTP

Utilice uno de los siguientes métodos HTTP.

* **[!UICONTROL GET]**: recupera datos de un servidor web basándose en sus parámetros. [!UICONTROL GET] solicita una representación del recurso especificado y recibe un mensaje de respuesta [!UICONTROL 200 OK] con el contenido solicitado si se realiza correctamente.
* **[!UICONTROL POST]**: envía datos a un servidor web en función de sus parámetros. Las solicitudes de [!UICONTROL POST] incluyen acciones como cargar un archivo. Si hay varios [!UICONTROL POST], el resultado puede ser diferente al de un solo [!UICONTROL POST], por lo que debe tener cuidado si envía varios [!UICONTROL POST] de forma involuntaria. Si un [!UICONTROL POST] se ha realizado correctamente, recibirá un mensaje de respuesta de [!UICONTROL 200 OK].
* **[!UICONTROL PUT]**: envía datos a una ubicación del servidor web en función de sus parámetros. Las solicitudes de [!UICONTROL PUT] incluyen acciones como cargar un archivo. La diferencia entre un [!UICONTROL PUT] y [!UICONTROL POST] es que el PUT es idempotente, lo que significa que el resultado de un único [!UICONTROL PUT] correcto es el mismo que muchos [!UICONTROL PUT]s idénticos. Si un PUT tiene éxito, recibe un mensaje de respuesta 200 (normalmente 201 o 204).
* **[!UICONTROL PATCH]**: (no disponible para algunos módulos de llamadas de API) Aplica modificaciones parciales a un recurso en un servidor web en función de sus parámetros. [!UICONTROL PATCH] no es idempotente, lo que significa que el resultado de varios [!UICONTROL PATCH] podría tener consecuencias no deseadas. Si un [!UICONTROL PATCH] tiene éxito, recibirá un mensaje de respuesta de 200 (normalmente 204).
* **[!UICONTROL DELETE]**: elimina el recurso especificado del servidor web en función de sus parámetros (si el recurso existe). Si un [!UICONTROL DELETE] se ha realizado correctamente, recibirá un mensaje de respuesta 200 OK.
