---
title: Cifrador de datos
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 74%

---

# Cifrador de datos

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Cifrador de datos](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/encryptor-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

[!DNL Adobe Workfront Fusion] Los módulos del [!UICONTROL cifrador de datos] le permiten cifrar cualquier dato de texto. Actualmente admiten el cifrado de mensajes mediante AES256 y PGP ([!UICONTROL OpenPGP]).

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
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Cifrado y descifrado de mensajes mediante PGP

Al cifrar y descifrar mediante PGP, es necesario utilizar un llavero y crear una clave privada o pública (o ambas).

Para obtener más información acerca de las claves públicas y privadas, consulte [Términos básicos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Para obtener más información sobre los llaveros, consulte [Claves en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## Los módulos del [!UICONTROL Cifrador de datos] y sus campos

Cuando está configurando módulos del [!UICONTROL Cifrador de datos], se muestran los campos siguientes. El título en negrita en un módulo indica un campo obligatorio.

### Cifrado de un mensaje PGP

Este módulo le permite cifrar un mensaje utilizando claves públicas y privadas.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Introduzca la clave privada del remitente. Esto puede autenticar la identidad del remitente.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Introduzca la clave pública del destinatario.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Escriba el mensaje que desea cifrar.</td>
    </tr>

### Descifrado de un mensaje PGP

Este módulo le permite descifrar un mensaje utilizando claves públicas y privadas.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Introduzca la clave privada del destinatario.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Introduzca la clave pública del destinatario. Esto puede autenticar la identidad del remitente.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Asigne el mensaje que desea descifrar.</td>
    </tr>
</table>
