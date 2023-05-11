---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: Utilizar TLS mutuo en módulos HTTP en Adobe Workfront Fusion
description: Puede utilizar TLS mutuos en los módulos HTTP de Adobe Workfront Fusion, lo que permite que ambas partes de la transacción de información verifiquen la identidad del otro.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: e67e6b6d3baf9f17a0a451fa4e1dbc365340f76e
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Utilizar TLS mutuo en módulos HTTP en [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion requiere un [!DNL Adobe Workfront Fusion] además de una licencia de Adobe Workfront.

## Resumen de TLS mutuo

Cuando envíe datos a través de Internet, es importante asegurarse de que se dirija a la ubicación correcta o que provenga de ella y de que solo el destinatario deseado pueda leerlos. Con TLS habilitado, el cliente (equipo que solicita información) utiliza certificados para verificar la identidad del servidor (equipo que proporciona información). Esto hace conexiones HTTP seguras.

TLS mutuo permite que esta confirmación de identidad funcione en ambos sentidos. Cuando el servidor envía su certificado para verificar su identidad al cliente, también solicita el certificado del cliente. Esto garantiza que el servidor no envíe información a un sitio o usuario que pueda usarla incorrectamente.

>[!INFO]
>
>**Ejemplo:**
>
>* **TLS**: Cuando una persona escribe &quot;MyGreatBank.com&quot; en un navegador, quiere estar seguro de que va a My Bueno Bank, no a un sitio web que pueda utilizar o vender su información bancaria. También quieren asegurarse de que la información de sus cuentas bancarias esté cifrada.
   >
   >   Cuando el navegador (el cliente) se conecta a MyGreatBank.com (el servidor), TLS requiere un certificado de MyGreatBank.com para verificar su identidad. El certificado lo proporciona una autoridad de certificación como [!DNL DigiCert] o [!DNL Thawte]. Dado que el explorador confía en la autoridad de certificación, permite la conexión.
>
>* **TLS mutuo**: MySoftware.com es un cliente de software que necesita información de la API MyGreatBank.com. MyGreatBank permite que sólo los clientes de confianza se conecten a sus servidores. Por lo tanto, además del TLS normal que verifica la identidad de MyGreatBank.com, el proceso TLS/autoridad de certificación también verifica la solicitud de MySoftware.com.


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
   <td> <p>[!UICONTROL Workfront Fusion para automatización e integración del trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Proporcionando su [!DNL Workfront Fusion] certificado público


Cuando se conecta a un servicio web con una solicitud HTTP, el servicio web suele requerir un [!DNL Workfront Fusion] certificado público de verificación. Esto permite que el servicio web compare el certificado presentado en la solicitud HTTP con el certificado del archivo, como una forma de garantizar que el certificado se encuentra en la lista de permitidos del servicio web.

Para obtener instrucciones sobre cómo cargar la variable [!DNL Adobe Workfront Fusion] certificado público de un servicio web, consulte la documentación del servicio web.

>[!NOTE]
>
>Es posible que deba proporcionar otra información además del certificado. Para obtener información sobre lo que requiere un servicio web, consulte la documentación de API del servicio web.

Puede utilizar los siguientes vínculos para descargar los certificados públicos de Workfront Fusion:

### Certificados para el 25 de mayo de 2023 - 9 de junio de 2024

>[!IMPORTANT]
>
>* Estos [!DNL Workfront Fusion] los certificados públicos expiran el 9 de junio de 2024. Cuando caduque el suyo, deberá cargar un nuevo certificado en el servicio web. Le recomendamos que:
   >
   >   * Tenga en cuenta la fecha de caducidad y configure un recordatorio para que cargue el certificado en el servicio web.
   >   * Marque esta página para encontrar fácilmente los nuevos certificados.
>
* Son certificados mTLS no comodín.
>

* [Descargar [!DNL Workfront Fusion] Certificado 2023](assets/fusion-prod-us-mtls-certificate.pem)
* [Descargar [!DNL Workfront Fusion] Certificado UE 2023](assets/fusion-prod-eu-mtls-certificate.pem)

   Para uso en la UE

### Certificados para el 14 de noviembre de 2022 - 15 de julio de 2023

>[!IMPORTANT]
>
>* Estos [!DNL Workfront Fusion] los certificados públicos expiran el 15 de julio de 2023.
>* Son certificados mTLS comodín.


* [Descargar [!DNL Workfront Fusion] Certificado 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Descargar [!DNL Workfront Fusion] Certificado UE 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   Para uso en la UE

## Habilitar TLS mutuo en [!DNL Workfront Fusion] Módulos HTTP

Todo [!DNL Workfront Fusion] [!UICONTROL HTTP] los módulos de solicitud tienen la opción de habilitar TLS mutuo.

Para habilitar el TLS mutuo en una [!UICONTROL HTTP] módulo de solicitud:

1. Agregue un [!UICONTROL HTTP] al escenario.
1. Empiece a configurar el módulo.

   Para obtener instrucciones sobre cómo configurar un [!UICONTROL HTTP] módulo de solicitud, consulte el artículo correspondiente en [[!UICONTROL HTTP] módulos](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Habilitar **[!UICONTROL Mostrar configuración avanzada]** cerca de la parte inferior del módulo.
1. Habilitar **[!UICONTROL Usar TLS mutuo]**.
