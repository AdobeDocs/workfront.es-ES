---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Recepción de un webhook de un servicio web
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 77%

---

# Recepción de un webhook de un servicio web

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Configurar un webhook para un servicio web sin un conector](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/receive-a-webhook-from-a-web-service.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Si un servicio web no está implementado como aplicación en [!DNL Adobe Workfront Fusion], pero admite el envío de webhooks, puede añadirlo dicho servicio a un escenario utilizando el módulo de webhook personalizado como activador instantáneo.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
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

## Recepción de un webhook

1. Añada el módulo **[!UICONTROL Webhooks] >[!UICONTROL Webhook personalizado]** a su escenario.
1. Haga clic en **[!UICONTROL Añadir]**, escriba un **[!UICONTROL nombre de webhook]** en el cuadro que se muestra y, a continuación, haga clic en **[!UICONTROL Guardar]**.

1. Haga clic en **[!UICONTROL Copiar dirección al portapapeles]** y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

1. Inicie sesión en el servicio web y haga lo siguiente allí:

   1. En el área [!UICONTROL Configuración] del servicio web, cree un webhook.
   1. Pegue la dirección que ha copiado en el portapapeles en el paso 3
   1. Seleccione el evento que activará el webhook.

1. En el escenario de [!DNL Workfront Fusion], especifique el evento o eventos que desea para activar el módulo [!UICONTROL Webhook personalizado].
1. Ejecute el escenario.

   Cuando se produce el evento o los eventos, el módulo [!UICONTROL Webhook personalizado] se activa y se ejecuta el escenario.
