---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Recibir un webhook de un servicio web
description: Si un servicio web no está implementado como aplicación en  [!DNL Adobe Workfront Fusion], pero admite el envío de webhooks, puede agregar el servicio a un escenario utilizando el módulo de webhook personalizado como déclencheur instantáneo.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Recibir un webhook de un servicio web

Si un servicio web no está implementado como aplicación en [!DNL Adobe Workfront Fusion], pero admite el envío de webhooks, puede agregar el servicio a un escenario utilizando el módulo de webhook personalizado como déclencheur instantáneo.

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

## Recibir un webhook

1. Agregue el módulo **[!UICONTROL Webhooks] >[!UICONTROL Webhook personalizado]** a su escenario.
1. Haga clic en **[!UICONTROL Agregar]**, escriba un **[!UICONTROL nombre de webhook]** en el cuadro que se muestra y, a continuación, haga clic en **[!UICONTROL Guardar]**.

1. Haga clic en **[!UICONTROL Copiar dirección al portapapeles]** y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

1. Inicie sesión en el servicio web y haga lo siguiente allí:

   1. En el área [!UICONTROL Configuración] del servicio web, cree un enlace web.
   1. Pegue la dirección que ha copiado en el portapapeles en el paso 3
   1. Seleccione el evento que almacenará en déclencheur el enlace web.

1. En el escenario [!DNL Workfront Fusion], especifique el evento o eventos que desea almacenar en déclencheur el módulo [!UICONTROL webhook personalizado].
1. Ejecute el escenario.

   Cuando ocurren el evento o los eventos, el módulo [!UICONTROL webhook personalizado] entra en déclencheur y se ejecuta el escenario.
