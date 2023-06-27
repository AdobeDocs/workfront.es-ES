---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Recibir un webhook de un servicio web
description: Si un servicio web no está implementado como aplicación en [!DNL Adobe Workfront Fusion], pero admite el envío de webhooks, puede añadir el servicio a un escenario utilizando el módulo de webhook personalizado como déclencheur instantáneo.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Recibir un webhook de un servicio web

Si un servicio web no está implementado como aplicación en [!DNL Adobe Workfront Fusion], pero admite el envío de webhooks, puede añadir el servicio a un escenario utilizando el módulo de webhook personalizado como déclencheur instantáneo.

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

## Recibir un webhook

1. Añada el **[!UICONTROL Webhooks] >[!UICONTROL Gancho web personalizado]** a su escenario.
1. Clic **[!UICONTROL Añadir]**, escriba a **[!UICONTROL Nombre del webhook]** en el cuadro que aparece y haga clic en **[!UICONTROL Guardar]**.

1. Clic **[!UICONTROL Copiar dirección al portapapeles]**, luego haga clic en **[!UICONTROL OK]**.

1. Inicie sesión en el servicio web y haga lo siguiente allí:

   1. En el [!UICONTROL Configuración] para el servicio web, cree un webhook.
   1. Pegue la dirección que ha copiado en el portapapeles en el paso 3
   1. Seleccione el evento que almacenará en déclencheur el enlace web.

1. En el [!DNL Workfront Fusion] , especifique el evento o eventos en los que desea almacenar en déclencheur el [!UICONTROL Gancho web personalizado] módulo.
1. Ejecute el escenario.

   Cuando se produce el evento o los eventos, la variable [!UICONTROL Gancho web personalizado] déclencheur del módulo y se ejecuta el escenario.
