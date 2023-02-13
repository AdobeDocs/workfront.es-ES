---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Recibir un enlace web desde un servicio web
description: Si un servicio web no está implementado actualmente como una aplicación en [!DNL Adobe Workfront Fusion], pero admite el envío de enlaces web, puede agregar el servicio a un escenario utilizando el módulo weblock personalizado como déclencheur instantáneo.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Recibir un enlace web desde un servicio web

Si un servicio web no está implementado actualmente como una aplicación en [!DNL Adobe Workfront Fusion], pero admite el envío de enlaces web, puede agregar el servicio a un escenario utilizando el módulo weblock personalizado como déclencheur instantáneo.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Recibir un enlace web

1. Agregue la variable **[!UICONTROL Enlaces web] >[!UICONTROL Vínculo web personalizado]** al escenario.
1. Haga clic en **[!UICONTROL Agregar]**, escriba a **[!UICONTROL Nombre del Weblock]** en el cuadro que aparece y haga clic en **[!UICONTROL Guardar]**.

1. Haga clic en **[!UICONTROL Copiar dirección al portapapeles]** y haga clic en **[!UICONTROL OK]**.

1. Inicie sesión en el servicio web y haga lo siguiente:

   1. En el [!UICONTROL Configuración] para el servicio web, cree un weblink.
   1. Pegue la dirección que ha copiado en el portapapeles en el paso 3 .
   1. Seleccione el evento que almacenará en déclencheur el vínculo web.

1. En el [!DNL Workfront Fusion] , especifique el evento o los eventos en los que desea almacenar el déclencheur [!UICONTROL Vínculo web personalizado] módulo.
1. Ejecute el escenario.

   Cuando se producen los eventos, la variable [!UICONTROL Vínculo web personalizado] déclencheur del módulo y se ejecuta el escenario.
